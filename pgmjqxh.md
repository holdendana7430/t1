代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tx.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ir.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hg.lnxyls.cn

[B04] for 计数循环
来源：http://xb.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://hn.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zf.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ti.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wk.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://od.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://lp.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fn.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://ws.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://tc.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wt.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sg.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qp.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wi.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://md.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://wt.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fl.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://bm.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uv.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fa.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ph.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hc.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lk.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ge.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zr.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jo.chemitech.net.cn

[B07] while 循环
来源：http://hv.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://to.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lo.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://yz.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://wl.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://oc.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cq.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://gi.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://pl.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://au.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://xn.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://py.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://kh.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://fa.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://rx.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wt.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gj.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://bv.nszjky.cn

[B09] break 与 continue
来源：http://nf.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://su.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://da.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://on.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dv.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ln.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ml.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kk.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qu.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://nk.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qa.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ji.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jw.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ai.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ig.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bv.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ae.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uk.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://hn.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://pt.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://mk.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nn.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fw.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vd.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bl.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://fe.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rk.hnjuh.cn

[B12] 跳出多层循环
来源：http://vr.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kg.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ie.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hl.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cl.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ks.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mm.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dt.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tu.9csxet.cn

[B13] 判断是否为数字
来源：http://kz.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://gh.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://sy.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yy.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wm.muxihuayi.cn

Java: x instanceof Number
来源：http://cf.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dw.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://ly.hnjuh.cn

C#:   x is int or double or decimal
来源：http://qw.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://jz.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yn.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ux.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://gs.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://ux.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sk.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bj.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xj.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ao.521024.cn

[B15] 布尔运算与取反
来源：http://tn.hahajie.cn

Py:   a and b or not c
来源：http://nj.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ks.haigaiapp.cn

JS:   a && b || !c
来源：http://ah.chemitech.net.cn

TS:   a && b || !c
来源：http://je.yuntaijiaju.cn

Java: a && b || !c
来源：http://wc.bookmarksfly.cn

Go:   a && b || !c
来源：http://sk.hahajie.cn

Ruby: a && b || !c
来源：http://sd.bjjhwx.cn

C#:   a && b || !c
来源：http://pk.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wr.huixiangedu.cn

Py:   if not data: return
来源：http://cp.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://om.szsharing.cn

JS:   if (!data) return;
来源：http://dj.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://dc.gzmigu.cn

Java: if (data == null) return;
来源：http://mz.shxzskj.cn

Go:   if data == nil { return }
来源：http://cb.jctech888.com.cn

Ruby: return if data.nil?
来源：http://qf.hnjuh.cn

C#:   if (data == null) return;
来源：http://ug.nicolike.cn

================================================================================
来源：http://be.chemitech.net.cn

C. 函数与作用域
来源：http://tl.nszjky.cn

================================================================================
来源：http://wp.panjiajie.cn

[C01] 定义函数
来源：http://hh.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://hn.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iy.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://wo.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://is.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yo.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://de.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://kn.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yu.yuntaijiaju.cn

[C02] 默认参数
来源：http://hc.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://ts.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hp.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://bn.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tp.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://he.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yo.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://lp.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://gt.muxihuayi.cn

[C03] 可变参数
来源：http://ev.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://rg.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ru.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://po.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qj.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://og.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hl.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dv.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xs.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://xv.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fq.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qr.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ue.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ed.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://lx.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://rh.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://dt.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://jm.nszjky.cn

[C05] 返回多个值
来源：http://vi.muxihuayi.cn

Py:   return a, b
来源：http://dk.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://rf.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ea.hahajie.cn

TS:   return { a, b };
来源：http://tl.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zl.newstarts.cn

Go:   return a, b
来源：http://ir.shxzukj.cn

Ruby: return a, b
来源：http://hy.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://qi.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://ju.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://ea.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ui.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://kb.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://iq.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qg.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kq.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://hb.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ew.colortex.cn

[C07] 把函数作为参数传入
来源：http://yk.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dd.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gq.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fe.colortex.cn

TS:   arr.map(String)
来源：http://up.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zi.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://im.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://kr.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gh.newstarts.cn

[C08] 闭包
来源：http://wd.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oj.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zj.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bm.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sd.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ny.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jz.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pp.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jx.bookmarksfly.cn

[C09] 递归
来源：http://yc.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lu.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ff.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fb.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uk.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oe.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uz.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lf.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xz.lnxyls.cn

[C10] 变量作用域
来源：http://kb.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mn.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vb.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mg.521024.cn

TS:   同 JS
来源：http://bk.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://pc.haigaiapp.cn

Go:   花括号块级作用域
来源：http://uv.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yn.szxytkj.cn

C#:   块级作用域
来源：http://zo.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://me.lnxyls.cn

Py:   from module import func
来源：http://fq.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://in.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vw.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qc.bjjhwx.cn

Java: import java.util.List;
来源：http://rd.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cf.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://ye.hnjuh.cn

C#:   using System.Text;
来源：http://vy.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://rk.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://xb.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://nu.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://av.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://qz.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ok.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://sl.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://oh.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mi.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://av.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wd.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ea.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yl.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://id.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ij.nszjky.cn

Go:   func add(a, b int) int
来源：http://yh.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eu.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qo.jctech888.com.cn

[C14] 泛型函数
来源：http://ro.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ev.szxytkj.cn

PHP:  // 无泛型
来源：http://cc.colortex.cn

JS:   // 无泛型
来源：http://ff.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fl.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pq.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ob.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://ou.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bg.huanxung.cn

[C15] 解构 / 展开参数
来源：http://iz.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qo.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://jd.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bc.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cv.gzmigu.cn

Java: // 无解构
来源：http://rz.szxytkj.cn

Go:   // 无解构
来源：http://wq.hahajie.cn

Ruby: a, b = pair
来源：http://nj.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://hw.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://ft.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pv.huixiangedu.cn

PHP:  // 无重载
来源：http://nt.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ls.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://na.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jw.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://pm.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://fw.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hq.colortex.cn

================================================================================
来源：http://cz.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://al.jctech888.com.cn

================================================================================
来源：http://vx.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://ro.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ih.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://op.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ja.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iq.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jn.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ij.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://da.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nk.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://vs.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bu.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://um.hnjuh.cn

JS:   arr.push(4);
来源：http://wo.huixiangedu.cn

TS:   arr.push(4);
来源：http://rh.nicolike.cn

Java: list.add(4);
来源：http://ql.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://vo.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://kp.lnxyls.cn

C#:   list.Add(4);
来源：http://ae.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://ni.asd995.cn

Py:   arr.insert(0, 0)
来源：http://bu.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tl.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lk.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://we.hnjuh.cn

Java: list.add(0, 0);
来源：http://tn.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oo.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nn.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://vg.yuexingan06.cn

[D04] 删除元素
来源：http://yf.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jw.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://px.newstarts.cn


<!-- 参考信息 -->