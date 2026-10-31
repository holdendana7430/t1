代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eh.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uc.nicolike.cn

[B07] while 循环
来源：http://nq.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://iy.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mx.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://ox.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://fb.asd995.cn

Java: while (i < 10) { i++; }
来源：http://js.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oi.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://mx.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://lw.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://do.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://yh.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zh.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://rd.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://gu.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://cd.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dc.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zf.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://ut.haigaiapp.cn

[B09] break 与 continue
来源：http://tw.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ve.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ve.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rj.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pg.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ru.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ip.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ks.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://jj.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://km.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bo.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vd.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sp.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vu.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qn.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nz.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://em.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://kn.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://ih.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://ir.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gw.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pf.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ln.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lr.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://sw.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ph.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://tr.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oz.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qp.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yx.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jr.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gc.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ag.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mv.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pm.bjjhwx.cn

[B13] 判断是否为数字
来源：http://nb.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://av.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://aq.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bq.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wy.colortex.cn

Java: x instanceof Number
来源：http://ee.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://id.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://hg.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://uu.nicolike.cn

[B14] 判断值是否在集合内
来源：http://wi.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xf.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ht.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://xo.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://fs.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kv.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pm.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xx.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ts.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://pd.panjiajie.cn

Py:   a and b or not c
来源：http://jt.szsharing.cn

PHP:  $a && $b || !$c
来源：http://ku.haigaiapp.cn

JS:   a && b || !c
来源：http://op.nicolike.cn

TS:   a && b || !c
来源：http://fs.nszjky.cn

Java: a && b || !c
来源：http://bl.colortex.cn

Go:   a && b || !c
来源：http://gb.muxihuayi.cn

Ruby: a && b || !c
来源：http://uk.yuntaijiaju.cn

C#:   a && b || !c
来源：http://lg.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ug.asd995.cn

Py:   if not data: return
来源：http://bh.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://dq.nicolike.cn

JS:   if (!data) return;
来源：http://wx.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://hn.hnjuh.cn

Java: if (data == null) return;
来源：http://to.haigaiapp.cn

Go:   if data == nil { return }
来源：http://yi.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://do.panjiajie.cn

C#:   if (data == null) return;
来源：http://ee.gzmigu.cn

================================================================================
来源：http://ks.jianghongdianzi.cn

C. 函数与作用域
来源：http://as.panjiajie.cn

================================================================================
来源：http://kq.521024.cn

[C01] 定义函数
来源：http://mo.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://ol.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rg.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://xk.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aa.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fp.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://em.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://vx.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ik.huanxung.cn

[C02] 默认参数
来源：http://bn.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://bk.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yq.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://ju.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yj.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jl.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ig.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://kt.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://io.huixiangedu.cn

[C03] 可变参数
来源：http://ua.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://ep.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vd.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://au.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vw.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eu.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nk.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://up.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zf.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://ib.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gn.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://go.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://il.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sq.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ey.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://lc.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://sm.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://iw.bookmarksfly.cn

[C05] 返回多个值
来源：http://ua.nszjky.cn

Py:   return a, b
来源：http://ig.shxzskj.cn

PHP:  return [$a, $b];
来源：http://us.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hh.szxytkj.cn

TS:   return { a, b };
来源：http://hq.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gu.szsharing.cn

Go:   return a, b
来源：http://uq.muxihuayi.cn

Ruby: return a, b
来源：http://mp.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://zy.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://tr.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://ku.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://el.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://ga.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://ch.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kk.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wy.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://uk.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mh.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://cz.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hr.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zc.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xm.bjjhwx.cn

TS:   arr.map(String)
来源：http://qt.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://we.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gm.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://kg.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tf.jianghongdianzi.cn

[C08] 闭包
来源：http://ha.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hl.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hu.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://if.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tb.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ok.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kc.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xm.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ex.shxzukj.cn

[C09] 递归
来源：http://dx.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bs.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uf.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lb.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sb.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tn.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hg.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eo.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rn.bjjhwx.cn

[C10] 变量作用域
来源：http://tt.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rb.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qc.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qg.shxzskj.cn

TS:   同 JS
来源：http://ir.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://lo.huanxung.cn

Go:   花括号块级作用域
来源：http://sp.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pp.haigaiapp.cn

C#:   块级作用域
来源：http://nf.szxytkj.cn

[C11] 模块导入与导出
来源：http://at.yuexingan06.cn

Py:   from module import func
来源：http://ux.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mo.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xu.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bg.newstarts.cn

Java: import java.util.List;
来源：http://eg.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ln.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://yx.bookmarksfly.cn

C#:   using System.Text;
来源：http://hq.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://mj.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://wl.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://bf.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://uu.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://lw.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bu.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://iy.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://mm.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qk.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://zk.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tv.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qq.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dw.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hv.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sc.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://nz.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oc.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gc.huanxung.cn

[C14] 泛型函数
来源：http://ie.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oi.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://rl.asd995.cn

JS:   // 无泛型
来源：http://uv.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qn.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rv.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ia.hnjuh.cn

Ruby: # 无泛型
来源：http://bz.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://su.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://lk.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qi.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://om.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zc.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aj.szxytkj.cn

Java: // 无解构
来源：http://hn.huixiangedu.cn

Go:   // 无解构
来源：http://gs.jctech888.com.cn

Ruby: a, b = pair
来源：http://zv.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://cd.9csxet.cn

[C16] 函数 / 方法重载
来源：http://gw.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qd.521024.cn

PHP:  // 无重载
来源：http://bq.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cm.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://eq.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yv.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://qc.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://mc.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aj.panjiajie.cn

================================================================================
来源：http://si.521024.cn

D. 数组 / 列表 / 集合
来源：http://rh.huixiangedu.cn

================================================================================
来源：http://hy.colortex.cn

[D01] 创建数组 / 列表
来源：http://nv.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mx.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dr.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ww.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yt.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://us.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://sy.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://yk.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pg.521024.cn

[D02] 追加元素到末尾
来源：http://ah.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ju.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pd.haigaiapp.cn

JS:   arr.push(4);
来源：http://yo.nszjky.cn

TS:   arr.push(4);
来源：http://bd.panjiajie.cn

Java: list.add(4);
来源：http://nm.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://fb.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://jt.nszjky.cn

C#:   list.Add(4);
来源：http://nc.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://wf.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://xh.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mo.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://re.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://dn.gzmigu.cn

Java: list.add(0, 0);
来源：http://ex.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://px.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ws.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://kn.shxzskj.cn

[D04] 删除元素
来源：http://yg.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nn.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://al.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sp.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://ap.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ax.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xg.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pe.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jg.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://hj.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rm.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rp.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ps.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://jf.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://uw.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://sc.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kr.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ui.shxzukj.cn

[D06] 数组长度
来源：http://pm.yuntaijiaju.cn

Py:   len(arr)
来源：http://en.jctech888.com.cn

PHP:  count($arr);
来源：http://im.szxytkj.cn

JS:   arr.length
来源：http://kz.yuexingan06.cn

TS:   arr.length
来源：http://mo.nicolike.cn

Java: list.size();
来源：http://zo.colortex.cn

Go:   len(arr)
来源：http://un.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://qz.asd995.cn

C#:   list.Count;
来源：http://ph.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://jv.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pl.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sr.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://zh.huanxung.cn


<!-- 参考信息 -->