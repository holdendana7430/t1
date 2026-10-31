代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://mq.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ym.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jw.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://vm.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://od.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://xw.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wi.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mb.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vt.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xw.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bk.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pz.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nd.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cj.shxzskj.cn

[B07] while 循环
来源：http://mb.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://tq.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hb.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://tn.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://im.colortex.cn

Java: while (i < 10) { i++; }
来源：http://gs.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pf.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://qg.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://nv.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://dk.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://tx.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://om.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://df.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://nt.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://zw.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lt.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ls.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://gd.haigaiapp.cn

[B09] break 与 continue
来源：http://gv.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zh.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kj.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hv.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wu.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dl.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mz.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cv.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ha.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ar.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cs.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vy.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dj.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aw.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fl.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fq.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ww.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://pg.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://go.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://im.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ik.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://im.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ce.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ml.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://sn.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://at.nicolike.cn

[B12] 跳出多层循环
来源：http://et.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nh.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ex.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fe.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hw.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oe.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gf.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tr.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cl.colortex.cn

[B13] 判断是否为数字
来源：http://ww.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://pn.9csxet.cn

PHP:  is_numeric($x)
来源：http://oz.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ho.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ui.shxzskj.cn

Java: x instanceof Number
来源：http://xf.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mj.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://fw.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://ec.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://lt.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eb.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ta.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://be.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://mg.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sk.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vx.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uk.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wq.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://qd.lnxyls.cn

Py:   a and b or not c
来源：http://wx.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://vs.lnxyls.cn

JS:   a && b || !c
来源：http://ry.szxytkj.cn

TS:   a && b || !c
来源：http://md.panjiajie.cn

Java: a && b || !c
来源：http://sc.szsharing.cn

Go:   a && b || !c
来源：http://dq.wgjwhj.cn

Ruby: a && b || !c
来源：http://zr.yuexingan06.cn

C#:   a && b || !c
来源：http://qz.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bq.asd995.cn

Py:   if not data: return
来源：http://hk.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://ml.bjjhwx.cn

JS:   if (!data) return;
来源：http://te.muxihuayi.cn

TS:   if (!data) return;
来源：http://xv.bjjhwx.cn

Java: if (data == null) return;
来源：http://ou.shxzskj.cn

Go:   if data == nil { return }
来源：http://oe.jctech888.com.cn

Ruby: return if data.nil?
来源：http://jc.shxzukj.cn

C#:   if (data == null) return;
来源：http://xy.shxzskj.cn

================================================================================
来源：http://cz.9csxet.cn

C. 函数与作用域
来源：http://hy.9csxet.cn

================================================================================
来源：http://hs.colortex.cn

[C01] 定义函数
来源：http://nd.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://sv.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wq.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://jz.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fn.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hw.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vu.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://ld.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zo.shxzukj.cn

[C02] 默认参数
来源：http://ff.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://zl.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vd.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://fj.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vj.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nc.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qf.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ly.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://dl.szsharing.cn

[C03] 可变参数
来源：http://si.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://vw.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kd.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vz.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vw.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oj.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://va.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pl.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vg.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://fo.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sc.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nl.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ws.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vh.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://rk.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://ih.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://jh.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://ub.shxzukj.cn

[C05] 返回多个值
来源：http://go.bookmarksfly.cn

Py:   return a, b
来源：http://fa.lnxyls.cn

PHP:  return [$a, $b];
来源：http://dr.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bz.nicolike.cn

TS:   return { a, b };
来源：http://lm.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ea.nicolike.cn

Go:   return a, b
来源：http://zq.bjjhwx.cn

Ruby: return a, b
来源：http://ud.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://wj.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://sy.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://mj.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ha.shxzskj.cn

JS:   const square = x => x * x;
来源：http://rx.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://cb.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gu.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://se.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://dt.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ys.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://lt.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pt.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://md.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qy.wgjwhj.cn

TS:   arr.map(String)
来源：http://gg.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vi.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hj.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://yq.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ry.nszjky.cn

[C08] 闭包
来源：http://cs.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ie.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tj.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zf.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ik.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vv.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vi.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gv.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ey.hnjuh.cn

[C09] 递归
来源：http://lq.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sp.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fm.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://he.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pk.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ki.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hf.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mo.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://te.bjjhwx.cn

[C10] 变量作用域
来源：http://wk.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ze.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cp.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tb.panjiajie.cn

TS:   同 JS
来源：http://sk.huanxung.cn

Java: 方法内为块级作用域
来源：http://cu.hnjuh.cn

Go:   花括号块级作用域
来源：http://nv.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pn.colortex.cn

C#:   块级作用域
来源：http://pi.szsharing.cn

[C11] 模块导入与导出
来源：http://ng.panjiajie.cn

Py:   from module import func
来源：http://qr.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gq.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tb.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ra.huanxung.cn

Java: import java.util.List;
来源：http://rr.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lf.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://zl.wgjwhj.cn

C#:   using System.Text;
来源：http://li.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://tf.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://tm.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://eo.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ki.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://fx.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tc.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://ug.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://th.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mp.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://fq.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ir.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wp.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fo.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zi.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lo.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://xe.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://or.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rn.shxzukj.cn

[C14] 泛型函数
来源：http://ul.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pm.hahajie.cn

PHP:  // 无泛型
来源：http://hc.bjjhwx.cn

JS:   // 无泛型
来源：http://hr.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vp.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sc.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ay.bookmarksfly.cn

Ruby: # 无泛型
来源：http://fq.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yi.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://zv.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fv.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://jd.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vn.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rd.9csxet.cn

Java: // 无解构
来源：http://fn.hahajie.cn

Go:   // 无解构
来源：http://iv.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://zc.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://qv.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://yx.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ac.bjjhwx.cn

PHP:  // 无重载
来源：http://mb.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kk.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://la.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ru.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://nj.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://wq.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ml.bookmarksfly.cn

================================================================================
来源：http://fu.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://ke.colortex.cn

================================================================================
来源：http://ue.huanxung.cn

[D01] 创建数组 / 列表
来源：http://lc.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cl.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cj.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sa.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rt.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fr.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://yl.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://bu.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cd.shxzskj.cn

[D02] 追加元素到末尾
来源：http://ja.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://in.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bo.newstarts.cn

JS:   arr.push(4);
来源：http://oo.hnjuh.cn

TS:   arr.push(4);
来源：http://ev.wgjwhj.cn

Java: list.add(4);
来源：http://sh.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://tt.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://zk.haigaiapp.cn

C#:   list.Add(4);
来源：http://hx.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://tv.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://pb.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rr.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vz.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://oe.yuexingan06.cn

Java: list.add(0, 0);
来源：http://gk.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nk.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nb.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://hk.chemitech.net.cn

[D04] 删除元素
来源：http://lf.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ek.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yp.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nq.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://tp.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qb.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qe.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xg.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yi.newstarts.cn

[D05] 访问与修改元素
来源：http://gd.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ax.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nk.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xt.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://hn.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://oq.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://fq.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hm.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xr.yuexingan06.cn

[D06] 数组长度
来源：http://vg.nszjky.cn


<!-- 参考信息 -->