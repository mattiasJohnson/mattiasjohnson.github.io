---
layout: post
title: "Java program: hitta primtalsfaktorer"
---
+ TOC
{:toc}

## Överblick
Uppgift: Göra ett program som hittar ett tals primtalsfaktorer.
Exempel: '78' >> '2 3 13'
Språk: Java

## Algoritm
Input: 'N'
1. Kolla så 'N' är ett positivt heltal
2. Kolla om 'N' är ett primtal
3. uppdaterar


## Koden

```java
protected boolean isPrime(long num) {

		if (num % 2 == 0) {
			return false;
		}

		for (int i = 3; i <= Math.sqrt(num); i += 2) {
			if (num % i == 0) {
				return false;
			}
		}

		return true;
	}
```

## Varför den fungerar

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer vestibulum in orci eget pellentesque. Ut fringilla finibus sollicitudin. Pellentesque tellus odio, consectetur id ullamcorper ut, convallis sit amet nisi. Sed orci velit, maximus non arcu eget, dictum lobortis nulla. In vitae neque et mi ullamcorper rhoncus non at arcu. Proin vitae egestas odio, ut efficitur risus. Nullam eu ornare quam. Vivamus eget ante vel libero ultrices tempus imperdiet et elit. Phasellus semper congue tellus gravida bibendum. Nam luctus odio quis orci congue, non feugiat sem scelerisque. Nulla volutpat commodo ipsum. Donec tellus nibh, interdum at mattis a, varius pulvinar neque. Vivamus luctus tempor felis, ut scelerisque est iaculis non.

## Avslut
dd

'''
