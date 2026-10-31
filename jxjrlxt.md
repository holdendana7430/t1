代发 wailian999

Py:   for i in range(10): print(i)
来源：http://hi.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qz.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://em.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yx.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iy.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fg.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://zm.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oc.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://ro.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://if.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nl.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://so.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zj.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pf.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://md.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://om.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hh.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://hk.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lb.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kx.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ci.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cj.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ta.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://is.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ln.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hl.szxytkj.cn

[B07] while 循环
来源：http://dg.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://vi.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://am.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://id.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://gq.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://nq.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hb.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://bj.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://vh.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://bi.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ua.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fh.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://ob.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://wc.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://sd.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pl.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lj.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://ww.haigaiapp.cn

[B09] break 与 continue
来源：http://aa.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ib.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qw.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rz.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tn.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jx.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://in.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://om.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eo.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://pl.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qn.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ia.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xz.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://al.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lz.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ax.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rh.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ss.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://hu.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ti.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://fk.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://un.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tm.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://de.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hg.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://zx.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aj.hnjuh.cn

[B12] 跳出多层循环
来源：http://tl.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gg.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mi.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sd.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gg.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bx.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ql.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ln.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ae.lnxyls.cn

[B13] 判断是否为数字
来源：http://ac.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://hi.szxytkj.cn

PHP:  is_numeric($x)
来源：http://xz.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pz.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://md.bjjhwx.cn

Java: x instanceof Number
来源：http://rl.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nl.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://ma.nszjky.cn

C#:   x is int or double or decimal
来源：http://dd.nszjky.cn

[B14] 判断值是否在集合内
来源：http://gd.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hh.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wa.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://li.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://vr.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gg.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://np.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lm.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://df.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://sp.wgjwhj.cn

Py:   a and b or not c
来源：http://me.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://je.bookmarksfly.cn

JS:   a && b || !c
来源：http://tb.shtwfgs.cn

TS:   a && b || !c
来源：http://wx.hahajie.cn

Java: a && b || !c
来源：http://bs.huanxung.cn

Go:   a && b || !c
来源：http://qf.lnxyls.cn

Ruby: a && b || !c
来源：http://iq.nicolike.cn

C#:   a && b || !c
来源：http://vi.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sb.jctech888.com.cn

Py:   if not data: return
来源：http://eg.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://sb.szsharing.cn

JS:   if (!data) return;
来源：http://xc.521024.cn

TS:   if (!data) return;
来源：http://ji.newstarts.cn

Java: if (data == null) return;
来源：http://xg.bjjhwx.cn

Go:   if data == nil { return }
来源：http://jf.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://xo.asd995.cn

C#:   if (data == null) return;
来源：http://jd.yuexingan06.cn

================================================================================
来源：http://ez.chemitech.net.cn

C. 函数与作用域
来源：http://jn.jctech888.com.cn

================================================================================
来源：http://kx.shxzskj.cn

[C01] 定义函数
来源：http://jh.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://sr.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ji.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ig.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cm.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nd.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vy.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://vi.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tf.huixinmuqiang.cn

[C02] 默认参数
来源：http://kk.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://dk.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vt.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://uc.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://em.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lb.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://we.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://fx.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://gq.shxzskj.cn

[C03] 可变参数
来源：http://bo.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://op.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kn.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uf.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ra.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ph.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zg.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kw.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lc.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://eg.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ip.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vt.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ih.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cs.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://vx.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://zz.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://ts.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://ti.shxzskj.cn

[C05] 返回多个值
来源：http://jp.newstarts.cn

Py:   return a, b
来源：http://er.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://ec.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fu.huanxung.cn

TS:   return { a, b };
来源：http://do.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jh.newstarts.cn

Go:   return a, b
来源：http://xr.huanxung.cn

Ruby: return a, b
来源：http://yz.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://oo.521024.cn

[C06] 匿名函数 / lambda
来源：http://ig.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://hs.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zl.shxzukj.cn

JS:   const square = x => x * x;
来源：http://wt.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://zz.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oq.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gb.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://iv.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vy.hahajie.cn

[C07] 把函数作为参数传入
来源：http://lq.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://go.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dz.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cs.panjiajie.cn

TS:   arr.map(String)
来源：http://gs.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ew.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sh.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://nz.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oy.huixiangedu.cn

[C08] 闭包
来源：http://or.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ky.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wh.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://py.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xn.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wb.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yq.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mc.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zy.chemitech.net.cn

[C09] 递归
来源：http://zv.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://po.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ou.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nh.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zy.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nz.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wq.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mw.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tz.jctech888.com.cn

[C10] 变量作用域
来源：http://dw.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gv.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rz.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pf.panjiajie.cn

TS:   同 JS
来源：http://sa.panjiajie.cn

Java: 方法内为块级作用域
来源：http://rs.haigaiapp.cn

Go:   花括号块级作用域
来源：http://lo.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lg.bjjhwx.cn

C#:   块级作用域
来源：http://ng.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://ai.newstarts.cn

Py:   from module import func
来源：http://ls.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vz.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fx.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ys.chemitech.net.cn

Java: import java.util.List;
来源：http://cq.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://if.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://mo.521024.cn

C#:   using System.Text;
来源：http://am.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://vg.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://ke.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://jp.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://gz.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://vv.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xb.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://xb.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://ur.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uz.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://eu.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wp.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sw.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fy.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oc.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lo.hnjuh.cn

Go:   func add(a, b int) int
来源：http://ls.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mm.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fs.hahajie.cn

[C14] 泛型函数
来源：http://mm.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rp.shxzukj.cn

PHP:  // 无泛型
来源：http://zl.huixiangedu.cn

JS:   // 无泛型
来源：http://fy.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rv.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tk.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zf.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://rf.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pz.521024.cn

[C15] 解构 / 展开参数
来源：http://el.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hr.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://kv.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zi.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://si.muxihuayi.cn

Java: // 无解构
来源：http://ia.yuexingan06.cn

Go:   // 无解构
来源：http://fw.panjiajie.cn

Ruby: a, b = pair
来源：http://hc.9csxet.cn

C#:   var (a, b) = pair;
来源：http://pu.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://cr.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iv.shtwfgs.cn

PHP:  // 无重载
来源：http://dz.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://no.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://yd.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tp.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://bu.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://tm.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cd.hahajie.cn

================================================================================
来源：http://tx.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://wg.huixinmuqiang.cn

================================================================================
来源：http://uh.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://ay.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nu.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://re.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vi.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ax.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nn.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://sg.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://mq.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bz.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://ug.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xj.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wl.shtwfgs.cn

JS:   arr.push(4);
来源：http://zf.muxihuayi.cn

TS:   arr.push(4);
来源：http://rb.szsharing.cn

Java: list.add(4);
来源：http://fk.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://di.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://yr.huixiangedu.cn

C#:   list.Add(4);
来源：http://la.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://yy.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://bi.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ai.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qh.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://yh.gzmigu.cn

Java: list.add(0, 0);
来源：http://yq.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yh.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jr.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://qd.yuntaijiaju.cn

[D04] 删除元素
来源：http://ho.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hc.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ps.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ps.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://sd.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pu.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://js.newstarts.cn


<!-- 参考信息 -->