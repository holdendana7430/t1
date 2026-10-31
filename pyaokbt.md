代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xe.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://wr.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eg.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hk.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ua.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fi.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xo.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pu.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nr.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lk.huanxung.cn

[B07] while 循环
来源：http://uj.colortex.cn

Py:   while i < 10: i += 1
来源：http://nz.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ik.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://wy.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://jm.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://cd.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hx.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://nz.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://wz.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ok.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://bz.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uz.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://pf.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://sx.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://ow.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wh.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ow.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://km.asd995.cn

[B09] break 与 continue
来源：http://hn.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qb.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eu.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xg.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ev.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://po.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ae.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kp.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ma.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://lu.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mu.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eu.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tm.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ln.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lf.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sc.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ba.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ru.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://oy.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://ir.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://uv.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cd.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zo.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hx.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rj.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://wk.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ek.huanxung.cn

[B12] 跳出多层循环
来源：http://tv.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fz.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ww.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://na.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mq.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ra.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vp.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ty.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zo.9csxet.cn

[B13] 判断是否为数字
来源：http://cw.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://kt.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://tr.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sb.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ez.chemitech.net.cn

Java: x instanceof Number
来源：http://wv.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ay.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://dp.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://hz.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://xz.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yw.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://je.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://gq.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://aq.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xb.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jk.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cy.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jl.shxzskj.cn

[B15] 布尔运算与取反
来源：http://au.hnjuh.cn

Py:   a and b or not c
来源：http://qk.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://wi.shxzukj.cn

JS:   a && b || !c
来源：http://al.jctech888.com.cn

TS:   a && b || !c
来源：http://fo.shxzukj.cn

Java: a && b || !c
来源：http://qn.shxzukj.cn

Go:   a && b || !c
来源：http://ie.bookmarksfly.cn

Ruby: a && b || !c
来源：http://tf.nicolike.cn

C#:   a && b || !c
来源：http://hp.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zu.shxzukj.cn

Py:   if not data: return
来源：http://ib.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://ym.gzmigu.cn

JS:   if (!data) return;
来源：http://ie.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://pj.yuexingan06.cn

Java: if (data == null) return;
来源：http://uu.panjiajie.cn

Go:   if data == nil { return }
来源：http://nl.asd995.cn

Ruby: return if data.nil?
来源：http://km.shxzskj.cn

C#:   if (data == null) return;
来源：http://ff.shxzukj.cn

================================================================================
来源：http://go.shxzskj.cn

C. 函数与作用域
来源：http://bc.muxihuayi.cn

================================================================================
来源：http://lc.huanxung.cn

[C01] 定义函数
来源：http://hs.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://yz.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vp.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://ku.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ur.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ws.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dc.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://ae.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rs.wgjwhj.cn

[C02] 默认参数
来源：http://jn.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://se.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qg.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://nb.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mm.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hu.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ob.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://ke.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://yg.huixinmuqiang.cn

[C03] 可变参数
来源：http://wt.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://sn.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yn.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ke.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ic.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qi.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://py.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://do.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kf.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://ij.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oy.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vf.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ov.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wq.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://ix.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://vq.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://pa.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://ix.shtwfgs.cn

[C05] 返回多个值
来源：http://dp.huanxung.cn

Py:   return a, b
来源：http://yr.huanxung.cn

PHP:  return [$a, $b];
来源：http://et.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hn.newstarts.cn

TS:   return { a, b };
来源：http://jr.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ry.asd995.cn

Go:   return a, b
来源：http://tg.jianghongdianzi.cn

Ruby: return a, b
来源：http://sm.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://cp.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://dd.colortex.cn

Py:   square = lambda x: x * x
来源：http://na.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lj.colortex.cn

JS:   const square = x => x * x;
来源：http://kr.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://bn.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dw.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bk.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://im.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pc.9csxet.cn

[C07] 把函数作为参数传入
来源：http://yn.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sk.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uy.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qo.9csxet.cn

TS:   arr.map(String)
来源：http://yv.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gq.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ep.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://jm.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ib.asd995.cn

[C08] 闭包
来源：http://ch.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rm.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yb.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tj.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qu.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yy.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ph.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cj.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kz.muxihuayi.cn

[C09] 递归
来源：http://xt.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wh.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pd.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://if.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gq.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dp.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eb.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zy.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ew.huixinmuqiang.cn

[C10] 变量作用域
来源：http://ab.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ct.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://an.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rd.szxytkj.cn

TS:   同 JS
来源：http://po.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://jk.lnxyls.cn

Go:   花括号块级作用域
来源：http://ld.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ra.bookmarksfly.cn

C#:   块级作用域
来源：http://of.jctech888.com.cn

[C11] 模块导入与导出
来源：http://eo.newstarts.cn

Py:   from module import func
来源：http://ys.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://os.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mi.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lw.shxzukj.cn

Java: import java.util.List;
来源：http://eq.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kf.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://vq.hahajie.cn

C#:   using System.Text;
来源：http://ba.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://ds.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://dk.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://oq.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://hz.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://hp.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nz.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://zh.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://ss.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mp.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://rh.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ep.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cl.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ur.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oh.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vq.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://dh.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uf.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jd.huixiangedu.cn

[C14] 泛型函数
来源：http://ob.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ab.newstarts.cn

PHP:  // 无泛型
来源：http://dc.haigaiapp.cn

JS:   // 无泛型
来源：http://gb.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://az.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zx.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zh.bookmarksfly.cn

Ruby: # 无泛型
来源：http://jb.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rb.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://de.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sr.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://sf.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bc.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ao.shxzskj.cn

Java: // 无解构
来源：http://ax.521024.cn

Go:   // 无解构
来源：http://qa.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://sy.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://dg.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://xv.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fa.9csxet.cn

PHP:  // 无重载
来源：http://bd.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://us.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://oy.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yu.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://zr.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://eo.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lq.gzmigu.cn

================================================================================
来源：http://ad.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://vo.colortex.cn

================================================================================
来源：http://xm.colortex.cn

[D01] 创建数组 / 列表
来源：http://hv.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mv.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bj.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xx.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lu.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oe.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://fx.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://ce.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hf.shxzskj.cn

[D02] 追加元素到末尾
来源：http://qi.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rr.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mz.shxzukj.cn

JS:   arr.push(4);
来源：http://zl.521024.cn

TS:   arr.push(4);
来源：http://mw.asd995.cn

Java: list.add(4);
来源：http://dm.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://os.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://we.bookmarksfly.cn

C#:   list.Add(4);
来源：http://tp.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ot.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://ef.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ye.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ey.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://cg.huixiangedu.cn

Java: list.add(0, 0);
来源：http://bp.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jc.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gz.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://ym.bjjhwx.cn

[D04] 删除元素
来源：http://cj.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ry.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tq.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ig.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://fh.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ic.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ky.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rm.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ot.chemitech.net.cn

[D05] 访问与修改元素
来源：http://ui.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ei.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qx.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vm.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://vt.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://cp.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://pn.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://in.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ah.gzmigu.cn

[D06] 数组长度
来源：http://jq.lnxyls.cn

Py:   len(arr)
来源：http://na.gzmigu.cn

PHP:  count($arr);
来源：http://fp.newstarts.cn

JS:   arr.length
来源：http://hy.shxzskj.cn

TS:   arr.length
来源：http://ef.gzmigu.cn


<!-- 参考信息 -->