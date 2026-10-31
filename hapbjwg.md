代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ot.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bk.asd995.cn

[B03] switch / match / case
来源：http://cn.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qg.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rm.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yd.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zy.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rs.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://de.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zt.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wy.shxzskj.cn

[B04] for 计数循环
来源：http://eg.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://sb.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://od.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hl.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hr.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vs.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gu.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://co.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ry.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://yu.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://en.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lp.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cj.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://og.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qo.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kp.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://gk.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tt.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ks.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://np.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hv.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lx.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yw.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gc.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://js.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sx.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ik.chemitech.net.cn

[B07] while 循环
来源：http://iw.colortex.cn

Py:   while i < 10: i += 1
来源：http://kz.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xa.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://fg.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://qi.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://qx.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qj.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://vl.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://bp.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://vq.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://xx.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aw.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://et.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://gz.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://rl.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gb.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uh.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://uu.hnjuh.cn

[B09] break 与 continue
来源：http://rp.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qt.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pr.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ih.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gq.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vp.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vc.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uy.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://pn.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rc.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zb.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qd.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xo.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ex.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uj.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rf.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vq.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://ya.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://xv.asd995.cn

PHP:  range(0, 10, 2);
来源：http://hj.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gc.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ef.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://da.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tf.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://zj.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ed.jctech888.com.cn

[B12] 跳出多层循环
来源：http://hq.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://st.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pu.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://om.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ch.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ky.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ah.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tu.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fc.huanxung.cn

[B13] 判断是否为数字
来源：http://sz.521024.cn

Py:   isinstance(x, (int, float))
来源：http://gy.panjiajie.cn

PHP:  is_numeric($x)
来源：http://va.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ua.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gi.muxihuayi.cn

Java: x instanceof Number
来源：http://nl.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mt.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://fz.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://hc.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://jx.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pq.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vp.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://zp.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://td.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iy.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bl.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qx.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oy.hahajie.cn

[B15] 布尔运算与取反
来源：http://zq.nicolike.cn

Py:   a and b or not c
来源：http://uu.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://qs.muxihuayi.cn

JS:   a && b || !c
来源：http://lz.huixinmuqiang.cn

TS:   a && b || !c
来源：http://yy.shxzukj.cn

Java: a && b || !c
来源：http://jx.gzmigu.cn

Go:   a && b || !c
来源：http://qe.shxzukj.cn

Ruby: a && b || !c
来源：http://pn.bjjhwx.cn

C#:   a && b || !c
来源：http://du.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qd.chemitech.net.cn

Py:   if not data: return
来源：http://gm.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://oz.bjjhwx.cn

JS:   if (!data) return;
来源：http://ql.szsharing.cn

TS:   if (!data) return;
来源：http://ov.521024.cn

Java: if (data == null) return;
来源：http://wm.wgjwhj.cn

Go:   if data == nil { return }
来源：http://gi.wgjwhj.cn

Ruby: return if data.nil?
来源：http://hh.9csxet.cn

C#:   if (data == null) return;
来源：http://ou.shtwfgs.cn

================================================================================
来源：http://km.szsharing.cn

C. 函数与作用域
来源：http://xt.bjjhwx.cn

================================================================================
来源：http://ke.asd995.cn

[C01] 定义函数
来源：http://rf.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://sg.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://be.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://fk.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fu.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ys.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zr.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://he.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nv.hnjuh.cn

[C02] 默认参数
来源：http://jq.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://mx.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oc.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://ge.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ud.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nd.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pa.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://yy.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://ka.shxzskj.cn

[C03] 可变参数
来源：http://vg.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://zj.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gz.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xx.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gm.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xi.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ft.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gb.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gd.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://ow.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qz.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sz.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wo.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tf.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://bk.521024.cn

Go:   // 无：用配置结构体参数
来源：http://yy.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://uv.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://wy.asd995.cn

[C05] 返回多个值
来源：http://zd.wgjwhj.cn

Py:   return a, b
来源：http://ak.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://rz.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ij.colortex.cn

TS:   return { a, b };
来源：http://vv.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qt.huanxung.cn

Go:   return a, b
来源：http://dy.hnjuh.cn

Ruby: return a, b
来源：http://ee.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://gl.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://pc.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://bn.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mj.szsharing.cn

JS:   const square = x => x * x;
来源：http://dq.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://zk.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://go.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://od.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://iy.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cw.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://wy.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eu.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pg.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ti.jctech888.com.cn

TS:   arr.map(String)
来源：http://ay.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ls.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eo.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ek.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zd.lnxyls.cn

[C08] 闭包
来源：http://pa.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sx.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xj.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cj.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lw.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ir.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ql.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pu.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ls.asd995.cn

[C09] 递归
来源：http://jm.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gj.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zb.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aa.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fp.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yu.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qg.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xx.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zm.colortex.cn

[C10] 变量作用域
来源：http://ly.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qd.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bt.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://br.chemitech.net.cn

TS:   同 JS
来源：http://zp.gzmigu.cn

Java: 方法内为块级作用域
来源：http://ur.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://al.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yp.haigaiapp.cn

C#:   块级作用域
来源：http://rb.haigaiapp.cn

[C11] 模块导入与导出
来源：http://gs.9csxet.cn

Py:   from module import func
来源：http://dr.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dg.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xl.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xp.lnxyls.cn

Java: import java.util.List;
来源：http://eu.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vu.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ga.bookmarksfly.cn

C#:   using System.Text;
来源：http://ad.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://jk.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://rk.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ry.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://jw.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://hk.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cv.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://hf.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://mm.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dg.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://vp.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ie.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ln.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rj.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ro.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fi.lnxyls.cn

Go:   func add(a, b int) int
来源：http://ix.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gl.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rx.9csxet.cn

[C14] 泛型函数
来源：http://nj.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lx.haigaiapp.cn

PHP:  // 无泛型
来源：http://gz.huixiangedu.cn

JS:   // 无泛型
来源：http://su.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ni.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mu.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://no.newstarts.cn

Ruby: # 无泛型
来源：http://xs.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dx.colortex.cn

[C15] 解构 / 展开参数
来源：http://mg.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ua.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://sq.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fw.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.huixiangedu.cn

Java: // 无解构
来源：http://yk.colortex.cn

Go:   // 无解构
来源：http://yn.9csxet.cn

Ruby: a, b = pair
来源：http://er.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://qe.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://md.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lf.nicolike.cn

PHP:  // 无重载
来源：http://dz.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uw.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://tm.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vt.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://di.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://wx.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bw.panjiajie.cn

================================================================================
来源：http://uj.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://mw.nicolike.cn

================================================================================
来源：http://ng.szsharing.cn

[D01] 创建数组 / 列表
来源：http://no.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ho.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vc.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://am.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pl.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lb.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://vp.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://ef.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eo.shxzskj.cn

[D02] 追加元素到末尾
来源：http://ka.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://up.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kl.chemitech.net.cn

JS:   arr.push(4);
来源：http://ic.huanxung.cn

TS:   arr.push(4);
来源：http://rj.panjiajie.cn

Java: list.add(4);
来源：http://hc.521024.cn

Go:   arr = append(arr, 4)
来源：http://tv.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://or.jctech888.com.cn

C#:   list.Add(4);
来源：http://in.newstarts.cn

[D03] 在指定位置插入元素
来源：http://zc.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://hg.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yx.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://au.wgjwhj.cn


<!-- 参考信息 -->