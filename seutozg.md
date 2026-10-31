代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ne.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sp.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bw.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ce.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vu.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ns.shxzskj.cn

[B07] while 循环
来源：http://dd.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://gn.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hq.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://hr.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://sq.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://zu.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zw.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://gl.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://lc.asd995.cn

[B08] do-while（至少执行一次）
来源：http://gt.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://mu.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ur.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://wz.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://sp.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://tm.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qs.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oz.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://bx.lnxyls.cn

[B09] break 与 continue
来源：http://vu.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ij.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bc.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nw.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ha.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xu.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kl.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dd.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.9csxet.cn

[B10] 遍历同时拿索引
来源：http://kg.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vs.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ts.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sy.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gm.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mc.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wr.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kz.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wz.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://zq.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://yb.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://wx.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hw.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ep.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sm.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fg.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://eg.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gp.muxihuayi.cn

[B12] 跳出多层循环
来源：http://xf.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tz.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mq.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://am.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nr.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bm.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://we.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lr.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://is.521024.cn

[B13] 判断是否为数字
来源：http://ux.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://wk.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://kz.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ns.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bd.gzmigu.cn

Java: x instanceof Number
来源：http://cn.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://am.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://hv.521024.cn

C#:   x is int or double or decimal
来源：http://zm.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://ul.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dj.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://el.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://kr.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://rt.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xc.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kk.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jh.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iv.newstarts.cn

[B15] 布尔运算与取反
来源：http://qy.lnxyls.cn

Py:   a and b or not c
来源：http://vm.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://vi.yuexingan06.cn

JS:   a && b || !c
来源：http://fv.asd995.cn

TS:   a && b || !c
来源：http://wh.bookmarksfly.cn

Java: a && b || !c
来源：http://fg.huixiangedu.cn

Go:   a && b || !c
来源：http://rq.nszjky.cn

Ruby: a && b || !c
来源：http://zo.hnjuh.cn

C#:   a && b || !c
来源：http://cv.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pt.bookmarksfly.cn

Py:   if not data: return
来源：http://nw.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://jv.szsharing.cn

JS:   if (!data) return;
来源：http://ke.shxzukj.cn

TS:   if (!data) return;
来源：http://uw.9csxet.cn

Java: if (data == null) return;
来源：http://ln.haigaiapp.cn

Go:   if data == nil { return }
来源：http://xc.shxzskj.cn

Ruby: return if data.nil?
来源：http://ze.huixiangedu.cn

C#:   if (data == null) return;
来源：http://rk.shxzukj.cn

================================================================================
来源：http://ed.gzmigu.cn

C. 函数与作用域
来源：http://zw.bjjhwx.cn

================================================================================
来源：http://of.bjjhwx.cn

[C01] 定义函数
来源：http://bx.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ic.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ci.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://ty.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oi.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gy.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://es.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://qh.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bo.hahajie.cn

[C02] 默认参数
来源：http://yx.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://yk.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://im.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://sn.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yu.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tn.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pn.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://fq.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://hb.jctech888.com.cn

[C03] 可变参数
来源：http://vr.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://cb.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gj.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vw.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kp.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sl.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://io.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kh.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ms.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://xt.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kd.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xg.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eu.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://in.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://kc.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://bj.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://qy.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://id.szxytkj.cn

[C05] 返回多个值
来源：http://zl.hnjuh.cn

Py:   return a, b
来源：http://ej.shxzskj.cn

PHP:  return [$a, $b];
来源：http://gn.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eb.bookmarksfly.cn

TS:   return { a, b };
来源：http://nq.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gx.nszjky.cn

Go:   return a, b
来源：http://wy.huanxung.cn

Ruby: return a, b
来源：http://lr.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://gv.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://re.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://pa.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kg.hnjuh.cn

JS:   const square = x => x * x;
来源：http://yh.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://fx.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cr.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lr.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://ua.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gu.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://gd.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ii.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lb.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wp.szsharing.cn

TS:   arr.map(String)
来源：http://ad.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ut.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sp.521024.cn

Ruby: arr.map(&:upcase)
来源：http://zw.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ff.521024.cn

[C08] 闭包
来源：http://rz.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sh.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mq.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://go.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xm.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zy.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nr.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oa.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ee.huixinmuqiang.cn

[C09] 递归
来源：http://tw.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ea.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://am.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fe.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jw.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kj.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ka.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qa.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jg.jianghongdianzi.cn

[C10] 变量作用域
来源：http://dn.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yw.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dw.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gg.shxzukj.cn

TS:   同 JS
来源：http://yh.nicolike.cn

Java: 方法内为块级作用域
来源：http://fk.szsharing.cn

Go:   花括号块级作用域
来源：http://je.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jt.huixiangedu.cn

C#:   块级作用域
来源：http://yd.newstarts.cn

[C11] 模块导入与导出
来源：http://cx.nicolike.cn

Py:   from module import func
来源：http://zk.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ff.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jc.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tu.colortex.cn

Java: import java.util.List;
来源：http://id.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jz.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://oe.gzmigu.cn

C#:   using System.Text;
来源：http://tg.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://pk.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://on.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://kf.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://xt.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://oc.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ii.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://oh.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://ou.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ia.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://ar.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dx.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dd.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://md.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cq.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ht.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://gv.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lk.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fz.shxzskj.cn

[C14] 泛型函数
来源：http://od.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rq.shxzskj.cn

PHP:  // 无泛型
来源：http://sy.hnjuh.cn

JS:   // 无泛型
来源：http://uh.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kb.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fs.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nw.lnxyls.cn

Ruby: # 无泛型
来源：http://qj.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oc.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://zy.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ai.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://oc.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oo.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wf.nszjky.cn

Java: // 无解构
来源：http://ps.gzmigu.cn

Go:   // 无解构
来源：http://sv.hnjuh.cn

Ruby: a, b = pair
来源：http://vf.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://ql.colortex.cn

[C16] 函数 / 方法重载
来源：http://wz.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cb.muxihuayi.cn

PHP:  // 无重载
来源：http://gt.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bf.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://mf.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ky.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://fj.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://dq.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ic.shxzukj.cn

================================================================================
来源：http://pu.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://oh.muxihuayi.cn

================================================================================
来源：http://we.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://il.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jh.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fk.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yi.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jl.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uh.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://zf.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://ox.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ku.9csxet.cn

[D02] 追加元素到末尾
来源：http://zh.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kp.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ba.521024.cn

JS:   arr.push(4);
来源：http://ag.muxihuayi.cn

TS:   arr.push(4);
来源：http://kc.asd995.cn

Java: list.add(4);
来源：http://ik.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://ow.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://eu.huanxung.cn

C#:   list.Add(4);
来源：http://dt.szsharing.cn

[D03] 在指定位置插入元素
来源：http://od.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://bg.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jp.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bx.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://mo.gzmigu.cn

Java: list.add(0, 0);
来源：http://wa.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ru.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fg.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://nj.muxihuayi.cn

[D04] 删除元素
来源：http://fw.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fv.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://me.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://al.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://ql.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kp.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://or.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nz.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://at.chemitech.net.cn

[D05] 访问与修改元素
来源：http://gc.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jk.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cn.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vp.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://rk.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://he.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ah.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bj.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bf.huixinmuqiang.cn

[D06] 数组长度
来源：http://ac.yuntaijiaju.cn

Py:   len(arr)
来源：http://li.hahajie.cn

PHP:  count($arr);
来源：http://dd.hnjuh.cn

JS:   arr.length
来源：http://uv.hnjuh.cn

TS:   arr.length
来源：http://cg.nszjky.cn

Java: list.size();
来源：http://wu.yuexingan06.cn

Go:   len(arr)
来源：http://jt.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://jk.yuntaijiaju.cn

C#:   list.Count;
来源：http://gp.521024.cn


<!-- 参考信息 -->