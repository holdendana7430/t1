代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yf.9csxet.cn

[B02] 多分支 else if / elif
来源：http://tu.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kf.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ry.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hl.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hy.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cu.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ec.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hy.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xg.jctech888.com.cn

[B03] switch / match / case
来源：http://iy.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fc.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kh.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gu.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kw.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wm.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hq.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ul.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yo.huixiangedu.cn

[B04] for 计数循环
来源：http://xj.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://cy.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://al.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ol.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ul.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yx.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sf.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://qh.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ri.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://fq.hahajie.cn

Py:   for item in arr: print(item)
来源：http://fl.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dy.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xs.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qe.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dk.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cs.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://li.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ax.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://ji.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iw.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vl.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://av.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cy.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qs.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tt.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jd.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ba.muxihuayi.cn

[B07] while 循环
来源：http://vi.nicolike.cn

Py:   while i < 10: i += 1
来源：http://xp.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fe.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://px.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://rk.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://mo.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lz.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://qa.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://mo.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://fo.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://vk.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ql.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://zm.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://ow.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://fr.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fd.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kc.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://es.521024.cn

[B09] break 与 continue
来源：http://bn.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yt.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xw.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wq.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kw.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nl.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ji.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hj.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://za.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://th.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gf.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fs.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bz.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ss.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qk.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pu.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yh.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mg.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://vj.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://qk.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://ls.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uc.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fo.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ye.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wj.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://yu.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mp.nicolike.cn

[B12] 跳出多层循环
来源：http://zw.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xk.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dh.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uu.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ov.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xn.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jy.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ps.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bl.shtwfgs.cn

[B13] 判断是否为数字
来源：http://pt.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://qw.szxytkj.cn

PHP:  is_numeric($x)
来源：http://hh.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ry.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lq.szsharing.cn

Java: x instanceof Number
来源：http://nf.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://va.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://to.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://do.nicolike.cn

[B14] 判断值是否在集合内
来源：http://ic.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cf.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lt.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://ie.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://za.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tn.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ae.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ss.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://th.colortex.cn

[B15] 布尔运算与取反
来源：http://hi.huixinmuqiang.cn

Py:   a and b or not c
来源：http://ce.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://as.nicolike.cn

JS:   a && b || !c
来源：http://wg.gzmigu.cn

TS:   a && b || !c
来源：http://if.szxytkj.cn

Java: a && b || !c
来源：http://gv.hnjuh.cn

Go:   a && b || !c
来源：http://mg.newstarts.cn

Ruby: a && b || !c
来源：http://fw.szxytkj.cn

C#:   a && b || !c
来源：http://ce.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hq.huanxung.cn

Py:   if not data: return
来源：http://by.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://wd.huanxung.cn

JS:   if (!data) return;
来源：http://ng.szxytkj.cn

TS:   if (!data) return;
来源：http://yv.bjjhwx.cn

Java: if (data == null) return;
来源：http://gs.9csxet.cn

Go:   if data == nil { return }
来源：http://fb.lnxyls.cn

Ruby: return if data.nil?
来源：http://kf.hahajie.cn

C#:   if (data == null) return;
来源：http://qt.chemitech.net.cn

================================================================================
来源：http://zn.colortex.cn

C. 函数与作用域
来源：http://zd.panjiajie.cn

================================================================================
来源：http://vi.521024.cn

[C01] 定义函数
来源：http://yu.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://br.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uk.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://jv.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jn.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hj.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tt.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://kp.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yu.shxzukj.cn

[C02] 默认参数
来源：http://pt.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://tl.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zn.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://jh.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cg.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sv.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xl.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://yt.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://ej.asd995.cn

[C03] 可变参数
来源：http://sy.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://ck.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://io.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rd.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ao.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aj.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ke.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ae.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jo.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://ln.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rx.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yh.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uo.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ak.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://ih.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://uf.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://gy.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://jj.bjjhwx.cn

[C05] 返回多个值
来源：http://al.shxzukj.cn

Py:   return a, b
来源：http://ex.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://bp.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sk.muxihuayi.cn

TS:   return { a, b };
来源：http://vn.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ao.521024.cn

Go:   return a, b
来源：http://hu.huanxung.cn

Ruby: return a, b
来源：http://yh.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://rj.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://eo.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://ym.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ve.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://dq.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://be.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ai.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pf.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://hs.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cs.colortex.cn

[C07] 把函数作为参数传入
来源：http://mu.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vw.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cr.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jd.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://qu.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oh.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cq.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ua.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lm.asd995.cn

[C08] 闭包
来源：http://gk.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hu.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jy.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://om.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ih.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nr.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zj.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jn.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wf.bjjhwx.cn

[C09] 递归
来源：http://cx.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wv.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://on.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://py.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lc.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kg.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qi.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://op.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mt.nszjky.cn

[C10] 变量作用域
来源：http://qt.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://za.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xu.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nh.shxzskj.cn

TS:   同 JS
来源：http://jv.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://gn.yuexingan06.cn

Go:   花括号块级作用域
来源：http://ch.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bz.newstarts.cn

C#:   块级作用域
来源：http://zm.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://hw.bjjhwx.cn

Py:   from module import func
来源：http://cd.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xg.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cf.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vc.shxzukj.cn

Java: import java.util.List;
来源：http://bu.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fe.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://da.huanxung.cn

C#:   using System.Text;
来源：http://wl.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://mx.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://rw.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://ud.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://fl.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://lg.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vn.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://ul.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://zh.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yu.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://ts.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bc.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bx.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uw.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mu.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ip.gzmigu.cn

Go:   func add(a, b int) int
来源：http://ik.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oq.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hl.colortex.cn

[C14] 泛型函数
来源：http://wo.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ht.szxytkj.cn

PHP:  // 无泛型
来源：http://zf.wgjwhj.cn

JS:   // 无泛型
来源：http://zq.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kz.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ji.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lo.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://cn.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pk.521024.cn

[C15] 解构 / 展开参数
来源：http://yh.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xg.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://zi.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wn.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ai.nszjky.cn

Java: // 无解构
来源：http://on.panjiajie.cn

Go:   // 无解构
来源：http://vf.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://rm.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://pr.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://zo.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tq.lnxyls.cn

PHP:  // 无重载
来源：http://zl.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zb.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://ue.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://au.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://gb.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://ha.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dz.gzmigu.cn

================================================================================
来源：http://oj.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://jg.yuexingan06.cn

================================================================================
来源：http://vm.521024.cn

[D01] 创建数组 / 列表
来源：http://ht.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://li.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vx.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fk.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fn.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lm.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://kk.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://td.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wu.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://ag.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ro.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pg.shtwfgs.cn

JS:   arr.push(4);
来源：http://it.hahajie.cn

TS:   arr.push(4);
来源：http://jx.szsharing.cn


<!-- 参考信息 -->