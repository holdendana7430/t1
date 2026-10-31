代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ej.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://et.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jt.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ry.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vm.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ll.colortex.cn

[B03] switch / match / case
来源：http://ek.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ik.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mf.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ft.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yf.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lw.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://an.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ia.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wm.nszjky.cn

[B04] for 计数循环
来源：http://xg.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://ap.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xr.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nt.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ig.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cx.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yg.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://th.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://df.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://ln.9csxet.cn

Py:   for item in arr: print(item)
来源：http://wv.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jg.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://at.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vy.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://de.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bp.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://pn.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pr.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://bo.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zt.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://or.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tu.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aa.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ux.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uo.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ej.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oc.huanxung.cn

[B07] while 循环
来源：http://tr.newstarts.cn

Py:   while i < 10: i += 1
来源：http://px.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qw.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://uu.521024.cn

TS:   while (i < 10) { i++; }
来源：http://zx.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://ao.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rc.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://hd.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://ou.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://du.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://yy.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ii.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://bk.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://ld.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://kq.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kk.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xf.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://an.colortex.cn

[B09] break 与 continue
来源：http://gq.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://id.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ug.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hl.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xi.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kz.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ba.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qz.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wx.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://or.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ge.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jx.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tb.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uw.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gh.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zb.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pe.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ov.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://xm.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://fe.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://xd.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oj.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ag.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pb.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ou.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://kb.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zn.gzmigu.cn

[B12] 跳出多层循环
来源：http://vr.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gz.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mc.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sc.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dr.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zf.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qr.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://er.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gm.newstarts.cn

[B13] 判断是否为数字
来源：http://su.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://mh.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://ho.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pq.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kl.lnxyls.cn

Java: x instanceof Number
来源：http://hw.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fl.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://hb.shxzukj.cn

C#:   x is int or double or decimal
来源：http://zs.szsharing.cn

[B14] 判断值是否在集合内
来源：http://fe.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://el.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sx.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://pi.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://op.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mx.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gp.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jf.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lw.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://xj.newstarts.cn

Py:   a and b or not c
来源：http://af.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://yp.yuexingan06.cn

JS:   a && b || !c
来源：http://gc.szxytkj.cn

TS:   a && b || !c
来源：http://uu.asd995.cn

Java: a && b || !c
来源：http://vi.lnxyls.cn

Go:   a && b || !c
来源：http://ii.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://nr.shtwfgs.cn

C#:   a && b || !c
来源：http://vc.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://as.gzmigu.cn

Py:   if not data: return
来源：http://ep.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://bm.shtwfgs.cn

JS:   if (!data) return;
来源：http://px.521024.cn

TS:   if (!data) return;
来源：http://ih.muxihuayi.cn

Java: if (data == null) return;
来源：http://cp.nicolike.cn

Go:   if data == nil { return }
来源：http://hn.jctech888.com.cn

Ruby: return if data.nil?
来源：http://sd.9csxet.cn

C#:   if (data == null) return;
来源：http://jr.bjjhwx.cn

================================================================================
来源：http://ut.9csxet.cn

C. 函数与作用域
来源：http://il.asd995.cn

================================================================================
来源：http://vv.newstarts.cn

[C01] 定义函数
来源：http://ix.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://zy.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fp.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://qg.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fi.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rf.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eo.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://li.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qd.wgjwhj.cn

[C02] 默认参数
来源：http://mh.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://xq.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://am.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://yz.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://is.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tk.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uv.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://ae.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://gr.chemitech.net.cn

[C03] 可变参数
来源：http://vw.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://ny.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mf.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pr.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kp.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://li.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ez.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bj.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mf.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://kl.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bi.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://um.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yh.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nv.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://rf.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://dp.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://my.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://ym.hahajie.cn

[C05] 返回多个值
来源：http://cp.chemitech.net.cn

Py:   return a, b
来源：http://uj.shxzukj.cn

PHP:  return [$a, $b];
来源：http://ip.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nj.jctech888.com.cn

TS:   return { a, b };
来源：http://xe.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xa.huixiangedu.cn

Go:   return a, b
来源：http://ew.nicolike.cn

Ruby: return a, b
来源：http://in.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ib.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://nj.nszjky.cn

Py:   square = lambda x: x * x
来源：http://ip.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bl.521024.cn

JS:   const square = x => x * x;
来源：http://vt.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://kw.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dy.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://un.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://bp.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bz.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://aq.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uc.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pt.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ed.yuexingan06.cn

TS:   arr.map(String)
来源：http://tj.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rj.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ao.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://yb.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pc.shtwfgs.cn

[C08] 闭包
来源：http://hr.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ft.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ai.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ca.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wa.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yp.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://du.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iy.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mh.colortex.cn

[C09] 递归
来源：http://rx.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hc.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kk.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rr.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qk.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wk.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ba.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jn.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oi.shxzskj.cn

[C10] 变量作用域
来源：http://ot.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sa.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lx.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fv.shtwfgs.cn

TS:   同 JS
来源：http://td.nicolike.cn

Java: 方法内为块级作用域
来源：http://as.huixiangedu.cn

Go:   花括号块级作用域
来源：http://jl.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fd.huixinmuqiang.cn

C#:   块级作用域
来源：http://km.colortex.cn

[C11] 模块导入与导出
来源：http://nh.shxzskj.cn

Py:   from module import func
来源：http://mi.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bm.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xg.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dc.huixiangedu.cn

Java: import java.util.List;
来源：http://pb.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ib.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://le.wgjwhj.cn

C#:   using System.Text;
来源：http://mm.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://nf.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://bg.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://as.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://ig.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://xz.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nd.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://yj.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://be.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qx.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://fu.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://li.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mx.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fy.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eu.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jw.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://ia.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zj.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nw.bookmarksfly.cn

[C14] 泛型函数
来源：http://eh.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://om.wgjwhj.cn

PHP:  // 无泛型
来源：http://cn.9csxet.cn

JS:   // 无泛型
来源：http://qx.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ot.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bc.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ty.haigaiapp.cn

Ruby: # 无泛型
来源：http://qr.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kh.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://of.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dt.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://db.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oc.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ez.colortex.cn

Java: // 无解构
来源：http://le.bjjhwx.cn

Go:   // 无解构
来源：http://ug.hnjuh.cn

Ruby: a, b = pair
来源：http://ng.asd995.cn

C#:   var (a, b) = pair;
来源：http://lw.newstarts.cn

[C16] 函数 / 方法重载
来源：http://sy.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ui.chemitech.net.cn

PHP:  // 无重载
来源：http://ey.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vf.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://ts.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ui.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://wl.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://eb.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ch.9csxet.cn

================================================================================
来源：http://ju.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://td.shxzukj.cn

================================================================================
来源：http://nk.asd995.cn

[D01] 创建数组 / 列表
来源：http://mp.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://um.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zr.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://or.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eq.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rs.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://nv.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://sm.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mp.hahajie.cn

[D02] 追加元素到末尾
来源：http://mb.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ah.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://br.hahajie.cn

JS:   arr.push(4);
来源：http://sm.shxzskj.cn

TS:   arr.push(4);
来源：http://gp.hnjuh.cn

Java: list.add(4);
来源：http://cg.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://ii.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://qz.shxzskj.cn

C#:   list.Add(4);
来源：http://ne.jianghongdianzi.cn


<!-- 参考信息 -->