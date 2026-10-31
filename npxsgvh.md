代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://wm.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ir.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://fq.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://ni.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://zm.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yx.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dq.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://ls.hnjuh.cn

[B09] break 与 continue
来源：http://sg.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xa.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ds.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nu.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vp.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lc.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wp.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xy.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mt.nicolike.cn

[B10] 遍历同时拿索引
来源：http://gi.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ch.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ga.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vp.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://au.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sk.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nw.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ap.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mw.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://xx.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://bj.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://uh.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://io.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yv.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ya.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iu.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://dt.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rz.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://tt.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uq.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kl.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tx.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tk.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kp.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sg.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mw.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lj.shtwfgs.cn

[B13] 判断是否为数字
来源：http://qe.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ig.nszjky.cn

PHP:  is_numeric($x)
来源：http://az.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cm.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hc.asd995.cn

Java: x instanceof Number
来源：http://tq.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://su.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://uz.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://wl.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://ev.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lw.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xq.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://ge.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://ug.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cf.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ns.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://da.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ee.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://wx.521024.cn

Py:   a and b or not c
来源：http://vh.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://wg.panjiajie.cn

JS:   a && b || !c
来源：http://ng.huixiangedu.cn

TS:   a && b || !c
来源：http://mi.9csxet.cn

Java: a && b || !c
来源：http://ib.huixiangedu.cn

Go:   a && b || !c
来源：http://me.huanxung.cn

Ruby: a && b || !c
来源：http://mn.panjiajie.cn

C#:   a && b || !c
来源：http://da.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uy.asd995.cn

Py:   if not data: return
来源：http://sp.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://av.shtwfgs.cn

JS:   if (!data) return;
来源：http://we.newstarts.cn

TS:   if (!data) return;
来源：http://cx.lnxyls.cn

Java: if (data == null) return;
来源：http://cv.chemitech.net.cn

Go:   if data == nil { return }
来源：http://de.huixiangedu.cn

Ruby: return if data.nil?
来源：http://ow.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://he.huixiangedu.cn

================================================================================
来源：http://xl.szsharing.cn

C. 函数与作用域
来源：http://sq.jianghongdianzi.cn

================================================================================
来源：http://ce.wgjwhj.cn

[C01] 定义函数
来源：http://lu.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://tc.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wl.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://kw.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hj.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sc.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kj.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://nm.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ld.nicolike.cn

[C02] 默认参数
来源：http://gd.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://yq.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dz.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://qj.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bk.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ys.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fx.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://kr.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://jh.asd995.cn

[C03] 可变参数
来源：http://sa.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://nd.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iq.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cv.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dg.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dm.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yz.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ex.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fs.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ls.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dj.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vx.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fs.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iu.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://cv.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ro.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://tb.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://ve.szsharing.cn

[C05] 返回多个值
来源：http://yj.huixiangedu.cn

Py:   return a, b
来源：http://tc.colortex.cn

PHP:  return [$a, $b];
来源：http://cr.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jj.huixiangedu.cn

TS:   return { a, b };
来源：http://hi.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wo.yuntaijiaju.cn

Go:   return a, b
来源：http://kz.colortex.cn

Ruby: return a, b
来源：http://pm.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://sz.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://en.9csxet.cn

Py:   square = lambda x: x * x
来源：http://xs.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wa.newstarts.cn

JS:   const square = x => x * x;
来源：http://hg.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://wn.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dg.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hw.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://nr.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ai.asd995.cn

[C07] 把函数作为参数传入
来源：http://fi.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vr.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xs.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://np.wgjwhj.cn

TS:   arr.map(String)
来源：http://py.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hq.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hx.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://zk.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://le.jctech888.com.cn

[C08] 闭包
来源：http://ib.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xh.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://az.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wk.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qq.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tl.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kd.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pi.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ji.nicolike.cn

[C09] 递归
来源：http://ih.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wb.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://by.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ew.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tm.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vc.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yv.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ra.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wl.lnxyls.cn

[C10] 变量作用域
来源：http://de.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jq.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qb.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://po.nszjky.cn

TS:   同 JS
来源：http://nr.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://tx.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://ld.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ay.yuexingan06.cn

C#:   块级作用域
来源：http://gb.bjjhwx.cn

[C11] 模块导入与导出
来源：http://lt.nszjky.cn

Py:   from module import func
来源：http://ea.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lc.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tv.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tl.yuexingan06.cn

Java: import java.util.List;
来源：http://ui.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ib.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://vs.bookmarksfly.cn

C#:   using System.Text;
来源：http://sl.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://cu.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://ox.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://or.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://sw.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://uz.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://om.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://rr.521024.cn

Ruby: -> { puts "run" }.call
来源：http://lf.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uz.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://dc.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hy.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gw.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bx.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pv.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tp.521024.cn

Go:   func add(a, b int) int
来源：http://ab.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vu.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bf.shtwfgs.cn

[C14] 泛型函数
来源：http://hi.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lw.521024.cn

PHP:  // 无泛型
来源：http://pv.gzmigu.cn

JS:   // 无泛型
来源：http://vh.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lp.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vi.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://to.newstarts.cn

Ruby: # 无泛型
来源：http://ns.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vg.colortex.cn

[C15] 解构 / 展开参数
来源：http://bd.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ik.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://gg.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ue.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rp.bjjhwx.cn

Java: // 无解构
来源：http://rm.asd995.cn

Go:   // 无解构
来源：http://uh.colortex.cn

Ruby: a, b = pair
来源：http://ke.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://ug.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://yw.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ck.szsharing.cn

PHP:  // 无重载
来源：http://pl.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ad.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://da.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uu.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://hw.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://yn.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yk.szxytkj.cn

================================================================================
来源：http://bq.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://tr.hahajie.cn

================================================================================
来源：http://op.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://wr.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dl.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fz.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kb.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uz.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ib.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://gp.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://ws.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jj.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://qg.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://og.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ao.haigaiapp.cn

JS:   arr.push(4);
来源：http://wr.nicolike.cn

TS:   arr.push(4);
来源：http://am.muxihuayi.cn

Java: list.add(4);
来源：http://lm.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://ou.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://cw.nszjky.cn

C#:   list.Add(4);
来源：http://ue.hahajie.cn

[D03] 在指定位置插入元素
来源：http://cm.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://ql.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xp.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ae.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://jx.panjiajie.cn

Java: list.add(0, 0);
来源：http://by.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pg.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ah.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://nr.shtwfgs.cn

[D04] 删除元素
来源：http://qa.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vp.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://us.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gy.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://an.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lr.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xk.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xz.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://io.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://ql.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ub.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ur.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iw.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://db.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://sy.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://et.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lp.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yi.bookmarksfly.cn

[D06] 数组长度
来源：http://nj.hnjuh.cn

Py:   len(arr)
来源：http://rf.yuexingan06.cn

PHP:  count($arr);
来源：http://yg.shxzskj.cn

JS:   arr.length
来源：http://kh.yuntaijiaju.cn

TS:   arr.length
来源：http://tx.colortex.cn

Java: list.size();
来源：http://ln.yuexingan06.cn

Go:   len(arr)
来源：http://jd.nszjky.cn

Ruby: arr.length; arr.size
来源：http://si.yuexingan06.cn

C#:   list.Count;
来源：http://jv.newstarts.cn

[D07] 切片 / 取子数组
来源：http://uj.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sk.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ne.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://ik.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://ig.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://hk.szxytkj.cn

Go:   arr[1:4]
来源：http://ss.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://eb.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://gy.colortex.cn

[D08] 合并两个数组
来源：http://pl.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://kp.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://at.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jh.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://ad.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ut.szxytkj.cn

Go:   append(a, b...)
来源：http://ei.jianghongdianzi.cn


<!-- 参考信息 -->