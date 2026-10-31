代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://by.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://de.yuexingan06.cn

[B03] switch / match / case
来源：http://ng.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qt.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://db.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qv.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cg.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zd.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jd.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yk.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ga.jianghongdianzi.cn

[B04] for 计数循环
来源：http://md.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://hh.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kq.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://se.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tm.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://my.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sy.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://gg.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gq.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://je.nszjky.cn

Py:   for item in arr: print(item)
来源：http://fr.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ol.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bo.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xe.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qd.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ze.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://sl.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vw.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://fh.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jv.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dw.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pp.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://my.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kn.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rh.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wg.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hd.szsharing.cn

[B07] while 循环
来源：http://li.huanxung.cn

Py:   while i < 10: i += 1
来源：http://an.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tm.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://bi.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://lv.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://xn.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cm.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://rr.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://pf.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://ng.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://rj.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ov.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://qa.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://zl.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://vh.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pa.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vv.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://df.wgjwhj.cn

[B09] break 与 continue
来源：http://un.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vl.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ep.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hp.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hw.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://op.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sy.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sc.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://yw.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vc.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bq.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vj.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fr.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pv.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dq.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uy.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ig.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://vs.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://sj.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://ol.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gz.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bp.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iy.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cm.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://le.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nu.szsharing.cn

[B12] 跳出多层循环
来源：http://vl.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ug.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jh.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yl.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ha.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qr.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bn.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kr.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://as.9csxet.cn

[B13] 判断是否为数字
来源：http://is.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://ak.nszjky.cn

PHP:  is_numeric($x)
来源：http://nb.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pv.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oe.yuexingan06.cn

Java: x instanceof Number
来源：http://ou.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jq.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://my.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://dx.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://ma.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://te.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dg.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://jk.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://uj.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lq.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zr.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yn.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ny.szsharing.cn

[B15] 布尔运算与取反
来源：http://po.szxytkj.cn

Py:   a and b or not c
来源：http://wq.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://or.haigaiapp.cn

JS:   a && b || !c
来源：http://aq.yuntaijiaju.cn

TS:   a && b || !c
来源：http://yd.nszjky.cn

Java: a && b || !c
来源：http://pl.shtwfgs.cn

Go:   a && b || !c
来源：http://ui.gzmigu.cn

Ruby: a && b || !c
来源：http://vn.yuexingan06.cn

C#:   a && b || !c
来源：http://iv.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lu.jctech888.com.cn

Py:   if not data: return
来源：http://zs.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://bs.bookmarksfly.cn

JS:   if (!data) return;
来源：http://ni.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://cd.huixiangedu.cn

Java: if (data == null) return;
来源：http://zn.shxzukj.cn

Go:   if data == nil { return }
来源：http://op.newstarts.cn

Ruby: return if data.nil?
来源：http://xa.hahajie.cn

C#:   if (data == null) return;
来源：http://su.yuntaijiaju.cn

================================================================================
来源：http://bg.colortex.cn

C. 函数与作用域
来源：http://ko.yuexingan06.cn

================================================================================
来源：http://lh.jianghongdianzi.cn

[C01] 定义函数
来源：http://by.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://xx.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dl.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://kj.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rh.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ns.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ba.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://us.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qd.jianghongdianzi.cn

[C02] 默认参数
来源：http://sf.asd995.cn

Py:   def greet(name="World"): return name
来源：http://le.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jo.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://fa.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qd.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qx.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gt.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://dw.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://wu.521024.cn

[C03] 可变参数
来源：http://ob.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://za.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bs.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://na.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cg.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nb.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gk.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tx.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ml.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://za.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wf.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jb.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qs.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nk.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://wn.521024.cn

Go:   // 无：用配置结构体参数
来源：http://ld.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://lm.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://lc.bookmarksfly.cn

[C05] 返回多个值
来源：http://zm.yuntaijiaju.cn

Py:   return a, b
来源：http://tw.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://ca.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ma.colortex.cn

TS:   return { a, b };
来源：http://ye.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vv.huixinmuqiang.cn

Go:   return a, b
来源：http://ta.colortex.cn

Ruby: return a, b
来源：http://qh.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ik.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://lt.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://et.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://td.nszjky.cn

JS:   const square = x => x * x;
来源：http://bz.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://ht.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sb.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ge.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://ff.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jk.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://ug.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vb.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yb.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vv.bookmarksfly.cn

TS:   arr.map(String)
来源：http://wd.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ig.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ur.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://nw.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qd.szxytkj.cn

[C08] 闭包
来源：http://qo.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qg.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bo.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dv.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://is.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rg.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lo.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hn.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cz.huixiangedu.cn

[C09] 递归
来源：http://hp.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jx.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vz.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cj.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zl.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xt.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://he.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eq.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://db.shxzukj.cn

[C10] 变量作用域
来源：http://sr.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nk.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qy.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uq.shxzskj.cn

TS:   同 JS
来源：http://wz.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://rq.asd995.cn

Go:   花括号块级作用域
来源：http://wz.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mv.jianghongdianzi.cn

C#:   块级作用域
来源：http://bu.gzmigu.cn

[C11] 模块导入与导出
来源：http://gl.panjiajie.cn

Py:   from module import func
来源：http://vl.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qo.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yq.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jd.yuntaijiaju.cn

Java: import java.util.List;
来源：http://uv.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kh.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://ds.colortex.cn

C#:   using System.Text;
来源：http://qo.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://ol.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://kf.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://yj.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://df.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://fd.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oy.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://cx.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://ki.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ld.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://el.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fu.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fm.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tx.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ia.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vq.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://qk.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://js.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pd.asd995.cn

[C14] 泛型函数
来源：http://jb.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ut.bjjhwx.cn

PHP:  // 无泛型
来源：http://ms.szsharing.cn

JS:   // 无泛型
来源：http://jv.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fq.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hy.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dl.szxytkj.cn

Ruby: # 无泛型
来源：http://pt.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vh.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://zj.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wd.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ir.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bw.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ia.haigaiapp.cn

Java: // 无解构
来源：http://gd.shtwfgs.cn

Go:   // 无解构
来源：http://tu.yuexingan06.cn

Ruby: a, b = pair
来源：http://lf.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://zq.newstarts.cn

[C16] 函数 / 方法重载
来源：http://sr.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dt.asd995.cn

PHP:  // 无重载
来源：http://tx.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vp.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://zb.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://en.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://co.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://dd.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tj.lnxyls.cn

================================================================================
来源：http://uy.521024.cn

D. 数组 / 列表 / 集合
来源：http://yo.asd995.cn

================================================================================
来源：http://xp.nszjky.cn

[D01] 创建数组 / 列表
来源：http://ok.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dj.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rp.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ua.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://es.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zs.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://ic.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://sa.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.szsharing.cn

[D02] 追加元素到末尾
来源：http://mj.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vm.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tf.yuexingan06.cn

JS:   arr.push(4);
来源：http://wj.jctech888.com.cn

TS:   arr.push(4);
来源：http://ro.nszjky.cn

Java: list.add(4);
来源：http://of.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://kd.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://ym.bookmarksfly.cn

C#:   list.Add(4);
来源：http://kf.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://av.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://xf.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wh.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ij.9csxet.cn


<!-- 参考信息 -->