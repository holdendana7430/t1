代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://db.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://om.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yk.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bm.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qp.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wv.huixinmuqiang.cn

[B07] while 循环
来源：http://ak.colortex.cn

Py:   while i < 10: i += 1
来源：http://vs.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hl.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://gy.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ys.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://cm.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ov.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://qf.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://mu.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://io.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://he.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://su.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://kz.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://ho.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://yr.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fx.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jc.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://ri.shxzskj.cn

[B09] break 与 continue
来源：http://lc.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cy.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jy.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hn.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xh.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pk.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hm.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pl.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xv.huanxung.cn

[B10] 遍历同时拿索引
来源：http://hn.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rx.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bh.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://me.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dl.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://el.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sb.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cr.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hl.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://hb.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://xt.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://ds.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zs.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oa.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://az.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ip.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://gu.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mx.nicolike.cn

[B12] 跳出多层循环
来源：http://ve.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wa.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eo.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://er.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rt.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ny.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cu.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zb.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mp.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://gd.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://og.colortex.cn

PHP:  is_numeric($x)
来源：http://fr.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pf.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qo.asd995.cn

Java: x instanceof Number
来源：http://ne.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gb.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://xk.lnxyls.cn

C#:   x is int or double or decimal
来源：http://iu.hahajie.cn

[B14] 判断值是否在集合内
来源：http://gp.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://op.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zi.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ve.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://rs.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yy.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ei.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tr.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xs.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://jw.chemitech.net.cn

Py:   a and b or not c
来源：http://le.newstarts.cn

PHP:  $a && $b || !$c
来源：http://kt.haigaiapp.cn

JS:   a && b || !c
来源：http://ye.bookmarksfly.cn

TS:   a && b || !c
来源：http://yv.szsharing.cn

Java: a && b || !c
来源：http://rc.shtwfgs.cn

Go:   a && b || !c
来源：http://iq.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://nm.jianghongdianzi.cn

C#:   a && b || !c
来源：http://ck.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xv.huixinmuqiang.cn

Py:   if not data: return
来源：http://bu.asd995.cn

PHP:  if (!$data) { return; }
来源：http://ln.gzmigu.cn

JS:   if (!data) return;
来源：http://lw.asd995.cn

TS:   if (!data) return;
来源：http://px.9csxet.cn

Java: if (data == null) return;
来源：http://qt.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://qn.shxzskj.cn

Ruby: return if data.nil?
来源：http://yp.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://zj.chemitech.net.cn

================================================================================
来源：http://pp.huixinmuqiang.cn

C. 函数与作用域
来源：http://fv.jctech888.com.cn

================================================================================
来源：http://ol.hnjuh.cn

[C01] 定义函数
来源：http://rp.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://yn.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rm.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://cp.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://or.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ck.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://br.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://vo.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uy.jctech888.com.cn

[C02] 默认参数
来源：http://is.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://pe.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ak.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://qt.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ba.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ev.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pw.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://dj.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://km.szsharing.cn

[C03] 可变参数
来源：http://kp.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://kb.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://df.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kn.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cv.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wx.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kz.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xv.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vi.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://ob.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rw.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ha.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dd.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yl.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://mw.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://zy.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://sk.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://sf.asd995.cn

[C05] 返回多个值
来源：http://bx.lnxyls.cn

Py:   return a, b
来源：http://qp.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://we.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jo.9csxet.cn

TS:   return { a, b };
来源：http://gw.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://af.bjjhwx.cn

Go:   return a, b
来源：http://lo.panjiajie.cn

Ruby: return a, b
来源：http://ve.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://rg.colortex.cn

[C06] 匿名函数 / lambda
来源：http://ry.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://qy.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ex.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://nl.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://nt.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://df.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rj.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://uu.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mh.hahajie.cn

[C07] 把函数作为参数传入
来源：http://kz.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fe.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bf.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mm.haigaiapp.cn

TS:   arr.map(String)
来源：http://fm.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ln.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fs.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://pj.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cj.bjjhwx.cn

[C08] 闭包
来源：http://qo.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jw.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ar.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ch.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mt.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sg.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pp.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hf.nicolike.cn

[C09] 递归
来源：http://mb.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ma.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hl.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ul.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kk.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sm.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nu.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lz.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hd.shxzskj.cn

[C10] 变量作用域
来源：http://rr.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aj.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ii.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ax.shxzukj.cn

TS:   同 JS
来源：http://kd.hnjuh.cn

Java: 方法内为块级作用域
来源：http://yx.haigaiapp.cn

Go:   花括号块级作用域
来源：http://gf.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rw.wgjwhj.cn

C#:   块级作用域
来源：http://vz.newstarts.cn

[C11] 模块导入与导出
来源：http://kf.gzmigu.cn

Py:   from module import func
来源：http://we.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bg.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://po.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cq.nszjky.cn

Java: import java.util.List;
来源：http://sf.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qz.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://jd.bookmarksfly.cn

C#:   using System.Text;
来源：http://iu.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://fe.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://cg.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://yo.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://gr.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://ww.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ns.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://px.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://ya.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qf.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://bq.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fu.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oh.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://co.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qp.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ce.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://ub.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lb.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zn.huixinmuqiang.cn

[C14] 泛型函数
来源：http://qo.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ck.shxzukj.cn

PHP:  // 无泛型
来源：http://nq.chemitech.net.cn

JS:   // 无泛型
来源：http://gb.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ak.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ra.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wn.yuexingan06.cn

Ruby: # 无泛型
来源：http://no.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ht.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://vi.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mf.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://gr.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zq.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xw.nicolike.cn

Java: // 无解构
来源：http://mn.nicolike.cn

Go:   // 无解构
来源：http://tv.chemitech.net.cn

Ruby: a, b = pair
来源：http://ay.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://vg.newstarts.cn

[C16] 函数 / 方法重载
来源：http://wt.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pl.jctech888.com.cn

PHP:  // 无重载
来源：http://kf.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sb.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://gn.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ww.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://pr.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://jn.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ni.szsharing.cn

================================================================================
来源：http://qx.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://ho.shxzskj.cn

================================================================================
来源：http://uy.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://je.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fj.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hk.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bq.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ey.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://un.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://cw.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://kz.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gg.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://gg.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eg.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fp.huixiangedu.cn

JS:   arr.push(4);
来源：http://fj.hahajie.cn

TS:   arr.push(4);
来源：http://ao.huixinmuqiang.cn

Java: list.add(4);
来源：http://gd.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://qu.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://oh.gzmigu.cn

C#:   list.Add(4);
来源：http://md.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://cl.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://sm.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hf.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tv.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://vb.jctech888.com.cn

Java: list.add(0, 0);
来源：http://jx.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fv.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bf.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://xd.hahajie.cn

[D04] 删除元素
来源：http://lz.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tv.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wa.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ef.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://ra.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fh.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://su.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nr.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pr.newstarts.cn

[D05] 访问与修改元素
来源：http://xi.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yv.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sq.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ie.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://vg.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://ln.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://gs.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bd.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ta.haigaiapp.cn

[D06] 数组长度
来源：http://zp.nszjky.cn

Py:   len(arr)
来源：http://nc.newstarts.cn

PHP:  count($arr);
来源：http://xk.521024.cn

JS:   arr.length
来源：http://mo.szxytkj.cn

TS:   arr.length
来源：http://hs.huixiangedu.cn

Java: list.size();
来源：http://yb.nszjky.cn

Go:   len(arr)
来源：http://vg.521024.cn

Ruby: arr.length; arr.size
来源：http://bb.asd995.cn

C#:   list.Count;
来源：http://qd.jctech888.com.cn


<!-- 参考信息 -->