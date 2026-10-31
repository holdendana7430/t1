代发 wailian999

Py:   for i in range(10): print(i)
来源：http://xl.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mb.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vj.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ss.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rs.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xu.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://my.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hq.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://hs.szsharing.cn

Py:   for item in arr: print(item)
来源：http://dw.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kd.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ne.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nn.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vt.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xk.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://bs.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fc.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://xt.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://su.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gg.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sy.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ia.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kx.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gr.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ea.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kn.jianghongdianzi.cn

[B07] while 循环
来源：http://qr.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://fz.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ui.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://jm.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://pf.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://hm.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jw.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://je.521024.cn

C#:   while (i < 10) { i++; }
来源：http://rv.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://ak.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://by.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dc.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://cg.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://bn.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://tx.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bz.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ic.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://kt.9csxet.cn

[B09] break 与 continue
来源：http://lh.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tt.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lc.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zv.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cm.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cf.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cz.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ae.colortex.cn

[B10] 遍历同时拿索引
来源：http://ks.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zc.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ao.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cr.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ni.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ht.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xh.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ra.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ao.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://vt.521024.cn

Py:   list(range(0, 10, 2))
来源：http://dp.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://ib.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kz.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gr.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bp.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tm.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://ls.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rs.asd995.cn

[B12] 跳出多层循环
来源：http://yr.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sq.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ee.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://du.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eb.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jt.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wb.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dz.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://id.wgjwhj.cn

[B13] 判断是否为数字
来源：http://up.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://fk.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://gk.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wh.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vb.panjiajie.cn

Java: x instanceof Number
来源：http://ik.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jz.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://yh.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://pt.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://dp.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pr.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qr.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://tp.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://ki.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hm.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xm.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cv.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zz.asd995.cn

[B15] 布尔运算与取反
来源：http://ca.szsharing.cn

Py:   a and b or not c
来源：http://cg.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://rs.nszjky.cn

JS:   a && b || !c
来源：http://kv.szxytkj.cn

TS:   a && b || !c
来源：http://pj.newstarts.cn

Java: a && b || !c
来源：http://bj.huixiangedu.cn

Go:   a && b || !c
来源：http://vy.lnxyls.cn

Ruby: a && b || !c
来源：http://aq.9csxet.cn

C#:   a && b || !c
来源：http://nr.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yg.huanxung.cn

Py:   if not data: return
来源：http://kl.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://fi.9csxet.cn

JS:   if (!data) return;
来源：http://fc.panjiajie.cn

TS:   if (!data) return;
来源：http://gu.shtwfgs.cn

Java: if (data == null) return;
来源：http://kl.shxzskj.cn

Go:   if data == nil { return }
来源：http://xh.bjjhwx.cn

Ruby: return if data.nil?
来源：http://sj.bjjhwx.cn

C#:   if (data == null) return;
来源：http://pj.szxytkj.cn

================================================================================
来源：http://nt.haigaiapp.cn

C. 函数与作用域
来源：http://no.nicolike.cn

================================================================================
来源：http://qq.panjiajie.cn

[C01] 定义函数
来源：http://fa.asd995.cn

Py:   def add(a, b): return a + b
来源：http://og.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xl.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://sr.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zv.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kd.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qh.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://uo.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://um.shxzukj.cn

[C02] 默认参数
来源：http://vr.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://gu.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cd.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://bs.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bq.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qd.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eu.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://cm.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://cp.lnxyls.cn

[C03] 可变参数
来源：http://uh.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ax.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jn.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qu.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ax.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bk.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bv.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gi.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qa.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://dt.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rn.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mf.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ru.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jm.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://qt.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://eg.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://nh.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://de.gzmigu.cn

[C05] 返回多个值
来源：http://ll.szxytkj.cn

Py:   return a, b
来源：http://fq.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://wb.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yd.hnjuh.cn

TS:   return { a, b };
来源：http://yb.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lz.newstarts.cn

Go:   return a, b
来源：http://gq.wgjwhj.cn

Ruby: return a, b
来源：http://qp.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://ed.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://fo.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://xt.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ya.szxytkj.cn

JS:   const square = x => x * x;
来源：http://ri.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://tp.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zj.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wc.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://ri.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qp.asd995.cn

[C07] 把函数作为参数传入
来源：http://pd.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vh.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xu.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dr.yuexingan06.cn

TS:   arr.map(String)
来源：http://zb.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jn.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zr.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://at.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ib.521024.cn

[C08] 闭包
来源：http://bj.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eg.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xn.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ua.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wi.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rv.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://je.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wq.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nz.shtwfgs.cn

[C09] 递归
来源：http://jx.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qt.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zp.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rb.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hj.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pn.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gz.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jh.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ir.shtwfgs.cn

[C10] 变量作用域
来源：http://el.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gv.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iw.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jq.bjjhwx.cn

TS:   同 JS
来源：http://ys.hahajie.cn

Java: 方法内为块级作用域
来源：http://sw.huanxung.cn

Go:   花括号块级作用域
来源：http://nn.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uq.yuexingan06.cn

C#:   块级作用域
来源：http://wt.shxzukj.cn

[C11] 模块导入与导出
来源：http://dx.huixiangedu.cn

Py:   from module import func
来源：http://ar.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aj.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gg.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mv.yuntaijiaju.cn

Java: import java.util.List;
来源：http://pu.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lk.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://ru.nicolike.cn

C#:   using System.Text;
来源：http://nl.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://ck.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://kp.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://fw.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://fv.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://pn.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zx.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://ne.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://hm.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cn.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://sm.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zw.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ir.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mj.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vf.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wq.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://df.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ur.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://st.shtwfgs.cn

[C14] 泛型函数
来源：http://ze.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ua.newstarts.cn

PHP:  // 无泛型
来源：http://fr.bookmarksfly.cn

JS:   // 无泛型
来源：http://wh.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rh.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rd.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ok.shtwfgs.cn

Ruby: # 无泛型
来源：http://ai.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qc.newstarts.cn

[C15] 解构 / 展开参数
来源：http://fd.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nq.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://em.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aj.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ki.huanxung.cn

Java: // 无解构
来源：http://wl.huixiangedu.cn

Go:   // 无解构
来源：http://xq.shxzskj.cn

Ruby: a, b = pair
来源：http://rj.9csxet.cn

C#:   var (a, b) = pair;
来源：http://bd.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://lr.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://km.colortex.cn

PHP:  // 无重载
来源：http://ec.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lu.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://gl.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vl.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://me.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://kp.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oj.bjjhwx.cn

================================================================================
来源：http://ce.colortex.cn

D. 数组 / 列表 / 集合
来源：http://ba.asd995.cn

================================================================================
来源：http://vh.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://fo.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ub.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lu.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lo.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fv.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cz.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://ad.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://xp.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mg.lnxyls.cn

[D02] 追加元素到末尾
来源：http://ty.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ih.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hd.chemitech.net.cn

JS:   arr.push(4);
来源：http://zw.521024.cn

TS:   arr.push(4);
来源：http://oh.lnxyls.cn

Java: list.add(4);
来源：http://ou.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://io.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://bs.shtwfgs.cn

C#:   list.Add(4);
来源：http://wr.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://aq.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://oj.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wq.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wr.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://it.wgjwhj.cn

Java: list.add(0, 0);
来源：http://qh.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://up.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xj.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://fh.huixiangedu.cn

[D04] 删除元素
来源：http://sn.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cr.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://an.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pa.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://sz.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wf.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qu.shtwfgs.cn


<!-- 参考信息 -->