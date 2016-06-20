---
layout: post
title: "Retouch Print in Java"
date: 2016-06-21 01:41:07
image: '/assets/img/'
description:'Refresh your basics in Java'
main-class:'java'
color:'#2DA0C3'
tags:java
categories:
twitter_text:'Retouch print in java'
introduction:
---
In this post we are refreshing our mind towards core how to use the various output statements in Java. While you print a statement, there resides several transaction between the Program and the JVM(Java Virtual Machine).In Java , all are byte based streams for reading input and showing result as output.In order to understand Java I/0 , you have to know how java deals with various integers, characters,bytes and other primitive data types. Most important thing is that to analyze  transformation of data types from one to another 

{% highlight java %}
package up2java;

/**
 *
 * @author Sabari Raja
 */
 
public class SamplePrintf {
 
    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        System.out.print("Welcome to Java Again");
        System.out.write(10);
        System.out.printf("%d%c",100,'%');
        System.out.write(9);
        System.out.print("pure coffee");
        System.out.println("\n taste me again");
    }
}

{% endhighlight %}

Above program describes about various possible printing output streams that are available in java. Here print(“ “) is normal operation like printing a sample text. While write(int) is some thing different. Its converts numeric value to byte. Usually write(9) is similar to using ‘\t’. Printf(“%d”,value) this method of printing is similar to printf in C. From release of Jdk 5.0, we have this facility of using printf. Println is for printing the statement with end of line. Main use to start newline.

while you compile and run the above program you will get following result
{% highlight java %}
Welcome to Java Again
100%     pure coffee
taste me again
{% endhighlight %}


