代发 wailian999

[B05] 遍历数组 / 列表
来源：http://sf.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://mx.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fv.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cy.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ge.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mn.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://by.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://be.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gd.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://sq.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pu.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://on.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zy.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pf.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lf.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ap.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yf.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hw.huixiangedu.cn

[B07] while 循环
来源：http://vv.nszjky.cn

Py:   while i < 10: i += 1
来源：http://kz.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ng.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://br.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://ub.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://bl.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gv.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://qt.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://cx.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://hr.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://xh.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eo.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://mw.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://eb.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://gx.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://um.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kp.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://ha.nszjky.cn

[B09] break 与 continue
来源：http://tj.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uv.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fy.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cv.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rz.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qe.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://od.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ek.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fg.521024.cn

[B10] 遍历同时拿索引
来源：http://bd.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cj.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://al.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fd.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jo.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bo.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pn.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vh.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yw.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://sy.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://sa.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://pj.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://si.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cc.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://on.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://se.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://ud.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pp.asd995.cn

[B12] 跳出多层循环
来源：http://cg.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ag.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rq.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://da.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://of.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ys.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qr.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qw.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://le.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://na.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://jv.gzmigu.cn

PHP:  is_numeric($x)
来源：http://af.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ux.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qj.muxihuayi.cn

Java: x instanceof Number
来源：http://pw.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mo.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://nq.panjiajie.cn

C#:   x is int or double or decimal
来源：http://ni.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://ql.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uj.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qz.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://yy.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://cv.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oh.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ps.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ln.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zv.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://di.szsharing.cn

Py:   a and b or not c
来源：http://fe.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://lo.huixiangedu.cn

JS:   a && b || !c
来源：http://ap.wgjwhj.cn

TS:   a && b || !c
来源：http://wa.huanxung.cn

Java: a && b || !c
来源：http://br.muxihuayi.cn

Go:   a && b || !c
来源：http://wy.gzmigu.cn

Ruby: a && b || !c
来源：http://ro.hnjuh.cn

C#:   a && b || !c
来源：http://pl.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://si.huixinmuqiang.cn

Py:   if not data: return
来源：http://gv.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://aj.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://za.nszjky.cn

TS:   if (!data) return;
来源：http://ld.nszjky.cn

Java: if (data == null) return;
来源：http://yn.huanxung.cn

Go:   if data == nil { return }
来源：http://fi.hnjuh.cn

Ruby: return if data.nil?
来源：http://lr.wgjwhj.cn

C#:   if (data == null) return;
来源：http://gw.asd995.cn

================================================================================
来源：http://eb.9csxet.cn

C. 函数与作用域
来源：http://zo.521024.cn

================================================================================
来源：http://uz.chemitech.net.cn

[C01] 定义函数
来源：http://yi.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://vu.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ao.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://uo.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ak.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pv.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jv.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://pe.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://me.nszjky.cn

[C02] 默认参数
来源：http://al.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://yw.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eg.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://bk.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nz.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vk.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mk.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ze.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://op.hnjuh.cn

[C03] 可变参数
来源：http://ff.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://zu.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hv.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://by.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uv.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iu.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iu.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fo.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gn.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://ju.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oq.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rw.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ms.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uw.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://iv.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://li.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://gy.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://em.bjjhwx.cn

[C05] 返回多个值
来源：http://zt.yuntaijiaju.cn

Py:   return a, b
来源：http://da.lnxyls.cn

PHP:  return [$a, $b];
来源：http://th.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yf.jianghongdianzi.cn

TS:   return { a, b };
来源：http://gl.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wb.asd995.cn

Go:   return a, b
来源：http://ze.colortex.cn

Ruby: return a, b
来源：http://kj.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://iy.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://qv.huanxung.cn

Py:   square = lambda x: x * x
来源：http://cg.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://al.asd995.cn

JS:   const square = x => x * x;
来源：http://hx.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://qm.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rb.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yd.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://uc.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nn.newstarts.cn

[C07] 把函数作为参数传入
来源：http://fk.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uo.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ps.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ps.asd995.cn

TS:   arr.map(String)
来源：http://rr.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sm.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yl.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://hd.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hi.newstarts.cn

[C08] 闭包
来源：http://fm.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iq.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ng.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dd.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rd.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ao.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iy.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bo.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sd.jianghongdianzi.cn

[C09] 递归
来源：http://xx.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bl.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mc.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://li.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vg.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gl.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://im.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ld.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ro.asd995.cn

[C10] 变量作用域
来源：http://ce.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://we.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oy.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lq.lnxyls.cn

TS:   同 JS
来源：http://mv.shxzukj.cn

Java: 方法内为块级作用域
来源：http://px.nicolike.cn

Go:   花括号块级作用域
来源：http://hl.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ht.lnxyls.cn

C#:   块级作用域
来源：http://uc.lnxyls.cn

[C11] 模块导入与导出
来源：http://by.huanxung.cn

Py:   from module import func
来源：http://vj.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qd.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wm.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jp.huixiangedu.cn

Java: import java.util.List;
来源：http://bj.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cu.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://tm.hahajie.cn

C#:   using System.Text;
来源：http://ui.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://ad.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://xy.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://ee.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ip.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://ba.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cw.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://iu.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://yx.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ct.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://ri.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://it.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vp.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tu.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tf.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lk.hahajie.cn

Go:   func add(a, b int) int
来源：http://tr.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uj.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bs.gzmigu.cn

[C14] 泛型函数
来源：http://sw.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nf.jctech888.com.cn

PHP:  // 无泛型
来源：http://gx.hnjuh.cn

JS:   // 无泛型
来源：http://cw.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dv.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ov.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aq.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://oq.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sd.huanxung.cn

[C15] 解构 / 展开参数
来源：http://ve.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ps.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://fh.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uq.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bx.gzmigu.cn

Java: // 无解构
来源：http://xb.nicolike.cn

Go:   // 无解构
来源：http://ts.shxzskj.cn

Ruby: a, b = pair
来源：http://pw.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://mg.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://fg.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ld.hahajie.cn

PHP:  // 无重载
来源：http://rf.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vv.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://hs.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qg.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://fa.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://zg.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://em.lnxyls.cn

================================================================================
来源：http://wd.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://pf.yuexingan06.cn

================================================================================
来源：http://tf.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://mw.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://im.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://po.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ze.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ou.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://il.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://wf.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://ns.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yd.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://sy.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://di.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ah.nszjky.cn

JS:   arr.push(4);
来源：http://an.nicolike.cn

TS:   arr.push(4);
来源：http://kk.gzmigu.cn

Java: list.add(4);
来源：http://sl.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://pu.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://pv.hahajie.cn

C#:   list.Add(4);
来源：http://rh.hahajie.cn

[D03] 在指定位置插入元素
来源：http://qm.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://ie.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pe.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kl.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://ko.muxihuayi.cn

Java: list.add(0, 0);
来源：http://gb.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ff.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oe.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://aj.panjiajie.cn

[D04] 删除元素
来源：http://li.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ix.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kq.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uc.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://nk.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wj.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gq.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fb.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://st.bjjhwx.cn

[D05] 访问与修改元素
来源：http://mv.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kd.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rb.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hb.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://zs.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://qe.yuntaijiaju.cn


<!-- 参考信息 -->