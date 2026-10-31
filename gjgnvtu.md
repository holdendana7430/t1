代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tt.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://af.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ni.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://og.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://af.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ee.haigaiapp.cn

[B03] switch / match / case
来源：http://vv.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ta.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kv.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bb.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tl.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ca.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://js.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yf.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qj.shtwfgs.cn

[B04] for 计数循环
来源：http://gv.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://jc.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oz.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tg.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ny.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uv.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fj.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://mt.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ng.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://ib.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://im.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://va.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ij.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xa.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eo.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vz.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://uu.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tl.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://ff.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gf.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fx.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lj.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zf.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sy.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ns.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kt.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ac.wgjwhj.cn

[B07] while 循环
来源：http://hx.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://bn.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uk.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://zq.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://bv.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://at.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tn.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://dd.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://iv.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://id.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://vr.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ec.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://il.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://fl.521024.cn

Java: do { i++; } while (i < 10);
来源：http://jp.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hg.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jt.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://vr.nicolike.cn

[B09] break 与 continue
来源：http://cp.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sl.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wi.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yz.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nf.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pe.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mp.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cl.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xr.hahajie.cn

[B10] 遍历同时拿索引
来源：http://rp.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mr.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://di.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://px.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rv.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://he.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ii.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dl.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ma.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://jf.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ne.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://er.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ji.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ay.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dr.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oo.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://rg.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cn.colortex.cn

[B12] 跳出多层循环
来源：http://rq.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gi.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://np.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tj.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pt.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qx.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mg.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iw.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lk.yuexingan06.cn

[B13] 判断是否为数字
来源：http://ua.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://xe.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://rh.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pt.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://et.bookmarksfly.cn

Java: x instanceof Number
来源：http://wc.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xx.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://ab.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://ol.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://ol.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xw.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pi.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://nb.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://tq.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ti.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gw.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ee.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cf.hnjuh.cn

[B15] 布尔运算与取反
来源：http://yz.bjjhwx.cn

Py:   a and b or not c
来源：http://rx.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://yw.shxzskj.cn

JS:   a && b || !c
来源：http://df.asd995.cn

TS:   a && b || !c
来源：http://rx.nszjky.cn

Java: a && b || !c
来源：http://tm.huixiangedu.cn

Go:   a && b || !c
来源：http://kt.newstarts.cn

Ruby: a && b || !c
来源：http://pe.wgjwhj.cn

C#:   a && b || !c
来源：http://gd.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://no.521024.cn

Py:   if not data: return
来源：http://gh.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://qa.9csxet.cn

JS:   if (!data) return;
来源：http://vc.szsharing.cn

TS:   if (!data) return;
来源：http://eo.chemitech.net.cn

Java: if (data == null) return;
来源：http://on.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://kr.jctech888.com.cn

Ruby: return if data.nil?
来源：http://kh.muxihuayi.cn

C#:   if (data == null) return;
来源：http://sa.jctech888.com.cn

================================================================================
来源：http://ml.muxihuayi.cn

C. 函数与作用域
来源：http://py.nszjky.cn

================================================================================
来源：http://gl.nicolike.cn

[C01] 定义函数
来源：http://mp.colortex.cn

Py:   def add(a, b): return a + b
来源：http://ou.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gj.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://pg.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://os.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bu.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wb.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://lu.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rz.jctech888.com.cn

[C02] 默认参数
来源：http://wn.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://eb.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yj.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://mz.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uj.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yb.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dy.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://lf.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://xs.chemitech.net.cn

[C03] 可变参数
来源：http://nh.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://fl.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zw.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oc.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pr.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hb.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xh.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bd.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qo.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://cx.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://il.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cl.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vk.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wc.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://ci.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://mu.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://ru.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://xl.nszjky.cn

[C05] 返回多个值
来源：http://dr.hahajie.cn

Py:   return a, b
来源：http://bj.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://bk.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qc.hnjuh.cn

TS:   return { a, b };
来源：http://cf.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oq.szsharing.cn

Go:   return a, b
来源：http://zy.muxihuayi.cn

Ruby: return a, b
来源：http://it.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://ap.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://ma.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://ia.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://km.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://qq.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://rg.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dk.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jl.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://no.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cj.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://lc.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://it.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tp.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lk.colortex.cn

TS:   arr.map(String)
来源：http://zh.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hi.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xy.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://zv.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sr.colortex.cn

[C08] 闭包
来源：http://gf.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tq.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nv.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cz.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fd.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rh.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hv.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ms.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ep.bjjhwx.cn

[C09] 递归
来源：http://vd.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cu.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ku.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dh.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ia.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ec.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ki.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gw.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://do.newstarts.cn

[C10] 变量作用域
来源：http://ox.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://za.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nz.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sg.gzmigu.cn

TS:   同 JS
来源：http://hi.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://jf.bjjhwx.cn

Go:   花括号块级作用域
来源：http://fi.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vr.yuexingan06.cn

C#:   块级作用域
来源：http://gd.jctech888.com.cn

[C11] 模块导入与导出
来源：http://lu.newstarts.cn

Py:   from module import func
来源：http://vb.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qt.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ci.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wp.shxzukj.cn

Java: import java.util.List;
来源：http://wy.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ez.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://bg.9csxet.cn

C#:   using System.Text;
来源：http://je.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://wr.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://ug.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://pr.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://dm.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://zf.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qe.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://tp.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://mm.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ll.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://gh.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mt.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://th.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oh.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://od.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ax.colortex.cn

Go:   func add(a, b int) int
来源：http://xv.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rf.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lq.nicolike.cn

[C14] 泛型函数
来源：http://qv.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rp.nszjky.cn

PHP:  // 无泛型
来源：http://wz.newstarts.cn

JS:   // 无泛型
来源：http://zu.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://st.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sm.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mg.jctech888.com.cn

Ruby: # 无泛型
来源：http://vs.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://io.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://dw.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qa.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://gl.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ji.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cn.huanxung.cn

Java: // 无解构
来源：http://xk.szsharing.cn

Go:   // 无解构
来源：http://gc.gzmigu.cn

Ruby: a, b = pair
来源：http://oz.szsharing.cn

C#:   var (a, b) = pair;
来源：http://ej.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://ze.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nq.9csxet.cn

PHP:  // 无重载
来源：http://wu.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://te.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://sa.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ze.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://eb.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://tg.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zg.newstarts.cn

================================================================================
来源：http://lj.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://hj.wgjwhj.cn

================================================================================
来源：http://rx.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://bq.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xf.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hq.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ch.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pe.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pp.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://sl.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://dt.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jx.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://hm.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qv.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cu.hnjuh.cn

JS:   arr.push(4);
来源：http://wx.huixiangedu.cn

TS:   arr.push(4);
来源：http://cj.bjjhwx.cn

Java: list.add(4);
来源：http://yf.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://wf.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://fe.shxzukj.cn

C#:   list.Add(4);
来源：http://tl.bookmarksfly.cn


<!-- 参考信息 -->