代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ga.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yz.jctech888.com.cn

[B03] switch / match / case
来源：http://ak.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gu.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fu.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ma.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eq.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uc.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tf.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tl.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wq.521024.cn

[B04] for 计数循环
来源：http://ze.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://hm.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yr.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ec.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jr.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jl.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://me.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://ky.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zw.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://hb.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://zf.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sv.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ep.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pv.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ck.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hc.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://dz.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cv.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://yj.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xi.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ea.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hu.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ka.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zl.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://co.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tv.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xk.shxzukj.cn

[B07] while 循环
来源：http://nl.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://ql.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lm.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://yg.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://lq.521024.cn

Java: while (i < 10) { i++; }
来源：http://ut.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kn.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://oj.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://yn.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://qc.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://ey.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mi.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ln.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://ay.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://ll.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bv.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ui.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://zr.shxzskj.cn

[B09] break 与 continue
来源：http://fj.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gz.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://om.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bb.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://od.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zi.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ex.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hd.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jy.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://mz.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://co.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oe.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zv.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bg.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kk.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dd.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jb.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vr.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://wl.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://pj.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://hw.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jf.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jm.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ra.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ga.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://ff.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hh.newstarts.cn

[B12] 跳出多层循环
来源：http://ei.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kp.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ri.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fg.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lv.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ou.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ne.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ji.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://np.muxihuayi.cn

[B13] 判断是否为数字
来源：http://ee.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://di.521024.cn

PHP:  is_numeric($x)
来源：http://ox.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zd.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ok.chemitech.net.cn

Java: x instanceof Number
来源：http://hb.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vj.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://fp.newstarts.cn

C#:   x is int or double or decimal
来源：http://wx.hahajie.cn

[B14] 判断值是否在集合内
来源：http://en.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nf.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ln.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://lc.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://tk.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ww.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gi.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pr.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://em.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://ep.jianghongdianzi.cn

Py:   a and b or not c
来源：http://tt.newstarts.cn

PHP:  $a && $b || !$c
来源：http://rh.521024.cn

JS:   a && b || !c
来源：http://je.huanxung.cn

TS:   a && b || !c
来源：http://jv.wgjwhj.cn

Java: a && b || !c
来源：http://lp.panjiajie.cn

Go:   a && b || !c
来源：http://ji.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://hm.huanxung.cn

C#:   a && b || !c
来源：http://gq.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pm.yuntaijiaju.cn

Py:   if not data: return
来源：http://km.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://gh.shxzskj.cn

JS:   if (!data) return;
来源：http://em.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://ee.9csxet.cn

Java: if (data == null) return;
来源：http://cc.shxzukj.cn

Go:   if data == nil { return }
来源：http://ek.newstarts.cn

Ruby: return if data.nil?
来源：http://pn.jctech888.com.cn

C#:   if (data == null) return;
来源：http://ol.yuexingan06.cn

================================================================================
来源：http://jl.huixiangedu.cn

C. 函数与作用域
来源：http://cb.gzmigu.cn

================================================================================
来源：http://no.nicolike.cn

[C01] 定义函数
来源：http://km.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://lr.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ga.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://da.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rt.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sh.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uv.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://we.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yi.shtwfgs.cn

[C02] 默认参数
来源：http://xk.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://ku.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://di.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://du.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fj.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cf.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hp.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://vz.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://in.yuntaijiaju.cn

[C03] 可变参数
来源：http://up.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://fp.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ju.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lj.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nd.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bz.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://az.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bs.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pd.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://ur.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://co.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gy.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pi.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hh.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ci.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://no.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://bz.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://as.bookmarksfly.cn

[C05] 返回多个值
来源：http://db.shtwfgs.cn

Py:   return a, b
来源：http://ts.gzmigu.cn

PHP:  return [$a, $b];
来源：http://zs.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ve.521024.cn

TS:   return { a, b };
来源：http://gy.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hx.jctech888.com.cn

Go:   return a, b
来源：http://od.nicolike.cn

Ruby: return a, b
来源：http://dz.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://uz.521024.cn

[C06] 匿名函数 / lambda
来源：http://ln.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://km.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pr.hnjuh.cn

JS:   const square = x => x * x;
来源：http://jy.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://cr.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dp.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ox.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://gm.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yh.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://eb.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gx.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://le.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zw.gzmigu.cn

TS:   arr.map(String)
来源：http://qb.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://al.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wu.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://zc.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gh.chemitech.net.cn

[C08] 闭包
来源：http://no.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dk.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jt.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kn.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ve.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://du.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ry.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yj.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nm.szsharing.cn

[C09] 递归
来源：http://ga.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gb.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qn.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ev.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tv.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fc.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://el.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mm.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bi.hahajie.cn

[C10] 变量作用域
来源：http://mj.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sy.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nq.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ov.bookmarksfly.cn

TS:   同 JS
来源：http://gi.asd995.cn

Java: 方法内为块级作用域
来源：http://on.szsharing.cn

Go:   花括号块级作用域
来源：http://wu.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gk.asd995.cn

C#:   块级作用域
来源：http://or.panjiajie.cn

[C11] 模块导入与导出
来源：http://xw.asd995.cn

Py:   from module import func
来源：http://fb.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hk.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ak.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fx.nicolike.cn

Java: import java.util.List;
来源：http://ro.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wm.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://za.wgjwhj.cn

C#:   using System.Text;
来源：http://ap.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ai.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://lu.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://pc.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://fo.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://ek.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://si.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://tm.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://io.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xt.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://mv.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oz.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://on.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dj.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jj.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lt.asd995.cn

Go:   func add(a, b int) int
来源：http://vo.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jc.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yb.muxihuayi.cn

[C14] 泛型函数
来源：http://tt.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fc.hahajie.cn

PHP:  // 无泛型
来源：http://qn.wgjwhj.cn

JS:   // 无泛型
来源：http://fi.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mk.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://no.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gu.wgjwhj.cn

Ruby: # 无泛型
来源：http://fp.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pz.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://bk.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mm.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://zb.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bd.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vj.jctech888.com.cn

Java: // 无解构
来源：http://nm.asd995.cn

Go:   // 无解构
来源：http://mw.szxytkj.cn

Ruby: a, b = pair
来源：http://gs.nszjky.cn

C#:   var (a, b) = pair;
来源：http://am.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://mo.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yi.bookmarksfly.cn

PHP:  // 无重载
来源：http://vu.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sx.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://ay.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uq.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://od.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://id.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dp.bjjhwx.cn

================================================================================
来源：http://ao.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://xw.huanxung.cn

================================================================================
来源：http://rz.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://jg.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rs.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sz.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gm.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dt.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zt.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://zs.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://wu.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://en.huanxung.cn

[D02] 追加元素到末尾
来源：http://kc.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pb.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dz.huanxung.cn

JS:   arr.push(4);
来源：http://my.szsharing.cn

TS:   arr.push(4);
来源：http://vn.jctech888.com.cn

Java: list.add(4);
来源：http://cs.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://hi.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ek.asd995.cn

C#:   list.Add(4);
来源：http://vm.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://fn.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://ct.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rb.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ou.szsharing.cn


<!-- 参考信息 -->