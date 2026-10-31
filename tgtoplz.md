代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mu.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yv.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rz.szsharing.cn

[B04] for 计数循环
来源：http://tg.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://uz.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://md.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://it.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yw.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ai.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ju.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://ai.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://is.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://ti.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://jz.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vl.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fg.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ve.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wp.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rw.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://ab.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fx.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://pr.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lq.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hc.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yz.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xf.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dd.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://an.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iu.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gb.bookmarksfly.cn

[B07] while 循环
来源：http://xc.nicolike.cn

Py:   while i < 10: i += 1
来源：http://xt.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kh.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://vq.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://sv.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://ou.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ex.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://rd.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://dr.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://rd.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://qi.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cz.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://rw.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://vh.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://fk.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ks.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pe.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://dq.hahajie.cn

[B09] break 与 continue
来源：http://yl.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rf.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yp.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cx.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yu.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qe.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xg.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jp.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pz.huanxung.cn

[B10] 遍历同时拿索引
来源：http://xj.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zg.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://id.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wm.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ip.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qz.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bg.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ej.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://em.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://ii.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://lf.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://oi.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ph.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ca.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://km.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cc.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://hv.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ct.lnxyls.cn

[B12] 跳出多层循环
来源：http://xo.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ke.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nj.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hn.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ao.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://av.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dn.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iz.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tw.gzmigu.cn

[B13] 判断是否为数字
来源：http://zv.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://fy.colortex.cn

PHP:  is_numeric($x)
来源：http://oh.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mb.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rw.colortex.cn

Java: x instanceof Number
来源：http://rq.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xb.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://yn.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://jz.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://gl.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vd.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sb.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://fa.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://hw.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ty.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fn.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ig.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lz.hnjuh.cn

[B15] 布尔运算与取反
来源：http://he.lnxyls.cn

Py:   a and b or not c
来源：http://fh.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://jn.shxzskj.cn

JS:   a && b || !c
来源：http://ee.yuexingan06.cn

TS:   a && b || !c
来源：http://qn.bookmarksfly.cn

Java: a && b || !c
来源：http://mg.hnjuh.cn

Go:   a && b || !c
来源：http://sx.newstarts.cn

Ruby: a && b || !c
来源：http://ig.shtwfgs.cn

C#:   a && b || !c
来源：http://fy.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://be.bjjhwx.cn

Py:   if not data: return
来源：http://tu.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://bc.gzmigu.cn

JS:   if (!data) return;
来源：http://bo.muxihuayi.cn

TS:   if (!data) return;
来源：http://uo.haigaiapp.cn

Java: if (data == null) return;
来源：http://wi.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://si.colortex.cn

Ruby: return if data.nil?
来源：http://sa.yuexingan06.cn

C#:   if (data == null) return;
来源：http://jy.gzmigu.cn

================================================================================
来源：http://sm.colortex.cn

C. 函数与作用域
来源：http://pt.gzmigu.cn

================================================================================
来源：http://xw.nicolike.cn

[C01] 定义函数
来源：http://hq.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://ew.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ul.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://kj.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xl.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ze.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fz.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://zo.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sm.yuntaijiaju.cn

[C02] 默认参数
来源：http://fv.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://pu.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jd.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://za.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://of.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://we.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ep.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://tb.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://vt.9csxet.cn

[C03] 可变参数
来源：http://ft.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://ja.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ib.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hj.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fn.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rh.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yt.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fx.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dt.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://tt.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pb.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cf.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ab.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dt.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://az.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://pu.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://qe.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://qk.nszjky.cn

[C05] 返回多个值
来源：http://mn.szxytkj.cn

Py:   return a, b
来源：http://mq.nicolike.cn

PHP:  return [$a, $b];
来源：http://fx.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lr.gzmigu.cn

TS:   return { a, b };
来源：http://vp.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ya.huanxung.cn

Go:   return a, b
来源：http://ec.muxihuayi.cn

Ruby: return a, b
来源：http://lo.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://ob.521024.cn

[C06] 匿名函数 / lambda
来源：http://kp.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ma.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yi.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://co.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://rw.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fv.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lt.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://hq.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://na.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://tm.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ym.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bx.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ip.huixiangedu.cn

TS:   arr.map(String)
来源：http://bp.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qr.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tp.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://wy.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://je.yuntaijiaju.cn

[C08] 闭包
来源：http://jv.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tb.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rj.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://px.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://za.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jg.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tn.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qv.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xl.asd995.cn

[C09] 递归
来源：http://op.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ff.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vg.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wj.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xf.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ij.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bq.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jg.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xy.haigaiapp.cn

[C10] 变量作用域
来源：http://tf.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ot.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cm.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gp.shtwfgs.cn

TS:   同 JS
来源：http://lh.lnxyls.cn

Java: 方法内为块级作用域
来源：http://da.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://tm.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sx.colortex.cn

C#:   块级作用域
来源：http://uw.shtwfgs.cn

[C11] 模块导入与导出
来源：http://sd.shxzskj.cn

Py:   from module import func
来源：http://cr.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wm.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wz.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dh.jctech888.com.cn

Java: import java.util.List;
来源：http://lg.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ij.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://dh.szxytkj.cn

C#:   using System.Text;
来源：http://by.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://cu.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://em.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://vt.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://rz.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://no.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uk.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://kb.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://oi.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ba.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://cx.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xx.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://up.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://as.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zp.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dw.521024.cn

Go:   func add(a, b int) int
来源：http://sy.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mx.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tw.9csxet.cn

[C14] 泛型函数
来源：http://ui.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uq.chemitech.net.cn

PHP:  // 无泛型
来源：http://vl.yuexingan06.cn

JS:   // 无泛型
来源：http://cx.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lp.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xp.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tv.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://sw.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hl.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://pe.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kk.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://qy.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dz.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gd.huixiangedu.cn

Java: // 无解构
来源：http://ep.lnxyls.cn

Go:   // 无解构
来源：http://dd.hnjuh.cn

Ruby: a, b = pair
来源：http://xk.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://sl.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://va.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sr.colortex.cn

PHP:  // 无重载
来源：http://ax.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ha.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://yy.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zf.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://ec.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://ag.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pn.huixiangedu.cn

================================================================================
来源：http://iv.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://at.yuntaijiaju.cn

================================================================================
来源：http://ia.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://nq.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pf.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ko.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zy.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kk.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tu.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://zm.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://zy.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ii.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://lx.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xo.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kg.nszjky.cn

JS:   arr.push(4);
来源：http://zk.bjjhwx.cn

TS:   arr.push(4);
来源：http://bt.521024.cn

Java: list.add(4);
来源：http://ry.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://tr.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://ek.9csxet.cn

C#:   list.Add(4);
来源：http://dz.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://vm.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://lp.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://un.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ox.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://re.asd995.cn

Java: list.add(0, 0);
来源：http://ic.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hj.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gl.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://tl.szsharing.cn

[D04] 删除元素
来源：http://md.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mt.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kx.chemitech.net.cn


<!-- 参考信息 -->