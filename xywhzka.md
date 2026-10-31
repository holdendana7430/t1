代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xc.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fr.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://of.szsharing.cn

[B04] for 计数循环
来源：http://im.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://jq.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zo.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tn.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sm.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://at.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dn.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://bi.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vs.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://od.nicolike.cn

Py:   for item in arr: print(item)
来源：http://jz.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wx.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uq.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cz.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rv.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tk.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://aq.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iz.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://nc.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yf.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://az.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://go.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lf.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://se.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vv.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://na.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://el.huixiangedu.cn

[B07] while 循环
来源：http://kj.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://fr.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bw.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://xn.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://uo.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://tk.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zj.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://nr.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://rr.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://rj.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://wm.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uv.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://ql.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://sh.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://yq.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pw.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lr.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://ym.shxzskj.cn

[B09] break 与 continue
来源：http://yz.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zr.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ga.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ew.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vr.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://km.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gq.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bk.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://et.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://ad.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rp.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yf.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lb.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ek.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://am.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cx.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cr.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dw.521024.cn

[B11] 生成数字序列 / 区间
来源：http://gf.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://no.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://bg.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sm.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cg.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qw.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ib.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://wy.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://un.521024.cn

[B12] 跳出多层循环
来源：http://gk.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bg.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://po.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pz.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dr.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://th.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://us.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gy.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ku.gzmigu.cn

[B13] 判断是否为数字
来源：http://le.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://dj.newstarts.cn

PHP:  is_numeric($x)
来源：http://km.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kh.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pm.panjiajie.cn

Java: x instanceof Number
来源：http://hc.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pr.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://pw.asd995.cn

C#:   x is int or double or decimal
来源：http://lx.szsharing.cn

[B14] 判断值是否在集合内
来源：http://qm.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://js.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bl.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://jx.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://sr.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ml.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qh.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://km.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://md.nszjky.cn

[B15] 布尔运算与取反
来源：http://oy.nicolike.cn

Py:   a and b or not c
来源：http://gf.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://hs.bjjhwx.cn

JS:   a && b || !c
来源：http://uk.huixinmuqiang.cn

TS:   a && b || !c
来源：http://at.nicolike.cn

Java: a && b || !c
来源：http://iu.shxzskj.cn

Go:   a && b || !c
来源：http://rr.521024.cn

Ruby: a && b || !c
来源：http://qk.huanxung.cn

C#:   a && b || !c
来源：http://cc.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bo.jctech888.com.cn

Py:   if not data: return
来源：http://bm.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://dq.huanxung.cn

JS:   if (!data) return;
来源：http://ha.yuexingan06.cn

TS:   if (!data) return;
来源：http://yd.shtwfgs.cn

Java: if (data == null) return;
来源：http://fr.jctech888.com.cn

Go:   if data == nil { return }
来源：http://cd.newstarts.cn

Ruby: return if data.nil?
来源：http://fi.huanxung.cn

C#:   if (data == null) return;
来源：http://zk.huanxung.cn

================================================================================
来源：http://pg.bookmarksfly.cn

C. 函数与作用域
来源：http://td.panjiajie.cn

================================================================================
来源：http://do.lnxyls.cn

[C01] 定义函数
来源：http://kc.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://wt.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fb.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://mo.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mn.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lc.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jf.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://bv.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fn.jianghongdianzi.cn

[C02] 默认参数
来源：http://nb.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://pf.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fx.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://qh.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wj.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qp.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gj.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://qz.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://jf.9csxet.cn

[C03] 可变参数
来源：http://bk.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://df.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wf.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ov.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zu.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uq.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tk.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fh.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://hy.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eb.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://el.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gr.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sc.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://oc.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://ar.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://di.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://sl.huanxung.cn

[C05] 返回多个值
来源：http://cb.huixiangedu.cn

Py:   return a, b
来源：http://sf.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://hv.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ga.jianghongdianzi.cn

TS:   return { a, b };
来源：http://sp.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mx.wgjwhj.cn

Go:   return a, b
来源：http://fo.lnxyls.cn

Ruby: return a, b
来源：http://sl.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://fx.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://ab.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://ol.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mj.huanxung.cn

JS:   const square = x => x * x;
来源：http://ui.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://xh.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xm.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ng.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://wt.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ff.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://qq.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hp.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://db.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pz.wgjwhj.cn

TS:   arr.map(String)
来源：http://pj.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gw.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uv.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://lh.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bz.wgjwhj.cn

[C08] 闭包
来源：http://pw.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ev.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dp.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qg.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://td.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ty.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yc.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ev.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dw.asd995.cn

[C09] 递归
来源：http://ml.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fe.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ua.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pi.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ki.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nj.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hs.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kn.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yi.gzmigu.cn

[C10] 变量作用域
来源：http://yy.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jp.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ed.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xr.lnxyls.cn

TS:   同 JS
来源：http://bw.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://mv.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://ll.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bt.bjjhwx.cn

C#:   块级作用域
来源：http://gm.colortex.cn

[C11] 模块导入与导出
来源：http://wh.chemitech.net.cn

Py:   from module import func
来源：http://rx.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fi.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yb.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kz.huanxung.cn

Java: import java.util.List;
来源：http://oa.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cc.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://pz.colortex.cn

C#:   using System.Text;
来源：http://tn.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://fn.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://yd.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://zy.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://wi.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://ao.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sa.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://vh.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://jx.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ut.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://gw.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://et.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ix.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vc.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://su.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ci.newstarts.cn

Go:   func add(a, b int) int
来源：http://xi.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ab.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cn.shtwfgs.cn

[C14] 泛型函数
来源：http://bm.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ar.szsharing.cn

PHP:  // 无泛型
来源：http://tp.hnjuh.cn

JS:   // 无泛型
来源：http://ty.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pt.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yi.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bo.newstarts.cn

Ruby: # 无泛型
来源：http://fk.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gt.huanxung.cn

[C15] 解构 / 展开参数
来源：http://zt.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lo.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://jz.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uf.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ht.521024.cn

Java: // 无解构
来源：http://as.newstarts.cn

Go:   // 无解构
来源：http://fp.shtwfgs.cn

Ruby: a, b = pair
来源：http://ys.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://jq.huanxung.cn

[C16] 函数 / 方法重载
来源：http://si.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://be.shtwfgs.cn

PHP:  // 无重载
来源：http://vs.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://da.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://zw.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oh.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://qm.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://rh.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qc.haigaiapp.cn

================================================================================
来源：http://eq.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://ch.asd995.cn

================================================================================
来源：http://ne.huanxung.cn

[D01] 创建数组 / 列表
来源：http://sn.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pi.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pe.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://di.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jg.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wm.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://gk.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://oo.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tb.shxzukj.cn

[D02] 追加元素到末尾
来源：http://ui.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pw.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hn.haigaiapp.cn

JS:   arr.push(4);
来源：http://zn.wgjwhj.cn

TS:   arr.push(4);
来源：http://mt.shtwfgs.cn

Java: list.add(4);
来源：http://bn.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://rl.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://kd.nszjky.cn

C#:   list.Add(4);
来源：http://kq.szsharing.cn

[D03] 在指定位置插入元素
来源：http://gv.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://sa.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yw.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hx.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://vi.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://wy.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://se.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ip.521024.cn

C#:   list.Insert(0, 0);
来源：http://cy.szsharing.cn

[D04] 删除元素
来源：http://nk.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nh.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xj.yuexingan06.cn


<!-- 参考信息 -->