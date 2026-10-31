代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ia.bjjhwx.cn

================================================================================
来源：http://zw.huixinmuqiang.cn

B. 流程控制
来源：http://ay.shxzskj.cn

================================================================================
来源：http://ur.szsharing.cn

[B01] 条件判断 if / else
来源：http://su.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ov.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lj.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://td.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yi.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cs.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zo.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oh.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ai.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://qb.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://km.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://by.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hu.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xm.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://je.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xb.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sb.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oo.szxytkj.cn

[B03] switch / match / case
来源：http://bv.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gi.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zb.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lt.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://um.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zg.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pu.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mt.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dv.chemitech.net.cn

[B04] for 计数循环
来源：http://va.521024.cn

Py:   for i in range(10): print(i)
来源：http://ms.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ol.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iz.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://th.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ap.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ep.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://dl.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://na.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://jk.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://du.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nq.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rr.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jm.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wo.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ws.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://sh.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ba.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://ww.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cp.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dh.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://um.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pc.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fn.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nt.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://al.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qs.muxihuayi.cn

[B07] while 循环
来源：http://bc.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://ws.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vh.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://ja.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://cp.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://pl.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://py.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://yc.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://bo.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://lh.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://me.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zs.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://vk.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://hr.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://bx.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ax.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://er.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://nh.9csxet.cn

[B09] break 与 continue
来源：http://rp.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jl.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://au.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lj.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tf.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yj.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gz.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ak.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wu.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://ka.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ju.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hm.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ek.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zq.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gj.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dv.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://es.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yb.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://lv.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://af.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://ce.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jp.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iw.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mj.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wr.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://zh.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bl.haigaiapp.cn

[B12] 跳出多层循环
来源：http://xj.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hf.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://db.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zm.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ry.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kp.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://av.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gy.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mq.haigaiapp.cn

[B13] 判断是否为数字
来源：http://nj.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://gg.521024.cn

PHP:  is_numeric($x)
来源：http://ai.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ha.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wm.chemitech.net.cn

Java: x instanceof Number
来源：http://xs.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://db.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://tk.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://ko.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://lm.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gc.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vy.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://ju.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://ia.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sc.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cu.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://af.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aq.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://gb.jianghongdianzi.cn

Py:   a and b or not c
来源：http://vj.hahajie.cn

PHP:  $a && $b || !$c
来源：http://kg.szxytkj.cn

JS:   a && b || !c
来源：http://nl.shtwfgs.cn

TS:   a && b || !c
来源：http://wj.asd995.cn

Java: a && b || !c
来源：http://dz.yuntaijiaju.cn

Go:   a && b || !c
来源：http://bk.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://zq.nszjky.cn

C#:   a && b || !c
来源：http://vz.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oe.yuexingan06.cn

Py:   if not data: return
来源：http://tl.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://cu.nszjky.cn

JS:   if (!data) return;
来源：http://ef.hahajie.cn

TS:   if (!data) return;
来源：http://ho.jctech888.com.cn

Java: if (data == null) return;
来源：http://mo.shxzskj.cn

Go:   if data == nil { return }
来源：http://vh.shxzskj.cn

Ruby: return if data.nil?
来源：http://ts.shxzukj.cn

C#:   if (data == null) return;
来源：http://rw.muxihuayi.cn

================================================================================
来源：http://lf.colortex.cn

C. 函数与作用域
来源：http://la.hahajie.cn

================================================================================
来源：http://hu.huanxung.cn

[C01] 定义函数
来源：http://lk.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://vu.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mi.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://xu.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lz.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ds.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wf.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://yq.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mq.chemitech.net.cn

[C02] 默认参数
来源：http://dj.521024.cn

Py:   def greet(name="World"): return name
来源：http://dc.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://er.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://je.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gz.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bb.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tx.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://td.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://nc.panjiajie.cn

[C03] 可变参数
来源：http://su.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://zv.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ec.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fb.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dz.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ms.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wv.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nl.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pz.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://um.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://on.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fw.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hp.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rr.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://sn.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://gk.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://lb.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://uz.panjiajie.cn

[C05] 返回多个值
来源：http://ui.521024.cn

Py:   return a, b
来源：http://ur.lnxyls.cn

PHP:  return [$a, $b];
来源：http://ud.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ps.hahajie.cn

TS:   return { a, b };
来源：http://nf.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jw.wgjwhj.cn

Go:   return a, b
来源：http://bt.chemitech.net.cn

Ruby: return a, b
来源：http://bd.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://fi.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://io.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://va.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qe.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://be.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://tj.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mv.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://at.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://li.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fn.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://nq.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dj.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vz.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qm.shxzskj.cn

TS:   arr.map(String)
来源：http://aw.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lv.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ci.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://ph.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cu.nicolike.cn

[C08] 闭包
来源：http://gl.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jk.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vq.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wm.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sn.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cr.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yh.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cp.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://if.panjiajie.cn

[C09] 递归
来源：http://pr.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://si.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gz.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vl.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aw.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cv.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dx.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://no.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cw.bjjhwx.cn

[C10] 变量作用域
来源：http://on.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sp.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oy.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bi.haigaiapp.cn

TS:   同 JS
来源：http://sb.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://jy.gzmigu.cn

Go:   花括号块级作用域
来源：http://ss.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oe.hahajie.cn

C#:   块级作用域
来源：http://cq.huixiangedu.cn

[C11] 模块导入与导出
来源：http://fy.asd995.cn

Py:   from module import func
来源：http://id.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kg.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fb.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bm.gzmigu.cn

Java: import java.util.List;
来源：http://fn.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dn.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://so.hnjuh.cn

C#:   using System.Text;
来源：http://kk.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://dj.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://nv.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://fg.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://xq.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://tw.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ws.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://vt.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://hs.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wd.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://nl.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vv.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sf.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dv.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tu.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pg.newstarts.cn

Go:   func add(a, b int) int
来源：http://rs.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wn.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dz.panjiajie.cn

[C14] 泛型函数
来源：http://ly.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qq.asd995.cn

PHP:  // 无泛型
来源：http://us.wgjwhj.cn

JS:   // 无泛型
来源：http://vp.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dz.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://al.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ob.lnxyls.cn

Ruby: # 无泛型
来源：http://ml.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oi.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://ez.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gb.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://dd.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ns.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wb.muxihuayi.cn

Java: // 无解构
来源：http://mo.shxzskj.cn

Go:   // 无解构
来源：http://sz.chemitech.net.cn

Ruby: a, b = pair
来源：http://jp.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://xu.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://ll.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kn.521024.cn

PHP:  // 无重载
来源：http://nb.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mn.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://cb.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rg.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://nz.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://zx.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vs.bookmarksfly.cn

================================================================================
来源：http://ko.asd995.cn

D. 数组 / 列表 / 集合
来源：http://yt.chemitech.net.cn

================================================================================
来源：http://sv.newstarts.cn

[D01] 创建数组 / 列表
来源：http://ii.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hy.huixiangedu.cn


<!-- 参考信息 -->