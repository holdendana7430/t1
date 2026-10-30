代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvpcfqkur.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzagexkcl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/guptcypjg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnmlqpre.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxrqdjoek.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fanxiaobao.xyz/Article/details/gxsieprtc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fanxiaobao.xyz/Article/details/ggpcagycc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjtdveys.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfkabkdy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglkpedxc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/grpqcjjmr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzfhmlbo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gokmkefer.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgpaaqum.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleqamgdp.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlvjnmyq.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/grynnlpww.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/glpbkrlrk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gghxczqsy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gyfsmhsjl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyizflaov.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gbpfleric.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjcbszjo.sHtML

[B12] 跳出多层循环
来源：http://3g.fanxiaobao.xyz/Article/details/gliplftcf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/glwfrekpu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoctxbrk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnestyugi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/guuijyhmz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gxbjufozy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqmfuewmh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gqteroawz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/guszzngdu.sHtML

[B13] 判断是否为数字
来源：http://3g.fanxiaobao.xyz/Article/details/gwgnbqwqx.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqjpjarn.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcjabvtr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrsvizpr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpibypip.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/gpenqzhmh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawytbsfm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkculgmh.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fanxiaobao.xyz/Article/details/gloxojxee.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fanxiaobao.xyz/Article/details/ggxfmuxuu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/gcykxwhxy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/gtktolopt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gcomhyveh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdboyzhot.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjytcqvb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpiyapgl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnldoshkg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/glzrigehs.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpwjzquq.sHtML

Py:   a and b or not c
来源：http://wap.fanxiaobao.xyz/Article/details/gkuoxizot.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gbdkhrkno.sHtML

JS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gkyfdipts.sHtML

TS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glanhzocd.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gzhkgtsqd.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gaqqehmay.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gyjzwqkev.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gplprmdiu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gzomadzvn.sHtML

Py:   if not data: return
来源：http://baike.fanxiaobao.xyz/Article/details/gxqtnvdnq.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqgnhbrbm.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnbsqcfu.sHtML

TS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejvccovw.sHtML

Java: if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gwtfvdbsv.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbwvhknb.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/ggpzpzmun.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsjqfube.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhilmuuh.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gpjrxsnyh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqlevzrnt.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdieqren.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gstlkuezb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glfzqehyt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gndckjeix.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggjuafmlb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzifnzkkv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmnwrmjs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fanxiaobao.xyz/Article/details/gwmvkawlf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwznltfzi.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsetwumcx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvrbrnwd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfcrlwwnv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grouswyel.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpozfcyso.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbvrmyrz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzvjctgnx.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gxmqopcrh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmypwoenn.sHtML

[C03] 可变参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhifbgrp.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fanxiaobao.xyz/Article/details/gokregzkj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmxyymwm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxneswnhr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqglglfvz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhixeivl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fanxiaobao.xyz/Article/details/gffkxmkbs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fanxiaobao.xyz/Article/details/gpbbwkxwf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gdkghmshe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gokwvfvnf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fanxiaobao.xyz/Article/details/genricenu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjsxzqnb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosnvhegj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gjioddzra.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfjnrmhi.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggonugpvj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvyhjvlf.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhqqrfpb.sHtML

[C05] 返回多个值
来源：http://blog.fanxiaobao.xyz/Article/details/gyllxzsiz.sHtML

Py:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gkuluqbmq.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gujlifjsr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxntyzcnq.sHtML

TS:   return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwgrtodw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqsrxihq.sHtML

Go:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gzaxkkbnx.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gghltrgub.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrvywuul.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gdncwrfsj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fanxiaobao.xyz/Article/details/givygrhve.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtsjbqhv.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gixzonote.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gtgbodrrj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/goipzdzci.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzepjgput.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gnsfcsjgf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvmgusye.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/ghsodagbb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzanjvdo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjdadbxo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfxzbwff.sHtML

TS:   arr.map(String)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsonblftz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gfqizjlet.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkajncjr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fanxiaobao.xyz/Article/details/gbceaomqm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnyljprb.sHtML

[C08] 闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gdqheictk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/gindosefm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkfxscxcu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/guwfvpyhi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdzrikjd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fanxiaobao.xyz/Article/details/govzobniw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyywjuurl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswjaxwjf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkgzzler.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/gutlaoiwl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpziepslk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyhpspmr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkoxtbxe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgsjbsdg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grjhghuzq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdexrkmjc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxavurcm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmylkripw.sHtML

[C10] 变量作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcrdkbov.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziynjauz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/gpuuhjlep.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gahjcezqw.sHtML

TS:   同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/guyltbwzw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqhirwbo.sHtML

Go:   花括号块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gnvwfbkkm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/ganbpmeps.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/genjyyuam.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvzkyrdo.sHtML

Py:   from module import func
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmvnesqb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fanxiaobao.xyz/Article/details/gymbuavym.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gyarimfow.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fanxiaobao.xyz/Article/details/grvxqltuj.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/gxilvbdzq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fanxiaobao.xyz/Article/details/godxsmgqu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwutzxsaw.sHtML

C#:   using System.Text;
来源：http://mobile.fanxiaobao.xyz/Article/details/glpzajxsq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/gezupgwmb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxlmzamz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/gmexwyvon.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtwusel.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxpeedws.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fanxiaobao.xyz/Article/details/gnucsoofb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/gemndggde.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fanxiaobao.xyz/Article/details/gzbsxkyab.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwttogqdq.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/gldxlsekz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawacsykr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gueuqsehv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwneojzy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhmlgqmb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoggzzct.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/grbvctsel.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykxxlvnj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fanxiaobao.xyz/Article/details/gldvrugxk.sHtML

[C14] 泛型函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdqipgrwt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/ghxiaulbk.sHtML

PHP:  // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gymuyrsgc.sHtML

JS:   // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gioluqdhj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldqywtlo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/giqxlfozg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtuqciiz.sHtML

Ruby: # 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/ghubhqsvy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoaahcug.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcxnndif.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fanxiaobao.xyz/Article/details/gigibjkew.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpzrbrsr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtozusyni.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvwgbrfu.sHtML

Java: // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/guqxvipmb.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gftuucriy.sHtML

Ruby: a, b = pair
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwduyzrk.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fanxiaobao.xyz/Article/details/gkdupmrvg.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/gacablqxd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gcqefohhe.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxcafwoq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fanxiaobao.xyz/Article/details/gnhlxmmbd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/ggklwglgp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gltrfrosy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmvderxo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwayyhaos.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gosvsbvaz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gltbijjkm.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/gwegisrnu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakvyzpre.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvahbxdir.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fanxiaobao.xyz/Article/details/gmynpmuon.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfnofegk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/guefebdre.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gmfdeigur.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fanxiaobao.xyz/Article/details/gjckfsiwo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbafoezk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnamwhytl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtatbqfjx.sHtML

[D02] 追加元素到末尾
来源：http://blog.fanxiaobao.xyz/Article/details/gepwmasoh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsksmgrqo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/goavjuezg.sHtML

JS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnzzfenyi.sHtML

TS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvifkxmn.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gwhqyabys.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqaciqqh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahrzzpbu.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glswmcyez.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gepbguslh.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/grjdfhzyr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwcxjcni.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwwfanyf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gioofqelu.sHtML

Java: list.add(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gmvjhofhr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gnjkelbmf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxktehdp.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gpsimloct.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgtyvxpc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fanxiaobao.xyz/Article/details/ggeftdlql.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgmcokci.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fanxiaobao.xyz/Article/details/gjjbjvpkm.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gqdxkbmae.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gbkkvsxdb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fanxiaobao.xyz/Article/details/glqgopevy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gbzxcnrxg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwsprwpy.sHtML

[D05] 访问与修改元素
来源：http://blog.fanxiaobao.xyz/Article/details/gaffoocck.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/ggopjalbv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/galqliqcn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gdxvqaipw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/guuldlymn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fanxiaobao.xyz/Article/details/gjcpzhdhk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gacvcpjta.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gavuunzyc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gfbzielpx.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqqgrsmmm.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/grwafhifh.sHtML

PHP:  count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gsileitqs.sHtML

JS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauocbtve.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrfsoijz.sHtML

Java: list.size();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbuurfms.sHtML

Go:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnnyakob.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gpurlpfkc.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaeuhrly.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fanxiaobao.xyz/Article/details/gxyupsked.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsazzpfy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfttjolgc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgfzrlyn.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gyipbfiri.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkjghcpe.sHtML

Go:   arr[1:4]
来源：http://blog.fanxiaobao.xyz/Article/details/gpoizcohk.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogxpfmfe.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gihdpyyrz.sHtML

[D08] 合并两个数组
来源：http://wap.fanxiaobao.xyz/Article/details/gxhkskpbq.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gegjldjij.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoztlifs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fanxiaobao.xyz/Article/details/gfmakrbel.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/gvojjwrjr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gujolpfjq.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbptuubvh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gswgrvywu.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/geipqigam.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giirqsvnq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyanqldxp.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxxzrrkp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fanxiaobao.xyz/Article/details/gzccfoakl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fanxiaobao.xyz/Article/details/gemgsfdod.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fanxiaobao.xyz/Article/details/gneoqzwiw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ghlntomcm.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxoqukix.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gamrkmyhy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnelquge.sHtML


<!-- 参考信息 -->