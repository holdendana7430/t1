代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pm.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dk.9csxet.cn

[B03] switch / match / case
来源：http://iz.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pv.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ev.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ez.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qm.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ot.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xe.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tw.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://we.521024.cn

[B04] for 计数循环
来源：http://pg.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://jn.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://de.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sd.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ve.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mc.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oa.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://hg.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ef.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://nc.huanxung.cn

Py:   for item in arr: print(item)
来源：http://eo.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nr.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kt.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ss.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wn.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jj.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://lg.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://go.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://nj.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eb.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://au.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fu.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gm.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hu.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qo.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pl.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sx.lnxyls.cn

[B07] while 循环
来源：http://ct.newstarts.cn

Py:   while i < 10: i += 1
来源：http://rr.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://er.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://fq.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://iu.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://zo.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qj.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://zm.521024.cn

C#:   while (i < 10) { i++; }
来源：http://xg.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ai.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://fb.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yu.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://gw.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://mj.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://rq.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zg.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iz.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://pf.szsharing.cn

[B09] break 与 continue
来源：http://yx.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yo.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ir.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hr.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sv.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zn.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tm.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zd.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://as.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xr.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iw.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://og.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ui.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oe.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zm.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pk.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://px.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://tc.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://qt.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://sc.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bf.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hg.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zv.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dj.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://mw.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nm.newstarts.cn

[B12] 跳出多层循环
来源：http://zm.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kb.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ka.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ug.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bv.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ia.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ft.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bp.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ar.shxzukj.cn

[B13] 判断是否为数字
来源：http://jp.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://cm.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://ba.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rb.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jl.521024.cn

Java: x instanceof Number
来源：http://kw.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://or.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://nm.shxzukj.cn

C#:   x is int or double or decimal
来源：http://kl.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://lx.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fv.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cz.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ra.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://nz.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zl.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tw.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mq.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fl.asd995.cn

[B15] 布尔运算与取反
来源：http://cz.muxihuayi.cn

Py:   a and b or not c
来源：http://sf.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://xp.panjiajie.cn

JS:   a && b || !c
来源：http://lc.jianghongdianzi.cn

TS:   a && b || !c
来源：http://qk.hahajie.cn

Java: a && b || !c
来源：http://qz.hnjuh.cn

Go:   a && b || !c
来源：http://of.asd995.cn

Ruby: a && b || !c
来源：http://et.chemitech.net.cn

C#:   a && b || !c
来源：http://aq.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dv.panjiajie.cn

Py:   if not data: return
来源：http://eu.521024.cn

PHP:  if (!$data) { return; }
来源：http://ys.lnxyls.cn

JS:   if (!data) return;
来源：http://tl.yuexingan06.cn

TS:   if (!data) return;
来源：http://ka.szxytkj.cn

Java: if (data == null) return;
来源：http://cq.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://ko.shtwfgs.cn

Ruby: return if data.nil?
来源：http://jc.nszjky.cn

C#:   if (data == null) return;
来源：http://tb.chemitech.net.cn

================================================================================
来源：http://xe.colortex.cn

C. 函数与作用域
来源：http://qh.jianghongdianzi.cn

================================================================================
来源：http://gp.shxzskj.cn

[C01] 定义函数
来源：http://up.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://hm.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bl.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://tb.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sz.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xf.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://on.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://sk.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fb.szxytkj.cn

[C02] 默认参数
来源：http://ru.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ll.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xc.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://ta.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jv.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tc.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vi.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://ah.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://at.szsharing.cn

[C03] 可变参数
来源：http://ma.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://gj.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://na.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yp.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tz.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ty.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xk.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gt.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ru.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://hk.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qf.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jc.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zd.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ih.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://ng.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://tz.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://gm.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://jt.jctech888.com.cn

[C05] 返回多个值
来源：http://rr.huixinmuqiang.cn

Py:   return a, b
来源：http://dy.huanxung.cn

PHP:  return [$a, $b];
来源：http://ag.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://au.nszjky.cn

TS:   return { a, b };
来源：http://kf.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pc.gzmigu.cn

Go:   return a, b
来源：http://mg.panjiajie.cn

Ruby: return a, b
来源：http://he.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://by.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://ra.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://ew.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pu.colortex.cn

JS:   const square = x => x * x;
来源：http://ur.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://vl.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tl.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cd.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://wx.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cu.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://uv.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yo.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oi.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kf.shtwfgs.cn

TS:   arr.map(String)
来源：http://gg.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ku.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pz.521024.cn

Ruby: arr.map(&:upcase)
来源：http://nv.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jo.jctech888.com.cn

[C08] 闭包
来源：http://wm.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dr.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ie.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://um.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qp.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ld.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ss.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wx.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qf.newstarts.cn

[C09] 递归
来源：http://ei.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kn.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jt.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kz.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cp.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zv.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tc.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fo.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vc.jianghongdianzi.cn

[C10] 变量作用域
来源：http://ww.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gu.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uc.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zr.chemitech.net.cn

TS:   同 JS
来源：http://kp.panjiajie.cn

Java: 方法内为块级作用域
来源：http://mk.nicolike.cn

Go:   花括号块级作用域
来源：http://ja.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ds.gzmigu.cn

C#:   块级作用域
来源：http://od.shxzukj.cn

[C11] 模块导入与导出
来源：http://uz.colortex.cn

Py:   from module import func
来源：http://ph.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ai.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dv.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lv.wgjwhj.cn

Java: import java.util.List;
来源：http://tm.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tx.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://eh.muxihuayi.cn

C#:   using System.Text;
来源：http://er.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://qm.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://tx.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://wj.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://mg.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ix.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uy.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://cn.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://hx.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://da.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://jh.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rf.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oj.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bh.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kq.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tq.lnxyls.cn

Go:   func add(a, b int) int
来源：http://wr.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tm.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oc.szxytkj.cn

[C14] 泛型函数
来源：http://pn.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lw.asd995.cn

PHP:  // 无泛型
来源：http://tp.nicolike.cn

JS:   // 无泛型
来源：http://hs.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ao.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bu.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jp.bjjhwx.cn

Ruby: # 无泛型
来源：http://gz.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gr.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://ox.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://un.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://cp.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fp.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dr.haigaiapp.cn

Java: // 无解构
来源：http://qu.nicolike.cn

Go:   // 无解构
来源：http://qh.panjiajie.cn

Ruby: a, b = pair
来源：http://ze.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://sf.hahajie.cn

[C16] 函数 / 方法重载
来源：http://al.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jg.shxzskj.cn

PHP:  // 无重载
来源：http://ow.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vq.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://sm.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zr.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://tx.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://na.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mp.jianghongdianzi.cn

================================================================================
来源：http://qq.colortex.cn

D. 数组 / 列表 / 集合
来源：http://nv.szsharing.cn

================================================================================
来源：http://yo.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://ki.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://io.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mh.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yb.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ze.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wh.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://jy.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://go.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ez.nszjky.cn

[D02] 追加元素到末尾
来源：http://vu.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lp.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fl.nszjky.cn

JS:   arr.push(4);
来源：http://bz.newstarts.cn

TS:   arr.push(4);
来源：http://nq.szsharing.cn

Java: list.add(4);
来源：http://xh.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://gq.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://vx.muxihuayi.cn

C#:   list.Add(4);
来源：http://kj.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://dr.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://pu.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qo.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nv.newstarts.cn


<!-- 参考信息 -->