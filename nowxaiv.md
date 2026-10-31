代发 wailian999

Py:   for i in range(10): print(i)
来源：http://di.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uy.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vd.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kc.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ws.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xz.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://ax.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://we.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://cb.huanxung.cn

Py:   for item in arr: print(item)
来源：http://cw.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iq.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://in.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qg.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jk.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://js.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://qc.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cy.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://hh.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ij.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zv.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qz.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qs.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://st.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ie.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ff.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yt.hahajie.cn

[B07] while 循环
来源：http://qy.newstarts.cn

Py:   while i < 10: i += 1
来源：http://jl.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ex.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://lx.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://tg.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://ah.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hr.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ve.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://pb.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://pl.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://kv.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://af.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://jy.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://jm.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://xm.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kn.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uw.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://vx.hnjuh.cn

[B09] break 与 continue
来源：http://bp.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cl.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vo.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nh.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ea.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qz.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fi.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nc.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rz.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://ad.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://to.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jo.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ps.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://se.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tn.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uv.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uf.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://um.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://rq.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://nl.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://ek.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rw.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wl.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://be.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ra.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://su.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zu.yuexingan06.cn

[B12] 跳出多层循环
来源：http://sa.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zg.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ua.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://js.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://so.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cv.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wz.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nc.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://au.yuexingan06.cn

[B13] 判断是否为数字
来源：http://sw.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://ch.newstarts.cn

PHP:  is_numeric($x)
来源：http://ju.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mp.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tz.lnxyls.cn

Java: x instanceof Number
来源：http://ek.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tk.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://fv.asd995.cn

C#:   x is int or double or decimal
来源：http://yk.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://ji.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iu.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pr.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://pp.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://ux.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zr.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gc.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kp.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lt.szsharing.cn

[B15] 布尔运算与取反
来源：http://ok.huanxung.cn

Py:   a and b or not c
来源：http://ky.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://sy.muxihuayi.cn

JS:   a && b || !c
来源：http://zq.shtwfgs.cn

TS:   a && b || !c
来源：http://to.yuexingan06.cn

Java: a && b || !c
来源：http://no.haigaiapp.cn

Go:   a && b || !c
来源：http://yv.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://mf.nszjky.cn

C#:   a && b || !c
来源：http://sk.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ya.muxihuayi.cn

Py:   if not data: return
来源：http://du.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://hr.521024.cn

JS:   if (!data) return;
来源：http://sl.nszjky.cn

TS:   if (!data) return;
来源：http://bt.asd995.cn

Java: if (data == null) return;
来源：http://pn.nszjky.cn

Go:   if data == nil { return }
来源：http://ay.wgjwhj.cn

Ruby: return if data.nil?
来源：http://ra.newstarts.cn

C#:   if (data == null) return;
来源：http://rl.nicolike.cn

================================================================================
来源：http://nl.lnxyls.cn

C. 函数与作用域
来源：http://ii.szxytkj.cn

================================================================================
来源：http://jt.shxzskj.cn

[C01] 定义函数
来源：http://zf.521024.cn

Py:   def add(a, b): return a + b
来源：http://uy.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ok.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://lo.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oh.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kh.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lp.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://rl.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pi.yuexingan06.cn

[C02] 默认参数
来源：http://hb.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://eq.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cp.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ae.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zz.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fj.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zh.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://hg.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://sq.huanxung.cn

[C03] 可变参数
来源：http://ve.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://oq.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kb.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sm.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uc.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ku.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sc.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fp.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jx.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://gz.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rx.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sh.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wm.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jy.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://rt.521024.cn

Go:   // 无：用配置结构体参数
来源：http://av.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://lv.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://qa.szsharing.cn

[C05] 返回多个值
来源：http://kv.huanxung.cn

Py:   return a, b
来源：http://nx.shxzukj.cn

PHP:  return [$a, $b];
来源：http://ad.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zf.bjjhwx.cn

TS:   return { a, b };
来源：http://gv.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ea.nicolike.cn

Go:   return a, b
来源：http://ck.szsharing.cn

Ruby: return a, b
来源：http://ho.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://wg.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://xz.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://vh.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ch.szxytkj.cn

JS:   const square = x => x * x;
来源：http://yc.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://fh.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vc.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ya.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://nw.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bp.asd995.cn

[C07] 把函数作为参数传入
来源：http://sl.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://so.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oy.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ci.bjjhwx.cn

TS:   arr.map(String)
来源：http://li.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ps.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hq.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://sm.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yp.newstarts.cn

[C08] 闭包
来源：http://vf.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nk.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://so.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vv.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eq.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://md.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fj.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://td.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fw.521024.cn

[C09] 递归
来源：http://pi.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gx.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kf.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qz.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ro.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pb.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nl.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rs.shxzukj.cn

[C10] 变量作用域
来源：http://lc.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cp.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yi.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rb.shxzskj.cn

TS:   同 JS
来源：http://aw.gzmigu.cn

Java: 方法内为块级作用域
来源：http://le.haigaiapp.cn

Go:   花括号块级作用域
来源：http://jk.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tw.asd995.cn

C#:   块级作用域
来源：http://rg.colortex.cn

[C11] 模块导入与导出
来源：http://hd.nszjky.cn

Py:   from module import func
来源：http://pn.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mi.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oa.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vb.shxzskj.cn

Java: import java.util.List;
来源：http://db.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cn.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://pd.haigaiapp.cn

C#:   using System.Text;
来源：http://hr.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://pt.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://bn.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://io.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://of.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://mt.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gd.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://bg.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://id.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ck.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://ks.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rz.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iy.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://he.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ky.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jt.9csxet.cn

Go:   func add(a, b int) int
来源：http://ob.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rl.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://en.bjjhwx.cn

[C14] 泛型函数
来源：http://wz.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ey.bookmarksfly.cn

PHP:  // 无泛型
来源：http://dd.9csxet.cn

JS:   // 无泛型
来源：http://yg.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pm.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aj.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://is.bjjhwx.cn

Ruby: # 无泛型
来源：http://wv.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fi.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://bh.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://et.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://ay.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lc.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ol.wgjwhj.cn

Java: // 无解构
来源：http://mb.newstarts.cn

Go:   // 无解构
来源：http://xz.hahajie.cn

Ruby: a, b = pair
来源：http://cr.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://sx.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ws.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yk.newstarts.cn

PHP:  // 无重载
来源：http://bl.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yr.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://jz.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hb.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://cn.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://sf.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rz.yuexingan06.cn

================================================================================
来源：http://fn.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://id.shtwfgs.cn

================================================================================
来源：http://qd.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://fb.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://op.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xj.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wa.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://on.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lc.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://qm.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://ru.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ge.9csxet.cn

[D02] 追加元素到末尾
来源：http://al.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://er.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xe.haigaiapp.cn

JS:   arr.push(4);
来源：http://ni.521024.cn

TS:   arr.push(4);
来源：http://fs.nicolike.cn

Java: list.add(4);
来源：http://oy.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://ci.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://ah.huixiangedu.cn

C#:   list.Add(4);
来源：http://of.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://sg.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://rk.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lt.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yd.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://mp.wgjwhj.cn

Java: list.add(0, 0);
来源：http://im.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pw.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cl.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://rz.hnjuh.cn

[D04] 删除元素
来源：http://tf.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://np.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://en.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hb.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://bi.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rl.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ue.gzmigu.cn


<!-- 参考信息 -->