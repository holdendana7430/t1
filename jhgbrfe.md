代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ft.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vv.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yv.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rp.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://up.lnxyls.cn

[B03] switch / match / case
来源：http://jp.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kx.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ou.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zq.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ap.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ax.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xn.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qf.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xq.9csxet.cn

[B04] for 计数循环
来源：http://lx.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://km.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mv.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lv.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pk.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hh.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kj.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://ys.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eg.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://ar.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://om.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ug.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://en.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fl.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tl.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qs.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://gx.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hl.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://qc.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eg.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fb.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://do.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ob.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cr.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yk.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ra.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ej.colortex.cn

[B07] while 循环
来源：http://sy.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://ki.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jp.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://dl.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://cm.asd995.cn

Java: while (i < 10) { i++; }
来源：http://ba.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sc.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://fv.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://hu.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://ph.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://sk.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vx.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://tn.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://jp.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://mc.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pu.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ti.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://sj.huixinmuqiang.cn

[B09] break 与 continue
来源：http://li.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gh.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zi.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zz.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fl.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://br.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rl.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ln.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nf.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ol.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oh.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://az.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://im.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fg.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ja.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kr.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xq.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nv.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://nf.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://du.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://to.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nd.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lf.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://en.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rx.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://mg.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wj.huixiangedu.cn

[B12] 跳出多层循环
来源：http://hh.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qx.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bd.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nw.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yd.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ka.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yj.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ka.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://al.hnjuh.cn

[B13] 判断是否为数字
来源：http://qs.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://aa.521024.cn

PHP:  is_numeric($x)
来源：http://gq.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gq.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cr.szxytkj.cn

Java: x instanceof Number
来源：http://wo.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yr.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://cp.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ft.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://zn.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nm.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://co.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://fo.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://wf.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ya.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lo.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://er.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sh.szxytkj.cn

[B15] 布尔运算与取反
来源：http://fz.wgjwhj.cn

Py:   a and b or not c
来源：http://bx.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://tx.nicolike.cn

JS:   a && b || !c
来源：http://co.asd995.cn

TS:   a && b || !c
来源：http://by.colortex.cn

Java: a && b || !c
来源：http://ru.shxzukj.cn

Go:   a && b || !c
来源：http://kf.hnjuh.cn

Ruby: a && b || !c
来源：http://ip.lnxyls.cn

C#:   a && b || !c
来源：http://pe.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mc.huanxung.cn

Py:   if not data: return
来源：http://xu.521024.cn

PHP:  if (!$data) { return; }
来源：http://mq.szxytkj.cn

JS:   if (!data) return;
来源：http://cz.asd995.cn

TS:   if (!data) return;
来源：http://oj.lnxyls.cn

Java: if (data == null) return;
来源：http://sp.colortex.cn

Go:   if data == nil { return }
来源：http://ks.haigaiapp.cn

Ruby: return if data.nil?
来源：http://lz.muxihuayi.cn

C#:   if (data == null) return;
来源：http://dw.newstarts.cn

================================================================================
来源：http://co.521024.cn

C. 函数与作用域
来源：http://wu.521024.cn

================================================================================
来源：http://jp.panjiajie.cn

[C01] 定义函数
来源：http://zn.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://xr.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hh.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://wx.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ho.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hc.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dc.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://ts.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lr.haigaiapp.cn

[C02] 默认参数
来源：http://in.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://yy.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vh.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://di.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hk.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ac.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pt.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://zg.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://kr.nicolike.cn

[C03] 可变参数
来源：http://iv.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://kz.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hp.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fv.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ri.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yx.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ix.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://in.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pc.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://pz.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://we.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mw.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eq.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jd.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://gq.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://rt.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://qf.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://gm.bookmarksfly.cn

[C05] 返回多个值
来源：http://xy.wgjwhj.cn

Py:   return a, b
来源：http://ny.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://dw.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sx.nszjky.cn

TS:   return { a, b };
来源：http://li.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lo.gzmigu.cn

Go:   return a, b
来源：http://xq.lnxyls.cn

Ruby: return a, b
来源：http://qi.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://fn.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://kv.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://ju.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kj.colortex.cn

JS:   const square = x => x * x;
来源：http://vp.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://nh.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vr.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uy.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://iq.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rz.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://ta.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jb.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ky.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gg.wgjwhj.cn

TS:   arr.map(String)
来源：http://qi.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mt.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bl.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://jk.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hl.521024.cn

[C08] 闭包
来源：http://bq.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tn.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sz.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oo.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cp.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ub.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wh.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vi.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mq.521024.cn

[C09] 递归
来源：http://yp.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xh.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ed.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lr.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hx.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bz.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qg.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://na.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sx.bjjhwx.cn

[C10] 变量作用域
来源：http://wl.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bo.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ex.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hg.bjjhwx.cn

TS:   同 JS
来源：http://id.panjiajie.cn

Java: 方法内为块级作用域
来源：http://zb.huixiangedu.cn

Go:   花括号块级作用域
来源：http://bs.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lx.newstarts.cn

C#:   块级作用域
来源：http://wo.muxihuayi.cn

[C11] 模块导入与导出
来源：http://bs.huixiangedu.cn

Py:   from module import func
来源：http://gy.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://km.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qb.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hn.gzmigu.cn

Java: import java.util.List;
来源：http://qs.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vs.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://pn.asd995.cn

C#:   using System.Text;
来源：http://ry.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://mr.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://uh.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://ok.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://ap.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://zw.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kd.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://qh.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://mw.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ys.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://xa.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tp.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sa.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tj.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cv.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lm.szxytkj.cn

Go:   func add(a, b int) int
来源：http://uh.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hl.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yu.hnjuh.cn

[C14] 泛型函数
来源：http://ip.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lm.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://vi.nicolike.cn

JS:   // 无泛型
来源：http://fq.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zj.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qo.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zq.panjiajie.cn

Ruby: # 无泛型
来源：http://tz.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jp.nicolike.cn

[C15] 解构 / 展开参数
来源：http://hd.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ns.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://be.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bq.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pl.jianghongdianzi.cn

Java: // 无解构
来源：http://kd.nicolike.cn

Go:   // 无解构
来源：http://gl.9csxet.cn

Ruby: a, b = pair
来源：http://uo.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://vn.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://ps.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hv.nszjky.cn

PHP:  // 无重载
来源：http://ni.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vd.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ds.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ak.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://kl.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://nh.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dp.shxzskj.cn

================================================================================
来源：http://iz.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://wg.wgjwhj.cn

================================================================================
来源：http://xd.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://fa.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zb.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gv.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qa.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gb.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kk.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://tc.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://aq.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fs.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://xj.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://om.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uy.chemitech.net.cn

JS:   arr.push(4);
来源：http://wz.szxytkj.cn

TS:   arr.push(4);
来源：http://mh.shtwfgs.cn

Java: list.add(4);
来源：http://do.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://sv.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://dm.nicolike.cn

C#:   list.Add(4);
来源：http://pt.szxytkj.cn


<!-- 参考信息 -->