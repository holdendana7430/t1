代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://te.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fu.shtwfgs.cn

[B07] while 循环
来源：http://ty.newstarts.cn

Py:   while i < 10: i += 1
来源：http://hv.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zf.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://rq.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://nr.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://rg.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sd.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://df.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://bj.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://iv.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://fp.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rh.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://me.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://tv.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://yd.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zr.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vw.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://fy.9csxet.cn

[B09] break 与 continue
来源：http://jf.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bz.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://do.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yw.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wt.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kw.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lq.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fa.asd995.cn

[B10] 遍历同时拿索引
来源：http://ks.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://td.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pu.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tp.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cd.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rn.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kq.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ni.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ye.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://bs.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://rh.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://fv.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nf.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pv.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ki.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ix.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://bo.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zh.bjjhwx.cn

[B12] 跳出多层循环
来源：http://mu.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gu.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lw.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qq.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bi.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://db.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vu.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uw.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nk.haigaiapp.cn

[B13] 判断是否为数字
来源：http://zc.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://jv.gzmigu.cn

PHP:  is_numeric($x)
来源：http://jz.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oo.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xs.jctech888.com.cn

Java: x instanceof Number
来源：http://ac.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lx.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://hv.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://kk.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://zu.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kd.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rl.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://le.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://qh.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yt.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qz.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pd.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zd.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://yp.szsharing.cn

Py:   a and b or not c
来源：http://hm.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://oh.yuexingan06.cn

JS:   a && b || !c
来源：http://hx.newstarts.cn

TS:   a && b || !c
来源：http://nr.gzmigu.cn

Java: a && b || !c
来源：http://wi.9csxet.cn

Go:   a && b || !c
来源：http://pu.haigaiapp.cn

Ruby: a && b || !c
来源：http://sd.hnjuh.cn

C#:   a && b || !c
来源：http://po.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mj.shxzukj.cn

Py:   if not data: return
来源：http://zr.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://uo.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://oq.newstarts.cn

TS:   if (!data) return;
来源：http://ns.huixiangedu.cn

Java: if (data == null) return;
来源：http://ye.wgjwhj.cn

Go:   if data == nil { return }
来源：http://cy.shxzukj.cn

Ruby: return if data.nil?
来源：http://ty.chemitech.net.cn

C#:   if (data == null) return;
来源：http://ij.bookmarksfly.cn

================================================================================
来源：http://zq.newstarts.cn

C. 函数与作用域
来源：http://dw.shtwfgs.cn

================================================================================
来源：http://rt.shxzskj.cn

[C01] 定义函数
来源：http://vx.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://pz.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ub.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://jp.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ut.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gv.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ov.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://nk.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://on.nicolike.cn

[C02] 默认参数
来源：http://mt.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://sf.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ev.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://ne.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tk.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sf.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ye.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://uq.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://vo.huixinmuqiang.cn

[C03] 可变参数
来源：http://oo.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://yy.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pg.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://no.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://id.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rf.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cd.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://co.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fo.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://pk.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gu.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qr.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dm.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qb.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://qn.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://iv.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://zb.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://xg.shtwfgs.cn

[C05] 返回多个值
来源：http://uz.jianghongdianzi.cn

Py:   return a, b
来源：http://il.nszjky.cn

PHP:  return [$a, $b];
来源：http://dx.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ch.panjiajie.cn

TS:   return { a, b };
来源：http://re.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fw.yuntaijiaju.cn

Go:   return a, b
来源：http://gk.asd995.cn

Ruby: return a, b
来源：http://bq.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://tk.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://ih.nszjky.cn

Py:   square = lambda x: x * x
来源：http://gr.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vs.nicolike.cn

JS:   const square = x => x * x;
来源：http://si.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://yp.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iy.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oi.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://ff.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rh.hahajie.cn

[C07] 把函数作为参数传入
来源：http://lw.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sm.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xw.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lx.bjjhwx.cn

TS:   arr.map(String)
来源：http://an.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hq.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sm.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://ea.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kn.yuexingan06.cn

[C08] 闭包
来源：http://jy.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://em.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vj.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xn.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tv.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bx.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://px.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jt.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ga.521024.cn

[C09] 递归
来源：http://df.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cj.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://is.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hv.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nf.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fo.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pl.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cl.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lq.panjiajie.cn

[C10] 变量作用域
来源：http://vn.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://to.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vq.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vv.haigaiapp.cn

TS:   同 JS
来源：http://yo.nszjky.cn

Java: 方法内为块级作用域
来源：http://ov.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://qx.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://en.lnxyls.cn

C#:   块级作用域
来源：http://oj.jctech888.com.cn

[C11] 模块导入与导出
来源：http://gq.wgjwhj.cn

Py:   from module import func
来源：http://ya.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://au.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rp.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kd.muxihuayi.cn

Java: import java.util.List;
来源：http://xg.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xf.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://nr.panjiajie.cn

C#:   using System.Text;
来源：http://rr.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://vj.colortex.cn

Py:   (lambda: print("run"))()
来源：http://tw.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://px.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://oj.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://wo.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qy.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://jd.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://kq.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cl.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://xs.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yn.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://th.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jd.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ze.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ae.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ma.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mx.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rs.newstarts.cn

[C14] 泛型函数
来源：http://wl.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://is.nszjky.cn

PHP:  // 无泛型
来源：http://zr.huanxung.cn

JS:   // 无泛型
来源：http://kq.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hg.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ml.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rq.huanxung.cn

Ruby: # 无泛型
来源：http://jn.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pc.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://yl.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tm.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://cu.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ph.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eq.haigaiapp.cn

Java: // 无解构
来源：http://gk.521024.cn

Go:   // 无解构
来源：http://si.yuexingan06.cn

Ruby: a, b = pair
来源：http://ar.newstarts.cn

C#:   var (a, b) = pair;
来源：http://ap.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://el.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oy.hahajie.cn

PHP:  // 无重载
来源：http://bm.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://je.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://hz.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://py.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://er.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://pm.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wc.nicolike.cn

================================================================================
来源：http://jd.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://bw.bookmarksfly.cn

================================================================================
来源：http://bd.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://wd.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xs.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fm.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ab.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mv.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://je.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://cm.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://wg.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ul.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://gg.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vv.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mi.szsharing.cn

JS:   arr.push(4);
来源：http://ax.521024.cn

TS:   arr.push(4);
来源：http://dd.huixinmuqiang.cn

Java: list.add(4);
来源：http://np.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://is.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://zk.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://nk.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://ao.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://ai.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ek.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ox.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://dg.yuexingan06.cn

Java: list.add(0, 0);
来源：http://ul.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rj.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ja.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://uz.huanxung.cn

[D04] 删除元素
来源：http://th.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wc.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zq.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wk.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://hd.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ne.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nk.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uy.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gc.9csxet.cn

[D05] 访问与修改元素
来源：http://ae.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bm.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ur.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nw.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://km.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://lm.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://px.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dp.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ki.huixiangedu.cn

[D06] 数组长度
来源：http://hp.yuntaijiaju.cn

Py:   len(arr)
来源：http://im.jianghongdianzi.cn

PHP:  count($arr);
来源：http://tf.521024.cn

JS:   arr.length
来源：http://zk.9csxet.cn

TS:   arr.length
来源：http://qk.chemitech.net.cn

Java: list.size();
来源：http://ce.colortex.cn

Go:   len(arr)
来源：http://zj.colortex.cn

Ruby: arr.length; arr.size
来源：http://yk.asd995.cn

C#:   list.Count;
来源：http://jk.colortex.cn

[D07] 切片 / 取子数组
来源：http://pf.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://se.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gl.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://dg.nicolike.cn


<!-- 参考信息 -->