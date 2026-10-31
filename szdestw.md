代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cq.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iu.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://df.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ey.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hs.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aw.lnxyls.cn

[B07] while 循环
来源：http://th.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://rg.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ak.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://mq.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://kw.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://fi.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tg.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://dw.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://xk.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://mh.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ih.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jv.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://qd.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://bw.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://pg.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cp.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hd.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://ji.gzmigu.cn

[B09] break 与 continue
来源：http://ba.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zi.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gc.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oc.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mq.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zo.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ck.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vq.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xl.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://hc.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nk.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ih.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hw.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qn.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://en.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wd.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dv.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fd.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://zy.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://yi.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://cl.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eb.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://av.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fs.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vz.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://wa.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iu.shtwfgs.cn

[B12] 跳出多层循环
来源：http://el.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uq.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zc.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nc.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jn.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ln.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zx.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uo.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xn.nicolike.cn

[B13] 判断是否为数字
来源：http://uj.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://ic.newstarts.cn

PHP:  is_numeric($x)
来源：http://to.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uk.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aq.shtwfgs.cn

Java: x instanceof Number
来源：http://rg.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ji.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://lz.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://ge.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://su.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zg.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kv.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://ns.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ci.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wg.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gd.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uq.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nn.gzmigu.cn

[B15] 布尔运算与取反
来源：http://vx.asd995.cn

Py:   a and b or not c
来源：http://qs.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://ij.chemitech.net.cn

JS:   a && b || !c
来源：http://jx.yuexingan06.cn

TS:   a && b || !c
来源：http://ev.wgjwhj.cn

Java: a && b || !c
来源：http://gf.huixinmuqiang.cn

Go:   a && b || !c
来源：http://kg.shtwfgs.cn

Ruby: a && b || !c
来源：http://qt.shtwfgs.cn

C#:   a && b || !c
来源：http://wu.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jf.yuntaijiaju.cn

Py:   if not data: return
来源：http://fa.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://zh.bookmarksfly.cn

JS:   if (!data) return;
来源：http://sg.colortex.cn

TS:   if (!data) return;
来源：http://vb.asd995.cn

Java: if (data == null) return;
来源：http://tr.haigaiapp.cn

Go:   if data == nil { return }
来源：http://su.huixiangedu.cn

Ruby: return if data.nil?
来源：http://ub.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://yh.wgjwhj.cn

================================================================================
来源：http://wy.bookmarksfly.cn

C. 函数与作用域
来源：http://oq.haigaiapp.cn

================================================================================
来源：http://we.panjiajie.cn

[C01] 定义函数
来源：http://cz.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://ex.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vg.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://nc.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ph.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xs.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vp.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://hk.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ty.shxzskj.cn

[C02] 默认参数
来源：http://ob.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://zc.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pt.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://pc.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yx.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://he.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ph.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://od.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://aw.nicolike.cn

[C03] 可变参数
来源：http://lk.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://ni.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gc.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ne.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bv.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dd.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ad.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jx.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://di.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://rw.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://on.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zk.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vx.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mm.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://tb.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://cb.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://ok.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://fh.nicolike.cn

[C05] 返回多个值
来源：http://xz.szxytkj.cn

Py:   return a, b
来源：http://cn.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://pb.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wg.wgjwhj.cn

TS:   return { a, b };
来源：http://hq.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dp.bjjhwx.cn

Go:   return a, b
来源：http://vo.szsharing.cn

Ruby: return a, b
来源：http://wp.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ft.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://dc.asd995.cn

Py:   square = lambda x: x * x
来源：http://bq.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yp.huanxung.cn

JS:   const square = x => x * x;
来源：http://gc.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://cf.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sh.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uu.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://qt.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vu.nicolike.cn

[C07] 把函数作为参数传入
来源：http://ua.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ej.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fp.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kc.newstarts.cn

TS:   arr.map(String)
来源：http://kc.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ye.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wk.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://zg.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fk.bookmarksfly.cn

[C08] 闭包
来源：http://fn.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bb.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lh.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fc.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zn.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ak.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zj.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cj.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://db.haigaiapp.cn

[C09] 递归
来源：http://hn.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kb.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fj.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vx.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pz.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tp.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rc.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://of.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sc.wgjwhj.cn

[C10] 变量作用域
来源：http://wy.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://do.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tl.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ok.521024.cn

TS:   同 JS
来源：http://ny.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://cg.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://wk.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://do.szsharing.cn

C#:   块级作用域
来源：http://ct.521024.cn

[C11] 模块导入与导出
来源：http://yz.nicolike.cn

Py:   from module import func
来源：http://mn.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yc.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yq.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ja.yuntaijiaju.cn

Java: import java.util.List;
来源：http://dx.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ab.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://qa.bookmarksfly.cn

C#:   using System.Text;
来源：http://sn.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://xk.colortex.cn

Py:   (lambda: print("run"))()
来源：http://eg.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://gk.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://gl.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://uw.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://el.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://xw.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://rq.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zy.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://fr.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ra.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ri.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pj.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xt.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tv.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://bh.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sp.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://de.lnxyls.cn

[C14] 泛型函数
来源：http://bh.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hc.bookmarksfly.cn

PHP:  // 无泛型
来源：http://eb.muxihuayi.cn

JS:   // 无泛型
来源：http://nf.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bx.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ry.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zh.wgjwhj.cn

Ruby: # 无泛型
来源：http://gp.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aq.nicolike.cn

[C15] 解构 / 展开参数
来源：http://rl.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fw.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://lb.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pa.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yw.wgjwhj.cn

Java: // 无解构
来源：http://nq.haigaiapp.cn

Go:   // 无解构
来源：http://qb.bjjhwx.cn

Ruby: a, b = pair
来源：http://ub.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://fn.huanxung.cn

[C16] 函数 / 方法重载
来源：http://ok.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pt.gzmigu.cn

PHP:  // 无重载
来源：http://kl.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ye.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://ri.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://us.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://qp.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://wo.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ov.jctech888.com.cn

================================================================================
来源：http://az.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://qx.shxzskj.cn

================================================================================
来源：http://jj.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://wu.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bx.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rv.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://md.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ez.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pv.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://ew.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://ck.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pk.colortex.cn

[D02] 追加元素到末尾
来源：http://mp.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cw.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dh.521024.cn

JS:   arr.push(4);
来源：http://ra.haigaiapp.cn

TS:   arr.push(4);
来源：http://ox.wgjwhj.cn

Java: list.add(4);
来源：http://nj.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://cm.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://vg.lnxyls.cn

C#:   list.Add(4);
来源：http://md.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://wx.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://lk.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cs.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fj.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://gv.shxzukj.cn

Java: list.add(0, 0);
来源：http://gg.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fo.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ei.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://kr.newstarts.cn

[D04] 删除元素
来源：http://bt.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cb.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ib.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fh.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://fz.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ts.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uy.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yh.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fm.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://gm.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xj.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fn.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yw.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://lj.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://lf.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://hp.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://js.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mw.jctech888.com.cn

[D06] 数组长度
来源：http://yo.lnxyls.cn

Py:   len(arr)
来源：http://ho.jianghongdianzi.cn

PHP:  count($arr);
来源：http://gr.haigaiapp.cn

JS:   arr.length
来源：http://xk.asd995.cn

TS:   arr.length
来源：http://vi.colortex.cn

Java: list.size();
来源：http://ri.shxzukj.cn

Go:   len(arr)
来源：http://rc.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://rf.bookmarksfly.cn

C#:   list.Count;
来源：http://xw.shxzskj.cn


<!-- 参考信息 -->