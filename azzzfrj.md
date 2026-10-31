代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://no.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nt.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rw.bjjhwx.cn

[B04] for 计数循环
来源：http://ij.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://cw.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gk.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rb.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cu.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zk.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://of.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://xx.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yt.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://sv.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://cx.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vi.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jx.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tj.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lw.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sz.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://zi.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://ei.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xa.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fq.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ad.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xa.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uh.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nh.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://et.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ar.nicolike.cn

[B07] while 循环
来源：http://uq.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://hw.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xh.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://pb.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://cl.colortex.cn

Java: while (i < 10) { i++; }
来源：http://zg.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hp.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://rm.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://lz.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://wl.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://xu.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ut.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://td.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://xw.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://zq.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ur.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://do.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://rg.jianghongdianzi.cn

[B09] break 与 continue
来源：http://jl.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ft.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bh.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tn.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://un.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pl.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zy.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ex.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oj.hahajie.cn

[B10] 遍历同时拿索引
来源：http://jw.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bb.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ep.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bj.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oc.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gc.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zk.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://at.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://za.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://wx.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://sp.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://xs.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://em.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xm.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oj.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dd.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://en.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qk.nicolike.cn

[B12] 跳出多层循环
来源：http://jj.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lo.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ef.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tb.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oe.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ur.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xq.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jn.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yu.yuexingan06.cn

[B13] 判断是否为数字
来源：http://ds.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://be.panjiajie.cn

PHP:  is_numeric($x)
来源：http://kx.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ae.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oh.wgjwhj.cn

Java: x instanceof Number
来源：http://vw.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vb.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://ga.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://ac.colortex.cn

[B14] 判断值是否在集合内
来源：http://tg.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qm.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rs.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://dv.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://tc.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gg.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kf.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lo.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://br.shxzskj.cn

[B15] 布尔运算与取反
来源：http://zq.huanxung.cn

Py:   a and b or not c
来源：http://sb.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://vu.nicolike.cn

JS:   a && b || !c
来源：http://so.gzmigu.cn

TS:   a && b || !c
来源：http://lf.huixiangedu.cn

Java: a && b || !c
来源：http://zn.hnjuh.cn

Go:   a && b || !c
来源：http://sf.wgjwhj.cn

Ruby: a && b || !c
来源：http://we.nszjky.cn

C#:   a && b || !c
来源：http://pn.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zs.nicolike.cn

Py:   if not data: return
来源：http://lo.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://rh.szxytkj.cn

JS:   if (!data) return;
来源：http://yn.shtwfgs.cn

TS:   if (!data) return;
来源：http://ox.lnxyls.cn

Java: if (data == null) return;
来源：http://zd.lnxyls.cn

Go:   if data == nil { return }
来源：http://in.nszjky.cn

Ruby: return if data.nil?
来源：http://kl.nicolike.cn

C#:   if (data == null) return;
来源：http://sj.newstarts.cn

================================================================================
来源：http://fz.jctech888.com.cn

C. 函数与作用域
来源：http://wf.jianghongdianzi.cn

================================================================================
来源：http://vg.jctech888.com.cn

[C01] 定义函数
来源：http://kd.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://ap.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ml.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://hf.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qe.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://es.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://by.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://ak.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jg.yuexingan06.cn

[C02] 默认参数
来源：http://ll.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://ov.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gp.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://cm.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://en.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xj.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qf.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://iy.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://mc.shtwfgs.cn

[C03] 可变参数
来源：http://og.521024.cn

Py:   def total(*args): return sum(args)
来源：http://ur.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ts.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gb.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://te.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ju.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fe.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iy.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sh.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://fz.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ty.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hu.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ol.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gl.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://ti.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://le.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://cr.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://aw.chemitech.net.cn

[C05] 返回多个值
来源：http://cm.huixiangedu.cn

Py:   return a, b
来源：http://ru.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://dd.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tz.chemitech.net.cn

TS:   return { a, b };
来源：http://ga.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lc.nszjky.cn

Go:   return a, b
来源：http://jj.521024.cn

Ruby: return a, b
来源：http://qe.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://ac.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://fn.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://ct.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eg.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://gi.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://pr.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wv.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ea.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://ry.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ru.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://uc.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ym.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://us.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://at.jctech888.com.cn

TS:   arr.map(String)
来源：http://zr.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iw.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ux.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://gf.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ie.huixiangedu.cn

[C08] 闭包
来源：http://gp.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uz.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nn.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gm.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fn.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ri.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wz.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wq.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ew.bookmarksfly.cn

[C09] 递归
来源：http://mb.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hg.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kc.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ie.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gc.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cf.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://er.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rb.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://il.asd995.cn

[C10] 变量作用域
来源：http://dw.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://id.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://na.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cq.521024.cn

TS:   同 JS
来源：http://sx.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://bu.hahajie.cn

Go:   花括号块级作用域
来源：http://rw.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ri.haigaiapp.cn

C#:   块级作用域
来源：http://dc.nszjky.cn

[C11] 模块导入与导出
来源：http://xc.hnjuh.cn

Py:   from module import func
来源：http://dn.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yd.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nz.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wz.nszjky.cn

Java: import java.util.List;
来源：http://in.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sd.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://hq.shtwfgs.cn

C#:   using System.Text;
来源：http://hb.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://hd.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://or.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://un.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://ev.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://wg.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oj.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://yb.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://yp.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://um.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://vk.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kw.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rf.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qu.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yu.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mb.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://lj.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jn.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bh.bookmarksfly.cn

[C14] 泛型函数
来源：http://ri.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hf.haigaiapp.cn

PHP:  // 无泛型
来源：http://um.gzmigu.cn

JS:   // 无泛型
来源：http://fy.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wm.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yx.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cs.nszjky.cn

Ruby: # 无泛型
来源：http://ra.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wt.9csxet.cn

[C15] 解构 / 展开参数
来源：http://ts.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ek.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://os.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dg.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rd.huixinmuqiang.cn

Java: // 无解构
来源：http://ck.huixinmuqiang.cn

Go:   // 无解构
来源：http://zh.huanxung.cn

Ruby: a, b = pair
来源：http://io.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://yp.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://sc.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sf.jianghongdianzi.cn

PHP:  // 无重载
来源：http://te.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ze.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ym.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mr.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://hc.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://ef.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://th.huanxung.cn

================================================================================
来源：http://ho.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://qu.yuexingan06.cn

================================================================================
来源：http://dv.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://ny.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yp.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xo.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zx.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rm.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rg.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://px.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://vi.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gg.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://nl.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gq.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gb.shxzskj.cn

JS:   arr.push(4);
来源：http://tq.bookmarksfly.cn

TS:   arr.push(4);
来源：http://il.huanxung.cn

Java: list.add(4);
来源：http://iz.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://mv.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://wg.huanxung.cn

C#:   list.Add(4);
来源：http://jz.colortex.cn

[D03] 在指定位置插入元素
来源：http://en.521024.cn

Py:   arr.insert(0, 0)
来源：http://iw.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tl.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bl.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://ks.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://ew.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://in.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rq.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://wl.nszjky.cn

[D04] 删除元素
来源：http://hx.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ib.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nm.huixiangedu.cn


<!-- 参考信息 -->