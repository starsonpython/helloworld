# helloworld
Test another repository

Python 2.7.14 (v2.7.14:84471935ed, Sep 16 2017, 20:19:30) [MSC v.1500 32 bit (Intel)] on win32
Type "copyright", "credits" or "license()" for more information.
>>> #！/usr/bin/env python
>>> #-*- coding:utf-8 -*-
>>> import random
>>> while 1:
	s = int(random.randint(1,3))
	if s == 1:
		ind = "石头"
	elif s == 2:
                ind = "剪刀"
        elif s == 3:
                ind = "布"

        m =  raw_input('输入 石头、剪刀、布，输入"end"结束游戏 ： ')

        blist=['石头','剪刀','布']
        if (m not in blist )and (m != 'end'):
                print "输入错误，请重新输入！"
        elif (m not in blist ) and ( m == 'end'):
                print "\n游戏推出中"
                break
        elif m == ind :
                print "电脑出了： " + ind + ",平局"
        elif ( m== '石头' and ind == '剪刀') or (m == '剪刀' and ind =='布' ) or (m == '布' and ind == '石头') :
                print "电脑出了： " + ind + "，你赢了！"
        elif ( m == '石头' and ind == '布') or ( m == '剪刀' and ind == '石头') or ( m == '布' and ind == '剪刀' ):
                print "电脑出了： " + ind + "，你输了！"
                
