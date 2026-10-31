代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pe.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rb.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qv.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://up.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lh.521024.cn

[B02] 多分支 else if / elif
来源：http://su.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cs.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lq.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nk.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bn.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gs.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://el.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cn.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.shtwfgs.cn

[B03] switch / match / case
来源：http://xb.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hx.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tr.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://th.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ni.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ub.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xh.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mr.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://em.chemitech.net.cn

[B04] for 计数循环
来源：http://wp.521024.cn

Py:   for i in range(10): print(i)
来源：http://ss.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yg.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jp.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nj.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://po.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ec.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ii.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wd.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://ji.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://yz.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rq.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oa.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kb.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ci.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gn.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://eo.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kp.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://fm.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sw.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wj.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wp.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vw.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jt.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wt.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jr.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ng.nicolike.cn

[B07] while 循环
来源：http://tz.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://ke.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fb.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://ma.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://gc.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://mm.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dd.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://gd.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://gr.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://xp.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://pp.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ue.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://xq.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://gl.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://fx.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sp.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wu.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://my.szxytkj.cn

[B09] break 与 continue
来源：http://af.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nx.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cf.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kc.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yx.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zi.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fg.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mi.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ny.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://os.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hk.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fo.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dd.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nf.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sh.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lr.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://af.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://la.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://xq.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://io.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://vw.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ge.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wx.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sb.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ss.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://cg.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xs.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://od.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gz.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lf.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dz.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yi.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mt.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kv.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ju.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://do.panjiajie.cn

[B13] 判断是否为数字
来源：http://gl.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://zi.521024.cn

PHP:  is_numeric($x)
来源：http://jz.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dv.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ta.gzmigu.cn

Java: x instanceof Number
来源：http://ny.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kp.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://zr.shxzukj.cn

C#:   x is int or double or decimal
来源：http://cq.asd995.cn

[B14] 判断值是否在集合内
来源：http://gd.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ep.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ih.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://sm.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://fu.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sh.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rn.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oy.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://se.hahajie.cn

[B15] 布尔运算与取反
来源：http://as.yuntaijiaju.cn

Py:   a and b or not c
来源：http://fl.huanxung.cn

PHP:  $a && $b || !$c
来源：http://kt.lnxyls.cn

JS:   a && b || !c
来源：http://ep.chemitech.net.cn

TS:   a && b || !c
来源：http://me.szxytkj.cn

Java: a && b || !c
来源：http://wm.huanxung.cn

Go:   a && b || !c
来源：http://gw.haigaiapp.cn

Ruby: a && b || !c
来源：http://fm.newstarts.cn

C#:   a && b || !c
来源：http://lr.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wd.521024.cn

Py:   if not data: return
来源：http://gp.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://ve.9csxet.cn

JS:   if (!data) return;
来源：http://kh.shxzskj.cn

TS:   if (!data) return;
来源：http://lg.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://sa.chemitech.net.cn

Go:   if data == nil { return }
来源：http://fg.shtwfgs.cn

Ruby: return if data.nil?
来源：http://dv.yuexingan06.cn

C#:   if (data == null) return;
来源：http://pw.huixinmuqiang.cn

================================================================================
来源：http://uj.lnxyls.cn

C. 函数与作用域
来源：http://ls.huixinmuqiang.cn

================================================================================
来源：http://tp.nszjky.cn

[C01] 定义函数
来源：http://yn.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ys.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sg.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://ts.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ar.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ct.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vp.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://vg.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wv.yuexingan06.cn

[C02] 默认参数
来源：http://jn.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://dz.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mb.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://gr.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rg.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cr.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cw.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://tf.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://it.bjjhwx.cn

[C03] 可变参数
来源：http://iv.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://st.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yn.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ya.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hn.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yl.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qg.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ah.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ai.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://fx.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dp.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kl.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://li.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dh.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://to.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://ls.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://vb.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://iu.panjiajie.cn

[C05] 返回多个值
来源：http://ij.521024.cn

Py:   return a, b
来源：http://bt.nszjky.cn

PHP:  return [$a, $b];
来源：http://lu.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vf.hahajie.cn

TS:   return { a, b };
来源：http://mp.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eu.jctech888.com.cn

Go:   return a, b
来源：http://ep.9csxet.cn

Ruby: return a, b
来源：http://gn.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://kx.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://jn.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://dy.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://as.nszjky.cn

JS:   const square = x => x * x;
来源：http://is.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://xk.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hq.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ai.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://sz.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://go.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://ir.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jo.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vp.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vm.yuexingan06.cn

TS:   arr.map(String)
来源：http://ou.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ct.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mn.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://qp.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ss.colortex.cn

[C08] 闭包
来源：http://oe.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iu.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sq.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://al.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jc.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vw.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fm.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sb.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pq.szsharing.cn

[C09] 递归
来源：http://ea.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mi.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qi.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://un.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cg.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sg.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://js.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ug.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hm.bjjhwx.cn

[C10] 变量作用域
来源：http://gs.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cu.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jn.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hk.nszjky.cn

TS:   同 JS
来源：http://sf.shxzukj.cn

Java: 方法内为块级作用域
来源：http://uq.shtwfgs.cn

Go:   花括号块级作用域
来源：http://gy.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://is.jctech888.com.cn

C#:   块级作用域
来源：http://fg.szsharing.cn

[C11] 模块导入与导出
来源：http://up.shxzukj.cn

Py:   from module import func
来源：http://bh.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vb.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://su.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ze.shxzskj.cn

Java: import java.util.List;
来源：http://sl.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xm.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://ze.shtwfgs.cn

C#:   using System.Text;
来源：http://kd.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://cz.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://sy.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://sd.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://yz.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://tp.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mz.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://fn.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://pl.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://is.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://tj.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bp.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pi.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lu.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yq.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sq.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://em.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sm.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qk.nicolike.cn

[C14] 泛型函数
来源：http://rx.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dy.panjiajie.cn

PHP:  // 无泛型
来源：http://ih.521024.cn

JS:   // 无泛型
来源：http://cr.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ji.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sg.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pv.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://un.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gl.colortex.cn

[C15] 解构 / 展开参数
来源：http://fq.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ra.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://wd.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bv.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ps.bjjhwx.cn

Java: // 无解构
来源：http://ib.jctech888.com.cn

Go:   // 无解构
来源：http://ak.haigaiapp.cn

Ruby: a, b = pair
来源：http://qy.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://tj.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://fi.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mm.asd995.cn

PHP:  // 无重载
来源：http://md.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tg.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://rx.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rx.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://aw.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://ci.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hb.shxzskj.cn

================================================================================
来源：http://my.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://dn.bookmarksfly.cn

================================================================================
来源：http://qr.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://gp.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pc.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rh.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ag.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wg.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ml.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://mi.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://jo.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xb.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://sa.wgjwhj.cn


<!-- 参考信息 -->