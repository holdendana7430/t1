代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gk.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kn.bjjhwx.cn

[B07] while 循环
来源：http://zr.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://wr.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ya.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://et.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://cg.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://ur.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zk.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://he.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://eo.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://lu.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://og.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://to.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://zr.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://ot.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://os.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sb.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qp.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://iy.muxihuayi.cn

[B09] break 与 continue
来源：http://an.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gb.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fj.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wr.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rt.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oa.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ft.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nv.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fl.szsharing.cn

[B10] 遍历同时拿索引
来源：http://fu.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mf.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jh.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uh.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://be.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jd.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qo.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pz.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nm.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://eg.521024.cn

Py:   list(range(0, 10, 2))
来源：http://lz.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://uy.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nf.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hv.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mt.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wa.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://to.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ew.panjiajie.cn

[B12] 跳出多层循环
来源：http://zm.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fj.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lt.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gw.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fm.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hr.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://na.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://os.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jj.9csxet.cn

[B13] 判断是否为数字
来源：http://xh.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://fz.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://kw.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pl.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fb.muxihuayi.cn

Java: x instanceof Number
来源：http://hh.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pr.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://iw.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://mx.asd995.cn

[B14] 判断值是否在集合内
来源：http://hl.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ux.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oi.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ro.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://yu.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lt.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eb.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kj.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ra.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://ki.muxihuayi.cn

Py:   a and b or not c
来源：http://xr.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://mf.wgjwhj.cn

JS:   a && b || !c
来源：http://yq.gzmigu.cn

TS:   a && b || !c
来源：http://xs.9csxet.cn

Java: a && b || !c
来源：http://ra.newstarts.cn

Go:   a && b || !c
来源：http://fk.gzmigu.cn

Ruby: a && b || !c
来源：http://xq.shtwfgs.cn

C#:   a && b || !c
来源：http://wt.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bb.huixiangedu.cn

Py:   if not data: return
来源：http://zs.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://le.gzmigu.cn

JS:   if (!data) return;
来源：http://ao.haigaiapp.cn

TS:   if (!data) return;
来源：http://bq.szxytkj.cn

Java: if (data == null) return;
来源：http://of.shxzukj.cn

Go:   if data == nil { return }
来源：http://py.chemitech.net.cn

Ruby: return if data.nil?
来源：http://fl.521024.cn

C#:   if (data == null) return;
来源：http://ar.newstarts.cn

================================================================================
来源：http://yz.nicolike.cn

C. 函数与作用域
来源：http://ml.newstarts.cn

================================================================================
来源：http://gl.jctech888.com.cn

[C01] 定义函数
来源：http://nf.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://gp.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bd.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://me.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cs.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qs.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ib.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://vn.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ck.szsharing.cn

[C02] 默认参数
来源：http://ts.asd995.cn

Py:   def greet(name="World"): return name
来源：http://ul.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://px.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://nc.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ly.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://md.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wp.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://wx.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://kv.bookmarksfly.cn

[C03] 可变参数
来源：http://lk.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://uu.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ah.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://co.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ns.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bn.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ig.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vs.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ao.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://tv.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ya.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ia.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nw.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fg.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://io.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://ei.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://zf.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://ju.521024.cn

[C05] 返回多个值
来源：http://hf.newstarts.cn

Py:   return a, b
来源：http://we.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://ja.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://my.huixinmuqiang.cn

TS:   return { a, b };
来源：http://nv.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ww.jctech888.com.cn

Go:   return a, b
来源：http://ib.lnxyls.cn

Ruby: return a, b
来源：http://gy.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://bk.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://dv.huanxung.cn

Py:   square = lambda x: x * x
来源：http://ex.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pd.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://zc.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://ea.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xo.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fv.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://cb.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oq.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://da.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ph.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fd.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ki.nicolike.cn

TS:   arr.map(String)
来源：http://id.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hw.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oc.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://pa.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ta.nicolike.cn

[C08] 闭包
来源：http://xn.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ry.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ig.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wz.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uz.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kc.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nd.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cv.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tk.haigaiapp.cn

[C09] 递归
来源：http://yb.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ym.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uo.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ab.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kb.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zb.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pr.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://na.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kr.nszjky.cn

[C10] 变量作用域
来源：http://my.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wc.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rm.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ep.haigaiapp.cn

TS:   同 JS
来源：http://ri.shxzukj.cn

Java: 方法内为块级作用域
来源：http://pi.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://wt.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://di.shtwfgs.cn

C#:   块级作用域
来源：http://xz.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://vu.huanxung.cn

Py:   from module import func
来源：http://qn.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://la.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pj.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vf.szxytkj.cn

Java: import java.util.List;
来源：http://gb.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ta.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ed.szsharing.cn

C#:   using System.Text;
来源：http://hw.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://fr.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://ec.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://dh.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://if.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://vj.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://la.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://jw.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://xb.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iv.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://mf.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dk.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uo.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://df.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ue.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mw.shxzskj.cn

Go:   func add(a, b int) int
来源：http://iq.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uj.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tg.bjjhwx.cn

[C14] 泛型函数
来源：http://ha.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dr.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://yr.jianghongdianzi.cn

JS:   // 无泛型
来源：http://pt.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bg.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://al.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vj.szsharing.cn

Ruby: # 无泛型
来源：http://fb.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ih.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://gt.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nq.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://nc.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xf.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jr.muxihuayi.cn

Java: // 无解构
来源：http://gd.asd995.cn

Go:   // 无解构
来源：http://rf.haigaiapp.cn

Ruby: a, b = pair
来源：http://if.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://iu.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://bz.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hj.szxytkj.cn

PHP:  // 无重载
来源：http://jq.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eo.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://ue.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qc.521024.cn

Go:   // 无重载：用不同函数名
来源：http://al.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://hn.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ir.nszjky.cn

================================================================================
来源：http://te.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://wd.nicolike.cn

================================================================================
来源：http://fy.newstarts.cn

[D01] 创建数组 / 列表
来源：http://jq.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://te.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fr.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jk.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dz.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pv.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://hk.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://bv.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ij.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://yy.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vo.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bd.shtwfgs.cn

JS:   arr.push(4);
来源：http://ol.colortex.cn

TS:   arr.push(4);
来源：http://ad.9csxet.cn

Java: list.add(4);
来源：http://jd.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://kj.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://dx.szxytkj.cn

C#:   list.Add(4);
来源：http://qo.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://fl.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://ve.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fl.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mu.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://dp.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://rs.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cg.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wv.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://sm.szsharing.cn

[D04] 删除元素
来源：http://gj.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sm.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hq.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qw.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://xn.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jn.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hv.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bw.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ku.yuexingan06.cn

[D05] 访问与修改元素
来源：http://so.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xr.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://so.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qp.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://qq.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://no.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://qd.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kw.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kq.shtwfgs.cn

[D06] 数组长度
来源：http://up.521024.cn

Py:   len(arr)
来源：http://rj.chemitech.net.cn

PHP:  count($arr);
来源：http://ga.nicolike.cn

JS:   arr.length
来源：http://bx.szxytkj.cn

TS:   arr.length
来源：http://ri.yuexingan06.cn

Java: list.size();
来源：http://hi.asd995.cn

Go:   len(arr)
来源：http://du.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://ej.nicolike.cn

C#:   list.Count;
来源：http://qy.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://ms.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xy.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pk.521024.cn

JS:   arr.slice(1, 4);
来源：http://uv.huixiangedu.cn


<!-- 参考信息 -->