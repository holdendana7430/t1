代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ks.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kj.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ut.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oq.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ic.haigaiapp.cn

[B03] switch / match / case
来源：http://pj.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ai.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yv.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ti.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hh.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qx.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oj.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dk.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pf.shtwfgs.cn

[B04] for 计数循环
来源：http://zs.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://pm.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ke.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zu.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://co.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ra.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ma.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://zs.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zf.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://vs.huanxung.cn

Py:   for item in arr: print(item)
来源：http://nw.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bn.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mj.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xf.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://my.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fx.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://er.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fa.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://nx.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rs.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bj.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cp.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vw.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tr.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oz.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://al.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pg.shxzskj.cn

[B07] while 循环
来源：http://ve.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://cr.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rh.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://rg.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://tw.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://rk.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rb.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://pn.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://dl.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://ul.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://ny.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oy.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://pn.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://ik.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://kd.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://do.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tq.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://by.newstarts.cn

[B09] break 与 continue
来源：http://rg.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oa.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ms.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qc.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ez.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dg.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gj.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bb.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://jl.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ff.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vn.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://li.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://me.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://td.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wr.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bf.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vz.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://lb.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ao.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://dt.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://he.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://go.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gj.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qi.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://ry.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://em.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://tm.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xw.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gd.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rg.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pz.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://up.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zj.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kv.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nd.chemitech.net.cn

[B13] 判断是否为数字
来源：http://gm.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://qz.gzmigu.cn

PHP:  is_numeric($x)
来源：http://ed.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mf.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ha.colortex.cn

Java: x instanceof Number
来源：http://qf.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ta.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://dx.nicolike.cn

C#:   x is int or double or decimal
来源：http://du.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://qq.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ry.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://us.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ed.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://ij.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gh.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qh.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qr.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ap.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://oh.asd995.cn

Py:   a and b or not c
来源：http://ua.huanxung.cn

PHP:  $a && $b || !$c
来源：http://dm.lnxyls.cn

JS:   a && b || !c
来源：http://ho.haigaiapp.cn

TS:   a && b || !c
来源：http://kf.9csxet.cn

Java: a && b || !c
来源：http://fz.yuexingan06.cn

Go:   a && b || !c
来源：http://zd.shtwfgs.cn

Ruby: a && b || !c
来源：http://yr.shtwfgs.cn

C#:   a && b || !c
来源：http://oc.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yv.haigaiapp.cn

Py:   if not data: return
来源：http://is.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://ra.nicolike.cn

JS:   if (!data) return;
来源：http://mo.yuexingan06.cn

TS:   if (!data) return;
来源：http://rm.bookmarksfly.cn

Java: if (data == null) return;
来源：http://hl.chemitech.net.cn

Go:   if data == nil { return }
来源：http://mf.huixiangedu.cn

Ruby: return if data.nil?
来源：http://fd.muxihuayi.cn

C#:   if (data == null) return;
来源：http://ex.shxzskj.cn

================================================================================
来源：http://fl.newstarts.cn

C. 函数与作用域
来源：http://kg.lnxyls.cn

================================================================================
来源：http://lj.nszjky.cn

[C01] 定义函数
来源：http://hg.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://ww.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://za.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://fc.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wj.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wx.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dv.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://ae.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fc.muxihuayi.cn

[C02] 默认参数
来源：http://pp.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://eq.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pf.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://nv.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rr.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vj.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kx.521024.cn

Ruby: def greet(name = "World") = name
来源：http://go.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://og.shxzskj.cn

[C03] 可变参数
来源：http://pj.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://om.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fu.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xu.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hd.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aa.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zn.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sm.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hh.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://fq.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lu.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ac.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cf.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uh.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://uo.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://gw.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://iu.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://nm.shtwfgs.cn

[C05] 返回多个值
来源：http://tg.bookmarksfly.cn

Py:   return a, b
来源：http://ne.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://jp.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://to.huixinmuqiang.cn

TS:   return { a, b };
来源：http://bd.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oz.huanxung.cn

Go:   return a, b
来源：http://rs.bookmarksfly.cn

Ruby: return a, b
来源：http://ia.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://tx.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://vx.nicolike.cn

Py:   square = lambda x: x * x
来源：http://dx.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rk.lnxyls.cn

JS:   const square = x => x * x;
来源：http://vr.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://wt.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gb.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xl.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://rs.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jd.colortex.cn

[C07] 把函数作为参数传入
来源：http://lp.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ek.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hk.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://js.jctech888.com.cn

TS:   arr.map(String)
来源：http://sf.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yr.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://is.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://qc.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nd.jianghongdianzi.cn

[C08] 闭包
来源：http://zp.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xu.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xv.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pm.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fx.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wf.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qi.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://st.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xz.panjiajie.cn

[C09] 递归
来源：http://ut.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oj.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kj.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jt.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xd.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ij.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iy.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hl.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ir.szxytkj.cn

[C10] 变量作用域
来源：http://ze.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://so.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wy.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://if.huanxung.cn

TS:   同 JS
来源：http://dq.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://dy.521024.cn

Go:   花括号块级作用域
来源：http://rz.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fy.nszjky.cn

C#:   块级作用域
来源：http://yo.lnxyls.cn

[C11] 模块导入与导出
来源：http://yv.chemitech.net.cn

Py:   from module import func
来源：http://lj.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://md.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jy.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jt.jctech888.com.cn

Java: import java.util.List;
来源：http://fz.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hp.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://nv.nicolike.cn

C#:   using System.Text;
来源：http://wm.521024.cn

[C12] 立即执行函数 IIFE
来源：http://go.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://dy.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://wl.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://hf.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://ul.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nl.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://mv.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://ro.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vl.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://rv.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ym.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hl.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sb.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lk.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sf.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://mx.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wl.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wc.bookmarksfly.cn

[C14] 泛型函数
来源：http://ke.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vp.gzmigu.cn

PHP:  // 无泛型
来源：http://um.bookmarksfly.cn

JS:   // 无泛型
来源：http://sm.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hx.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dv.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hm.muxihuayi.cn

Ruby: # 无泛型
来源：http://xj.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qv.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://bu.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hy.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://es.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ml.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tv.huixinmuqiang.cn

Java: // 无解构
来源：http://he.huanxung.cn

Go:   // 无解构
来源：http://vg.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://ut.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://gx.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://jp.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oo.nszjky.cn

PHP:  // 无重载
来源：http://mf.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wr.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://mq.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xp.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://il.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://zq.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uq.yuexingan06.cn

================================================================================
来源：http://ag.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://lq.asd995.cn

================================================================================
来源：http://ng.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://ly.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ss.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ek.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://co.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yw.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ak.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://tp.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://tu.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ek.huanxung.cn

[D02] 追加元素到末尾
来源：http://nh.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hn.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vy.521024.cn

JS:   arr.push(4);
来源：http://vt.asd995.cn

TS:   arr.push(4);
来源：http://vp.bookmarksfly.cn

Java: list.add(4);
来源：http://sg.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://kz.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://kc.szsharing.cn

C#:   list.Add(4);
来源：http://th.shxzskj.cn


<!-- 参考信息 -->