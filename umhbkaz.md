代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nf.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vg.nicolike.cn

[B07] while 循环
来源：http://ns.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://un.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://we.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://rh.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://vl.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://ep.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yl.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://sq.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://te.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://wb.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://yl.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aj.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://ug.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://om.521024.cn

Java: do { i++; } while (i < 10);
来源：http://gr.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ga.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://am.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://ad.huixiangedu.cn

[B09] break 与 continue
来源：http://qk.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oj.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oo.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qy.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qj.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gc.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tt.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ry.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://wv.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sl.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yn.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ye.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zp.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sl.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oc.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nh.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oj.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ay.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://ka.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://cy.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tl.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bq.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hv.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qo.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://re.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cj.szsharing.cn

[B12] 跳出多层循环
来源：http://vv.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sr.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bn.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ld.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uv.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rd.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tl.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fu.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ng.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://ke.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ky.szxytkj.cn

PHP:  is_numeric($x)
来源：http://wt.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mn.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://re.gzmigu.cn

Java: x instanceof Number
来源：http://qc.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rs.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://ym.9csxet.cn

C#:   x is int or double or decimal
来源：http://kr.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://gg.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lx.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dm.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://fy.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://xh.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rk.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sf.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zf.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://py.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://lk.bjjhwx.cn

Py:   a and b or not c
来源：http://zl.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://bd.szxytkj.cn

JS:   a && b || !c
来源：http://on.gzmigu.cn

TS:   a && b || !c
来源：http://as.521024.cn

Java: a && b || !c
来源：http://af.hahajie.cn

Go:   a && b || !c
来源：http://ot.szsharing.cn

Ruby: a && b || !c
来源：http://fc.shtwfgs.cn

C#:   a && b || !c
来源：http://iw.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dj.shxzukj.cn

Py:   if not data: return
来源：http://xy.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://dr.bookmarksfly.cn

JS:   if (!data) return;
来源：http://op.jctech888.com.cn

TS:   if (!data) return;
来源：http://te.nicolike.cn

Java: if (data == null) return;
来源：http://om.panjiajie.cn

Go:   if data == nil { return }
来源：http://vl.jctech888.com.cn

Ruby: return if data.nil?
来源：http://qk.gzmigu.cn

C#:   if (data == null) return;
来源：http://og.huixinmuqiang.cn

================================================================================
来源：http://ts.jctech888.com.cn

C. 函数与作用域
来源：http://uy.colortex.cn

================================================================================
来源：http://pj.newstarts.cn

[C01] 定义函数
来源：http://dd.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://ws.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pk.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://nm.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ls.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gr.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kb.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://xd.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qt.szxytkj.cn

[C02] 默认参数
来源：http://gf.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://ij.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vo.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://cm.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bg.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pu.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eu.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://mh.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://sf.jctech888.com.cn

[C03] 可变参数
来源：http://ag.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://lg.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://if.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bb.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ex.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uv.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ae.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://td.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://px.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://kf.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vw.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ep.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ny.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oj.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://rx.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://rn.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://af.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://lf.haigaiapp.cn

[C05] 返回多个值
来源：http://gh.9csxet.cn

Py:   return a, b
来源：http://lp.gzmigu.cn

PHP:  return [$a, $b];
来源：http://wd.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vz.huanxung.cn

TS:   return { a, b };
来源：http://ez.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wz.wgjwhj.cn

Go:   return a, b
来源：http://jh.haigaiapp.cn

Ruby: return a, b
来源：http://xh.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://bb.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://dx.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://vd.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nx.asd995.cn

JS:   const square = x => x * x;
来源：http://kl.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://us.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fh.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ab.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://tf.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ko.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://yt.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mt.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ee.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rw.bookmarksfly.cn

TS:   arr.map(String)
来源：http://lz.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zr.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pu.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://kt.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rz.jctech888.com.cn

[C08] 闭包
来源：http://ny.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cy.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ml.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ee.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gy.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wo.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hi.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cv.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nt.haigaiapp.cn

[C09] 递归
来源：http://dv.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aq.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zx.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ec.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bi.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lq.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kb.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ck.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dz.colortex.cn

[C10] 变量作用域
来源：http://rq.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lc.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ue.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fq.gzmigu.cn

TS:   同 JS
来源：http://ss.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://zd.yuexingan06.cn

Go:   花括号块级作用域
来源：http://bk.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eb.jianghongdianzi.cn

C#:   块级作用域
来源：http://uu.szxytkj.cn

[C11] 模块导入与导出
来源：http://ma.shxzskj.cn

Py:   from module import func
来源：http://zg.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vx.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://na.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xn.yuntaijiaju.cn

Java: import java.util.List;
来源：http://pd.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rb.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://xp.yuntaijiaju.cn

C#:   using System.Text;
来源：http://me.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://bu.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://me.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://dc.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://qj.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://nl.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kd.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://cb.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://is.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://th.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://gw.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tx.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hu.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zl.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lu.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wi.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://tc.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vo.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wk.hahajie.cn

[C14] 泛型函数
来源：http://sr.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ke.colortex.cn

PHP:  // 无泛型
来源：http://zg.szxytkj.cn

JS:   // 无泛型
来源：http://fi.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yi.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ja.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fa.newstarts.cn

Ruby: # 无泛型
来源：http://oe.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vz.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://ua.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fa.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://nt.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bx.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cl.szxytkj.cn

Java: // 无解构
来源：http://jf.haigaiapp.cn

Go:   // 无解构
来源：http://ut.gzmigu.cn

Ruby: a, b = pair
来源：http://er.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://bk.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://ky.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dm.muxihuayi.cn

PHP:  // 无重载
来源：http://gy.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ir.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://mb.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cc.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://up.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://mr.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ts.lnxyls.cn

================================================================================
来源：http://bt.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ej.newstarts.cn

================================================================================
来源：http://sd.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://cp.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://re.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qu.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wo.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ix.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xm.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ol.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://hm.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jv.hnjuh.cn

[D02] 追加元素到末尾
来源：http://fy.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oz.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zn.nicolike.cn

JS:   arr.push(4);
来源：http://mv.wgjwhj.cn

TS:   arr.push(4);
来源：http://js.hnjuh.cn

Java: list.add(4);
来源：http://us.521024.cn

Go:   arr = append(arr, 4)
来源：http://po.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://dp.9csxet.cn

C#:   list.Add(4);
来源：http://lf.colortex.cn

[D03] 在指定位置插入元素
来源：http://zv.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://mq.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ww.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xn.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://qz.colortex.cn

Java: list.add(0, 0);
来源：http://jd.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fm.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tg.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://zg.panjiajie.cn

[D04] 删除元素
来源：http://bk.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jk.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sm.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eh.asd995.cn

TS:   arr.splice(0, 1);
来源：http://mz.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kf.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ip.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zm.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ya.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://uz.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zz.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ww.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cm.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://zn.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://hv.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://xk.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jg.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gj.panjiajie.cn

[D06] 数组长度
来源：http://ns.huanxung.cn

Py:   len(arr)
来源：http://xr.yuntaijiaju.cn

PHP:  count($arr);
来源：http://ib.yuntaijiaju.cn

JS:   arr.length
来源：http://fm.chemitech.net.cn

TS:   arr.length
来源：http://ig.haigaiapp.cn

Java: list.size();
来源：http://ez.jianghongdianzi.cn

Go:   len(arr)
来源：http://zk.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://qw.jctech888.com.cn

C#:   list.Count;
来源：http://sl.9csxet.cn

[D07] 切片 / 取子数组
来源：http://ds.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cu.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://is.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://zr.asd995.cn


<!-- 参考信息 -->