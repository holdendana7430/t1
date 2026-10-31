代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tj.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://ki.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mq.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bx.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fa.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ud.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yy.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rt.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cz.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ts.asd995.cn

[B03] switch / match / case
来源：http://fu.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nc.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://py.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vh.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ld.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://up.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://os.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://od.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://be.newstarts.cn

[B04] for 计数循环
来源：http://qq.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://cc.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ti.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nz.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qq.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ev.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sn.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://bo.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ov.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://xp.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://rp.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zt.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ns.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nf.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jn.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vo.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://cr.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zu.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://la.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qw.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yh.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://md.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hj.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sb.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vj.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ok.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mp.yuntaijiaju.cn

[B07] while 循环
来源：http://te.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://vk.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://va.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://wx.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://zx.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://fm.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pk.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://gk.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://nb.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://zz.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://fl.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qv.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://uz.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://jy.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://wp.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zv.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sz.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://fw.huixiangedu.cn

[B09] break 与 continue
来源：http://ai.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qg.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mz.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nf.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://et.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tc.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ft.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bq.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rm.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://vw.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://si.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ko.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uu.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ze.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iu.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://po.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ff.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yn.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://co.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://mw.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://nl.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ie.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://al.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qz.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://si.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://zi.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kn.yuexingan06.cn

[B12] 跳出多层循环
来源：http://bp.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://md.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xp.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ns.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://me.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fz.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qq.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hi.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ei.szsharing.cn

[B13] 判断是否为数字
来源：http://aa.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://ci.szxytkj.cn

PHP:  is_numeric($x)
来源：http://qs.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://po.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wo.newstarts.cn

Java: x instanceof Number
来源：http://uq.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iy.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://qq.nszjky.cn

C#:   x is int or double or decimal
来源：http://ew.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://uy.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qo.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vg.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://fi.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://ei.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mj.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://an.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qa.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bw.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://ra.chemitech.net.cn

Py:   a and b or not c
来源：http://of.huanxung.cn

PHP:  $a && $b || !$c
来源：http://jo.shtwfgs.cn

JS:   a && b || !c
来源：http://oh.shxzskj.cn

TS:   a && b || !c
来源：http://au.yuntaijiaju.cn

Java: a && b || !c
来源：http://ts.muxihuayi.cn

Go:   a && b || !c
来源：http://ev.shxzskj.cn

Ruby: a && b || !c
来源：http://vs.asd995.cn

C#:   a && b || !c
来源：http://zc.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ij.muxihuayi.cn

Py:   if not data: return
来源：http://jm.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://jm.colortex.cn

JS:   if (!data) return;
来源：http://bg.bookmarksfly.cn

TS:   if (!data) return;
来源：http://pe.shxzskj.cn

Java: if (data == null) return;
来源：http://wq.chemitech.net.cn

Go:   if data == nil { return }
来源：http://xw.huixiangedu.cn

Ruby: return if data.nil?
来源：http://te.haigaiapp.cn

C#:   if (data == null) return;
来源：http://bb.shxzukj.cn

================================================================================
来源：http://nz.huixiangedu.cn

C. 函数与作用域
来源：http://ov.nicolike.cn

================================================================================
来源：http://tn.hahajie.cn

[C01] 定义函数
来源：http://cq.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://qw.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mg.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://ao.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ve.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cp.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wy.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://qa.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://az.colortex.cn

[C02] 默认参数
来源：http://ww.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://ka.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eq.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://xb.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tx.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fq.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mx.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://yx.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://go.colortex.cn

[C03] 可变参数
来源：http://wx.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://ac.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ae.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zn.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yb.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jk.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xc.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pi.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sn.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://ex.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wc.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ej.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rk.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vf.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://nq.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://df.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://yj.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://yj.jctech888.com.cn

[C05] 返回多个值
来源：http://gu.haigaiapp.cn

Py:   return a, b
来源：http://ad.szsharing.cn

PHP:  return [$a, $b];
来源：http://me.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lj.hnjuh.cn

TS:   return { a, b };
来源：http://vx.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://me.newstarts.cn

Go:   return a, b
来源：http://os.jianghongdianzi.cn

Ruby: return a, b
来源：http://rv.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://ky.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://th.newstarts.cn

Py:   square = lambda x: x * x
来源：http://dl.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ot.shxzskj.cn

JS:   const square = x => x * x;
来源：http://uc.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://ga.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kj.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://md.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://nr.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bn.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://en.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dj.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ou.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ka.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://my.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zk.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gd.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://yx.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jk.9csxet.cn

[C08] 闭包
来源：http://vm.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ul.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qt.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xc.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://px.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pe.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ua.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kl.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yp.haigaiapp.cn

[C09] 递归
来源：http://lo.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://az.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vj.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gz.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fy.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hl.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jm.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rm.gzmigu.cn

[C10] 变量作用域
来源：http://xt.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mt.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mb.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ig.szsharing.cn

TS:   同 JS
来源：http://yy.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://sy.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://mv.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yj.huixiangedu.cn

C#:   块级作用域
来源：http://sn.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://ji.asd995.cn

Py:   from module import func
来源：http://vt.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mn.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tb.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wq.521024.cn

Java: import java.util.List;
来源：http://cs.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sr.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://ka.yuntaijiaju.cn

C#:   using System.Text;
来源：http://sd.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://ay.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://jh.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://hc.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://ip.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://uu.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sb.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://cb.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://mg.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xv.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://iu.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hu.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hj.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ts.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lv.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bi.521024.cn

Go:   func add(a, b int) int
来源：http://vo.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jh.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dt.521024.cn

[C14] 泛型函数
来源：http://qw.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hk.hnjuh.cn

PHP:  // 无泛型
来源：http://ze.gzmigu.cn

JS:   // 无泛型
来源：http://kp.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kc.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ad.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eq.bookmarksfly.cn

Ruby: # 无泛型
来源：http://jp.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vw.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://yd.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cv.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://vc.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sf.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tv.shxzukj.cn

Java: // 无解构
来源：http://cl.bjjhwx.cn

Go:   // 无解构
来源：http://ge.9csxet.cn

Ruby: a, b = pair
来源：http://ks.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://zh.nszjky.cn

[C16] 函数 / 方法重载
来源：http://oy.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sg.nszjky.cn

PHP:  // 无重载
来源：http://ty.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cf.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://pa.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lt.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://ek.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://qx.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uc.huanxung.cn

================================================================================
来源：http://sm.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://le.bookmarksfly.cn

================================================================================
来源：http://yt.nicolike.cn

[D01] 创建数组 / 列表
来源：http://gk.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mh.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hq.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yh.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bc.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dx.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://il.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://xl.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wz.lnxyls.cn

[D02] 追加元素到末尾
来源：http://du.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qn.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://py.lnxyls.cn

JS:   arr.push(4);
来源：http://hl.shxzskj.cn

TS:   arr.push(4);
来源：http://al.newstarts.cn


<!-- 参考信息 -->