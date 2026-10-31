代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gr.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ga.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://xi.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nd.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://ju.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://um.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ei.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uk.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ip.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://en.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yn.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://ro.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dz.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://ee.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mz.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jt.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yq.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oh.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hj.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://db.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eb.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iu.9csxet.cn

[B07] while 循环
来源：http://ps.nszjky.cn

Py:   while i < 10: i += 1
来源：http://nw.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tz.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://rv.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://ue.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://aq.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dl.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://fl.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://hn.521024.cn

[B08] do-while（至少执行一次）
来源：http://ub.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://aa.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vg.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://ss.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://vx.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://on.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wu.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mi.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://oo.nszjky.cn

[B09] break 与 continue
来源：http://lw.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://by.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yp.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ds.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mm.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ys.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pz.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://la.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aq.newstarts.cn

[B10] 遍历同时拿索引
来源：http://nq.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://po.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xw.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ul.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tl.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://re.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tx.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nw.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oq.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://qx.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://ft.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://lg.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sg.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vj.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sn.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tm.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://bh.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tq.hahajie.cn

[B12] 跳出多层循环
来源：http://zs.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fq.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nl.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uz.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jp.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mm.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vg.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vp.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cn.huanxung.cn

[B13] 判断是否为数字
来源：http://ui.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://xf.gzmigu.cn

PHP:  is_numeric($x)
来源：http://aj.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rr.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wu.521024.cn

Java: x instanceof Number
来源：http://ba.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://md.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://xu.szsharing.cn

C#:   x is int or double or decimal
来源：http://lm.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://ue.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zb.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iq.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://hr.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://lz.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mk.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://el.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vd.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rm.hnjuh.cn

[B15] 布尔运算与取反
来源：http://vr.shxzukj.cn

Py:   a and b or not c
来源：http://di.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://fq.lnxyls.cn

JS:   a && b || !c
来源：http://mt.asd995.cn

TS:   a && b || !c
来源：http://nv.huixinmuqiang.cn

Java: a && b || !c
来源：http://wo.huixiangedu.cn

Go:   a && b || !c
来源：http://nf.huixiangedu.cn

Ruby: a && b || !c
来源：http://jn.lnxyls.cn

C#:   a && b || !c
来源：http://mr.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://af.colortex.cn

Py:   if not data: return
来源：http://rm.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://ve.colortex.cn

JS:   if (!data) return;
来源：http://fz.nicolike.cn

TS:   if (!data) return;
来源：http://pb.szxytkj.cn

Java: if (data == null) return;
来源：http://ft.yuexingan06.cn

Go:   if data == nil { return }
来源：http://fi.asd995.cn

Ruby: return if data.nil?
来源：http://qb.nszjky.cn

C#:   if (data == null) return;
来源：http://ru.521024.cn

================================================================================
来源：http://nn.bookmarksfly.cn

C. 函数与作用域
来源：http://tj.9csxet.cn

================================================================================
来源：http://oq.huixiangedu.cn

[C01] 定义函数
来源：http://wz.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://gy.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ft.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://nw.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hr.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ty.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hk.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://bt.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rp.yuexingan06.cn

[C02] 默认参数
来源：http://ej.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://li.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://em.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://sy.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wp.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wx.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lb.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://hb.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ql.9csxet.cn

[C03] 可变参数
来源：http://bo.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://tu.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nc.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cg.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fd.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bj.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zb.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yh.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bv.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://oz.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xl.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lk.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zi.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://db.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://ih.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://ww.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://sg.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://co.jctech888.com.cn

[C05] 返回多个值
来源：http://tr.muxihuayi.cn

Py:   return a, b
来源：http://wm.lnxyls.cn

PHP:  return [$a, $b];
来源：http://nl.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iu.jianghongdianzi.cn

TS:   return { a, b };
来源：http://ug.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://av.yuntaijiaju.cn

Go:   return a, b
来源：http://xv.lnxyls.cn

Ruby: return a, b
来源：http://jj.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://jt.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://qi.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://qu.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sp.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://tq.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://yr.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ti.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ti.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://wa.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iu.szsharing.cn

[C07] 把函数作为参数传入
来源：http://in.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ks.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nh.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gb.nicolike.cn

TS:   arr.map(String)
来源：http://ij.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://at.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://it.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://td.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fx.shxzskj.cn

[C08] 闭包
来源：http://jp.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qx.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wu.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yh.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ak.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://se.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nh.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://my.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sg.hnjuh.cn

[C09] 递归
来源：http://so.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mp.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ul.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jz.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wm.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ck.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bm.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ed.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kb.hnjuh.cn

[C10] 变量作用域
来源：http://bi.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ea.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jj.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yn.huanxung.cn

TS:   同 JS
来源：http://cs.colortex.cn

Java: 方法内为块级作用域
来源：http://nz.haigaiapp.cn

Go:   花括号块级作用域
来源：http://yj.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fa.nszjky.cn

C#:   块级作用域
来源：http://tw.hnjuh.cn

[C11] 模块导入与导出
来源：http://oz.9csxet.cn

Py:   from module import func
来源：http://oh.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ie.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hj.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jf.nicolike.cn

Java: import java.util.List;
来源：http://vf.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ph.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://ur.shxzukj.cn

C#:   using System.Text;
来源：http://re.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://xo.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://ju.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://nn.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://ud.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://mg.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xp.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://gg.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://sm.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sq.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://ua.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vk.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xw.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rn.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tq.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qu.9csxet.cn

Go:   func add(a, b int) int
来源：http://rd.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fr.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xn.colortex.cn

[C14] 泛型函数
来源：http://yp.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ys.asd995.cn

PHP:  // 无泛型
来源：http://fa.lnxyls.cn

JS:   // 无泛型
来源：http://bx.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dj.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iy.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://es.shtwfgs.cn

Ruby: # 无泛型
来源：http://jj.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vb.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://eu.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vj.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://zt.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pk.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jk.shtwfgs.cn

Java: // 无解构
来源：http://kk.szsharing.cn

Go:   // 无解构
来源：http://mv.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://zm.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://nz.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://ms.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://me.bjjhwx.cn

PHP:  // 无重载
来源：http://kx.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ql.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://do.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oh.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ze.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://us.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rx.hnjuh.cn

================================================================================
来源：http://ti.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://iv.hahajie.cn

================================================================================
来源：http://di.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://qw.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://og.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rm.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yf.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wc.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cx.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://ql.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://du.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hk.hahajie.cn

[D02] 追加元素到末尾
来源：http://kz.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iw.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cs.9csxet.cn

JS:   arr.push(4);
来源：http://sg.muxihuayi.cn

TS:   arr.push(4);
来源：http://jh.asd995.cn

Java: list.add(4);
来源：http://as.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://vq.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://jk.szsharing.cn

C#:   list.Add(4);
来源：http://ez.nszjky.cn

[D03] 在指定位置插入元素
来源：http://rv.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://lp.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ge.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qh.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://oc.hnjuh.cn

Java: list.add(0, 0);
来源：http://yz.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://du.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nv.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://es.nszjky.cn

[D04] 删除元素
来源：http://xi.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cc.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uv.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mu.521024.cn

TS:   arr.splice(0, 1);
来源：http://pu.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vp.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nj.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ki.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xs.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://uq.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ne.szxytkj.cn


<!-- 参考信息 -->