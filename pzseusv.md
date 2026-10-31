代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://cq.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://js.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wa.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://rz.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ez.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://ke.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://re.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nx.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pw.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ps.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://da.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bm.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ik.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gy.jctech888.com.cn

[B07] while 循环
来源：http://yd.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://tj.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gw.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://pg.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://eq.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://yj.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ni.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://ko.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://hd.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://zm.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://us.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ql.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://tw.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://ct.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://ne.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wp.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pb.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://mx.jianghongdianzi.cn

[B09] break 与 continue
来源：http://yw.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wu.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ss.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ql.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zw.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://za.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ep.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ux.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pk.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://aw.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yt.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kw.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xf.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uu.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xn.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://po.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vm.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wb.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://yi.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://bm.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://ek.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ow.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://za.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xk.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ty.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://cc.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gp.haigaiapp.cn

[B12] 跳出多层循环
来源：http://ub.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ne.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mt.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ap.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dh.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fr.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fz.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ri.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bx.hnjuh.cn

[B13] 判断是否为数字
来源：http://ck.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://bg.hahajie.cn

PHP:  is_numeric($x)
来源：http://bq.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wu.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lb.panjiajie.cn

Java: x instanceof Number
来源：http://hg.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vh.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://lk.nszjky.cn

C#:   x is int or double or decimal
来源：http://iv.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://uo.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zv.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yn.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://sz.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://jh.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lf.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sq.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ke.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ec.szsharing.cn

[B15] 布尔运算与取反
来源：http://lm.bjjhwx.cn

Py:   a and b or not c
来源：http://be.newstarts.cn

PHP:  $a && $b || !$c
来源：http://mg.wgjwhj.cn

JS:   a && b || !c
来源：http://ev.9csxet.cn

TS:   a && b || !c
来源：http://te.colortex.cn

Java: a && b || !c
来源：http://ij.wgjwhj.cn

Go:   a && b || !c
来源：http://cz.szxytkj.cn

Ruby: a && b || !c
来源：http://za.huanxung.cn

C#:   a && b || !c
来源：http://os.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pj.gzmigu.cn

Py:   if not data: return
来源：http://aq.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://yi.wgjwhj.cn

JS:   if (!data) return;
来源：http://hm.gzmigu.cn

TS:   if (!data) return;
来源：http://gc.nszjky.cn

Java: if (data == null) return;
来源：http://zn.newstarts.cn

Go:   if data == nil { return }
来源：http://jx.shxzukj.cn

Ruby: return if data.nil?
来源：http://oz.shxzukj.cn

C#:   if (data == null) return;
来源：http://kl.newstarts.cn

================================================================================
来源：http://sy.jctech888.com.cn

C. 函数与作用域
来源：http://dz.hnjuh.cn

================================================================================
来源：http://zd.gzmigu.cn

[C01] 定义函数
来源：http://nj.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://wq.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ff.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://tl.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bo.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cd.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yi.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://vo.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ua.szxytkj.cn

[C02] 默认参数
来源：http://cn.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://uv.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dh.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qv.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gz.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://km.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nj.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ns.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ej.lnxyls.cn

[C03] 可变参数
来源：http://sr.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://cx.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://up.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://on.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lo.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pf.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://un.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qh.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ao.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://iq.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hp.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kp.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ey.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ds.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://jm.521024.cn

Go:   // 无：用配置结构体参数
来源：http://oz.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://je.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://yr.haigaiapp.cn

[C05] 返回多个值
来源：http://mp.huixiangedu.cn

Py:   return a, b
来源：http://yh.szsharing.cn

PHP:  return [$a, $b];
来源：http://jf.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jo.521024.cn

TS:   return { a, b };
来源：http://ur.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wy.bookmarksfly.cn

Go:   return a, b
来源：http://fv.shxzukj.cn

Ruby: return a, b
来源：http://aq.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://jt.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://lw.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://so.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kv.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://bh.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://qg.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lu.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uy.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://ja.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qg.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://fg.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kx.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ri.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://io.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kg.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xc.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://fx.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gy.hahajie.cn

[C08] 闭包
来源：http://ex.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nc.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://by.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tm.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vc.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hm.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wm.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://og.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lj.521024.cn

[C09] 递归
来源：http://mq.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qa.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iw.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wa.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uw.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lt.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://un.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kq.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ap.jctech888.com.cn

[C10] 变量作用域
来源：http://ej.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ak.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qi.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ar.huixinmuqiang.cn

TS:   同 JS
来源：http://gc.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ip.hahajie.cn

Go:   花括号块级作用域
来源：http://oq.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dc.newstarts.cn

C#:   块级作用域
来源：http://yn.jctech888.com.cn

[C11] 模块导入与导出
来源：http://iv.lnxyls.cn

Py:   from module import func
来源：http://mw.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tk.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aq.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ty.lnxyls.cn

Java: import java.util.List;
来源：http://lr.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ac.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ch.hahajie.cn

C#:   using System.Text;
来源：http://vo.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://ds.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://rb.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://bb.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://ph.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://ef.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nm.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://ub.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://vo.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://km.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://tr.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ca.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://su.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wt.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hh.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wc.colortex.cn

Go:   func add(a, b int) int
来源：http://re.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dv.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://it.yuntaijiaju.cn

[C14] 泛型函数
来源：http://lc.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://be.bookmarksfly.cn

PHP:  // 无泛型
来源：http://aw.shxzskj.cn

JS:   // 无泛型
来源：http://hq.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ko.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pl.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cq.chemitech.net.cn

Ruby: # 无泛型
来源：http://oa.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jn.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://os.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ma.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://zy.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ju.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ag.nszjky.cn

Java: // 无解构
来源：http://vj.newstarts.cn

Go:   // 无解构
来源：http://bt.shxzukj.cn

Ruby: a, b = pair
来源：http://ad.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://kg.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://ir.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ql.bookmarksfly.cn

PHP:  // 无重载
来源：http://co.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xu.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://ce.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xt.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://qj.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://xc.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tn.huixinmuqiang.cn

================================================================================
来源：http://wb.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://it.newstarts.cn

================================================================================
来源：http://am.colortex.cn

[D01] 创建数组 / 列表
来源：http://su.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gs.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hp.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bf.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://js.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sp.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://rd.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://zk.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xz.gzmigu.cn

[D02] 追加元素到末尾
来源：http://up.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://os.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dv.asd995.cn

JS:   arr.push(4);
来源：http://nl.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://mo.shxzukj.cn

Java: list.add(4);
来源：http://wt.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://sn.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://uv.shxzukj.cn

C#:   list.Add(4);
来源：http://dw.nicolike.cn

[D03] 在指定位置插入元素
来源：http://ne.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://nj.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ok.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ji.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://nf.huixiangedu.cn

Java: list.add(0, 0);
来源：http://bw.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ya.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wp.colortex.cn

C#:   list.Insert(0, 0);
来源：http://yj.chemitech.net.cn

[D04] 删除元素
来源：http://fl.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hg.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lk.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qt.521024.cn

TS:   arr.splice(0, 1);
来源：http://pb.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eo.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jg.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://af.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jx.yuexingan06.cn

[D05] 访问与修改元素
来源：http://wj.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bd.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pn.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ht.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://yo.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://mc.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://uj.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://je.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ug.gzmigu.cn

[D06] 数组长度
来源：http://qg.yuexingan06.cn


<!-- 参考信息 -->