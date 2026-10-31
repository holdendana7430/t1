代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qg.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ed.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nv.chemitech.net.cn

[B04] for 计数循环
来源：http://eb.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://gm.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://la.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oo.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sg.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://am.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ck.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://xu.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xr.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://kj.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://ug.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bl.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zd.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kv.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vb.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vy.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://to.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://up.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://ez.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iu.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zs.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pt.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ng.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mx.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dm.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ds.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://of.szxytkj.cn

[B07] while 循环
来源：http://cj.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://sx.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iy.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://yy.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://bf.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://yo.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xh.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://ou.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://ae.colortex.cn

[B08] do-while（至少执行一次）
来源：http://yu.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://ot.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rd.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://dg.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://ur.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://ya.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ls.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yc.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://aq.shtwfgs.cn

[B09] break 与 continue
来源：http://xv.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aj.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://go.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jl.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ia.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://er.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wo.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zg.nicolike.cn

[B10] 遍历同时拿索引
来源：http://bl.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xg.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hp.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ov.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yq.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fb.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ci.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yc.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yr.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://ew.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://vd.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://bm.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qm.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://am.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jm.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gi.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://au.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://za.szsharing.cn

[B12] 跳出多层循环
来源：http://hy.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ui.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ki.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sd.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ni.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nm.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cn.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jj.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lv.panjiajie.cn

[B13] 判断是否为数字
来源：http://yb.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://on.colortex.cn

PHP:  is_numeric($x)
来源：http://hg.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jx.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://co.lnxyls.cn

Java: x instanceof Number
来源：http://od.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xk.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://xi.asd995.cn

C#:   x is int or double or decimal
来源：http://jo.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://xy.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gv.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ji.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://ir.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://gy.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gx.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wf.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wb.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mt.hahajie.cn

[B15] 布尔运算与取反
来源：http://gh.hnjuh.cn

Py:   a and b or not c
来源：http://xg.newstarts.cn

PHP:  $a && $b || !$c
来源：http://ep.nicolike.cn

JS:   a && b || !c
来源：http://ur.wgjwhj.cn

TS:   a && b || !c
来源：http://tx.lnxyls.cn

Java: a && b || !c
来源：http://gx.shxzukj.cn

Go:   a && b || !c
来源：http://br.521024.cn

Ruby: a && b || !c
来源：http://zi.panjiajie.cn

C#:   a && b || !c
来源：http://zb.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mf.chemitech.net.cn

Py:   if not data: return
来源：http://yg.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ww.nszjky.cn

JS:   if (!data) return;
来源：http://xw.chemitech.net.cn

TS:   if (!data) return;
来源：http://fh.nszjky.cn

Java: if (data == null) return;
来源：http://sb.hnjuh.cn

Go:   if data == nil { return }
来源：http://zn.shtwfgs.cn

Ruby: return if data.nil?
来源：http://mi.hnjuh.cn

C#:   if (data == null) return;
来源：http://ic.muxihuayi.cn

================================================================================
来源：http://er.szxytkj.cn

C. 函数与作用域
来源：http://cv.bjjhwx.cn

================================================================================
来源：http://db.hahajie.cn

[C01] 定义函数
来源：http://oq.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://hn.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xe.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://zp.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uc.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cx.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bv.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://qk.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://il.colortex.cn

[C02] 默认参数
来源：http://cc.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://ek.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://io.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://bn.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ow.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ep.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jk.521024.cn

Ruby: def greet(name = "World") = name
来源：http://rn.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://mg.shtwfgs.cn

[C03] 可变参数
来源：http://ft.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://og.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vz.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://po.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uc.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sm.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gt.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hx.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ha.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://ai.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://az.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bm.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gt.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ng.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ne.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://ma.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://ra.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://kw.nicolike.cn

[C05] 返回多个值
来源：http://sc.nicolike.cn

Py:   return a, b
来源：http://fo.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://wl.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cr.hahajie.cn

TS:   return { a, b };
来源：http://vn.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xy.jianghongdianzi.cn

Go:   return a, b
来源：http://ij.yuexingan06.cn

Ruby: return a, b
来源：http://yt.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://cl.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://wj.521024.cn

Py:   square = lambda x: x * x
来源：http://aw.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bq.asd995.cn

JS:   const square = x => x * x;
来源：http://bt.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://cd.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yx.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gl.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://tc.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sy.nszjky.cn

[C07] 把函数作为参数传入
来源：http://dj.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sk.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eo.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ot.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://gm.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yd.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bq.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://xv.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wh.huixiangedu.cn

[C08] 闭包
来源：http://ib.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://we.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xb.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fd.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ew.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lx.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gf.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sx.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wr.gzmigu.cn

[C09] 递归
来源：http://an.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://id.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fd.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sr.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mx.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uc.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://io.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xg.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hy.jctech888.com.cn

[C10] 变量作用域
来源：http://cs.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vg.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qk.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zf.huixiangedu.cn

TS:   同 JS
来源：http://tr.colortex.cn

Java: 方法内为块级作用域
来源：http://im.lnxyls.cn

Go:   花括号块级作用域
来源：http://jp.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xr.wgjwhj.cn

C#:   块级作用域
来源：http://un.9csxet.cn

[C11] 模块导入与导出
来源：http://xg.huanxung.cn

Py:   from module import func
来源：http://dz.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ng.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lr.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ou.gzmigu.cn

Java: import java.util.List;
来源：http://ro.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rw.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://fy.jianghongdianzi.cn

C#:   using System.Text;
来源：http://nl.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://fg.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://kr.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://xh.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://ii.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://vt.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ws.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://pz.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://hu.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fu.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://zu.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jd.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jy.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ro.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mi.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ud.9csxet.cn

Go:   func add(a, b int) int
来源：http://fe.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dj.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oq.hahajie.cn

[C14] 泛型函数
来源：http://qv.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vr.nicolike.cn

PHP:  // 无泛型
来源：http://ol.shxzukj.cn

JS:   // 无泛型
来源：http://bd.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fl.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sl.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uq.huixiangedu.cn

Ruby: # 无泛型
来源：http://ah.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pg.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://pd.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nv.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://nk.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://np.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ru.shxzukj.cn

Java: // 无解构
来源：http://fb.asd995.cn

Go:   // 无解构
来源：http://tp.asd995.cn

Ruby: a, b = pair
来源：http://gr.9csxet.cn

C#:   var (a, b) = pair;
来源：http://gk.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://eu.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qo.szxytkj.cn

PHP:  // 无重载
来源：http://gy.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tw.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://og.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tp.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://nv.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://jr.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://va.yuexingan06.cn

================================================================================
来源：http://uw.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://jd.szsharing.cn

================================================================================
来源：http://sc.szsharing.cn

[D01] 创建数组 / 列表
来源：http://zt.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://de.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dv.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bk.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bm.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zr.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://tx.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://wl.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ae.gzmigu.cn

[D02] 追加元素到末尾
来源：http://gc.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sd.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fx.gzmigu.cn

JS:   arr.push(4);
来源：http://sx.hnjuh.cn

TS:   arr.push(4);
来源：http://rj.jctech888.com.cn

Java: list.add(4);
来源：http://jn.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://rd.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://vt.9csxet.cn

C#:   list.Add(4);
来源：http://mg.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://me.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://bv.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://es.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://id.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://ty.panjiajie.cn

Java: list.add(0, 0);
来源：http://jx.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wn.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ok.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://ns.yuntaijiaju.cn

[D04] 删除元素
来源：http://ts.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zv.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qk.szsharing.cn


<!-- 参考信息 -->