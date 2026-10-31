代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fc.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ub.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://wd.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ti.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://pl.521024.cn

Py:   for item in arr: print(item)
来源：http://ep.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://st.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ib.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hq.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vs.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://an.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://gj.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oi.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://ui.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://km.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ru.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lk.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zt.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oq.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tg.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cb.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ty.asd995.cn

[B07] while 循环
来源：http://qw.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://wm.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eg.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://hj.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://qb.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://ga.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xq.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://de.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://xk.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://qj.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://pw.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rs.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://jb.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://hc.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://im.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hd.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pd.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://gv.jctech888.com.cn

[B09] break 与 continue
来源：http://lz.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gh.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zp.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oi.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cw.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dj.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fx.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gg.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wk.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://fw.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ot.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ab.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xq.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ns.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://do.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gp.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gt.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://em.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://qs.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://xk.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://fc.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ij.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iy.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xu.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pc.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://ra.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ky.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://ut.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kj.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://go.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hx.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bo.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fx.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wu.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ha.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ky.huixiangedu.cn

[B13] 判断是否为数字
来源：http://ee.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://qa.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://hz.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hy.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ha.newstarts.cn

Java: x instanceof Number
来源：http://xz.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wm.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://zw.9csxet.cn

C#:   x is int or double or decimal
来源：http://hq.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://xx.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rt.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jr.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://ay.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://uq.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rd.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://te.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fx.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sj.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://xe.haigaiapp.cn

Py:   a and b or not c
来源：http://gy.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://kd.yuexingan06.cn

JS:   a && b || !c
来源：http://nd.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ee.szsharing.cn

Java: a && b || !c
来源：http://gg.szxytkj.cn

Go:   a && b || !c
来源：http://mi.521024.cn

Ruby: a && b || !c
来源：http://ff.nszjky.cn

C#:   a && b || !c
来源：http://qi.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://od.521024.cn

Py:   if not data: return
来源：http://jl.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://vh.shxzukj.cn

JS:   if (!data) return;
来源：http://xy.shtwfgs.cn

TS:   if (!data) return;
来源：http://zs.szxytkj.cn

Java: if (data == null) return;
来源：http://fm.asd995.cn

Go:   if data == nil { return }
来源：http://bx.lnxyls.cn

Ruby: return if data.nil?
来源：http://il.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://hs.shtwfgs.cn

================================================================================
来源：http://bg.nszjky.cn

C. 函数与作用域
来源：http://st.wgjwhj.cn

================================================================================
来源：http://ra.asd995.cn

[C01] 定义函数
来源：http://yi.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://gp.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iv.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://uv.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mw.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ki.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hr.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://ss.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tr.yuexingan06.cn

[C02] 默认参数
来源：http://er.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://te.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://im.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://zb.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lc.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://br.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rh.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://hi.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://fv.shxzskj.cn

[C03] 可变参数
来源：http://cy.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://gh.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pt.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zm.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xg.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mc.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jy.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://je.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://np.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://sk.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ei.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nr.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ng.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://by.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://rq.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://hv.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://er.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://eu.muxihuayi.cn

[C05] 返回多个值
来源：http://pp.wgjwhj.cn

Py:   return a, b
来源：http://pg.asd995.cn

PHP:  return [$a, $b];
来源：http://mb.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fj.bjjhwx.cn

TS:   return { a, b };
来源：http://pk.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xn.shtwfgs.cn

Go:   return a, b
来源：http://bw.bookmarksfly.cn

Ruby: return a, b
来源：http://hk.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://tq.521024.cn

[C06] 匿名函数 / lambda
来源：http://ou.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://wc.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://op.newstarts.cn

JS:   const square = x => x * x;
来源：http://ld.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://rj.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hj.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kj.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://ri.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ay.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://gc.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cq.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nf.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yg.shxzukj.cn

TS:   arr.map(String)
来源：http://ka.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lx.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dt.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://us.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qk.jianghongdianzi.cn

[C08] 闭包
来源：http://kq.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gz.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dz.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://os.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bx.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rn.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gw.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gn.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lg.huixiangedu.cn

[C09] 递归
来源：http://ft.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gz.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ur.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xg.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uy.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mo.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fm.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ec.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yd.wgjwhj.cn

[C10] 变量作用域
来源：http://ll.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://il.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qs.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://km.szxytkj.cn

TS:   同 JS
来源：http://ln.asd995.cn

Java: 方法内为块级作用域
来源：http://ge.shtwfgs.cn

Go:   花括号块级作用域
来源：http://cl.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bh.jianghongdianzi.cn

C#:   块级作用域
来源：http://ih.huanxung.cn

[C11] 模块导入与导出
来源：http://vb.szxytkj.cn

Py:   from module import func
来源：http://ze.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sr.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rr.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fz.jianghongdianzi.cn

Java: import java.util.List;
来源：http://yv.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iu.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://gr.nszjky.cn

C#:   using System.Text;
来源：http://nj.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://ah.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://lf.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://kj.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ay.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://dr.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jp.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://wx.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ec.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sb.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://av.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ao.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gj.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qb.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zb.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://zi.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rw.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ii.huixiangedu.cn

[C14] 泛型函数
来源：http://my.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gk.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://co.jianghongdianzi.cn

JS:   // 无泛型
来源：http://rg.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://me.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tw.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hm.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://fb.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ff.nszjky.cn

[C15] 解构 / 展开参数
来源：http://yy.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ct.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://vn.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aw.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bn.colortex.cn

Java: // 无解构
来源：http://yf.hahajie.cn

Go:   // 无解构
来源：http://bn.shxzskj.cn

Ruby: a, b = pair
来源：http://hm.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://qf.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://kr.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kw.hnjuh.cn

PHP:  // 无重载
来源：http://ox.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tc.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://ad.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cq.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://dl.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://ao.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nb.szsharing.cn

================================================================================
来源：http://yd.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://po.huanxung.cn

================================================================================
来源：http://yn.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://aa.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://df.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aj.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gs.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xs.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nz.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://ty.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://um.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://td.9csxet.cn

[D02] 追加元素到末尾
来源：http://qs.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tz.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wp.asd995.cn

JS:   arr.push(4);
来源：http://ho.szxytkj.cn

TS:   arr.push(4);
来源：http://ke.yuexingan06.cn

Java: list.add(4);
来源：http://bk.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://cx.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://dn.hnjuh.cn

C#:   list.Add(4);
来源：http://uu.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://xd.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://vt.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ia.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pd.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://tp.asd995.cn

Java: list.add(0, 0);
来源：http://im.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nt.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jl.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://do.muxihuayi.cn

[D04] 删除元素
来源：http://aq.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vt.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ra.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ok.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://ug.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ha.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yu.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gf.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tt.newstarts.cn

[D05] 访问与修改元素
来源：http://wd.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://by.szsharing.cn


<!-- 参考信息 -->