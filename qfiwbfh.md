代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://av.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vn.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eg.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rm.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yz.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zy.gzmigu.cn

[B03] switch / match / case
来源：http://og.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pu.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oh.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gh.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vd.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sv.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yb.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ze.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yc.huanxung.cn

[B04] for 计数循环
来源：http://ul.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://dc.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fj.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pr.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uq.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qk.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xg.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://cz.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hr.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://el.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://nq.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vo.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gt.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nr.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://su.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nf.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://kb.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tx.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://cb.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cv.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uc.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vv.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://li.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ex.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nu.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rr.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lu.nicolike.cn

[B07] while 循环
来源：http://pw.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://iz.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bx.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://yi.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://yt.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://md.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wt.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://kj.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://eg.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://zd.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ua.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sd.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://xc.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://jm.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://id.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hc.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qj.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://tb.lnxyls.cn

[B09] break 与 continue
来源：http://zx.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pb.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zn.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://et.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ib.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pq.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ed.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wt.nicolike.cn

[B10] 遍历同时拿索引
来源：http://sn.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sq.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cv.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ky.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pd.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mr.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xm.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zy.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mv.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://rf.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://zf.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://hk.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aa.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rr.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pq.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rx.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://uc.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cu.panjiajie.cn

[B12] 跳出多层循环
来源：http://fl.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jq.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pw.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zl.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tk.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hy.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lt.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://au.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hs.jctech888.com.cn

[B13] 判断是否为数字
来源：http://jk.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://nr.newstarts.cn

PHP:  is_numeric($x)
来源：http://gr.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xf.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rs.lnxyls.cn

Java: x instanceof Number
来源：http://jh.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hj.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://fr.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://gf.hahajie.cn

[B14] 判断值是否在集合内
来源：http://nl.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gu.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://un.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://hh.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://gg.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xq.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ld.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://si.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fl.nszjky.cn

[B15] 布尔运算与取反
来源：http://kt.colortex.cn

Py:   a and b or not c
来源：http://xl.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://ja.colortex.cn

JS:   a && b || !c
来源：http://aj.hahajie.cn

TS:   a && b || !c
来源：http://qs.huixiangedu.cn

Java: a && b || !c
来源：http://fo.nicolike.cn

Go:   a && b || !c
来源：http://gd.bookmarksfly.cn

Ruby: a && b || !c
来源：http://so.panjiajie.cn

C#:   a && b || !c
来源：http://bt.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ju.shxzskj.cn

Py:   if not data: return
来源：http://hr.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://bh.yuexingan06.cn

JS:   if (!data) return;
来源：http://aq.521024.cn

TS:   if (!data) return;
来源：http://ip.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://bo.newstarts.cn

Go:   if data == nil { return }
来源：http://vc.colortex.cn

Ruby: return if data.nil?
来源：http://vc.shxzukj.cn

C#:   if (data == null) return;
来源：http://ww.gzmigu.cn

================================================================================
来源：http://yg.9csxet.cn

C. 函数与作用域
来源：http://be.lnxyls.cn

================================================================================
来源：http://lk.wgjwhj.cn

[C01] 定义函数
来源：http://mq.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://ld.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hm.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://my.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tw.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aj.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ub.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://hl.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hb.jctech888.com.cn

[C02] 默认参数
来源：http://jw.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://qi.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ic.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://gy.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zo.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hm.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://da.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://fr.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://ug.shtwfgs.cn

[C03] 可变参数
来源：http://qv.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://lp.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gu.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ap.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ma.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zo.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qa.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mh.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kk.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://mu.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hm.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gb.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dl.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lh.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://wd.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://ye.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://qc.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://yk.bjjhwx.cn

[C05] 返回多个值
来源：http://kf.panjiajie.cn

Py:   return a, b
来源：http://ou.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://rb.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://io.huanxung.cn

TS:   return { a, b };
来源：http://bm.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cz.jctech888.com.cn

Go:   return a, b
来源：http://wt.shxzukj.cn

Ruby: return a, b
来源：http://ze.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://gz.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://cl.hahajie.cn

Py:   square = lambda x: x * x
来源：http://do.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cy.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://pe.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://cy.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rf.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sy.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://mc.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ty.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://he.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jc.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oy.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sw.haigaiapp.cn

TS:   arr.map(String)
来源：http://vs.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ec.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ky.521024.cn

Ruby: arr.map(&:upcase)
来源：http://wm.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ak.chemitech.net.cn

[C08] 闭包
来源：http://oo.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nq.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yg.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jx.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vn.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oi.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yb.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gx.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kl.bjjhwx.cn

[C09] 递归
来源：http://eq.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vx.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qs.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xm.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sg.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cc.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gt.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ry.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gb.huixiangedu.cn

[C10] 变量作用域
来源：http://yg.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sf.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kx.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ac.huixiangedu.cn

TS:   同 JS
来源：http://ja.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://fh.szsharing.cn

Go:   花括号块级作用域
来源：http://sj.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iy.yuexingan06.cn

C#:   块级作用域
来源：http://ol.newstarts.cn

[C11] 模块导入与导出
来源：http://cx.nszjky.cn

Py:   from module import func
来源：http://bb.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://id.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yb.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zk.lnxyls.cn

Java: import java.util.List;
来源：http://xm.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rt.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://bj.szxytkj.cn

C#:   using System.Text;
来源：http://jw.521024.cn

[C12] 立即执行函数 IIFE
来源：http://hg.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://oj.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://uu.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://iy.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://xa.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yh.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://gj.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://ao.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ct.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://bu.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ru.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kw.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nw.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qq.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ah.hnjuh.cn

Go:   func add(a, b int) int
来源：http://cd.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pc.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://go.huixinmuqiang.cn

[C14] 泛型函数
来源：http://ko.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gk.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://ub.9csxet.cn

JS:   // 无泛型
来源：http://rp.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ew.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ns.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://we.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://bi.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tc.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://sm.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yy.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://et.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://od.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gg.jctech888.com.cn

Java: // 无解构
来源：http://rv.shxzukj.cn

Go:   // 无解构
来源：http://xt.shxzskj.cn

Ruby: a, b = pair
来源：http://yb.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://ho.nicolike.cn

[C16] 函数 / 方法重载
来源：http://cw.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ca.szsharing.cn

PHP:  // 无重载
来源：http://va.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nt.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://fh.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dd.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://yk.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://ne.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gq.gzmigu.cn

================================================================================
来源：http://qh.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://av.haigaiapp.cn

================================================================================
来源：http://uk.szsharing.cn

[D01] 创建数组 / 列表
来源：http://at.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ff.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wd.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zx.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pr.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bu.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://kf.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://qi.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ib.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://iw.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ij.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://px.szsharing.cn

JS:   arr.push(4);
来源：http://ct.521024.cn

TS:   arr.push(4);
来源：http://ub.lnxyls.cn

Java: list.add(4);
来源：http://lk.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://rl.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://rn.bjjhwx.cn

C#:   list.Add(4);
来源：http://lb.muxihuayi.cn


<!-- 参考信息 -->