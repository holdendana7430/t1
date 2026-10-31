代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aw.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qt.huixiangedu.cn

[B07] while 循环
来源：http://vj.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://qf.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cj.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://gu.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://ig.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://ye.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hj.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://hk.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://mm.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://bo.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://mq.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kh.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://po.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://dz.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://az.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dy.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vq.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://rp.szsharing.cn

[B09] break 与 continue
来源：http://uw.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ki.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rv.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vw.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dg.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ei.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oh.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nk.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cr.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ab.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dd.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ar.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xx.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ir.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rq.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://br.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uu.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cs.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://wr.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://bq.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://yw.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cb.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yq.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rm.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ps.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://aq.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ug.shxzukj.cn

[B12] 跳出多层循环
来源：http://cy.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dl.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sf.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zk.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ec.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://be.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ho.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tl.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://js.panjiajie.cn

[B13] 判断是否为数字
来源：http://oz.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://py.shxzskj.cn

PHP:  is_numeric($x)
来源：http://ie.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ww.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cv.chemitech.net.cn

Java: x instanceof Number
来源：http://zt.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mw.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://hl.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://an.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://ql.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ke.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ck.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://mr.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://mm.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dp.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ka.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jn.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jy.nicolike.cn

[B15] 布尔运算与取反
来源：http://jh.nszjky.cn

Py:   a and b or not c
来源：http://ju.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://ji.shxzukj.cn

JS:   a && b || !c
来源：http://ft.huanxung.cn

TS:   a && b || !c
来源：http://oi.nicolike.cn

Java: a && b || !c
来源：http://cz.jianghongdianzi.cn

Go:   a && b || !c
来源：http://dk.hnjuh.cn

Ruby: a && b || !c
来源：http://wd.colortex.cn

C#:   a && b || !c
来源：http://pn.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lm.colortex.cn

Py:   if not data: return
来源：http://vf.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://rn.yuexingan06.cn

JS:   if (!data) return;
来源：http://rz.muxihuayi.cn

TS:   if (!data) return;
来源：http://sl.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://iu.bjjhwx.cn

Go:   if data == nil { return }
来源：http://gq.szsharing.cn

Ruby: return if data.nil?
来源：http://qq.nszjky.cn

C#:   if (data == null) return;
来源：http://yl.szsharing.cn

================================================================================
来源：http://ej.huixiangedu.cn

C. 函数与作用域
来源：http://ad.hnjuh.cn

================================================================================
来源：http://lg.shtwfgs.cn

[C01] 定义函数
来源：http://tl.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://xo.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wm.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://tr.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iz.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xs.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qk.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://og.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vk.bookmarksfly.cn

[C02] 默认参数
来源：http://xd.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://dc.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ls.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://dh.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dp.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xx.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wc.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://ih.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://ak.muxihuayi.cn

[C03] 可变参数
来源：http://hy.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://ln.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xd.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cj.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vh.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wj.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yu.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wt.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nw.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://kn.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zk.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xe.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://by.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iv.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ta.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://hx.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://sp.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://im.szxytkj.cn

[C05] 返回多个值
来源：http://om.shxzskj.cn

Py:   return a, b
来源：http://en.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://tt.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dn.huixiangedu.cn

TS:   return { a, b };
来源：http://ua.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://za.asd995.cn

Go:   return a, b
来源：http://wd.muxihuayi.cn

Ruby: return a, b
来源：http://ml.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://rc.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://ot.nicolike.cn

Py:   square = lambda x: x * x
来源：http://oj.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qf.hahajie.cn

JS:   const square = x => x * x;
来源：http://ri.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://sl.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fc.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rp.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://ok.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bo.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://tw.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bt.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ja.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://it.bookmarksfly.cn

TS:   arr.map(String)
来源：http://vo.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oy.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wl.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://fi.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xg.shxzskj.cn

[C08] 闭包
来源：http://tp.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yb.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zv.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sr.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mh.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ld.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mm.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sl.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xn.chemitech.net.cn

[C09] 递归
来源：http://bs.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tf.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vl.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jg.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nh.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fe.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ia.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dx.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bp.hahajie.cn

[C10] 变量作用域
来源：http://km.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jn.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bq.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fu.colortex.cn

TS:   同 JS
来源：http://ot.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://ev.chemitech.net.cn

Go:   花括号块级作用域
来源：http://td.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vb.9csxet.cn

C#:   块级作用域
来源：http://aq.huixiangedu.cn

[C11] 模块导入与导出
来源：http://gh.huixinmuqiang.cn

Py:   from module import func
来源：http://fx.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kn.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gm.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ny.hahajie.cn

Java: import java.util.List;
来源：http://kq.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hm.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://in.wgjwhj.cn

C#:   using System.Text;
来源：http://le.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://fq.colortex.cn

Py:   (lambda: print("run"))()
来源：http://mi.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://vm.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://ux.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://ma.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yr.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://nb.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://ak.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xu.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://qg.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fi.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ga.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xu.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gp.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rd.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://ph.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xk.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ie.gzmigu.cn

[C14] 泛型函数
来源：http://gd.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qv.chemitech.net.cn

PHP:  // 无泛型
来源：http://sn.muxihuayi.cn

JS:   // 无泛型
来源：http://go.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ca.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uq.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ez.jctech888.com.cn

Ruby: # 无泛型
来源：http://xk.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sx.nszjky.cn

[C15] 解构 / 展开参数
来源：http://hd.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lp.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://me.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ty.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ze.bjjhwx.cn

Java: // 无解构
来源：http://im.muxihuayi.cn

Go:   // 无解构
来源：http://jd.nicolike.cn

Ruby: a, b = pair
来源：http://xf.szsharing.cn

C#:   var (a, b) = pair;
来源：http://lz.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://jf.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rt.haigaiapp.cn

PHP:  // 无重载
来源：http://hc.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kq.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://jo.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://if.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ot.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://vn.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vb.panjiajie.cn

================================================================================
来源：http://tj.colortex.cn

D. 数组 / 列表 / 集合
来源：http://za.huixinmuqiang.cn

================================================================================
来源：http://hc.nszjky.cn

[D01] 创建数组 / 列表
来源：http://co.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vr.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ts.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fe.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jj.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jv.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://tm.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://xu.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fy.colortex.cn

[D02] 追加元素到末尾
来源：http://cx.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uk.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xt.haigaiapp.cn

JS:   arr.push(4);
来源：http://bm.yuexingan06.cn

TS:   arr.push(4);
来源：http://xa.jctech888.com.cn

Java: list.add(4);
来源：http://qh.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://ub.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://am.colortex.cn

C#:   list.Add(4);
来源：http://zh.colortex.cn

[D03] 在指定位置插入元素
来源：http://hp.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://dw.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hf.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zc.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://hg.shxzskj.cn

Java: list.add(0, 0);
来源：http://wu.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ns.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wa.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://nv.shxzskj.cn

[D04] 删除元素
来源：http://nh.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://od.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://km.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cw.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://yw.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ru.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://px.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yn.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://th.chemitech.net.cn

[D05] 访问与修改元素
来源：http://ls.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rp.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iv.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uv.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://xp.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://wj.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://wv.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sc.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mv.szxytkj.cn

[D06] 数组长度
来源：http://ho.yuexingan06.cn

Py:   len(arr)
来源：http://yh.gzmigu.cn

PHP:  count($arr);
来源：http://di.huixinmuqiang.cn

JS:   arr.length
来源：http://pw.jianghongdianzi.cn

TS:   arr.length
来源：http://og.huixiangedu.cn

Java: list.size();
来源：http://gx.9csxet.cn

Go:   len(arr)
来源：http://qo.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://lb.asd995.cn

C#:   list.Count;
来源：http://vh.9csxet.cn

[D07] 切片 / 取子数组
来源：http://od.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kn.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://og.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://he.szsharing.cn


<!-- 参考信息 -->