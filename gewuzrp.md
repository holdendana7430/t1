代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cb.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nv.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ia.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jg.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://me.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://fa.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zm.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sa.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mu.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yt.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://za.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://us.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rk.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://td.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nr.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ey.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ts.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ty.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yj.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zb.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qx.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dg.bookmarksfly.cn

[B07] while 循环
来源：http://bd.9csxet.cn

Py:   while i < 10: i += 1
来源：http://ut.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dq.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://lw.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://sk.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://ch.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wg.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://ah.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://ap.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://yv.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://ml.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sr.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://iu.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://hv.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://xy.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ha.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gl.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://lf.521024.cn

[B09] break 与 continue
来源：http://da.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kl.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cy.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tx.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hs.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ix.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gb.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ja.521024.cn

[B10] 遍历同时拿索引
来源：http://lx.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lp.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dn.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jl.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ga.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ft.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ky.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kj.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://md.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://ew.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://ll.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://tm.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://al.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xh.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kj.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ru.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://yz.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qz.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ff.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ni.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rz.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zy.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lh.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hk.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aj.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bc.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nr.nicolike.cn

[B13] 判断是否为数字
来源：http://ee.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://hl.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://yx.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ja.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tq.yuntaijiaju.cn

Java: x instanceof Number
来源：http://cz.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://if.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://rw.nszjky.cn

C#:   x is int or double or decimal
来源：http://tl.hahajie.cn

[B14] 判断值是否在集合内
来源：http://sr.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://je.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ir.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://zi.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://lq.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fi.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tj.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ji.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yi.huanxung.cn

[B15] 布尔运算与取反
来源：http://aj.huixinmuqiang.cn

Py:   a and b or not c
来源：http://hx.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://me.521024.cn

JS:   a && b || !c
来源：http://in.jianghongdianzi.cn

TS:   a && b || !c
来源：http://sf.haigaiapp.cn

Java: a && b || !c
来源：http://bu.nszjky.cn

Go:   a && b || !c
来源：http://kl.szsharing.cn

Ruby: a && b || !c
来源：http://ry.shxzukj.cn

C#:   a && b || !c
来源：http://pm.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mk.szxytkj.cn

Py:   if not data: return
来源：http://lh.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://cx.hnjuh.cn

JS:   if (!data) return;
来源：http://hh.nicolike.cn

TS:   if (!data) return;
来源：http://hj.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://xy.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://wn.huixiangedu.cn

Ruby: return if data.nil?
来源：http://wu.huanxung.cn

C#:   if (data == null) return;
来源：http://al.bookmarksfly.cn

================================================================================
来源：http://yd.jctech888.com.cn

C. 函数与作用域
来源：http://lh.szsharing.cn

================================================================================
来源：http://sx.panjiajie.cn

[C01] 定义函数
来源：http://kv.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://mx.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fk.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://tt.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://du.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wk.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qc.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://my.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hd.panjiajie.cn

[C02] 默认参数
来源：http://dk.asd995.cn

Py:   def greet(name="World"): return name
来源：http://df.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uv.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://ei.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xk.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vm.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qt.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://ji.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://my.wgjwhj.cn

[C03] 可变参数
来源：http://pn.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://vu.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hw.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ug.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ca.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iv.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ar.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hd.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gp.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://tx.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uw.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sk.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zn.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oe.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://gm.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://xg.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://pp.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://kk.colortex.cn

[C05] 返回多个值
来源：http://kj.chemitech.net.cn

Py:   return a, b
来源：http://bk.shxzukj.cn

PHP:  return [$a, $b];
来源：http://em.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tr.asd995.cn

TS:   return { a, b };
来源：http://bc.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tt.huanxung.cn

Go:   return a, b
来源：http://zt.521024.cn

Ruby: return a, b
来源：http://yo.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://bj.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://aj.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ep.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qa.nicolike.cn

JS:   const square = x => x * x;
来源：http://ao.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://gg.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cq.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xx.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://ur.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gd.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://cg.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dh.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://re.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uj.wgjwhj.cn

TS:   arr.map(String)
来源：http://aj.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ue.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yb.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://zi.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wb.wgjwhj.cn

[C08] 闭包
来源：http://sx.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ba.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ax.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://er.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yo.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pe.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pj.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tr.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nd.bookmarksfly.cn

[C09] 递归
来源：http://mk.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kf.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dx.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ty.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jt.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dz.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://in.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dd.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ay.huixiangedu.cn

[C10] 变量作用域
来源：http://cc.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gy.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nw.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wb.huanxung.cn

TS:   同 JS
来源：http://yg.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://zd.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://lp.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tc.bjjhwx.cn

C#:   块级作用域
来源：http://cw.szxytkj.cn

[C11] 模块导入与导出
来源：http://da.colortex.cn

Py:   from module import func
来源：http://dl.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lc.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cv.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ml.szxytkj.cn

Java: import java.util.List;
来源：http://gc.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zr.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://ik.szsharing.cn

C#:   using System.Text;
来源：http://nr.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://tr.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://gg.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://bj.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://df.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ex.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qt.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://ah.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://je.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gm.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://hk.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vo.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hi.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hg.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gw.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://km.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://yu.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zj.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xi.chemitech.net.cn

[C14] 泛型函数
来源：http://ra.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nl.panjiajie.cn

PHP:  // 无泛型
来源：http://do.huanxung.cn

JS:   // 无泛型
来源：http://nf.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jl.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ck.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://em.bookmarksfly.cn

Ruby: # 无泛型
来源：http://ok.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lb.nicolike.cn

[C15] 解构 / 展开参数
来源：http://rs.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ju.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://qe.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://un.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aj.jctech888.com.cn

Java: // 无解构
来源：http://jp.yuntaijiaju.cn

Go:   // 无解构
来源：http://lx.panjiajie.cn

Ruby: a, b = pair
来源：http://aa.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://uw.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://tl.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bn.szxytkj.cn

PHP:  // 无重载
来源：http://ua.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zp.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://mt.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fl.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://rx.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://dm.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nk.colortex.cn

================================================================================
来源：http://gc.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://kj.colortex.cn

================================================================================
来源：http://yz.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://tb.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mz.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://od.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dx.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dr.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rh.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://cd.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://ih.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://so.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://ye.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://is.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cy.9csxet.cn

JS:   arr.push(4);
来源：http://ws.yuexingan06.cn

TS:   arr.push(4);
来源：http://iq.panjiajie.cn

Java: list.add(4);
来源：http://xy.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://ux.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://il.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://sm.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://bb.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://hl.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hp.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://si.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://rh.shxzskj.cn

Java: list.add(0, 0);
来源：http://tp.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xe.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://js.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://tt.yuntaijiaju.cn

[D04] 删除元素
来源：http://mq.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tx.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yv.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tg.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://uu.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bc.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ks.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tr.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ga.yuexingan06.cn

[D05] 访问与修改元素
来源：http://tc.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jx.nszjky.cn


<!-- 参考信息 -->