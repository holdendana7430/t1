代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vu.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kp.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mj.yuexingan06.cn

[B04] for 计数循环
来源：http://cy.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://vp.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vm.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gw.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wl.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wh.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vd.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://ij.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ou.521024.cn

[B05] 遍历数组 / 列表
来源：http://bz.szsharing.cn

Py:   for item in arr: print(item)
来源：http://bi.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xl.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yx.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lu.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mq.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oh.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://ua.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ic.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://tf.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://it.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gl.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vy.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gd.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iq.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bt.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mh.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sm.jctech888.com.cn

[B07] while 循环
来源：http://ls.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://xm.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tj.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://ml.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://nm.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://tq.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mw.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://uy.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://kr.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://ps.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://fp.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xl.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://uv.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://cg.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://sy.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dq.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ng.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://di.nicolike.cn

[B09] break 与 continue
来源：http://vu.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gw.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wi.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fz.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qy.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jl.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tt.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ml.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://rf.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ed.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ld.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sq.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qc.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bc.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ys.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xm.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bd.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://zt.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://lu.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://yc.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tr.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vg.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rf.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ol.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://tz.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wo.szsharing.cn

[B12] 跳出多层循环
来源：http://nu.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://au.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fg.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jd.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vf.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lq.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cq.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://as.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zb.lnxyls.cn

[B13] 判断是否为数字
来源：http://vu.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://kk.asd995.cn

PHP:  is_numeric($x)
来源：http://tr.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ey.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xa.hnjuh.cn

Java: x instanceof Number
来源：http://yo.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yr.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://ov.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://mp.asd995.cn

[B14] 判断值是否在集合内
来源：http://lk.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rn.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hr.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://al.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://lz.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xz.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vs.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zr.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ce.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://yb.wgjwhj.cn

Py:   a and b or not c
来源：http://aa.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://jt.521024.cn

JS:   a && b || !c
来源：http://fo.chemitech.net.cn

TS:   a && b || !c
来源：http://no.shxzskj.cn

Java: a && b || !c
来源：http://ct.jianghongdianzi.cn

Go:   a && b || !c
来源：http://ve.colortex.cn

Ruby: a && b || !c
来源：http://sz.bjjhwx.cn

C#:   a && b || !c
来源：http://nj.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vd.gzmigu.cn

Py:   if not data: return
来源：http://hi.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://ia.521024.cn

JS:   if (!data) return;
来源：http://oh.shxzskj.cn

TS:   if (!data) return;
来源：http://vj.gzmigu.cn

Java: if (data == null) return;
来源：http://bb.huanxung.cn

Go:   if data == nil { return }
来源：http://ph.szxytkj.cn

Ruby: return if data.nil?
来源：http://qj.jctech888.com.cn

C#:   if (data == null) return;
来源：http://uo.huixinmuqiang.cn

================================================================================
来源：http://dt.chemitech.net.cn

C. 函数与作用域
来源：http://fv.shtwfgs.cn

================================================================================
来源：http://rh.yuntaijiaju.cn

[C01] 定义函数
来源：http://tu.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://gs.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tl.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://ig.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bw.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dm.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rk.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://yn.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wd.huanxung.cn

[C02] 默认参数
来源：http://gc.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://eb.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xf.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://vn.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hs.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://za.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iw.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://ij.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://eu.panjiajie.cn

[C03] 可变参数
来源：http://qc.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://fg.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wf.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ht.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jt.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ge.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mg.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lx.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cu.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://hy.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xk.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://st.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ij.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vt.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://jr.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://ob.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://aq.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://nl.panjiajie.cn

[C05] 返回多个值
来源：http://ia.newstarts.cn

Py:   return a, b
来源：http://jy.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://oq.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hw.lnxyls.cn

TS:   return { a, b };
来源：http://qj.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hb.huanxung.cn

Go:   return a, b
来源：http://se.9csxet.cn

Ruby: return a, b
来源：http://ge.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://ap.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://nv.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://rx.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pz.shxzukj.cn

JS:   const square = x => x * x;
来源：http://jh.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://so.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xn.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eu.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://fh.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fu.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://gz.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hq.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nt.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bw.huixiangedu.cn

TS:   arr.map(String)
来源：http://bw.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dc.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dn.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ni.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qr.chemitech.net.cn

[C08] 闭包
来源：http://op.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jv.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vs.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rt.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://az.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kt.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mo.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yn.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fk.panjiajie.cn

[C09] 递归
来源：http://fu.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nq.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gd.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eb.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fy.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://df.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ol.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uo.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ce.shxzskj.cn

[C10] 变量作用域
来源：http://il.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mp.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dw.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tl.hahajie.cn

TS:   同 JS
来源：http://az.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://if.hnjuh.cn

Go:   花括号块级作用域
来源：http://rw.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cx.bookmarksfly.cn

C#:   块级作用域
来源：http://za.shxzskj.cn

[C11] 模块导入与导出
来源：http://bo.jctech888.com.cn

Py:   from module import func
来源：http://ed.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yp.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ya.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://we.asd995.cn

Java: import java.util.List;
来源：http://lt.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zl.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://gv.shxzskj.cn

C#:   using System.Text;
来源：http://eh.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://ij.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://lt.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://wn.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ld.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://oh.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oo.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://dq.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://ko.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nl.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://mz.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ua.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hd.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vm.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ob.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ks.gzmigu.cn

Go:   func add(a, b int) int
来源：http://tx.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qu.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cx.huixiangedu.cn

[C14] 泛型函数
来源：http://kv.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hm.gzmigu.cn

PHP:  // 无泛型
来源：http://dj.gzmigu.cn

JS:   // 无泛型
来源：http://xy.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wl.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dm.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yv.bjjhwx.cn

Ruby: # 无泛型
来源：http://jo.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xv.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://rs.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ij.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://kg.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ks.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fe.bookmarksfly.cn

Java: // 无解构
来源：http://he.nszjky.cn

Go:   // 无解构
来源：http://hh.szxytkj.cn

Ruby: a, b = pair
来源：http://fx.nicolike.cn

C#:   var (a, b) = pair;
来源：http://sm.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://rv.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ey.lnxyls.cn

PHP:  // 无重载
来源：http://wz.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rr.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://kl.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jz.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://yd.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://tu.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tt.lnxyls.cn

================================================================================
来源：http://jr.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://pp.newstarts.cn

================================================================================
来源：http://zu.newstarts.cn

[D01] 创建数组 / 列表
来源：http://tx.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ax.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hi.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xc.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sh.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gl.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://mn.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://av.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://km.9csxet.cn

[D02] 追加元素到末尾
来源：http://nf.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sk.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ez.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://lz.nicolike.cn

TS:   arr.push(4);
来源：http://bo.panjiajie.cn

Java: list.add(4);
来源：http://oj.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://pk.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://oe.muxihuayi.cn

C#:   list.Add(4);
来源：http://ac.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://nn.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://ip.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://by.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ks.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://rt.shxzukj.cn

Java: list.add(0, 0);
来源：http://ol.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://am.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xk.asd995.cn

C#:   list.Insert(0, 0);
来源：http://xh.colortex.cn

[D04] 删除元素
来源：http://sl.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ho.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ae.colortex.cn


<!-- 参考信息 -->