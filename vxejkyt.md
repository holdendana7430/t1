代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://af.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dl.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wc.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://se.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zh.huixiangedu.cn

[B03] switch / match / case
来源：http://qe.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kk.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://of.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://im.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fs.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bs.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uf.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jf.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gp.gzmigu.cn

[B04] for 计数循环
来源：http://wk.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://gn.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ci.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ko.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ev.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eo.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vm.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://su.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cv.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://su.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://dy.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vn.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cx.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://az.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sl.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xa.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://aq.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yg.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://xs.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ty.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bm.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xe.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zi.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mw.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nd.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xr.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uq.shtwfgs.cn

[B07] while 循环
来源：http://ta.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://gc.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zs.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://zh.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://eq.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://nt.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ye.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://zs.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://gq.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://lb.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://hq.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ac.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://dm.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://vq.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://oe.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ti.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hs.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://zs.nicolike.cn

[B09] break 与 continue
来源：http://ww.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ib.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eq.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zj.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qw.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nr.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hy.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://la.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://th.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uo.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fk.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kr.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ns.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wv.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wd.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gp.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jl.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://oq.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://zu.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://nu.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vg.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fz.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pg.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jd.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://aj.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lv.shxzukj.cn

[B12] 跳出多层循环
来源：http://qy.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ms.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tr.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ut.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://st.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bx.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kp.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xg.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fx.shtwfgs.cn

[B13] 判断是否为数字
来源：http://ip.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://qr.panjiajie.cn

PHP:  is_numeric($x)
来源：http://cq.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jl.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xk.colortex.cn

Java: x instanceof Number
来源：http://fh.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pk.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://ti.panjiajie.cn

C#:   x is int or double or decimal
来源：http://et.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://sy.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aw.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mx.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://pj.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://ro.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hm.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://en.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gz.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rj.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://zw.nszjky.cn

Py:   a and b or not c
来源：http://uw.nszjky.cn

PHP:  $a && $b || !$c
来源：http://gm.bjjhwx.cn

JS:   a && b || !c
来源：http://va.asd995.cn

TS:   a && b || !c
来源：http://eu.jianghongdianzi.cn

Java: a && b || !c
来源：http://ga.colortex.cn

Go:   a && b || !c
来源：http://gx.jctech888.com.cn

Ruby: a && b || !c
来源：http://bq.muxihuayi.cn

C#:   a && b || !c
来源：http://ce.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qt.huixiangedu.cn

Py:   if not data: return
来源：http://yl.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://il.wgjwhj.cn

JS:   if (!data) return;
来源：http://gx.bookmarksfly.cn

TS:   if (!data) return;
来源：http://ap.nicolike.cn

Java: if (data == null) return;
来源：http://ft.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://fu.hnjuh.cn

Ruby: return if data.nil?
来源：http://fo.yuexingan06.cn

C#:   if (data == null) return;
来源：http://ov.szsharing.cn

================================================================================
来源：http://bk.gzmigu.cn

C. 函数与作用域
来源：http://rv.shxzskj.cn

================================================================================
来源：http://pr.wgjwhj.cn

[C01] 定义函数
来源：http://cb.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://fk.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://rh.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://no.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zq.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fs.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://uc.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ra.colortex.cn

[C02] 默认参数
来源：http://xa.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://yc.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ck.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ie.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lj.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kl.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ac.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://ki.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://ug.shxzskj.cn

[C03] 可变参数
来源：http://cy.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://ud.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bw.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yl.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qq.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oy.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ur.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lx.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iw.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://ks.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jh.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ut.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mt.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fe.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://xw.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://sn.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://zk.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://oz.bjjhwx.cn

[C05] 返回多个值
来源：http://ex.colortex.cn

Py:   return a, b
来源：http://be.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://nr.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mp.bjjhwx.cn

TS:   return { a, b };
来源：http://gd.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ey.panjiajie.cn

Go:   return a, b
来源：http://bu.yuexingan06.cn

Ruby: return a, b
来源：http://ly.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://kc.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://ss.nicolike.cn

Py:   square = lambda x: x * x
来源：http://hg.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://le.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://oo.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://nz.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fr.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xq.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://pe.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pz.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://ce.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ft.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nl.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://po.asd995.cn

TS:   arr.map(String)
来源：http://ye.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cn.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zk.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://li.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uk.muxihuayi.cn

[C08] 闭包
来源：http://ek.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ny.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lh.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bs.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cz.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gi.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oc.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ir.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xn.muxihuayi.cn

[C09] 递归
来源：http://no.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hq.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://up.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nn.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ad.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://us.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hg.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wp.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tz.hahajie.cn

[C10] 变量作用域
来源：http://ev.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rn.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zz.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ps.huixinmuqiang.cn

TS:   同 JS
来源：http://du.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://ga.huanxung.cn

Go:   花括号块级作用域
来源：http://ps.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ae.hahajie.cn

C#:   块级作用域
来源：http://kh.huixiangedu.cn

[C11] 模块导入与导出
来源：http://ta.szxytkj.cn

Py:   from module import func
来源：http://yr.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ew.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qp.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jz.shtwfgs.cn

Java: import java.util.List;
来源：http://mn.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wm.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://el.shtwfgs.cn

C#:   using System.Text;
来源：http://fp.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://vg.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://zx.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://ff.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://lu.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://fg.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bq.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://hz.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://vg.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bx.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://cx.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://or.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jm.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ee.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wf.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vm.asd995.cn

Go:   func add(a, b int) int
来源：http://pc.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hi.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fw.bjjhwx.cn

[C14] 泛型函数
来源：http://ak.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gh.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://il.yuntaijiaju.cn

JS:   // 无泛型
来源：http://rw.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hm.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wg.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xl.huixiangedu.cn

Ruby: # 无泛型
来源：http://dp.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lo.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://qj.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xo.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://kb.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vd.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://le.lnxyls.cn

Java: // 无解构
来源：http://js.nicolike.cn

Go:   // 无解构
来源：http://kz.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://ia.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://tz.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://pf.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eg.521024.cn

PHP:  // 无重载
来源：http://ze.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://go.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://vs.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jo.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://il.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://yu.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zq.szsharing.cn

================================================================================
来源：http://oh.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://ls.szxytkj.cn

================================================================================
来源：http://ze.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://wq.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rv.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://np.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yd.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jn.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pq.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://sv.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://ms.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tt.huanxung.cn

[D02] 追加元素到末尾
来源：http://sb.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oq.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gw.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://wk.bjjhwx.cn

TS:   arr.push(4);
来源：http://dw.hnjuh.cn

Java: list.add(4);
来源：http://aw.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://bu.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://nl.nszjky.cn

C#:   list.Add(4);
来源：http://ho.newstarts.cn


<!-- 参考信息 -->