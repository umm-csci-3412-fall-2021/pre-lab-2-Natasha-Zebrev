# Leak report

There was extra space allocated that was never freed. However, it would still be used until the string was checked if it was
cleaned. After it was checked to see if the string was empty, the memory was able to be freed.
