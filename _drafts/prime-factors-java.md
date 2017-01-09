---
layout: post
title: "Java program: hitta primtalsfaktorer"
---
+ TOC
{:toc}

## Problembeskrivning
För att hitta primtalsfaktorer behöver man ha en metod som testar om ett tal är ett primtal.
Den kan sedan optimeras lite med hjälp av lite matematik.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer vestibulum in orci eget pellentesque. Ut fringilla finibus sollicitudin. Pellentesque tellus odio, consectetur id ullamcorper ut, convallis sit amet nisi. Sed orci velit, maximus non arcu eget, dictum lobortis nulla. In vitae neque et mi ullamcorper rhoncus non at arcu. Proin vitae egestas odio, ut efficitur risus. Nullam eu ornare quam. Vivamus eget ante vel libero ultrices tempus imperdiet et elit. Phasellus semper congue tellus gravida bibendum. Nam luctus odio quis orci congue, non feugiat sem scelerisque. Nulla volutpat commodo ipsum. Donec tellus nibh, interdum at mattis a, varius pulvinar neque. Vivamus luctus tempor felis, ut scelerisque est iaculis non.

## Hitta primtalet
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer vestibulum in orci eget pellentesque. Ut fringilla finibus sollicitudin. Pellentesque tellus odio, consectetur id ullamcorper ut, convallis sit amet nisi. Sed orci velit, maximus non arcu eget, dictum lobortis nulla. In vitae neque et mi ullamcorper rhoncus non at arcu. Proin vitae egestas odio, ut efficitur risus. Nullam eu ornare quam. Vivamus eget ante vel libero ultrices tempus imperdiet et elit. Phasellus semper congue tellus gravida bibendum. Nam luctus odio quis orci congue, non feugiat sem scelerisque. Nulla volutpat commodo ipsum. Donec tellus nibh, interdum at mattis a, varius pulvinar neque. Vivamus luctus tempor felis, ut scelerisque est iaculis non.
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer vestibulum in orci eget pellentesque. Ut fringilla finibus sollicitudin. Pellentesque tellus odio, consectetur id ullamcorper ut, convallis sit amet nisi. Sed orci velit, maximus non arcu eget, dictum lobortis nulla. In vitae neque et mi ullamcorper rhoncus non at arcu. Proin vitae egestas odio, ut efficitur risus. Nullam eu ornare quam. Vivamus eget ante vel libero ultrices tempus imperdiet et elit.

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/NoFLJLJ7abE" frameborder="0" allowfullscreen="true"> </iframe>
</figure>

## Koden

{% highlight Java %}
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
{% endhighlight %}

## Varför den fungerar

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer vestibulum in orci eget pellentesque. Ut fringilla finibus sollicitudin. Pellentesque tellus odio, consectetur id ullamcorper ut, convallis sit amet nisi. Sed orci velit, maximus non arcu eget, dictum lobortis nulla. In vitae neque et mi ullamcorper rhoncus non at arcu. Proin vitae egestas odio, ut efficitur risus. Nullam eu ornare quam. Vivamus eget ante vel libero ultrices tempus imperdiet et elit. Phasellus semper congue tellus gravida bibendum. Nam luctus odio quis orci congue, non feugiat sem scelerisque. Nulla volutpat commodo ipsum. Donec tellus nibh, interdum at mattis a, varius pulvinar neque. Vivamus luctus tempor felis, ut scelerisque est iaculis non.

## Avslut
dd

'''
