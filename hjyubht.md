代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://se.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ez.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://cc.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pr.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://fm.nszjky.cn

Py:   for item in arr: print(item)
来源：http://cv.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vh.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ed.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xh.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ki.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ym.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://nl.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kh.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://eb.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ww.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dt.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ru.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://up.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://li.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qe.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bq.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ps.hnjuh.cn

[B07] while 循环
来源：http://gy.521024.cn

Py:   while i < 10: i += 1
来源：http://dv.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ha.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://bx.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://fw.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://nh.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vn.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://az.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://rb.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://xz.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://zc.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kf.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://lz.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://ro.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://lc.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pj.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oe.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://jt.shxzukj.cn

[B09] break 与 continue
来源：http://ik.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qx.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vm.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://en.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uw.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://di.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ds.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wr.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uh.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://lb.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hm.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://io.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xv.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ht.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://es.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ub.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rp.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nu.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://sl.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://tf.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://kg.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ra.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xf.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ot.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kt.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://mz.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sj.szxytkj.cn

[B12] 跳出多层循环
来源：http://mq.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ai.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xc.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fb.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ls.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gy.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rz.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ok.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fp.colortex.cn

[B13] 判断是否为数字
来源：http://li.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://yg.hnjuh.cn

PHP:  is_numeric($x)
来源：http://mp.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ys.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yx.yuexingan06.cn

Java: x instanceof Number
来源：http://hw.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ds.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://by.nicolike.cn

C#:   x is int or double or decimal
来源：http://an.nszjky.cn

[B14] 判断值是否在集合内
来源：http://rr.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://id.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ha.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://za.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://dl.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ht.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qk.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sw.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vk.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://yw.wgjwhj.cn

Py:   a and b or not c
来源：http://cn.asd995.cn

PHP:  $a && $b || !$c
来源：http://nv.hahajie.cn

JS:   a && b || !c
来源：http://rz.bookmarksfly.cn

TS:   a && b || !c
来源：http://gl.wgjwhj.cn

Java: a && b || !c
来源：http://fs.bookmarksfly.cn

Go:   a && b || !c
来源：http://cs.jctech888.com.cn

Ruby: a && b || !c
来源：http://qv.shtwfgs.cn

C#:   a && b || !c
来源：http://sj.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fw.shxzskj.cn

Py:   if not data: return
来源：http://if.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://ty.muxihuayi.cn

JS:   if (!data) return;
来源：http://dg.gzmigu.cn

TS:   if (!data) return;
来源：http://qz.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://le.chemitech.net.cn

Go:   if data == nil { return }
来源：http://ht.shxzskj.cn

Ruby: return if data.nil?
来源：http://dk.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://qd.shtwfgs.cn

================================================================================
来源：http://qj.shxzukj.cn

C. 函数与作用域
来源：http://ii.nicolike.cn

================================================================================
来源：http://zt.9csxet.cn

[C01] 定义函数
来源：http://ub.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://fp.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ph.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://hh.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qg.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://km.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vy.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://yq.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cp.shxzskj.cn

[C02] 默认参数
来源：http://ie.colortex.cn

Py:   def greet(name="World"): return name
来源：http://bn.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cl.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://mt.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ie.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jv.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pq.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ww.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://ee.nszjky.cn

[C03] 可变参数
来源：http://be.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://yj.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ae.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://co.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tb.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fs.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dx.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zc.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ao.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://po.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vk.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hr.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zq.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yf.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://bp.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://in.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://qr.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://gf.szsharing.cn

[C05] 返回多个值
来源：http://bg.chemitech.net.cn

Py:   return a, b
来源：http://hc.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://tv.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vl.huixinmuqiang.cn

TS:   return { a, b };
来源：http://nu.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ph.yuntaijiaju.cn

Go:   return a, b
来源：http://ni.521024.cn

Ruby: return a, b
来源：http://fu.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://pf.521024.cn

[C06] 匿名函数 / lambda
来源：http://kd.szsharing.cn

Py:   square = lambda x: x * x
来源：http://iv.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ls.lnxyls.cn

JS:   const square = x => x * x;
来源：http://el.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://sv.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://js.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hg.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://is.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vw.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://je.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lp.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rz.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rv.521024.cn

TS:   arr.map(String)
来源：http://ng.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zy.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yg.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://cp.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gc.shtwfgs.cn

[C08] 闭包
来源：http://fw.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oz.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ud.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ee.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yf.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nq.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sf.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pl.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mn.newstarts.cn

[C09] 递归
来源：http://jd.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jr.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vo.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ru.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ob.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gg.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://si.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nj.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ff.yuntaijiaju.cn

[C10] 变量作用域
来源：http://br.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zz.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rg.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mj.asd995.cn

TS:   同 JS
来源：http://br.shxzukj.cn

Java: 方法内为块级作用域
来源：http://dw.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://br.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vl.panjiajie.cn

C#:   块级作用域
来源：http://bs.nszjky.cn

[C11] 模块导入与导出
来源：http://xx.szsharing.cn

Py:   from module import func
来源：http://qo.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ey.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mj.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://le.jianghongdianzi.cn

Java: import java.util.List;
来源：http://ln.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kt.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://jp.szsharing.cn

C#:   using System.Text;
来源：http://mk.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://xf.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://wg.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://bu.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://df.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://of.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bv.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://bu.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://pq.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dl.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://ok.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oi.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://id.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://of.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cq.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yk.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://ks.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mu.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ex.9csxet.cn

[C14] 泛型函数
来源：http://du.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kc.shtwfgs.cn

PHP:  // 无泛型
来源：http://rx.shtwfgs.cn

JS:   // 无泛型
来源：http://vs.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zf.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ez.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cf.jctech888.com.cn

Ruby: # 无泛型
来源：http://qw.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zf.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://db.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qr.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://rw.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mo.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ww.newstarts.cn

Java: // 无解构
来源：http://li.521024.cn

Go:   // 无解构
来源：http://qt.szsharing.cn

Ruby: a, b = pair
来源：http://jt.colortex.cn

C#:   var (a, b) = pair;
来源：http://ue.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://yj.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pt.colortex.cn

PHP:  // 无重载
来源：http://xb.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cb.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://ec.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wy.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://hb.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://yx.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sk.lnxyls.cn

================================================================================
来源：http://et.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://ku.nicolike.cn

================================================================================
来源：http://ie.nszjky.cn

[D01] 创建数组 / 列表
来源：http://cr.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uu.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ib.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vy.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ml.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pz.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ow.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://au.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ot.hahajie.cn

[D02] 追加元素到末尾
来源：http://sh.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mv.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zi.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://ho.shxzskj.cn

TS:   arr.push(4);
来源：http://gz.huanxung.cn

Java: list.add(4);
来源：http://xz.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://yv.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ra.shxzskj.cn

C#:   list.Add(4);
来源：http://lq.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://gz.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://ki.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dw.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bh.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://hy.colortex.cn

Java: list.add(0, 0);
来源：http://cr.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hn.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ld.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://xk.hahajie.cn

[D04] 删除元素
来源：http://oi.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cd.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jq.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aw.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://ef.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ak.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cn.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://js.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kd.asd995.cn

[D05] 访问与修改元素
来源：http://ce.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ou.521024.cn


<!-- 参考信息 -->