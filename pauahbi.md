代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nn.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sy.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xf.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://su.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mc.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ew.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yr.huixiangedu.cn

[B04] for 计数循环
来源：http://ox.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://gc.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gs.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qb.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gu.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bc.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dj.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://em.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ic.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://cy.newstarts.cn

Py:   for item in arr: print(item)
来源：http://cr.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zl.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ie.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kx.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fp.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ou.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://bf.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ug.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://vl.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ry.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wy.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oa.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ee.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tv.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ll.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ct.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uq.9csxet.cn

[B07] while 循环
来源：http://lf.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://ng.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vj.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://ke.521024.cn

TS:   while (i < 10) { i++; }
来源：http://ef.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://pz.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sy.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://py.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ms.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://ov.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://qq.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nv.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://pg.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://xe.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://mi.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vu.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bc.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://kc.chemitech.net.cn

[B09] break 与 continue
来源：http://an.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vg.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fo.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nn.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uy.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pr.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fb.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nd.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mw.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://jh.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hb.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eq.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cx.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yc.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bt.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://db.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yi.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ny.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://ra.521024.cn

Py:   list(range(0, 10, 2))
来源：http://sb.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://aw.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vz.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ay.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mp.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ox.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://hb.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fz.wgjwhj.cn

[B12] 跳出多层循环
来源：http://eu.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pd.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://by.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ld.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ai.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://br.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://li.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qx.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zw.yuexingan06.cn

[B13] 判断是否为数字
来源：http://dw.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://vl.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://in.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bw.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dx.wgjwhj.cn

Java: x instanceof Number
来源：http://bz.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lj.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://yb.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://gk.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://fm.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eu.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fy.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://fe.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://he.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://km.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ek.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wr.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zl.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://ym.bjjhwx.cn

Py:   a and b or not c
来源：http://ab.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://jt.huanxung.cn

JS:   a && b || !c
来源：http://lr.nszjky.cn

TS:   a && b || !c
来源：http://ld.gzmigu.cn

Java: a && b || !c
来源：http://iu.521024.cn

Go:   a && b || !c
来源：http://bj.lnxyls.cn

Ruby: a && b || !c
来源：http://nh.jianghongdianzi.cn

C#:   a && b || !c
来源：http://dn.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ni.colortex.cn

Py:   if not data: return
来源：http://po.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://mo.szsharing.cn

JS:   if (!data) return;
来源：http://yj.jctech888.com.cn

TS:   if (!data) return;
来源：http://qt.chemitech.net.cn

Java: if (data == null) return;
来源：http://jy.haigaiapp.cn

Go:   if data == nil { return }
来源：http://ko.gzmigu.cn

Ruby: return if data.nil?
来源：http://jf.wgjwhj.cn

C#:   if (data == null) return;
来源：http://ct.chemitech.net.cn

================================================================================
来源：http://kb.wgjwhj.cn

C. 函数与作用域
来源：http://dj.panjiajie.cn

================================================================================
来源：http://mu.szsharing.cn

[C01] 定义函数
来源：http://aj.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://td.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ph.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://fv.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sk.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pt.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://et.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://xc.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hb.haigaiapp.cn

[C02] 默认参数
来源：http://th.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://of.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ev.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://yc.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sa.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xk.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nj.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://yq.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://le.hnjuh.cn

[C03] 可变参数
来源：http://vk.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://jk.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hf.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pi.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://na.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yw.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dw.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pd.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://so.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://mg.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lm.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ao.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eh.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gs.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://kp.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://us.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://oz.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://dz.nszjky.cn

[C05] 返回多个值
来源：http://sx.shxzskj.cn

Py:   return a, b
来源：http://ut.521024.cn

PHP:  return [$a, $b];
来源：http://is.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cf.haigaiapp.cn

TS:   return { a, b };
来源：http://yd.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sg.yuexingan06.cn

Go:   return a, b
来源：http://yh.hahajie.cn

Ruby: return a, b
来源：http://gh.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://gt.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://wa.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://at.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wg.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://sb.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://fo.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dx.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ir.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://pn.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ni.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://hf.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eh.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fx.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fb.bjjhwx.cn

TS:   arr.map(String)
来源：http://bs.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zr.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yq.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://ke.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://it.wgjwhj.cn

[C08] 闭包
来源：http://kt.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ch.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xr.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ak.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bo.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xe.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zr.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xi.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ee.bookmarksfly.cn

[C09] 递归
来源：http://xn.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nn.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://in.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vn.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bf.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aq.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ot.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fr.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ao.muxihuayi.cn

[C10] 变量作用域
来源：http://tl.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://em.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ng.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cg.newstarts.cn

TS:   同 JS
来源：http://so.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://ja.wgjwhj.cn

Go:   花括号块级作用域
来源：http://dx.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://su.jianghongdianzi.cn

C#:   块级作用域
来源：http://tv.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://jv.hahajie.cn

Py:   from module import func
来源：http://rz.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ap.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tg.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ze.asd995.cn

Java: import java.util.List;
来源：http://fv.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://er.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://lh.9csxet.cn

C#:   using System.Text;
来源：http://uy.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://tu.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://xp.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://uk.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ku.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://ug.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vm.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://jh.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://wz.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://di.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://zm.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aj.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tn.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sb.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zq.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ct.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://tp.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rv.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lr.lnxyls.cn

[C14] 泛型函数
来源：http://lc.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yt.bjjhwx.cn

PHP:  // 无泛型
来源：http://tl.jctech888.com.cn

JS:   // 无泛型
来源：http://de.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vq.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dg.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mi.bookmarksfly.cn

Ruby: # 无泛型
来源：http://jf.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://le.asd995.cn

[C15] 解构 / 展开参数
来源：http://rm.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cq.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://nc.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xs.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qp.newstarts.cn

Java: // 无解构
来源：http://cp.shxzskj.cn

Go:   // 无解构
来源：http://wv.shxzukj.cn

Ruby: a, b = pair
来源：http://aq.colortex.cn

C#:   var (a, b) = pair;
来源：http://bw.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://wr.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yx.shtwfgs.cn

PHP:  // 无重载
来源：http://zv.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yh.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://er.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hf.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://en.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://sy.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xc.huixinmuqiang.cn

================================================================================
来源：http://tt.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://ks.bookmarksfly.cn

================================================================================
来源：http://vu.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://xl.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nc.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vv.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qx.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pp.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qr.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://cj.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://ju.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dr.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://tm.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xq.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sv.nicolike.cn

JS:   arr.push(4);
来源：http://oi.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://uz.huixinmuqiang.cn

Java: list.add(4);
来源：http://zb.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://zx.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://bv.panjiajie.cn

C#:   list.Add(4);
来源：http://hr.newstarts.cn

[D03] 在指定位置插入元素
来源：http://ky.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://ep.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zd.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://de.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://da.lnxyls.cn

Java: list.add(0, 0);
来源：http://dh.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vu.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bz.bookmarksfly.cn


<!-- 参考信息 -->