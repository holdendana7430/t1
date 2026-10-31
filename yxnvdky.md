代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mp.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wl.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://py.9csxet.cn

[B04] for 计数循环
来源：http://pp.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://wa.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gi.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jq.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zc.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cd.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://px.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://st.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://id.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://zj.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://rw.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xz.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jk.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yp.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zz.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fd.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://fo.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yp.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://oq.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fq.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pf.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oe.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ft.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ik.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fy.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mf.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bn.muxihuayi.cn

[B07] while 循环
来源：http://xk.nszjky.cn

Py:   while i < 10: i += 1
来源：http://zl.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://se.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://ob.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://it.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://iz.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bw.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://sr.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://re.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://ev.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://dr.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gq.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://vt.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://ht.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://sl.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pb.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eb.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://xr.newstarts.cn

[B09] break 与 continue
来源：http://lz.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ye.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yu.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fp.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ri.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ng.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ip.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tc.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ly.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://ne.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wh.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cf.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://av.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hj.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zy.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pq.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nx.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gv.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://tp.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://ut.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://tt.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sg.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wq.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vj.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://in.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://er.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://md.shxzukj.cn

[B12] 跳出多层循环
来源：http://em.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nv.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zj.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ub.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fl.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hc.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oq.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vd.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ji.lnxyls.cn

[B13] 判断是否为数字
来源：http://cb.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://xn.asd995.cn

PHP:  is_numeric($x)
来源：http://it.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cg.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ju.huixinmuqiang.cn

Java: x instanceof Number
来源：http://gd.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jd.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://po.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://ed.huanxung.cn

[B14] 判断值是否在集合内
来源：http://ga.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tj.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qw.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://wm.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://oa.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bm.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kn.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mo.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oa.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://vt.jianghongdianzi.cn

Py:   a and b or not c
来源：http://rs.colortex.cn

PHP:  $a && $b || !$c
来源：http://go.nicolike.cn

JS:   a && b || !c
来源：http://xr.shtwfgs.cn

TS:   a && b || !c
来源：http://pv.shtwfgs.cn

Java: a && b || !c
来源：http://ss.shtwfgs.cn

Go:   a && b || !c
来源：http://gk.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://ve.huixinmuqiang.cn

C#:   a && b || !c
来源：http://jr.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cv.bookmarksfly.cn

Py:   if not data: return
来源：http://en.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://ha.szxytkj.cn

JS:   if (!data) return;
来源：http://jo.521024.cn

TS:   if (!data) return;
来源：http://wq.bjjhwx.cn

Java: if (data == null) return;
来源：http://wa.shtwfgs.cn

Go:   if data == nil { return }
来源：http://hs.jctech888.com.cn

Ruby: return if data.nil?
来源：http://rl.wgjwhj.cn

C#:   if (data == null) return;
来源：http://hr.szxytkj.cn

================================================================================
来源：http://ub.nszjky.cn

C. 函数与作用域
来源：http://cw.gzmigu.cn

================================================================================
来源：http://hc.haigaiapp.cn

[C01] 定义函数
来源：http://jb.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://vp.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qf.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://gf.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ha.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ww.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ye.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://ai.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yo.jctech888.com.cn

[C02] 默认参数
来源：http://xl.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://hv.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sm.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://af.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lz.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bu.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ff.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://ct.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ka.gzmigu.cn

[C03] 可变参数
来源：http://tg.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://cb.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nx.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pd.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ig.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ru.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ro.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fa.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ax.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://mz.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qa.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fx.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eu.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ol.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://qa.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://jp.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://qq.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://uf.bjjhwx.cn

[C05] 返回多个值
来源：http://dx.wgjwhj.cn

Py:   return a, b
来源：http://pd.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://er.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://as.szxytkj.cn

TS:   return { a, b };
来源：http://of.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yo.jianghongdianzi.cn

Go:   return a, b
来源：http://ke.huixinmuqiang.cn

Ruby: return a, b
来源：http://lb.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://hk.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://rl.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://cb.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ek.shxzukj.cn

JS:   const square = x => x * x;
来源：http://xk.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://si.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lf.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://se.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://ig.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lw.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://dq.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iq.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mc.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yu.haigaiapp.cn

TS:   arr.map(String)
来源：http://sy.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ap.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://du.521024.cn

Ruby: arr.map(&:upcase)
来源：http://dv.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ze.szsharing.cn

[C08] 闭包
来源：http://oy.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xi.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ab.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bw.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jk.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ck.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ws.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ie.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://he.hahajie.cn

[C09] 递归
来源：http://ho.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rr.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sd.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pn.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://om.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fn.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qy.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fe.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ed.colortex.cn

[C10] 变量作用域
来源：http://pp.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lv.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wb.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qm.shtwfgs.cn

TS:   同 JS
来源：http://re.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://jo.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://aa.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uh.nicolike.cn

C#:   块级作用域
来源：http://gq.huanxung.cn

[C11] 模块导入与导出
来源：http://oz.asd995.cn

Py:   from module import func
来源：http://rt.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pj.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pd.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hd.huixinmuqiang.cn

Java: import java.util.List;
来源：http://bf.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://io.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://vw.shxzskj.cn

C#:   using System.Text;
来源：http://ez.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://za.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://jh.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://ja.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://wf.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://qc.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gs.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://mp.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://vk.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ft.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://km.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mk.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nj.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eb.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://da.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ns.9csxet.cn

Go:   func add(a, b int) int
来源：http://et.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gr.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ak.jianghongdianzi.cn

[C14] 泛型函数
来源：http://kb.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yb.asd995.cn

PHP:  // 无泛型
来源：http://zt.bjjhwx.cn

JS:   // 无泛型
来源：http://yr.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yo.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qt.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uu.huanxung.cn

Ruby: # 无泛型
来源：http://ma.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ul.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://ag.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cv.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://dy.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ni.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pb.9csxet.cn

Java: // 无解构
来源：http://dm.shxzskj.cn

Go:   // 无解构
来源：http://sf.521024.cn

Ruby: a, b = pair
来源：http://wr.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://bx.huanxung.cn

[C16] 函数 / 方法重载
来源：http://uu.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vv.wgjwhj.cn

PHP:  // 无重载
来源：http://il.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://en.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://lo.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ug.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://bb.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://pd.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qg.newstarts.cn

================================================================================
来源：http://ew.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://cy.nicolike.cn

================================================================================
来源：http://bn.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://sb.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jf.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fb.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hk.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ii.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dz.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://qr.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://mo.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gl.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://to.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xd.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wj.521024.cn

JS:   arr.push(4);
来源：http://wh.huanxung.cn

TS:   arr.push(4);
来源：http://ya.haigaiapp.cn

Java: list.add(4);
来源：http://ke.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://dl.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://bu.chemitech.net.cn

C#:   list.Add(4);
来源：http://mt.nszjky.cn

[D03] 在指定位置插入元素
来源：http://pr.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://cz.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nj.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rr.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://to.shtwfgs.cn

Java: list.add(0, 0);
来源：http://ui.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bg.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iv.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://ao.jctech888.com.cn

[D04] 删除元素
来源：http://sn.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fq.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fd.wgjwhj.cn


<!-- 参考信息 -->