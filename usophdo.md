代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cr.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://tj.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://mm.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://xf.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://su.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dx.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://vf.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://pb.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://xi.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ix.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jy.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://pf.szsharing.cn

[B09] break 与 continue
来源：http://uw.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xm.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bo.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rl.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lw.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zv.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ye.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nl.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ad.newstarts.cn

[B10] 遍历同时拿索引
来源：http://az.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gb.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hd.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qe.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oo.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dn.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bf.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qe.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oe.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://fh.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://zb.521024.cn

PHP:  range(0, 10, 2);
来源：http://hb.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fh.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ug.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://de.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sb.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://bn.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://al.shxzukj.cn

[B12] 跳出多层循环
来源：http://tz.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dj.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://re.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pc.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://us.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ep.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sz.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nx.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wk.chemitech.net.cn

[B13] 判断是否为数字
来源：http://wg.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://wn.gzmigu.cn

PHP:  is_numeric($x)
来源：http://bx.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oj.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xd.asd995.cn

Java: x instanceof Number
来源：http://lr.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uf.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://ht.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://ho.521024.cn

[B14] 判断值是否在集合内
来源：http://le.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yy.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zt.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://ni.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ab.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hr.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ml.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cq.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hl.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://ya.asd995.cn

Py:   a and b or not c
来源：http://ss.colortex.cn

PHP:  $a && $b || !$c
来源：http://zg.huanxung.cn

JS:   a && b || !c
来源：http://ws.521024.cn

TS:   a && b || !c
来源：http://xe.haigaiapp.cn

Java: a && b || !c
来源：http://se.gzmigu.cn

Go:   a && b || !c
来源：http://wz.shxzukj.cn

Ruby: a && b || !c
来源：http://gk.panjiajie.cn

C#:   a && b || !c
来源：http://lb.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zp.huixinmuqiang.cn

Py:   if not data: return
来源：http://uy.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://md.panjiajie.cn

JS:   if (!data) return;
来源：http://ts.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://po.muxihuayi.cn

Java: if (data == null) return;
来源：http://xu.nicolike.cn

Go:   if data == nil { return }
来源：http://ss.hahajie.cn

Ruby: return if data.nil?
来源：http://qd.bjjhwx.cn

C#:   if (data == null) return;
来源：http://hs.bookmarksfly.cn

================================================================================
来源：http://gy.huixiangedu.cn

C. 函数与作用域
来源：http://fg.bookmarksfly.cn

================================================================================
来源：http://we.asd995.cn

[C01] 定义函数
来源：http://oi.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://sg.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vr.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://kb.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ef.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mr.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yt.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://jf.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://af.wgjwhj.cn

[C02] 默认参数
来源：http://qv.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://al.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cs.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://bc.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kl.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cc.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xg.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://rx.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://lj.szsharing.cn

[C03] 可变参数
来源：http://og.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://uh.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rz.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hp.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://we.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wr.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pf.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ll.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vv.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://og.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://di.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ba.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mc.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dn.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://tx.521024.cn

Go:   // 无：用配置结构体参数
来源：http://ik.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://wx.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://ut.9csxet.cn

[C05] 返回多个值
来源：http://kt.gzmigu.cn

Py:   return a, b
来源：http://gx.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://eu.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qk.nszjky.cn

TS:   return { a, b };
来源：http://yf.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jl.huixinmuqiang.cn

Go:   return a, b
来源：http://ee.asd995.cn

Ruby: return a, b
来源：http://ww.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://qa.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://jv.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://ww.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://to.hahajie.cn

JS:   const square = x => x * x;
来源：http://iv.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://xh.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://to.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dc.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://gg.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iu.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://dy.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sx.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://re.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lc.gzmigu.cn

TS:   arr.map(String)
来源：http://bx.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ej.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zt.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://at.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xq.panjiajie.cn

[C08] 闭包
来源：http://uw.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yx.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fg.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dm.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aw.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hq.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yu.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vb.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kw.colortex.cn

[C09] 递归
来源：http://ci.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gp.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lh.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wo.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bf.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lc.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dr.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gx.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pp.shxzukj.cn

[C10] 变量作用域
来源：http://qs.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mm.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kr.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vt.gzmigu.cn

TS:   同 JS
来源：http://iw.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://cl.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://dx.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rz.jctech888.com.cn

C#:   块级作用域
来源：http://cp.szsharing.cn

[C11] 模块导入与导出
来源：http://re.szsharing.cn

Py:   from module import func
来源：http://vr.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dc.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lw.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ko.nszjky.cn

Java: import java.util.List;
来源：http://bc.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rm.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://sh.szsharing.cn

C#:   using System.Text;
来源：http://ox.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://ko.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://ty.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://ne.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://vi.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://lx.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ex.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://ko.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://ds.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://do.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://rd.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vy.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sy.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gx.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mr.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yd.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://eq.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rw.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cb.szxytkj.cn

[C14] 泛型函数
来源：http://xy.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://li.huixiangedu.cn

PHP:  // 无泛型
来源：http://ha.huixiangedu.cn

JS:   // 无泛型
来源：http://sa.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ir.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wb.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rm.bookmarksfly.cn

Ruby: # 无泛型
来源：http://xq.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xe.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://ya.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jl.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://vu.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oz.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qq.newstarts.cn

Java: // 无解构
来源：http://iq.lnxyls.cn

Go:   // 无解构
来源：http://fp.muxihuayi.cn

Ruby: a, b = pair
来源：http://ej.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://bz.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://ad.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zw.huixinmuqiang.cn

PHP:  // 无重载
来源：http://rz.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cp.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ve.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cu.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://yb.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://fl.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ay.jctech888.com.cn

================================================================================
来源：http://lv.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://gj.jctech888.com.cn

================================================================================
来源：http://sw.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://rb.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zo.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qu.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qy.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ws.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bs.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://qr.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://yp.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gx.521024.cn

[D02] 追加元素到末尾
来源：http://nh.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://im.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kf.lnxyls.cn

JS:   arr.push(4);
来源：http://cw.521024.cn

TS:   arr.push(4);
来源：http://pb.huanxung.cn

Java: list.add(4);
来源：http://sc.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://pa.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://de.szsharing.cn

C#:   list.Add(4);
来源：http://hp.hahajie.cn

[D03] 在指定位置插入元素
来源：http://kr.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://wr.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vy.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nz.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://my.szxytkj.cn

Java: list.add(0, 0);
来源：http://is.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gm.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vo.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://pk.szsharing.cn

[D04] 删除元素
来源：http://vn.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fa.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vd.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zo.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://hb.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ki.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ln.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eg.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gh.huanxung.cn

[D05] 访问与修改元素
来源：http://wj.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sh.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rg.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gg.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://cc.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://eb.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://vh.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gi.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ns.haigaiapp.cn

[D06] 数组长度
来源：http://tx.muxihuayi.cn

Py:   len(arr)
来源：http://kf.bookmarksfly.cn

PHP:  count($arr);
来源：http://qu.521024.cn

JS:   arr.length
来源：http://gg.hnjuh.cn

TS:   arr.length
来源：http://et.panjiajie.cn

Java: list.size();
来源：http://rq.yuntaijiaju.cn

Go:   len(arr)
来源：http://qk.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://pb.bookmarksfly.cn

C#:   list.Count;
来源：http://nn.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://zy.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gx.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ko.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://yo.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://ek.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://uh.lnxyls.cn

Go:   arr[1:4]
来源：http://da.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://nc.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://rb.nszjky.cn

[D08] 合并两个数组
来源：http://jj.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://rk.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://xv.asd995.cn


<!-- 参考信息 -->