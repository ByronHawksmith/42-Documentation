# Writing an int value to the write() function

```c
#include <unistd.h>

int	main(void) 
{
	int	*a;
	int	val;

	val = 50;
	a = &val;

	write(1, a, 1);
}
```
