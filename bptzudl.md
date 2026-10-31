代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ps.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lc.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mc.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jw.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bj.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jk.hnjuh.cn

[B03] switch / match / case
来源：http://pk.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ab.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zj.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://af.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cu.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xi.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uj.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ey.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pb.yuntaijiaju.cn

[B04] for 计数循环
来源：http://zf.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://ac.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hm.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xa.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tl.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dl.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ko.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://co.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ev.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://qm.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://xr.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ao.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zd.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ea.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xi.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lh.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://is.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kd.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://tf.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qc.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ed.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ey.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zq.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gz.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://se.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xn.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lk.colortex.cn

[B07] while 循环
来源：http://rl.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://qj.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bb.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://vy.521024.cn

TS:   while (i < 10) { i++; }
来源：http://sz.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://kt.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zq.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://wr.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://lc.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://of.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://oz.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ch.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://no.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://wv.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://dq.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iw.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mx.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://ya.wgjwhj.cn

[B09] break 与 continue
来源：http://vz.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zx.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bm.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ld.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gc.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nr.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lb.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vd.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://sz.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xe.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ex.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://is.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lr.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lh.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pg.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://am.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kq.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://cc.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://px.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://te.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://st.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dd.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vi.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wo.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://vr.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bm.nicolike.cn

[B12] 跳出多层循环
来源：http://tj.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qk.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://da.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qt.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jv.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://va.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ql.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aj.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://co.jctech888.com.cn

[B13] 判断是否为数字
来源：http://hr.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://ii.9csxet.cn

PHP:  is_numeric($x)
来源：http://iq.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tr.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yd.szsharing.cn

Java: x instanceof Number
来源：http://ww.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://co.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://nq.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://zx.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://va.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rz.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zo.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://fe.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://gu.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uk.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jo.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kv.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ee.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://uu.jctech888.com.cn

Py:   a and b or not c
来源：http://vd.szsharing.cn

PHP:  $a && $b || !$c
来源：http://mq.nicolike.cn

JS:   a && b || !c
来源：http://xt.muxihuayi.cn

TS:   a && b || !c
来源：http://ec.jctech888.com.cn

Java: a && b || !c
来源：http://ti.hahajie.cn

Go:   a && b || !c
来源：http://ap.huixiangedu.cn

Ruby: a && b || !c
来源：http://oe.gzmigu.cn

C#:   a && b || !c
来源：http://tb.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aj.lnxyls.cn

Py:   if not data: return
来源：http://es.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://hi.9csxet.cn

JS:   if (!data) return;
来源：http://fc.szsharing.cn

TS:   if (!data) return;
来源：http://ah.hnjuh.cn

Java: if (data == null) return;
来源：http://rp.panjiajie.cn

Go:   if data == nil { return }
来源：http://ln.nicolike.cn

Ruby: return if data.nil?
来源：http://uq.gzmigu.cn

C#:   if (data == null) return;
来源：http://fh.szsharing.cn

================================================================================
来源：http://cs.muxihuayi.cn

C. 函数与作用域
来源：http://ut.lnxyls.cn

================================================================================
来源：http://ar.colortex.cn

[C01] 定义函数
来源：http://rp.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://fg.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pr.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://bs.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mz.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ng.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eq.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ag.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lt.nszjky.cn

[C02] 默认参数
来源：http://tl.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://ez.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vb.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://vc.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hj.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jg.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zm.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://vl.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://um.521024.cn

[C03] 可变参数
来源：http://rp.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://qk.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ga.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pd.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vn.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wa.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pp.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aa.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ud.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://mw.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uo.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ia.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eq.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://li.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://qv.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://vr.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://dt.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://ja.hnjuh.cn

[C05] 返回多个值
来源：http://wv.huanxung.cn

Py:   return a, b
来源：http://da.lnxyls.cn

PHP:  return [$a, $b];
来源：http://op.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yx.nicolike.cn

TS:   return { a, b };
来源：http://vf.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lo.wgjwhj.cn

Go:   return a, b
来源：http://fz.panjiajie.cn

Ruby: return a, b
来源：http://ns.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://mm.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://le.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://uz.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ns.nicolike.cn

JS:   const square = x => x * x;
来源：http://gn.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://bj.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ys.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://av.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://rt.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yo.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://ax.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xe.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wi.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://go.szxytkj.cn

TS:   arr.map(String)
来源：http://xp.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://av.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bj.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://if.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zh.521024.cn

[C08] 闭包
来源：http://hy.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bx.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bu.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jm.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://if.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://up.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://au.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gx.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bj.lnxyls.cn

[C09] 递归
来源：http://kt.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zz.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yn.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xq.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kp.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rm.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ci.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nh.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gg.yuntaijiaju.cn

[C10] 变量作用域
来源：http://rb.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zj.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iq.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ok.521024.cn

TS:   同 JS
来源：http://eo.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://il.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://ci.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sp.muxihuayi.cn

C#:   块级作用域
来源：http://av.hahajie.cn

[C11] 模块导入与导出
来源：http://qo.hnjuh.cn

Py:   from module import func
来源：http://pr.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dn.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eh.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xs.shxzukj.cn

Java: import java.util.List;
来源：http://fm.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uk.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://nt.muxihuayi.cn

C#:   using System.Text;
来源：http://cd.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://op.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://vt.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://jk.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://zw.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://mc.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vt.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://ul.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://jr.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ih.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://ns.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://td.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yh.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rg.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pn.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://az.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://ek.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cp.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tm.szxytkj.cn

[C14] 泛型函数
来源：http://ot.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lj.szsharing.cn

PHP:  // 无泛型
来源：http://wa.bookmarksfly.cn

JS:   // 无泛型
来源：http://hl.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wh.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zx.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zy.nicolike.cn

Ruby: # 无泛型
来源：http://km.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aa.colortex.cn

[C15] 解构 / 展开参数
来源：http://en.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ky.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://dp.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gk.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cv.colortex.cn

Java: // 无解构
来源：http://xv.yuexingan06.cn

Go:   // 无解构
来源：http://xd.newstarts.cn

Ruby: a, b = pair
来源：http://re.szsharing.cn

C#:   var (a, b) = pair;
来源：http://by.521024.cn

[C16] 函数 / 方法重载
来源：http://ix.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ri.huanxung.cn

PHP:  // 无重载
来源：http://en.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ub.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://wc.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://om.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://eh.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://bl.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cq.nicolike.cn

================================================================================
来源：http://oc.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://zw.colortex.cn

================================================================================
来源：http://cc.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://mp.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ky.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yi.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lo.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xt.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sh.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://cd.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://mt.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ua.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://tp.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://km.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vj.shtwfgs.cn

JS:   arr.push(4);
来源：http://nq.yuexingan06.cn

TS:   arr.push(4);
来源：http://cn.haigaiapp.cn

Java: list.add(4);
来源：http://wj.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://hn.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://he.shxzskj.cn

C#:   list.Add(4);
来源：http://he.jctech888.com.cn


<!-- 参考信息 -->