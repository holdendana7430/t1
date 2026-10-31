代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://at.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://xl.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ep.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://li.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kj.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ob.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ae.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oq.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sq.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ph.jctech888.com.cn

[B03] switch / match / case
来源：http://hp.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ab.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qo.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://im.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jy.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nf.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bb.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tx.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://af.wgjwhj.cn

[B04] for 计数循环
来源：http://ht.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://fl.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://em.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lw.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hi.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://un.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rj.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://nx.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mx.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://hd.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://rz.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qc.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qv.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tf.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ak.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hr.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://jm.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zm.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://qz.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nu.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lc.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pe.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ly.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vk.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zb.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sd.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ne.huixiangedu.cn

[B07] while 循环
来源：http://wp.hahajie.cn

Py:   while i < 10: i += 1
来源：http://do.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ai.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://mv.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://uf.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://el.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mn.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://fz.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://bc.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://kr.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://pi.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hr.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://uz.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://qm.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://jf.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sg.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://aa.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://zz.shtwfgs.cn

[B09] break 与 continue
来源：http://yc.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cx.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mw.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://se.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pg.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ah.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lr.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vs.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rw.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://zi.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sw.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jd.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pq.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vd.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mc.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mc.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://un.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://it.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://ya.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://ia.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://ye.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ra.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uo.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bs.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zi.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://eh.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bw.nszjky.cn

[B12] 跳出多层循环
来源：http://ag.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wu.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jr.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://za.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pr.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uo.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://op.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xv.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zt.szsharing.cn

[B13] 判断是否为数字
来源：http://rr.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://zo.panjiajie.cn

PHP:  is_numeric($x)
来源：http://as.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hw.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://re.huanxung.cn

Java: x instanceof Number
来源：http://ce.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lj.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://yp.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://ea.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://xk.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qq.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vq.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://ix.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://dk.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gt.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://en.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ux.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kz.panjiajie.cn

[B15] 布尔运算与取反
来源：http://ld.szsharing.cn

Py:   a and b or not c
来源：http://go.521024.cn

PHP:  $a && $b || !$c
来源：http://yj.huixinmuqiang.cn

JS:   a && b || !c
来源：http://ou.huixiangedu.cn

TS:   a && b || !c
来源：http://kc.panjiajie.cn

Java: a && b || !c
来源：http://za.yuexingan06.cn

Go:   a && b || !c
来源：http://dg.bookmarksfly.cn

Ruby: a && b || !c
来源：http://zq.shxzukj.cn

C#:   a && b || !c
来源：http://nz.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tp.jianghongdianzi.cn

Py:   if not data: return
来源：http://nq.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://um.wgjwhj.cn

JS:   if (!data) return;
来源：http://ck.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://jf.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://dy.shtwfgs.cn

Go:   if data == nil { return }
来源：http://kd.bjjhwx.cn

Ruby: return if data.nil?
来源：http://et.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://su.wgjwhj.cn

================================================================================
来源：http://zh.muxihuayi.cn

C. 函数与作用域
来源：http://jm.nszjky.cn

================================================================================
来源：http://cj.szxytkj.cn

[C01] 定义函数
来源：http://ju.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://jo.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zj.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://zf.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kn.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mz.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pw.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://zt.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ym.yuexingan06.cn

[C02] 默认参数
来源：http://sw.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://ox.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hw.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://md.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://re.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bb.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oi.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://ij.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://vl.wgjwhj.cn

[C03] 可变参数
来源：http://qv.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://ua.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cd.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fs.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bk.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qx.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sc.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jm.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wq.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://ad.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lk.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mo.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hy.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aa.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://lh.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://gl.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://cf.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://qz.jianghongdianzi.cn

[C05] 返回多个值
来源：http://gz.yuexingan06.cn

Py:   return a, b
来源：http://uj.huanxung.cn

PHP:  return [$a, $b];
来源：http://xu.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mc.szxytkj.cn

TS:   return { a, b };
来源：http://nz.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yd.jianghongdianzi.cn

Go:   return a, b
来源：http://zi.haigaiapp.cn

Ruby: return a, b
来源：http://py.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ni.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://ts.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://ji.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bg.huanxung.cn

JS:   const square = x => x * x;
来源：http://uv.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://sn.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hg.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://es.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://iv.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wy.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://vd.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://do.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sv.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oo.bookmarksfly.cn

TS:   arr.map(String)
来源：http://zu.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cz.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hr.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://bl.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ih.jctech888.com.cn

[C08] 闭包
来源：http://th.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vd.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kb.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hp.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oe.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eb.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ko.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bk.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ra.huixinmuqiang.cn

[C09] 递归
来源：http://ao.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bc.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rv.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ij.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://op.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gb.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wx.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rx.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cw.lnxyls.cn

[C10] 变量作用域
来源：http://qt.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xj.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ui.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zy.bjjhwx.cn

TS:   同 JS
来源：http://tn.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://qp.shxzskj.cn

Go:   花括号块级作用域
来源：http://do.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qu.huixinmuqiang.cn

C#:   块级作用域
来源：http://bt.panjiajie.cn

[C11] 模块导入与导出
来源：http://uy.asd995.cn

Py:   from module import func
来源：http://pi.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cg.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cz.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gk.haigaiapp.cn

Java: import java.util.List;
来源：http://qo.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ag.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://rl.asd995.cn

C#:   using System.Text;
来源：http://jt.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://zh.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://hw.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://rp.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://se.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://ok.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://op.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://ri.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://ta.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lq.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://pt.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://js.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bu.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://du.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dq.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zw.newstarts.cn

Go:   func add(a, b int) int
来源：http://gf.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pe.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yp.bookmarksfly.cn

[C14] 泛型函数
来源：http://ll.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vg.gzmigu.cn

PHP:  // 无泛型
来源：http://ui.bjjhwx.cn

JS:   // 无泛型
来源：http://rv.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ks.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qg.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mw.lnxyls.cn

Ruby: # 无泛型
来源：http://ux.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rx.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://av.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cp.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://wu.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zp.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wn.yuexingan06.cn

Java: // 无解构
来源：http://ov.shxzskj.cn

Go:   // 无解构
来源：http://ch.szsharing.cn

Ruby: a, b = pair
来源：http://bu.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://gx.colortex.cn

[C16] 函数 / 方法重载
来源：http://eo.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ma.lnxyls.cn

PHP:  // 无重载
来源：http://no.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mq.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://bo.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nu.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://rd.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://mc.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://as.newstarts.cn

================================================================================
来源：http://ar.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://zk.shtwfgs.cn

================================================================================
来源：http://kp.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://rx.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hk.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pq.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bn.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ha.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://td.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://fk.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://um.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jr.hnjuh.cn

[D02] 追加元素到末尾
来源：http://qd.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://um.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sr.yuexingan06.cn

JS:   arr.push(4);
来源：http://jq.szxytkj.cn

TS:   arr.push(4);
来源：http://an.hnjuh.cn


<!-- 参考信息 -->