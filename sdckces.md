代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zn.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qy.shxzukj.cn

[B07] while 循环
来源：http://ry.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://bz.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lk.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://sa.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://vf.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://ij.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://je.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://hz.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://nl.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://ib.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://zs.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cp.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://ee.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://cv.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://zj.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mn.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rc.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://na.szxytkj.cn

[B09] break 与 continue
来源：http://uw.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jb.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hg.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ff.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://as.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gu.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ep.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qv.newstarts.cn

[B10] 遍历同时拿索引
来源：http://ip.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vj.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sz.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tw.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fq.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tc.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cx.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vl.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bk.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://no.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://ep.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://ni.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qy.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vc.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ta.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fw.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://et.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zh.chemitech.net.cn

[B12] 跳出多层循环
来源：http://jz.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zk.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://de.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ow.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rc.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pk.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vh.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qf.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yq.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://kd.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://px.newstarts.cn

PHP:  is_numeric($x)
来源：http://nu.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oc.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gk.bookmarksfly.cn

Java: x instanceof Number
来源：http://mw.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oh.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://hy.shxzukj.cn

C#:   x is int or double or decimal
来源：http://qh.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://oz.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qz.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kx.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ae.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://nd.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vl.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yi.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ub.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rl.panjiajie.cn

[B15] 布尔运算与取反
来源：http://ay.muxihuayi.cn

Py:   a and b or not c
来源：http://fb.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://ho.shxzukj.cn

JS:   a && b || !c
来源：http://da.9csxet.cn

TS:   a && b || !c
来源：http://sa.bookmarksfly.cn

Java: a && b || !c
来源：http://wo.chemitech.net.cn

Go:   a && b || !c
来源：http://zf.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://nn.szsharing.cn

C#:   a && b || !c
来源：http://uy.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ou.huixiangedu.cn

Py:   if not data: return
来源：http://yi.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://hu.panjiajie.cn

JS:   if (!data) return;
来源：http://oe.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://fc.newstarts.cn

Java: if (data == null) return;
来源：http://in.szsharing.cn

Go:   if data == nil { return }
来源：http://uq.szxytkj.cn

Ruby: return if data.nil?
来源：http://xq.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://sz.lnxyls.cn

================================================================================
来源：http://sf.huixiangedu.cn

C. 函数与作用域
来源：http://vj.haigaiapp.cn

================================================================================
来源：http://jk.521024.cn

[C01] 定义函数
来源：http://sw.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://pi.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ec.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://jb.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hh.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bi.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sr.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://og.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rr.yuexingan06.cn

[C02] 默认参数
来源：http://ga.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://lw.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wq.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://uc.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qz.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cq.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iq.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://bs.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://vd.521024.cn

[C03] 可变参数
来源：http://lu.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://oo.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yf.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ds.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iu.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://di.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bk.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://df.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qm.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://pn.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lt.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qk.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xz.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yw.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://lk.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://hq.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://lf.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://za.bookmarksfly.cn

[C05] 返回多个值
来源：http://og.huixinmuqiang.cn

Py:   return a, b
来源：http://lz.panjiajie.cn

PHP:  return [$a, $b];
来源：http://ch.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vt.huixinmuqiang.cn

TS:   return { a, b };
来源：http://yn.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lj.bookmarksfly.cn

Go:   return a, b
来源：http://ap.nicolike.cn

Ruby: return a, b
来源：http://xp.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://cw.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://je.521024.cn

Py:   square = lambda x: x * x
来源：http://ny.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vy.panjiajie.cn

JS:   const square = x => x * x;
来源：http://qe.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://px.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xl.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fg.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://xd.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wh.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://yh.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ws.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wq.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://br.hnjuh.cn

TS:   arr.map(String)
来源：http://yg.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fs.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uv.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://jc.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ie.hahajie.cn

[C08] 闭包
来源：http://nz.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vs.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gf.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cb.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eh.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ft.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zn.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ry.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ws.bookmarksfly.cn

[C09] 递归
来源：http://pr.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dt.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qu.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wy.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://io.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://um.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ca.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://og.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ba.asd995.cn

[C10] 变量作用域
来源：http://yd.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dl.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ot.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rs.huixiangedu.cn

TS:   同 JS
来源：http://np.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://uj.yuexingan06.cn

Go:   花括号块级作用域
来源：http://pl.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qr.szsharing.cn

C#:   块级作用域
来源：http://jw.newstarts.cn

[C11] 模块导入与导出
来源：http://za.521024.cn

Py:   from module import func
来源：http://pc.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tm.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wr.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iz.muxihuayi.cn

Java: import java.util.List;
来源：http://be.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ya.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://gc.huixinmuqiang.cn

C#:   using System.Text;
来源：http://jg.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://dd.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://cb.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://wp.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://hy.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://vf.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ji.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://tf.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://cr.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mm.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://yi.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bp.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://go.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eg.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oa.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yp.nicolike.cn

Go:   func add(a, b int) int
来源：http://qa.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tm.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dc.lnxyls.cn

[C14] 泛型函数
来源：http://qh.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gc.nszjky.cn

PHP:  // 无泛型
来源：http://ku.nicolike.cn

JS:   // 无泛型
来源：http://xc.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://du.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ri.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xn.shxzskj.cn

Ruby: # 无泛型
来源：http://cq.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yv.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://oq.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kb.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://qv.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lv.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://up.newstarts.cn

Java: // 无解构
来源：http://yn.hnjuh.cn

Go:   // 无解构
来源：http://wg.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://gv.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://uc.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://jf.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lg.asd995.cn

PHP:  // 无重载
来源：http://wb.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wx.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://kq.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ns.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://vr.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://qv.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qb.yuntaijiaju.cn

================================================================================
来源：http://yj.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://dr.gzmigu.cn

================================================================================
来源：http://ry.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://ph.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ie.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eq.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yb.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://es.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uc.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://tp.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://wa.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cw.newstarts.cn

[D02] 追加元素到末尾
来源：http://yb.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ot.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ba.lnxyls.cn

JS:   arr.push(4);
来源：http://rb.panjiajie.cn

TS:   arr.push(4);
来源：http://nb.wgjwhj.cn

Java: list.add(4);
来源：http://zp.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://tx.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://kg.huanxung.cn

C#:   list.Add(4);
来源：http://rj.nszjky.cn

[D03] 在指定位置插入元素
来源：http://zj.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://tz.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lw.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vj.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://wg.shxzskj.cn

Java: list.add(0, 0);
来源：http://cj.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ag.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yo.521024.cn

C#:   list.Insert(0, 0);
来源：http://mi.hahajie.cn

[D04] 删除元素
来源：http://fc.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cp.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yx.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ng.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://qz.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vt.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bp.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ea.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://em.521024.cn

[D05] 访问与修改元素
来源：http://qn.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sx.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qi.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://en.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://uo.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://uj.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://qt.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ta.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wm.huanxung.cn

[D06] 数组长度
来源：http://mn.bjjhwx.cn

Py:   len(arr)
来源：http://de.yuntaijiaju.cn

PHP:  count($arr);
来源：http://er.hahajie.cn

JS:   arr.length
来源：http://dz.huanxung.cn

TS:   arr.length
来源：http://cq.gzmigu.cn

Java: list.size();
来源：http://ke.muxihuayi.cn

Go:   len(arr)
来源：http://bq.9csxet.cn

Ruby: arr.length; arr.size
来源：http://ug.yuntaijiaju.cn

C#:   list.Count;
来源：http://bu.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://au.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jg.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yg.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://wg.yuexingan06.cn


<!-- 参考信息 -->