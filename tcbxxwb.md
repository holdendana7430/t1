代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://bg.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://it.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://mr.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://lg.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kk.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://my.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://yf.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://hb.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://kz.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jm.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://hz.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://hz.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://jh.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nz.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rg.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://oo.jianghongdianzi.cn

[B09] break 与 continue
来源：http://pg.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yn.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ke.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ef.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hd.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tx.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xf.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://px.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pm.521024.cn

[B10] 遍历同时拿索引
来源：http://xs.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xa.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bp.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pa.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jp.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zg.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bs.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xr.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fk.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://bo.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://io.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://xj.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mu.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qx.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vt.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gq.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://nv.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ns.lnxyls.cn

[B12] 跳出多层循环
来源：http://dg.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hf.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pm.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lr.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ps.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kj.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cv.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://na.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jd.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://kz.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://ye.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://zv.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ub.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kb.nszjky.cn

Java: x instanceof Number
来源：http://ls.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rz.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://cm.asd995.cn

C#:   x is int or double or decimal
来源：http://vr.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://ss.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vi.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://is.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ny.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://wq.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eo.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bt.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://td.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ny.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://vs.gzmigu.cn

Py:   a and b or not c
来源：http://hr.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://ri.huixinmuqiang.cn

JS:   a && b || !c
来源：http://tk.hahajie.cn

TS:   a && b || !c
来源：http://mv.yuntaijiaju.cn

Java: a && b || !c
来源：http://jo.chemitech.net.cn

Go:   a && b || !c
来源：http://bf.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://tk.9csxet.cn

C#:   a && b || !c
来源：http://id.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vn.shtwfgs.cn

Py:   if not data: return
来源：http://qm.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://ph.shxzskj.cn

JS:   if (!data) return;
来源：http://ko.panjiajie.cn

TS:   if (!data) return;
来源：http://ri.jctech888.com.cn

Java: if (data == null) return;
来源：http://nr.bjjhwx.cn

Go:   if data == nil { return }
来源：http://tc.yuexingan06.cn

Ruby: return if data.nil?
来源：http://wx.lnxyls.cn

C#:   if (data == null) return;
来源：http://ha.jctech888.com.cn

================================================================================
来源：http://mu.haigaiapp.cn

C. 函数与作用域
来源：http://nm.asd995.cn

================================================================================
来源：http://fi.panjiajie.cn

[C01] 定义函数
来源：http://gv.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://ix.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bg.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ib.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nl.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ws.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ay.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://xk.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ob.huixinmuqiang.cn

[C02] 默认参数
来源：http://kj.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://kl.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mt.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://fp.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://or.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qx.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dr.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://ef.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://dl.colortex.cn

[C03] 可变参数
来源：http://xl.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://gj.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yw.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nq.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bd.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wz.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fe.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ea.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ps.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://qx.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rh.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ij.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xr.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hc.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://kn.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://nd.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://tx.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://tv.lnxyls.cn

[C05] 返回多个值
来源：http://kw.hahajie.cn

Py:   return a, b
来源：http://yo.asd995.cn

PHP:  return [$a, $b];
来源：http://ai.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wp.hnjuh.cn

TS:   return { a, b };
来源：http://yg.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iz.colortex.cn

Go:   return a, b
来源：http://io.haigaiapp.cn

Ruby: return a, b
来源：http://lx.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://tu.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://xe.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://tc.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uy.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://iq.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://nr.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rd.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gt.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://cw.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cy.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://ow.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hc.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bt.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yb.szsharing.cn

TS:   arr.map(String)
来源：http://bk.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ty.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://sd.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://es.bookmarksfly.cn

[C08] 闭包
来源：http://vw.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://je.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wy.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vs.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://om.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cw.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cn.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aq.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xm.huixinmuqiang.cn

[C09] 递归
来源：http://tq.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qe.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gv.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ow.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gj.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mv.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dg.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uh.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://we.panjiajie.cn

[C10] 变量作用域
来源：http://yk.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uo.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yr.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aj.bookmarksfly.cn

TS:   同 JS
来源：http://ue.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://kg.lnxyls.cn

Go:   花括号块级作用域
来源：http://ot.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dg.haigaiapp.cn

C#:   块级作用域
来源：http://wn.chemitech.net.cn

[C11] 模块导入与导出
来源：http://qa.hnjuh.cn

Py:   from module import func
来源：http://tf.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bi.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qa.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://re.yuntaijiaju.cn

Java: import java.util.List;
来源：http://vn.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iw.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://it.bookmarksfly.cn

C#:   using System.Text;
来源：http://oq.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://ow.521024.cn

Py:   (lambda: print("run"))()
来源：http://io.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://ej.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://ck.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://cz.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://by.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://dh.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://ao.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gu.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://qc.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zy.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ze.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hl.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ce.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ka.szsharing.cn

Go:   func add(a, b int) int
来源：http://re.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://av.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wt.yuexingan06.cn

[C14] 泛型函数
来源：http://tz.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wd.nicolike.cn

PHP:  // 无泛型
来源：http://bt.yuexingan06.cn

JS:   // 无泛型
来源：http://zl.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ty.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gs.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jo.bjjhwx.cn

Ruby: # 无泛型
来源：http://zp.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ba.nszjky.cn

[C15] 解构 / 展开参数
来源：http://gm.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zm.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://rx.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pr.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dc.yuntaijiaju.cn

Java: // 无解构
来源：http://sk.shtwfgs.cn

Go:   // 无解构
来源：http://am.szxytkj.cn

Ruby: a, b = pair
来源：http://yf.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://hx.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://jm.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://so.gzmigu.cn

PHP:  // 无重载
来源：http://jb.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hd.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://zx.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nm.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://sd.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://li.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ju.asd995.cn

================================================================================
来源：http://ui.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://va.bjjhwx.cn

================================================================================
来源：http://xm.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://qz.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hj.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wu.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cp.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wt.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xa.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://em.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://ez.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://di.shxzukj.cn

[D02] 追加元素到末尾
来源：http://di.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://do.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gw.szxytkj.cn

JS:   arr.push(4);
来源：http://eo.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://ry.yuntaijiaju.cn

Java: list.add(4);
来源：http://ta.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://in.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://en.chemitech.net.cn

C#:   list.Add(4);
来源：http://mm.9csxet.cn

[D03] 在指定位置插入元素
来源：http://jm.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://kf.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vb.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kj.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://om.lnxyls.cn

Java: list.add(0, 0);
来源：http://lf.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iz.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eo.asd995.cn

C#:   list.Insert(0, 0);
来源：http://ou.hahajie.cn

[D04] 删除元素
来源：http://tb.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wd.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://to.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ro.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://pi.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://el.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ih.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ux.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wh.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://oq.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ip.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fl.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yx.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://eq.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://yz.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://tv.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ca.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hd.bjjhwx.cn

[D06] 数组长度
来源：http://fn.nszjky.cn

Py:   len(arr)
来源：http://qc.shxzskj.cn

PHP:  count($arr);
来源：http://og.nicolike.cn

JS:   arr.length
来源：http://as.shxzukj.cn

TS:   arr.length
来源：http://yj.gzmigu.cn

Java: list.size();
来源：http://no.bookmarksfly.cn

Go:   len(arr)
来源：http://tu.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://if.jianghongdianzi.cn

C#:   list.Count;
来源：http://eu.colortex.cn

[D07] 切片 / 取子数组
来源：http://ac.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ro.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rz.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://hs.colortex.cn

TS:   arr.slice(1, 4);
来源：http://lk.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://gr.szsharing.cn

Go:   arr[1:4]
来源：http://nj.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://ue.asd995.cn


<!-- 参考信息 -->