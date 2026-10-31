代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dj.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://xw.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eh.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yw.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yj.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://no.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tm.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bx.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vm.szsharing.cn

[B03] switch / match / case
来源：http://ly.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://am.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dh.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xg.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xq.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cq.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vr.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ci.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cz.lnxyls.cn

[B04] for 计数循环
来源：http://ot.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://ix.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zf.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zz.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kw.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://py.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sq.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://pu.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ys.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://nm.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://ce.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wq.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kc.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oc.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dz.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wq.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://xf.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vd.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://kr.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wi.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fi.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ou.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bm.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yb.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uk.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ij.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cq.yuexingan06.cn

[B07] while 循环
来源：http://nd.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://bz.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yr.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://zr.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://ng.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://to.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://df.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://di.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://ux.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://os.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://ag.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oh.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://nt.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://pw.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://as.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://le.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zy.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://mf.szsharing.cn

[B09] break 与 continue
来源：http://aa.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dy.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eg.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bf.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://er.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yl.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://st.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vi.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vv.newstarts.cn

[B10] 遍历同时拿索引
来源：http://xp.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oe.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ep.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://se.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://td.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uh.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zb.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://le.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bn.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://ye.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://ck.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://ea.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ui.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zq.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ry.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pc.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://jg.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pj.szxytkj.cn

[B12] 跳出多层循环
来源：http://qx.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cm.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gz.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vl.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kt.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tm.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dr.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ex.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yx.newstarts.cn

[B13] 判断是否为数字
来源：http://sw.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://ip.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://ve.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tn.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sd.muxihuayi.cn

Java: x instanceof Number
来源：http://zu.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ke.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://hb.nszjky.cn

C#:   x is int or double or decimal
来源：http://av.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://zk.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pb.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zr.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://pc.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://fk.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vl.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sb.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ex.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fw.lnxyls.cn

[B15] 布尔运算与取反
来源：http://ym.chemitech.net.cn

Py:   a and b or not c
来源：http://tq.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://vm.shtwfgs.cn

JS:   a && b || !c
来源：http://ci.yuntaijiaju.cn

TS:   a && b || !c
来源：http://ad.jctech888.com.cn

Java: a && b || !c
来源：http://yy.bjjhwx.cn

Go:   a && b || !c
来源：http://rj.shtwfgs.cn

Ruby: a && b || !c
来源：http://nc.muxihuayi.cn

C#:   a && b || !c
来源：http://vx.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uu.newstarts.cn

Py:   if not data: return
来源：http://im.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://qu.bjjhwx.cn

JS:   if (!data) return;
来源：http://wg.9csxet.cn

TS:   if (!data) return;
来源：http://nm.shtwfgs.cn

Java: if (data == null) return;
来源：http://ru.chemitech.net.cn

Go:   if data == nil { return }
来源：http://cv.yuexingan06.cn

Ruby: return if data.nil?
来源：http://jb.jctech888.com.cn

C#:   if (data == null) return;
来源：http://st.huixiangedu.cn

================================================================================
来源：http://mf.shtwfgs.cn

C. 函数与作用域
来源：http://qj.wgjwhj.cn

================================================================================
来源：http://kd.wgjwhj.cn

[C01] 定义函数
来源：http://rg.colortex.cn

Py:   def add(a, b): return a + b
来源：http://kj.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pm.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://ag.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bh.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tf.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gr.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://pt.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fa.hahajie.cn

[C02] 默认参数
来源：http://vc.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://cf.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tz.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ty.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iu.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://er.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ib.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://bm.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ga.szxytkj.cn

[C03] 可变参数
来源：http://qw.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://it.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pm.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://so.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pe.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oe.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://li.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wv.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cy.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://hp.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fh.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ow.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hv.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yi.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://zq.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://fz.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://au.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://aa.gzmigu.cn

[C05] 返回多个值
来源：http://ya.wgjwhj.cn

Py:   return a, b
来源：http://dk.hahajie.cn

PHP:  return [$a, $b];
来源：http://ve.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hu.hnjuh.cn

TS:   return { a, b };
来源：http://yb.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iu.panjiajie.cn

Go:   return a, b
来源：http://ny.wgjwhj.cn

Ruby: return a, b
来源：http://ye.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://oe.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://jq.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://tn.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dv.hnjuh.cn

JS:   const square = x => x * x;
来源：http://hk.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://fm.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ws.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cr.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://bt.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fq.asd995.cn

[C07] 把函数作为参数传入
来源：http://ww.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fm.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gq.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yq.nicolike.cn

TS:   arr.map(String)
来源：http://xt.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qs.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ky.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://cd.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dz.wgjwhj.cn

[C08] 闭包
来源：http://lw.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ku.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ll.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ih.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pr.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zr.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://po.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ks.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://op.asd995.cn

[C09] 递归
来源：http://qb.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ix.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lt.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rm.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wl.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lf.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zu.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jv.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rl.szxytkj.cn

[C10] 变量作用域
来源：http://bj.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://au.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bj.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ho.hnjuh.cn

TS:   同 JS
来源：http://ux.nicolike.cn

Java: 方法内为块级作用域
来源：http://mv.hahajie.cn

Go:   花括号块级作用域
来源：http://cg.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sz.huanxung.cn

C#:   块级作用域
来源：http://dx.chemitech.net.cn

[C11] 模块导入与导出
来源：http://zf.hahajie.cn

Py:   from module import func
来源：http://wo.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://in.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://as.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dp.yuexingan06.cn

Java: import java.util.List;
来源：http://qf.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xg.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://oz.colortex.cn

C#:   using System.Text;
来源：http://qu.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://pa.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://tl.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://wn.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://bg.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://ue.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wm.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://uy.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://hx.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ku.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://um.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yb.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ot.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tf.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ai.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dx.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://sx.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ft.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ab.huanxung.cn

[C14] 泛型函数
来源：http://hw.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ub.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://mi.szxytkj.cn

JS:   // 无泛型
来源：http://sq.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fj.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rh.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zw.wgjwhj.cn

Ruby: # 无泛型
来源：http://rp.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ac.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://fg.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ls.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://wd.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oq.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ot.521024.cn

Java: // 无解构
来源：http://nf.colortex.cn

Go:   // 无解构
来源：http://cw.huixiangedu.cn

Ruby: a, b = pair
来源：http://ez.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://hz.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://lx.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sl.szxytkj.cn

PHP:  // 无重载
来源：http://oz.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zh.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://yc.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://em.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://io.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://ix.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xn.asd995.cn

================================================================================
来源：http://um.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://sa.wgjwhj.cn

================================================================================
来源：http://mv.szsharing.cn

[D01] 创建数组 / 列表
来源：http://jb.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tj.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jd.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://np.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uf.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://az.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://xu.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://bg.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bd.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://hh.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pj.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rq.haigaiapp.cn

JS:   arr.push(4);
来源：http://bx.nicolike.cn

TS:   arr.push(4);
来源：http://ee.huanxung.cn


<!-- 参考信息 -->