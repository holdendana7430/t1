代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xw.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nl.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hj.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ju.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xy.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fh.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tj.shxzskj.cn

[B04] for 计数循环
来源：http://nd.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://ep.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pb.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lq.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rm.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://od.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sh.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://sn.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ad.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://hx.nicolike.cn

Py:   for item in arr: print(item)
来源：http://gd.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ls.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ny.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oq.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wf.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gw.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://lj.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pb.521024.cn

[B06] 遍历字典 / 对象
来源：http://dl.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ux.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cb.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ig.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pn.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rs.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://av.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lj.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xx.huixiangedu.cn

[B07] while 循环
来源：http://gl.9csxet.cn

Py:   while i < 10: i += 1
来源：http://lk.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lc.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://uw.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://cd.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://jg.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rd.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://uo.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://nq.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://ce.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://fo.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dy.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://dp.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://bx.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://sb.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://id.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pq.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://zp.jctech888.com.cn

[B09] break 与 continue
来源：http://dr.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iu.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yl.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yi.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vq.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://md.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ds.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pj.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fi.nicolike.cn

[B10] 遍历同时拿索引
来源：http://wb.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://re.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cy.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uk.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ts.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ts.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://im.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://in.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ny.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://nm.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://js.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://wl.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aq.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cb.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ob.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ww.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://rh.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ki.gzmigu.cn

[B12] 跳出多层循环
来源：http://oe.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ju.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jy.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qx.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gb.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://it.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://di.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nj.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rf.colortex.cn

[B13] 判断是否为数字
来源：http://ot.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://ef.shxzskj.cn

PHP:  is_numeric($x)
来源：http://gu.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wv.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cu.huixinmuqiang.cn

Java: x instanceof Number
来源：http://es.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lb.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://mn.szxytkj.cn

C#:   x is int or double or decimal
来源：http://uv.nicolike.cn

[B14] 判断值是否在集合内
来源：http://xe.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yt.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mg.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://ek.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://zi.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://un.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://na.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mi.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://of.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://az.huixinmuqiang.cn

Py:   a and b or not c
来源：http://dy.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://gr.9csxet.cn

JS:   a && b || !c
来源：http://nx.haigaiapp.cn

TS:   a && b || !c
来源：http://xp.huanxung.cn

Java: a && b || !c
来源：http://sg.huanxung.cn

Go:   a && b || !c
来源：http://ej.shxzukj.cn

Ruby: a && b || !c
来源：http://lw.szsharing.cn

C#:   a && b || !c
来源：http://ip.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tz.szsharing.cn

Py:   if not data: return
来源：http://ls.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://xr.bookmarksfly.cn

JS:   if (!data) return;
来源：http://lh.hahajie.cn

TS:   if (!data) return;
来源：http://ti.panjiajie.cn

Java: if (data == null) return;
来源：http://ug.muxihuayi.cn

Go:   if data == nil { return }
来源：http://wh.lnxyls.cn

Ruby: return if data.nil?
来源：http://en.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://wa.bookmarksfly.cn

================================================================================
来源：http://sz.9csxet.cn

C. 函数与作用域
来源：http://zo.muxihuayi.cn

================================================================================
来源：http://vo.szsharing.cn

[C01] 定义函数
来源：http://rx.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://cb.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xf.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://az.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ig.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sz.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ld.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://jz.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cf.lnxyls.cn

[C02] 默认参数
来源：http://ck.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://ug.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ze.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://hg.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pp.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gl.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://gd.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://dz.nicolike.cn

[C03] 可变参数
来源：http://oy.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://sk.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lg.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qj.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fr.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jf.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lw.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wv.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://po.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://qg.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eg.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sx.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ad.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vj.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://cf.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://hu.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://am.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://xj.nszjky.cn

[C05] 返回多个值
来源：http://uw.haigaiapp.cn

Py:   return a, b
来源：http://wv.hahajie.cn

PHP:  return [$a, $b];
来源：http://ef.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bx.521024.cn

TS:   return { a, b };
来源：http://ep.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zc.haigaiapp.cn

Go:   return a, b
来源：http://wn.bookmarksfly.cn

Ruby: return a, b
来源：http://vr.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://sb.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://nb.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://zs.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yi.gzmigu.cn

JS:   const square = x => x * x;
来源：http://tc.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://uo.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oc.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hq.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://xy.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rp.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://cb.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jr.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gp.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dg.521024.cn

TS:   arr.map(String)
来源：http://ku.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xw.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gc.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://mj.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yd.jctech888.com.cn

[C08] 闭包
来源：http://bo.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yn.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ce.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mo.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cb.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zp.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yu.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wm.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rl.yuexingan06.cn

[C09] 递归
来源：http://ly.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sv.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sj.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mm.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xd.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vj.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ks.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xl.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mk.muxihuayi.cn

[C10] 变量作用域
来源：http://xv.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nf.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fh.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uu.shtwfgs.cn

TS:   同 JS
来源：http://ik.9csxet.cn

Java: 方法内为块级作用域
来源：http://ye.newstarts.cn

Go:   花括号块级作用域
来源：http://af.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yo.huanxung.cn

C#:   块级作用域
来源：http://qo.shxzskj.cn

[C11] 模块导入与导出
来源：http://sa.bjjhwx.cn

Py:   from module import func
来源：http://er.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sr.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dk.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zf.bjjhwx.cn

Java: import java.util.List;
来源：http://im.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sn.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ag.yuntaijiaju.cn

C#:   using System.Text;
来源：http://sg.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://vn.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://im.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://he.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://mk.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://kh.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kz.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://qv.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://uz.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kx.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://iv.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eg.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iv.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dk.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qw.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ls.asd995.cn

Go:   func add(a, b int) int
来源：http://jp.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qq.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vw.nicolike.cn

[C14] 泛型函数
来源：http://xr.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fu.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://gk.nszjky.cn

JS:   // 无泛型
来源：http://cw.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nu.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gj.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fr.shtwfgs.cn

Ruby: # 无泛型
来源：http://hp.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jt.huanxung.cn

[C15] 解构 / 展开参数
来源：http://eb.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fu.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://yk.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dd.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://px.panjiajie.cn

Java: // 无解构
来源：http://gf.shxzukj.cn

Go:   // 无解构
来源：http://md.gzmigu.cn

Ruby: a, b = pair
来源：http://xo.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://ws.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://tb.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ek.nicolike.cn

PHP:  // 无重载
来源：http://py.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gw.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://tz.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hw.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://fn.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://kw.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nb.yuntaijiaju.cn

================================================================================
来源：http://cj.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://ef.szsharing.cn

================================================================================
来源：http://qf.asd995.cn

[D01] 创建数组 / 列表
来源：http://fm.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gu.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ls.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oh.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://se.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tm.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://fp.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://ix.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pf.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://hg.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qh.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kr.bjjhwx.cn

JS:   arr.push(4);
来源：http://da.hnjuh.cn

TS:   arr.push(4);
来源：http://rk.shtwfgs.cn

Java: list.add(4);
来源：http://dj.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://kw.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://vk.huanxung.cn

C#:   list.Add(4);
来源：http://vh.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://kz.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://qb.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bs.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lj.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://kt.asd995.cn

Java: list.add(0, 0);
来源：http://xi.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://le.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://na.nicolike.cn


<!-- 参考信息 -->