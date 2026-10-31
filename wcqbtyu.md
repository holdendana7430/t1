代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bx.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://oy.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lc.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://op.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ms.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ap.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jd.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uh.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hj.colortex.cn

[B03] switch / match / case
来源：http://vy.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eg.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sa.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yo.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pd.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wq.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hw.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ka.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gv.szxytkj.cn

[B04] for 计数循环
来源：http://iq.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://sz.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qx.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mr.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tg.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gb.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rw.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://af.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dk.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://zi.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://lv.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tw.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wf.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yz.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uu.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://my.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://bd.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nl.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://fg.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fb.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bt.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qt.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sg.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yk.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mg.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vr.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://am.bookmarksfly.cn

[B07] while 循环
来源：http://fx.asd995.cn

Py:   while i < 10: i += 1
来源：http://yg.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://no.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://my.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://oe.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://al.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eb.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://le.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://aq.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://fd.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://cz.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://we.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://ai.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://ux.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://nf.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lt.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zo.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://ik.huixiangedu.cn

[B09] break 与 continue
来源：http://vp.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vj.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ha.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://he.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oy.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fg.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gp.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://la.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rf.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://qf.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lf.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rq.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gh.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jc.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://af.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hi.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rr.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yv.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://td.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://by.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://ij.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ac.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ru.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ng.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ld.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://jv.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ul.gzmigu.cn

[B12] 跳出多层循环
来源：http://ls.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kd.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://az.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kk.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ru.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ib.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://va.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mn.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nd.hahajie.cn

[B13] 判断是否为数字
来源：http://eo.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://gz.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://mp.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sy.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hh.wgjwhj.cn

Java: x instanceof Number
来源：http://yc.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fv.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://hb.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://xk.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://dj.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fb.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xu.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://lq.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://dc.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://da.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kn.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ao.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ha.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://ns.shxzskj.cn

Py:   a and b or not c
来源：http://da.nszjky.cn

PHP:  $a && $b || !$c
来源：http://mg.9csxet.cn

JS:   a && b || !c
来源：http://ot.9csxet.cn

TS:   a && b || !c
来源：http://mr.asd995.cn

Java: a && b || !c
来源：http://nx.shxzskj.cn

Go:   a && b || !c
来源：http://mg.lnxyls.cn

Ruby: a && b || !c
来源：http://yp.nszjky.cn

C#:   a && b || !c
来源：http://oh.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ef.521024.cn

Py:   if not data: return
来源：http://dr.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://mm.9csxet.cn

JS:   if (!data) return;
来源：http://yk.szxytkj.cn

TS:   if (!data) return;
来源：http://dp.lnxyls.cn

Java: if (data == null) return;
来源：http://fo.gzmigu.cn

Go:   if data == nil { return }
来源：http://sz.521024.cn

Ruby: return if data.nil?
来源：http://rw.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://im.hahajie.cn

================================================================================
来源：http://lz.jianghongdianzi.cn

C. 函数与作用域
来源：http://yz.szsharing.cn

================================================================================
来源：http://is.szsharing.cn

[C01] 定义函数
来源：http://qh.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://fu.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ad.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ez.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bv.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dt.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tk.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://op.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rt.9csxet.cn

[C02] 默认参数
来源：http://ak.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://fk.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nl.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://io.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ns.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iy.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://re.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://tp.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://so.hnjuh.cn

[C03] 可变参数
来源：http://dv.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://zu.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ih.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pa.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://om.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wr.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ni.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://je.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://la.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://mp.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ki.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ya.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kb.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dc.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://ax.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://uj.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://uz.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://bb.wgjwhj.cn

[C05] 返回多个值
来源：http://nz.colortex.cn

Py:   return a, b
来源：http://xm.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://yx.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fd.wgjwhj.cn

TS:   return { a, b };
来源：http://sf.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oe.gzmigu.cn

Go:   return a, b
来源：http://ld.wgjwhj.cn

Ruby: return a, b
来源：http://ul.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://zu.asd995.cn

[C06] 匿名函数 / lambda
来源：http://zm.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://fe.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://po.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://zf.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://kh.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vs.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jb.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://tm.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sr.huanxung.cn

[C07] 把函数作为参数传入
来源：http://uw.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://go.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://es.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xa.521024.cn

TS:   arr.map(String)
来源：http://io.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://le.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gg.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://hu.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ew.newstarts.cn

[C08] 闭包
来源：http://tg.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mo.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vs.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ia.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rg.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xe.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bf.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mr.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ni.shxzukj.cn

[C09] 递归
来源：http://qc.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fq.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tn.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xv.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ge.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ye.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sp.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fx.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ba.muxihuayi.cn

[C10] 变量作用域
来源：http://ht.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://an.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nv.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qb.szsharing.cn

TS:   同 JS
来源：http://ka.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://qn.jctech888.com.cn

Go:   花括号块级作用域
来源：http://qh.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wg.yuexingan06.cn

C#:   块级作用域
来源：http://za.jctech888.com.cn

[C11] 模块导入与导出
来源：http://pn.yuntaijiaju.cn

Py:   from module import func
来源：http://sc.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://us.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wo.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://us.chemitech.net.cn

Java: import java.util.List;
来源：http://gy.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lr.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://un.huanxung.cn

C#:   using System.Text;
来源：http://zo.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://hb.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://ix.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ee.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://jm.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://yo.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rz.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://wk.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://gr.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pa.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://sf.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iy.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fg.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zg.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dv.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ef.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://ay.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nh.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dn.hahajie.cn

[C14] 泛型函数
来源：http://nm.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://or.panjiajie.cn

PHP:  // 无泛型
来源：http://ts.lnxyls.cn

JS:   // 无泛型
来源：http://jw.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kj.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xg.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hl.shxzukj.cn

Ruby: # 无泛型
来源：http://gi.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nq.szsharing.cn

[C15] 解构 / 展开参数
来源：http://uw.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ov.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://rj.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jy.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uy.panjiajie.cn

Java: // 无解构
来源：http://ro.shtwfgs.cn

Go:   // 无解构
来源：http://hb.hnjuh.cn

Ruby: a, b = pair
来源：http://nn.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://iw.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://ys.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tf.muxihuayi.cn

PHP:  // 无重载
来源：http://yb.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zk.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://kz.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mv.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://ka.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://go.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xt.yuexingan06.cn

================================================================================
来源：http://wz.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://jd.yuexingan06.cn

================================================================================
来源：http://pb.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://bv.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bk.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nk.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ji.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rq.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uj.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://nz.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://nu.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dh.panjiajie.cn

[D02] 追加元素到末尾
来源：http://wl.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eu.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jf.shtwfgs.cn

JS:   arr.push(4);
来源：http://ay.shxzukj.cn

TS:   arr.push(4);
来源：http://ls.panjiajie.cn


<!-- 参考信息 -->