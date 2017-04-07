---
layout: post
title:  "Mon premier post !"
date:   2017-03-28 17:00:55 +0200
categories: jekyll update
---
<!-- start slipsum code -->

Well, the way they make shows is, they make one show. That show's called a pilot. Then they show that show 
to the people who make shows, and on the strength of that one show they decide if they're going to make 
more shows. Some pilots get picked and become television programs. Some don't, become nothing. 
She starred in one of the ones that became nothing.

Now that we know who you are, I know who I am. I'm not a mistake! It all makes sense! In a comic, you know how you can tell who the arch-villain's going to be? He's the exact opposite of the hero. And most times they're friends, like you and me! I should've known way back when... You know why, David? Because of the kids. They called me Mr Glass.

You think water moves fast? You should see ice. It moves like it has a mind. Like it knows it killed the world once and got a taste for murder. After the avalanche, it took us a week to climb out. Now, I don't know exactly when we turned on each other, but I know that seven of us survived the slide... and only five made it out. Now we took an oath, that I'm breaking now. We said we'd say it was the snow that killed the other two, but it wasn't. Nature is lethal but it doesn't hold a candle to man.

{% highlight ruby %}
require 'organ_cooker/shared'

module OrganCooker
  class Project
    include Shared

    attr_reader :name
    attr_reader :temperature
    attr_reader :diapason

    def temperature=(temp)
      raise ArgumentError, 'The temperature must be a number.' unless temp.is_a? Numeric
      raise ArgumentError, 'The temperature must be beetween -20°C & 40°C' if temp < -20 || temp > 40
      @temperature = temp
    end

    def diapason=(diap)
      raise ArgumentError, 'The diapason must be a number.' unless diap.is_a? Numeric
      raise ArgumentError, 'The diapason must be positive' if diap.zero? || diap.negative?
      @diapason = diap
    end

    def initialize(name, temperature = 18, diapason = 440)
      self.name        = name
      self.temperature = temperature
      self.diapason    = diapason
    end

    def speed_of_sound
      331.5 + 0.607 * @temperature
    end

    def to_s
      "==== Project: #{@name} ===="
    end
  end
end
{% endhighlight %}

Now that there is the Tec-9, a crappy spray gun from South Miami. This gun is advertised as the most popular gun in American crime. Do you believe that shit? It actually says that in the little book that comes with it: the most popular gun in American crime. Like they're actually proud of that shit. 

Your bones don't break, mine do. That's clear. Your cells react to bacteria and viruses differently than mine. You don't get sick, I do. That's also clear. But for some reason, you and I react the exact same way to water. We swallow it too fast, we choke. We get some in our lungs, we drown. However unreal it may seem, we are connected, you and I. We're on the same curve, just on opposite ends.

Look, just because I don't be givin' no man a foot massage don't make it right for Marsellus to throw Antwone into a glass motherfuckin' house, fuckin' up the way the nigger talks. Motherfucker do that shit to me, he better paralyze my ass, 'cause I'll kill the motherfucker, know what I'm sayin'?

Do you see any Teletubbies in here? Do you see a slender plastic tag clipped to my shirt with my name printed on it? Do you see a little Asian child with a blank expression on his face sitting outside on a mechanical helicopter that shakes when you put quarters in it? No? Well, that's what you see at a toy store. And you must think you're in a toy store, because you're here shopping for an infant named Jeb.

You think water moves fast? You should see ice. It moves like it has a mind. Like it knows it killed the world once and got a taste for murder. After the avalanche, it took us a week to climb out. Now, I don't know exactly when we turned on each other, but I know that seven of us survived the slide... and only five made it out. Now we took an oath, that I'm breaking now. We said we'd say it was the snow that killed the other two, but it wasn't. Nature is lethal but it doesn't hold a candle to man.

<!-- end slipsum code -->
