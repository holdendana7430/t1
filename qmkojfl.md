代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tp.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uv.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wj.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qm.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ti.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://as.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gz.hahajie.cn

[B04] for 计数循环
来源：http://hs.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://dc.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hq.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yy.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ox.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pk.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tx.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://mn.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cp.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://fd.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://wz.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ii.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yt.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ml.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mf.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oy.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://mu.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ca.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://rb.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cu.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vr.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tt.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ur.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uq.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uz.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fl.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wi.szxytkj.cn

[B07] while 循环
来源：http://be.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://ur.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ot.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://gx.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://wa.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://jt.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fh.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://kw.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://wz.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://wy.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://rl.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sg.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://ng.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://fw.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://pv.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ln.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rn.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://qp.asd995.cn

[B09] break 与 continue
来源：http://ih.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yn.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cs.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rr.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kk.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bb.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tr.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://am.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ne.newstarts.cn

[B10] 遍历同时拿索引
来源：http://fc.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xy.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pq.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mm.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://id.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zb.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://de.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fb.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://th.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://pb.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://vn.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://yl.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eg.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jw.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yk.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rx.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://hs.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yw.panjiajie.cn

[B12] 跳出多层循环
来源：http://up.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ez.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wh.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xa.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hu.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ib.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aj.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kr.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ag.shxzskj.cn

[B13] 判断是否为数字
来源：http://um.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://rk.lnxyls.cn

PHP:  is_numeric($x)
来源：http://zo.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://el.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wn.521024.cn

Java: x instanceof Number
来源：http://lw.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zu.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://na.gzmigu.cn

C#:   x is int or double or decimal
来源：http://qm.asd995.cn

[B14] 判断值是否在集合内
来源：http://le.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iu.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hn.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://gm.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://eu.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ul.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ir.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ao.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tg.szxytkj.cn

[B15] 布尔运算与取反
来源：http://aj.muxihuayi.cn

Py:   a and b or not c
来源：http://br.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://tb.szsharing.cn

JS:   a && b || !c
来源：http://cc.szsharing.cn

TS:   a && b || !c
来源：http://xr.lnxyls.cn

Java: a && b || !c
来源：http://jl.szsharing.cn

Go:   a && b || !c
来源：http://qv.nszjky.cn

Ruby: a && b || !c
来源：http://mn.huanxung.cn

C#:   a && b || !c
来源：http://wu.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jg.huixinmuqiang.cn

Py:   if not data: return
来源：http://jf.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://yv.gzmigu.cn

JS:   if (!data) return;
来源：http://pi.huanxung.cn

TS:   if (!data) return;
来源：http://ri.szxytkj.cn

Java: if (data == null) return;
来源：http://of.newstarts.cn

Go:   if data == nil { return }
来源：http://ft.nicolike.cn

Ruby: return if data.nil?
来源：http://zz.hnjuh.cn

C#:   if (data == null) return;
来源：http://ja.yuntaijiaju.cn

================================================================================
来源：http://mz.shxzskj.cn

C. 函数与作用域
来源：http://bj.nszjky.cn

================================================================================
来源：http://aw.bookmarksfly.cn

[C01] 定义函数
来源：http://yw.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://kw.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zj.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://mv.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qn.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oe.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ut.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://px.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://go.hahajie.cn

[C02] 默认参数
来源：http://lf.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://xg.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gc.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ds.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pg.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rz.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gt.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://rv.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://oo.jctech888.com.cn

[C03] 可变参数
来源：http://ch.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://vl.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zr.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ra.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ol.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fw.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qp.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gz.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://op.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://fu.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zn.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rm.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lo.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uu.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://lb.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://ho.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://sq.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://gp.shxzskj.cn

[C05] 返回多个值
来源：http://iz.szsharing.cn

Py:   return a, b
来源：http://ei.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://et.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ac.haigaiapp.cn

TS:   return { a, b };
来源：http://sg.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mg.lnxyls.cn

Go:   return a, b
来源：http://xf.hahajie.cn

Ruby: return a, b
来源：http://op.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://gf.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://vn.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://ux.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oa.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://pk.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://bv.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pu.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pe.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://mv.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://na.szsharing.cn

[C07] 把函数作为参数传入
来源：http://hv.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cd.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qr.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wy.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://bk.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://av.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gk.521024.cn

Ruby: arr.map(&:upcase)
来源：http://kl.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tv.hnjuh.cn

[C08] 闭包
来源：http://gq.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fi.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fk.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nu.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pe.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ow.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oi.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pj.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yv.jctech888.com.cn

[C09] 递归
来源：http://tc.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kl.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ds.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lo.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bd.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://du.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kg.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yj.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eh.szxytkj.cn

[C10] 变量作用域
来源：http://by.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bu.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cw.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yl.9csxet.cn

TS:   同 JS
来源：http://gm.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://kr.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://gc.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://km.521024.cn

C#:   块级作用域
来源：http://uf.nszjky.cn

[C11] 模块导入与导出
来源：http://mg.yuntaijiaju.cn

Py:   from module import func
来源：http://cr.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kh.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yh.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zz.newstarts.cn

Java: import java.util.List;
来源：http://vn.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rf.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://lj.bjjhwx.cn

C#:   using System.Text;
来源：http://qr.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://hj.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://ui.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://cc.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://zy.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://pd.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mg.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://zs.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://bx.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gp.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://rj.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vt.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ty.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fn.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ri.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bl.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ci.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uj.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zq.yuexingan06.cn

[C14] 泛型函数
来源：http://zu.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jy.szsharing.cn

PHP:  // 无泛型
来源：http://wn.szsharing.cn

JS:   // 无泛型
来源：http://zt.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ly.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gv.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jh.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://rh.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ro.colortex.cn

[C15] 解构 / 展开参数
来源：http://cg.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xo.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://ka.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ns.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rj.asd995.cn

Java: // 无解构
来源：http://lk.szxytkj.cn

Go:   // 无解构
来源：http://vx.szxytkj.cn

Ruby: a, b = pair
来源：http://oo.nicolike.cn

C#:   var (a, b) = pair;
来源：http://qm.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://nq.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hl.panjiajie.cn

PHP:  // 无重载
来源：http://qa.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vz.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://gv.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mq.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://nr.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://mj.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wz.huixinmuqiang.cn

================================================================================
来源：http://uu.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://gk.huanxung.cn

================================================================================
来源：http://uf.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://cj.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yy.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lw.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oa.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pz.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xi.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://yb.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://pp.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nh.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://zx.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ec.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pn.haigaiapp.cn

JS:   arr.push(4);
来源：http://qh.lnxyls.cn

TS:   arr.push(4);
来源：http://oq.asd995.cn

Java: list.add(4);
来源：http://fd.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://oa.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://oy.yuexingan06.cn

C#:   list.Add(4);
来源：http://sy.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://kf.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://gp.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zs.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ln.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://ys.haigaiapp.cn

Java: list.add(0, 0);
来源：http://fo.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ix.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zb.yuexingan06.cn


<!-- 参考信息 -->