代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bb.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kx.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qg.shxzukj.cn

[B04] for 计数循环
来源：http://yi.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://gt.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pk.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tr.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lg.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qk.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jk.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://vb.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uk.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://nb.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://ls.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://as.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rn.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tw.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bl.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://st.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://oz.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ef.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://rn.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sz.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qg.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ak.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xc.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ww.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bq.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pc.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kx.huanxung.cn

[B07] while 循环
来源：http://ii.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://mb.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fa.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://aj.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://ji.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://lu.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ah.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://vx.521024.cn

C#:   while (i < 10) { i++; }
来源：http://ub.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://en.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://lf.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rp.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://de.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://wj.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://wt.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eh.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rz.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://ff.asd995.cn

[B09] break 与 continue
来源：http://xd.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xz.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://in.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tt.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yp.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ms.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hy.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nb.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lc.newstarts.cn

[B10] 遍历同时拿索引
来源：http://ow.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eg.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cf.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ot.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nj.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gw.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vt.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gm.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kz.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://pk.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://xj.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://hd.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pi.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pu.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pt.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ex.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://xk.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://du.yuexingan06.cn

[B12] 跳出多层循环
来源：http://cs.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gs.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hi.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nw.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fo.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zt.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jz.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ib.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fk.panjiajie.cn

[B13] 判断是否为数字
来源：http://pe.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://zg.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://tg.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ls.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nr.huixiangedu.cn

Java: x instanceof Number
来源：http://iq.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cf.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://iq.hahajie.cn

C#:   x is int or double or decimal
来源：http://mq.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://gf.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gk.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cs.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://vo.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://aw.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://le.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zp.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ge.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zn.hnjuh.cn

[B15] 布尔运算与取反
来源：http://xs.shtwfgs.cn

Py:   a and b or not c
来源：http://zb.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://kd.9csxet.cn

JS:   a && b || !c
来源：http://vy.colortex.cn

TS:   a && b || !c
来源：http://it.hahajie.cn

Java: a && b || !c
来源：http://ny.asd995.cn

Go:   a && b || !c
来源：http://vl.bookmarksfly.cn

Ruby: a && b || !c
来源：http://tk.newstarts.cn

C#:   a && b || !c
来源：http://io.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bo.9csxet.cn

Py:   if not data: return
来源：http://qn.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://lz.panjiajie.cn

JS:   if (!data) return;
来源：http://if.shtwfgs.cn

TS:   if (!data) return;
来源：http://pp.muxihuayi.cn

Java: if (data == null) return;
来源：http://eb.521024.cn

Go:   if data == nil { return }
来源：http://vv.lnxyls.cn

Ruby: return if data.nil?
来源：http://hy.hahajie.cn

C#:   if (data == null) return;
来源：http://xo.bookmarksfly.cn

================================================================================
来源：http://ff.yuntaijiaju.cn

C. 函数与作用域
来源：http://sn.lnxyls.cn

================================================================================
来源：http://hr.yuexingan06.cn

[C01] 定义函数
来源：http://iv.colortex.cn

Py:   def add(a, b): return a + b
来源：http://qn.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rm.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://fh.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mv.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mq.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ig.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://mg.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cq.chemitech.net.cn

[C02] 默认参数
来源：http://ds.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://bs.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bf.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://fn.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oh.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lj.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ws.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://dp.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://bd.panjiajie.cn

[C03] 可变参数
来源：http://jl.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://ep.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jo.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wd.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dm.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ol.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wm.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kf.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pb.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://na.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xi.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hf.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ad.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mk.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://eb.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://hg.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://wc.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://dv.hahajie.cn

[C05] 返回多个值
来源：http://rs.haigaiapp.cn

Py:   return a, b
来源：http://my.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://pr.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ml.szsharing.cn

TS:   return { a, b };
来源：http://vk.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mi.szxytkj.cn

Go:   return a, b
来源：http://ym.shtwfgs.cn

Ruby: return a, b
来源：http://mk.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://zk.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://kc.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://uh.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wo.colortex.cn

JS:   const square = x => x * x;
来源：http://xe.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://sd.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ei.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bh.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://hn.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pz.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://qw.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zc.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://me.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bj.shxzukj.cn

TS:   arr.map(String)
来源：http://mm.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://if.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xb.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://nt.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ar.gzmigu.cn

[C08] 闭包
来源：http://xw.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rn.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ls.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://js.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://im.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vs.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bo.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ap.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ch.huixinmuqiang.cn

[C09] 递归
来源：http://yq.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bc.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://al.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kb.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xh.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ql.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qv.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sx.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://um.newstarts.cn

[C10] 变量作用域
来源：http://hc.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vk.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kh.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ar.huixinmuqiang.cn

TS:   同 JS
来源：http://yi.nicolike.cn

Java: 方法内为块级作用域
来源：http://zm.bjjhwx.cn

Go:   花括号块级作用域
来源：http://mo.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zl.szxytkj.cn

C#:   块级作用域
来源：http://jh.521024.cn

[C11] 模块导入与导出
来源：http://ob.colortex.cn

Py:   from module import func
来源：http://td.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lz.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yv.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eh.huixiangedu.cn

Java: import java.util.List;
来源：http://wa.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://et.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://rb.huixiangedu.cn

C#:   using System.Text;
来源：http://as.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://ci.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://lx.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://ts.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://gx.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://xl.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qh.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://sr.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://xd.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://af.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://pq.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zi.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qw.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iw.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pt.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gg.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://ym.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ly.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ce.bookmarksfly.cn

[C14] 泛型函数
来源：http://wu.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xx.chemitech.net.cn

PHP:  // 无泛型
来源：http://ei.yuexingan06.cn

JS:   // 无泛型
来源：http://hn.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ny.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pm.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tn.shxzskj.cn

Ruby: # 无泛型
来源：http://ah.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sf.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://kp.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jr.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://bi.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bb.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aw.shxzukj.cn

Java: // 无解构
来源：http://en.yuntaijiaju.cn

Go:   // 无解构
来源：http://lr.asd995.cn

Ruby: a, b = pair
来源：http://qa.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://yl.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://ae.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cz.nszjky.cn

PHP:  // 无重载
来源：http://qr.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ru.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://im.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wj.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://zz.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://ds.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qt.nszjky.cn

================================================================================
来源：http://vs.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://yx.9csxet.cn

================================================================================
来源：http://ws.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://ca.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nc.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qx.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fv.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sw.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gv.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://mz.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://qb.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jp.521024.cn

[D02] 追加元素到末尾
来源：http://ls.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lj.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mh.huanxung.cn

JS:   arr.push(4);
来源：http://ku.colortex.cn

TS:   arr.push(4);
来源：http://qd.jianghongdianzi.cn

Java: list.add(4);
来源：http://tg.asd995.cn

Go:   arr = append(arr, 4)
来源：http://mf.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://ja.newstarts.cn

C#:   list.Add(4);
来源：http://ba.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://nn.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://ro.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iv.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vi.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://df.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://hv.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dy.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yo.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://jl.yuntaijiaju.cn

[D04] 删除元素
来源：http://qj.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://px.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uo.bookmarksfly.cn


<!-- 参考信息 -->