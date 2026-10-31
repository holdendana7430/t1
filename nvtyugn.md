代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://mc.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://br.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://ch.asd995.cn

Java: while (i < 10) { i++; }
来源：http://bu.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vw.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://ks.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://vm.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://kb.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://tf.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://of.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://vq.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://nq.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://dd.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dj.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sl.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://vb.yuexingan06.cn

[B09] break 与 continue
来源：http://fj.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gg.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iy.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sl.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sd.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dd.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ai.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qc.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fm.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://bl.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nh.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://st.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qe.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://br.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ry.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://by.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hv.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://es.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://kr.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://tq.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://xg.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oj.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://if.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lb.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ag.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://an.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ux.asd995.cn

[B12] 跳出多层循环
来源：http://jk.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vt.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hg.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wp.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jm.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rq.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jg.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xx.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sd.gzmigu.cn

[B13] 判断是否为数字
来源：http://jh.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://kk.lnxyls.cn

PHP:  is_numeric($x)
来源：http://jb.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://me.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sv.shxzukj.cn

Java: x instanceof Number
来源：http://zg.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eb.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://dt.9csxet.cn

C#:   x is int or double or decimal
来源：http://ym.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://lf.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jf.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gh.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://ps.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://zg.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zm.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tt.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ka.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vm.521024.cn

[B15] 布尔运算与取反
来源：http://vv.panjiajie.cn

Py:   a and b or not c
来源：http://lr.nszjky.cn

PHP:  $a && $b || !$c
来源：http://jo.haigaiapp.cn

JS:   a && b || !c
来源：http://sg.yuntaijiaju.cn

TS:   a && b || !c
来源：http://gp.colortex.cn

Java: a && b || !c
来源：http://xc.chemitech.net.cn

Go:   a && b || !c
来源：http://vv.9csxet.cn

Ruby: a && b || !c
来源：http://dz.shxzskj.cn

C#:   a && b || !c
来源：http://xr.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://so.chemitech.net.cn

Py:   if not data: return
来源：http://xy.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://ua.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://mb.jctech888.com.cn

TS:   if (!data) return;
来源：http://ax.9csxet.cn

Java: if (data == null) return;
来源：http://fg.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://sg.shtwfgs.cn

Ruby: return if data.nil?
来源：http://cf.huanxung.cn

C#:   if (data == null) return;
来源：http://bc.bjjhwx.cn

================================================================================
来源：http://ar.colortex.cn

C. 函数与作用域
来源：http://hj.9csxet.cn

================================================================================
来源：http://xn.lnxyls.cn

[C01] 定义函数
来源：http://hg.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://ep.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://la.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://gu.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tx.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://me.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ay.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://sw.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lt.wgjwhj.cn

[C02] 默认参数
来源：http://xz.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://ch.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aj.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://go.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xo.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zz.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ix.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://fg.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://wy.chemitech.net.cn

[C03] 可变参数
来源：http://zy.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://ov.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uj.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://su.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nr.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ww.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gu.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wd.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://de.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://gs.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ji.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jo.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gq.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rf.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://id.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://wb.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://ad.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://lt.gzmigu.cn

[C05] 返回多个值
来源：http://ai.shxzukj.cn

Py:   return a, b
来源：http://yu.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://va.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lx.yuntaijiaju.cn

TS:   return { a, b };
来源：http://fv.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wr.shtwfgs.cn

Go:   return a, b
来源：http://kw.gzmigu.cn

Ruby: return a, b
来源：http://hz.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://lm.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://wz.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://mx.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gu.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://lg.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://gh.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jr.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nk.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://sa.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dr.nszjky.cn

[C07] 把函数作为参数传入
来源：http://if.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hy.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vq.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pm.newstarts.cn

TS:   arr.map(String)
来源：http://kr.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vx.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kt.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://cb.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hx.colortex.cn

[C08] 闭包
来源：http://ct.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gd.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uw.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://to.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ye.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nq.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://km.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bs.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ij.huixinmuqiang.cn

[C09] 递归
来源：http://mk.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vb.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wa.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pb.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://it.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lz.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yr.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cw.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zf.hahajie.cn

[C10] 变量作用域
来源：http://gb.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dt.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oo.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tj.bjjhwx.cn

TS:   同 JS
来源：http://be.lnxyls.cn

Java: 方法内为块级作用域
来源：http://lm.huixiangedu.cn

Go:   花括号块级作用域
来源：http://vl.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kc.wgjwhj.cn

C#:   块级作用域
来源：http://xt.jctech888.com.cn

[C11] 模块导入与导出
来源：http://zj.huixiangedu.cn

Py:   from module import func
来源：http://rg.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ci.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qj.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wx.bjjhwx.cn

Java: import java.util.List;
来源：http://ow.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bp.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://kc.9csxet.cn

C#:   using System.Text;
来源：http://ws.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://sc.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://uq.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://mj.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://xf.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://pp.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oo.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://vq.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://ma.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jz.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://xb.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bk.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ez.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dc.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://of.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vp.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://ii.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wl.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ex.nicolike.cn

[C14] 泛型函数
来源：http://fl.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lo.gzmigu.cn

PHP:  // 无泛型
来源：http://xq.huixiangedu.cn

JS:   // 无泛型
来源：http://ja.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lo.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pz.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aa.gzmigu.cn

Ruby: # 无泛型
来源：http://tl.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ft.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://iz.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qq.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://bz.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ac.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qe.huixinmuqiang.cn

Java: // 无解构
来源：http://sk.lnxyls.cn

Go:   // 无解构
来源：http://go.szxytkj.cn

Ruby: a, b = pair
来源：http://yi.nszjky.cn

C#:   var (a, b) = pair;
来源：http://sx.9csxet.cn

[C16] 函数 / 方法重载
来源：http://wb.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dq.yuntaijiaju.cn

PHP:  // 无重载
来源：http://sv.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://df.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://se.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xl.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://oc.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://hl.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qw.shtwfgs.cn

================================================================================
来源：http://xc.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://bg.9csxet.cn

================================================================================
来源：http://do.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://hj.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://co.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xh.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jt.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ca.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ur.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://px.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://ws.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fs.hahajie.cn

[D02] 追加元素到末尾
来源：http://af.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bj.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wc.szsharing.cn

JS:   arr.push(4);
来源：http://qj.chemitech.net.cn

TS:   arr.push(4);
来源：http://hz.9csxet.cn

Java: list.add(4);
来源：http://rx.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://zs.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://bd.521024.cn

C#:   list.Add(4);
来源：http://at.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://su.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://xq.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dp.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dw.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://cs.huixiangedu.cn

Java: list.add(0, 0);
来源：http://ge.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hk.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zn.521024.cn

C#:   list.Insert(0, 0);
来源：http://tw.muxihuayi.cn

[D04] 删除元素
来源：http://yl.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fy.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cs.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ao.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://mn.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bk.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cv.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lo.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lp.newstarts.cn

[D05] 访问与修改元素
来源：http://vh.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jt.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ga.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ch.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://na.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://xg.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://sj.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://to.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bs.nszjky.cn

[D06] 数组长度
来源：http://wo.jianghongdianzi.cn

Py:   len(arr)
来源：http://ja.newstarts.cn

PHP:  count($arr);
来源：http://oo.chemitech.net.cn

JS:   arr.length
来源：http://xt.yuexingan06.cn

TS:   arr.length
来源：http://hs.szsharing.cn

Java: list.size();
来源：http://lu.huixinmuqiang.cn

Go:   len(arr)
来源：http://or.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://ba.wgjwhj.cn

C#:   list.Count;
来源：http://cc.521024.cn

[D07] 切片 / 取子数组
来源：http://ig.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bs.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fo.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://po.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://lh.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://ob.panjiajie.cn

Go:   arr[1:4]
来源：http://bo.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://on.asd995.cn


<!-- 参考信息 -->