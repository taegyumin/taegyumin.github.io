---
layout: post
title:  "어느 한 컴퓨터공학과 학생이 유명한 교수님을 찾아가 물었다."
date:   2020-04-02 01:52:35 +0900
categories: jekyll update
---

	어느 한 컴퓨터공학과 학생이 유명한 교수님을 찾아가 물었다.
	"재귀함수가 뭔가요?"
	"잘 들어보게. 옛날옛날 한 산 꼭대기에 이세상 모든 지식을 통달한 선인이 있었어. 마을 사람들은 모두 그 선인에게 수많은 질문을 했고, 모두 지혜롭게 대답해 주었지. 그의 답은 대부분 옳았다고 하네.
	그런데 어느 날, 그 선인에게 한 선비가 찾아와서 물었어.
	"재귀함수가 뭔가요?"
	"잘 들어보게. 옛날옛날 한 산 꼭대기에 이세상 모든 지식을...

{% highlight ruby %}
# -*- coding: utf-8 -*-

def clever_student
	
	puts "One day a student majoring in computer science went to a reputable professor and asked. \n"

	def clever_student(n)

		#if n>10
		#	return 0
		#end

		puts " \"What is the recursive function?\" \n \"Listen carefully. Once upon a time there was a man who mastered all the knowledge of the world at the top of a mountain. The villagers all asked him a lot of questions, and he answered them all wisely. Most of his answers were correct. But one day, a student came to him and asked."
		
		n += 1
		return clever_student(n)
	end
	
	clever_student(0)
end

clever_student
#=> SystemStackError (stack level too deep)
{% endhighlight %}
