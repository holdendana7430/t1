代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kr.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ek.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fh.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vz.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fx.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ch.hahajie.cn

[B03] switch / match / case
来源：http://tw.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://me.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ve.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wg.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ab.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nh.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ch.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kq.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qh.asd995.cn

[B04] for 计数循环
来源：http://wq.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://zi.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mu.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uo.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qf.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vz.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nv.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://lr.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ns.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://hp.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://fd.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hr.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gp.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nu.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ha.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ve.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://tp.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ip.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://qu.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qn.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dt.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vl.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yc.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mu.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qs.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ul.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://md.szxytkj.cn

[B07] while 循环
来源：http://vd.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://di.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rl.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://ys.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://il.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://yv.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oj.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://ko.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://ju.colortex.cn

[B08] do-while（至少执行一次）
来源：http://uw.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://kc.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oo.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://bz.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://mi.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://lv.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zj.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://za.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://jq.newstarts.cn

[B09] break 与 continue
来源：http://bv.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ut.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bd.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iu.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yp.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fu.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://id.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tv.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://xl.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hq.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dm.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://er.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gr.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jj.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vc.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ii.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vc.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://qz.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://bc.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://xs.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ab.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fy.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jp.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kt.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://ff.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zc.lnxyls.cn

[B12] 跳出多层循环
来源：http://ys.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cr.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jv.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cg.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ed.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yu.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wb.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xe.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wx.szsharing.cn

[B13] 判断是否为数字
来源：http://kl.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://ha.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://um.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ux.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ai.szxytkj.cn

Java: x instanceof Number
来源：http://pj.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://en.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://rf.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://ru.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://bb.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://il.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rp.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://hp.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://iq.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://io.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aq.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nf.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ne.shxzskj.cn

[B15] 布尔运算与取反
来源：http://dk.huanxung.cn

Py:   a and b or not c
来源：http://ax.nszjky.cn

PHP:  $a && $b || !$c
来源：http://do.szsharing.cn

JS:   a && b || !c
来源：http://fp.huixinmuqiang.cn

TS:   a && b || !c
来源：http://ns.hahajie.cn

Java: a && b || !c
来源：http://lp.haigaiapp.cn

Go:   a && b || !c
来源：http://ry.shtwfgs.cn

Ruby: a && b || !c
来源：http://ke.521024.cn

C#:   a && b || !c
来源：http://wr.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sd.shtwfgs.cn

Py:   if not data: return
来源：http://rn.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://da.yuexingan06.cn

JS:   if (!data) return;
来源：http://lk.bookmarksfly.cn

TS:   if (!data) return;
来源：http://il.shxzukj.cn

Java: if (data == null) return;
来源：http://hy.hnjuh.cn

Go:   if data == nil { return }
来源：http://aq.huixiangedu.cn

Ruby: return if data.nil?
来源：http://fi.panjiajie.cn

C#:   if (data == null) return;
来源：http://ff.huanxung.cn

================================================================================
来源：http://su.9csxet.cn

C. 函数与作用域
来源：http://lc.jianghongdianzi.cn

================================================================================
来源：http://qv.huixinmuqiang.cn

[C01] 定义函数
来源：http://tg.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://hi.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wv.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://nk.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xy.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tg.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qj.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://ei.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sz.jianghongdianzi.cn

[C02] 默认参数
来源：http://vn.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://ga.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pg.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://fa.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bi.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jd.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kj.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ax.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://ug.chemitech.net.cn

[C03] 可变参数
来源：http://dr.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://vn.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ta.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wu.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kh.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eq.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dy.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qz.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zr.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://az.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://up.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://or.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ny.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oc.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://um.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://gn.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://rc.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://sy.bjjhwx.cn

[C05] 返回多个值
来源：http://dq.lnxyls.cn

Py:   return a, b
来源：http://ny.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://so.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wj.haigaiapp.cn

TS:   return { a, b };
来源：http://gw.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xw.szxytkj.cn

Go:   return a, b
来源：http://uy.panjiajie.cn

Ruby: return a, b
来源：http://nu.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://jt.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://cg.nicolike.cn

Py:   square = lambda x: x * x
来源：http://mc.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gy.nszjky.cn

JS:   const square = x => x * x;
来源：http://lu.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://gu.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ku.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eb.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://xs.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ur.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://lr.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lh.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jd.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sh.chemitech.net.cn

TS:   arr.map(String)
来源：http://oq.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qx.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ww.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://ht.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ur.hahajie.cn

[C08] 闭包
来源：http://wv.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://by.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://im.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://km.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ab.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qc.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tr.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ii.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qh.wgjwhj.cn

[C09] 递归
来源：http://lk.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rr.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wc.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zm.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://te.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tg.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gc.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jv.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://no.szsharing.cn

[C10] 变量作用域
来源：http://bs.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bf.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eg.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mm.9csxet.cn

TS:   同 JS
来源：http://nn.nicolike.cn

Java: 方法内为块级作用域
来源：http://lr.gzmigu.cn

Go:   花括号块级作用域
来源：http://je.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://on.nszjky.cn

C#:   块级作用域
来源：http://jo.asd995.cn

[C11] 模块导入与导出
来源：http://rn.nszjky.cn

Py:   from module import func
来源：http://nf.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ul.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rf.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://is.wgjwhj.cn

Java: import java.util.List;
来源：http://zs.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://em.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://og.shtwfgs.cn

C#:   using System.Text;
来源：http://qw.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://hk.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://mp.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://rl.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://fh.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://vz.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cj.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://kc.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://tr.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ty.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://ju.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lj.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ff.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tu.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vh.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ym.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://wd.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uc.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wl.nszjky.cn

[C14] 泛型函数
来源：http://fq.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ka.huanxung.cn

PHP:  // 无泛型
来源：http://ls.hahajie.cn

JS:   // 无泛型
来源：http://uf.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ha.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rm.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xy.gzmigu.cn

Ruby: # 无泛型
来源：http://ii.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oo.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://ir.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lx.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://nw.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ei.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uy.haigaiapp.cn

Java: // 无解构
来源：http://dr.huanxung.cn

Go:   // 无解构
来源：http://cx.jctech888.com.cn

Ruby: a, b = pair
来源：http://nm.521024.cn

C#:   var (a, b) = pair;
来源：http://he.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://bb.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uj.shxzukj.cn

PHP:  // 无重载
来源：http://wk.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ym.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ho.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dz.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://ee.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://lv.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gj.9csxet.cn

================================================================================
来源：http://og.asd995.cn

D. 数组 / 列表 / 集合
来源：http://gn.huanxung.cn

================================================================================
来源：http://co.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://id.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pn.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gx.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pd.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sh.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ft.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://be.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://gl.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pe.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://ws.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cp.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ae.shxzukj.cn

JS:   arr.push(4);
来源：http://it.hahajie.cn

TS:   arr.push(4);
来源：http://ju.szsharing.cn

Java: list.add(4);
来源：http://vo.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://bo.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://si.panjiajie.cn

C#:   list.Add(4);
来源：http://uo.huixinmuqiang.cn


<!-- 参考信息 -->