代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://qu.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://le.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://qq.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://ij.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fk.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://as.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://bw.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://sm.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://ah.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://td.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://ek.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://wg.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://kb.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ki.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ud.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://pt.chemitech.net.cn

[B09] break 与 continue
来源：http://st.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ic.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lx.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ny.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ew.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://on.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hg.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ej.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kq.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://kt.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gl.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ld.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jo.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oq.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zt.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bi.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ug.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ka.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://uf.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://xk.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://if.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cs.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jy.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mi.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tx.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://eg.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ma.yuexingan06.cn

[B12] 跳出多层循环
来源：http://yd.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fa.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vi.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://st.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ff.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qq.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sa.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pk.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ip.9csxet.cn

[B13] 判断是否为数字
来源：http://bh.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://ry.huanxung.cn

PHP:  is_numeric($x)
来源：http://sm.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nt.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://te.gzmigu.cn

Java: x instanceof Number
来源：http://ud.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ga.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://in.nicolike.cn

C#:   x is int or double or decimal
来源：http://hx.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://lb.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xs.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pn.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://cb.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://gk.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hk.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cn.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://au.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ci.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://lc.colortex.cn

Py:   a and b or not c
来源：http://vx.hahajie.cn

PHP:  $a && $b || !$c
来源：http://da.colortex.cn

JS:   a && b || !c
来源：http://hu.lnxyls.cn

TS:   a && b || !c
来源：http://iw.shxzskj.cn

Java: a && b || !c
来源：http://ai.shxzukj.cn

Go:   a && b || !c
来源：http://yr.newstarts.cn

Ruby: a && b || !c
来源：http://fj.chemitech.net.cn

C#:   a && b || !c
来源：http://nm.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://om.9csxet.cn

Py:   if not data: return
来源：http://uz.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://dy.nszjky.cn

JS:   if (!data) return;
来源：http://dn.shtwfgs.cn

TS:   if (!data) return;
来源：http://qu.gzmigu.cn

Java: if (data == null) return;
来源：http://xr.colortex.cn

Go:   if data == nil { return }
来源：http://vv.szxytkj.cn

Ruby: return if data.nil?
来源：http://yj.nszjky.cn

C#:   if (data == null) return;
来源：http://kk.wgjwhj.cn

================================================================================
来源：http://yl.jctech888.com.cn

C. 函数与作用域
来源：http://fi.colortex.cn

================================================================================
来源：http://kq.huanxung.cn

[C01] 定义函数
来源：http://sd.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://pz.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ou.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://el.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zk.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ml.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://im.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://th.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ax.bjjhwx.cn

[C02] 默认参数
来源：http://bz.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://oo.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kn.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://cd.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dp.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://re.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ub.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://to.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://id.chemitech.net.cn

[C03] 可变参数
来源：http://ky.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://pf.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://en.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kd.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jr.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wq.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vg.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zt.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yt.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://dy.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://is.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pu.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ia.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fz.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://uu.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://tl.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://xf.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://vr.chemitech.net.cn

[C05] 返回多个值
来源：http://bb.yuexingan06.cn

Py:   return a, b
来源：http://nt.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://jt.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tc.huixinmuqiang.cn

TS:   return { a, b };
来源：http://kh.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cz.gzmigu.cn

Go:   return a, b
来源：http://cv.bjjhwx.cn

Ruby: return a, b
来源：http://cn.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://df.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://ed.newstarts.cn

Py:   square = lambda x: x * x
来源：http://yo.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://av.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://pj.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://xc.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wj.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pn.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://fm.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ka.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://qa.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sj.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hl.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yp.hnjuh.cn

TS:   arr.map(String)
来源：http://fi.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wm.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sc.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://dr.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ke.bookmarksfly.cn

[C08] 闭包
来源：http://oo.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rt.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://do.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bb.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ue.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ed.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yv.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bn.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lt.chemitech.net.cn

[C09] 递归
来源：http://ju.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bp.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ze.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nq.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ig.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nm.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rt.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yj.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mn.asd995.cn

[C10] 变量作用域
来源：http://et.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xg.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ve.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fo.gzmigu.cn

TS:   同 JS
来源：http://bo.newstarts.cn

Java: 方法内为块级作用域
来源：http://mm.szsharing.cn

Go:   花括号块级作用域
来源：http://uj.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hk.shtwfgs.cn

C#:   块级作用域
来源：http://eb.nszjky.cn

[C11] 模块导入与导出
来源：http://cl.9csxet.cn

Py:   from module import func
来源：http://lu.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ni.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zw.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ov.huixinmuqiang.cn

Java: import java.util.List;
来源：http://uj.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sg.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ba.jctech888.com.cn

C#:   using System.Text;
来源：http://az.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://ze.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://cv.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://ze.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://cc.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://ei.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mv.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ep.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://xw.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sj.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://cn.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yb.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ee.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ql.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gz.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jj.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://pz.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dr.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fj.gzmigu.cn

[C14] 泛型函数
来源：http://al.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ux.gzmigu.cn

PHP:  // 无泛型
来源：http://km.hnjuh.cn

JS:   // 无泛型
来源：http://ep.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://na.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ca.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tw.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://xg.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pw.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://ih.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tw.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://nm.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xq.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ra.9csxet.cn

Java: // 无解构
来源：http://fd.panjiajie.cn

Go:   // 无解构
来源：http://ve.haigaiapp.cn

Ruby: a, b = pair
来源：http://ek.9csxet.cn

C#:   var (a, b) = pair;
来源：http://ng.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://ed.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mw.lnxyls.cn

PHP:  // 无重载
来源：http://ud.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xz.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ft.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://if.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://rr.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://in.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wx.lnxyls.cn

================================================================================
来源：http://nl.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://tn.gzmigu.cn

================================================================================
来源：http://fz.szsharing.cn

[D01] 创建数组 / 列表
来源：http://oe.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xd.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tm.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://po.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xs.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gt.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://py.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://fe.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zi.9csxet.cn

[D02] 追加元素到末尾
来源：http://hm.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yq.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vx.shxzskj.cn

JS:   arr.push(4);
来源：http://tv.nszjky.cn

TS:   arr.push(4);
来源：http://wr.jctech888.com.cn

Java: list.add(4);
来源：http://oi.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://hl.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://tp.szsharing.cn

C#:   list.Add(4);
来源：http://bb.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://lv.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://jt.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dt.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mx.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://qe.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://vy.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vz.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ya.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://ro.huixiangedu.cn

[D04] 删除元素
来源：http://ss.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://td.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jx.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pa.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://vu.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eh.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pz.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vg.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rj.hahajie.cn

[D05] 访问与修改元素
来源：http://jl.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sy.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://in.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ba.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://dy.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://wq.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://cu.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cv.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cg.hahajie.cn

[D06] 数组长度
来源：http://sb.hnjuh.cn

Py:   len(arr)
来源：http://rv.9csxet.cn

PHP:  count($arr);
来源：http://fd.muxihuayi.cn

JS:   arr.length
来源：http://bq.chemitech.net.cn

TS:   arr.length
来源：http://yp.colortex.cn

Java: list.size();
来源：http://gq.shxzskj.cn

Go:   len(arr)
来源：http://jc.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://ju.9csxet.cn

C#:   list.Count;
来源：http://qb.huanxung.cn

[D07] 切片 / 取子数组
来源：http://gc.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://la.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qc.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://fm.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://sz.9csxet.cn

Java: list.subList(1, 4);
来源：http://wv.newstarts.cn

Go:   arr[1:4]
来源：http://gn.huanxung.cn

Ruby: arr[1, 3]
来源：http://gb.haigaiapp.cn


<!-- 参考信息 -->