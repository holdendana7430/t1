代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://tk.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fv.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://io.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://wo.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kw.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://ng.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mj.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://li.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wb.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wh.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fo.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vo.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bd.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sy.nszjky.cn

[B07] while 循环
来源：http://if.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://yb.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xe.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://ty.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://qa.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://ia.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zg.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://oa.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://vr.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://pe.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://mm.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://os.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://no.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://nn.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://km.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wr.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ku.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://of.hahajie.cn

[B09] break 与 continue
来源：http://sf.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://we.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rz.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bn.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ex.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gi.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wx.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ep.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://fo.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ll.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ff.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jy.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ms.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://de.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iw.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kt.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hw.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://xe.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://io.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://wt.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ub.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ne.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bj.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jm.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://ay.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xx.chemitech.net.cn

[B12] 跳出多层循环
来源：http://ao.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wv.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ck.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kg.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wf.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kb.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tq.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nb.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ij.hnjuh.cn

[B13] 判断是否为数字
来源：http://pj.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://sx.lnxyls.cn

PHP:  is_numeric($x)
来源：http://xk.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gp.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yr.huixiangedu.cn

Java: x instanceof Number
来源：http://dx.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mv.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://bo.gzmigu.cn

C#:   x is int or double or decimal
来源：http://lb.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://gu.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://js.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yu.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://gy.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://so.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ci.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wz.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ml.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://de.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://mx.nicolike.cn

Py:   a and b or not c
来源：http://ar.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://ng.shxzukj.cn

JS:   a && b || !c
来源：http://mp.yuexingan06.cn

TS:   a && b || !c
来源：http://ym.chemitech.net.cn

Java: a && b || !c
来源：http://iz.jianghongdianzi.cn

Go:   a && b || !c
来源：http://vt.panjiajie.cn

Ruby: a && b || !c
来源：http://qo.wgjwhj.cn

C#:   a && b || !c
来源：http://hx.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kt.yuexingan06.cn

Py:   if not data: return
来源：http://pn.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://pw.jctech888.com.cn

JS:   if (!data) return;
来源：http://re.wgjwhj.cn

TS:   if (!data) return;
来源：http://zx.521024.cn

Java: if (data == null) return;
来源：http://mv.hnjuh.cn

Go:   if data == nil { return }
来源：http://on.hahajie.cn

Ruby: return if data.nil?
来源：http://zm.nszjky.cn

C#:   if (data == null) return;
来源：http://rp.panjiajie.cn

================================================================================
来源：http://xi.newstarts.cn

C. 函数与作用域
来源：http://va.hnjuh.cn

================================================================================
来源：http://mn.yuexingan06.cn

[C01] 定义函数
来源：http://rz.colortex.cn

Py:   def add(a, b): return a + b
来源：http://zy.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tn.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://zq.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xs.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nx.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yg.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://om.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zi.yuntaijiaju.cn

[C02] 默认参数
来源：http://lm.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://ni.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dk.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://lj.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qt.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xx.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ck.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://up.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ye.nszjky.cn

[C03] 可变参数
来源：http://ob.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://xl.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bm.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://si.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bw.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ux.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sm.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ks.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bh.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://qo.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xa.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hx.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yk.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yd.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://bx.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://yr.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://ai.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://ud.shtwfgs.cn

[C05] 返回多个值
来源：http://yp.haigaiapp.cn

Py:   return a, b
来源：http://mr.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://jq.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://go.colortex.cn

TS:   return { a, b };
来源：http://jt.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://he.yuntaijiaju.cn

Go:   return a, b
来源：http://tg.newstarts.cn

Ruby: return a, b
来源：http://hw.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://bc.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://yq.521024.cn

Py:   square = lambda x: x * x
来源：http://wf.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zg.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://cd.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://fq.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vl.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nl.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://ch.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fd.szsharing.cn

[C07] 把函数作为参数传入
来源：http://ak.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fw.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lc.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zs.panjiajie.cn

TS:   arr.map(String)
来源：http://nq.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nv.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jy.521024.cn

Ruby: arr.map(&:upcase)
来源：http://gq.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cj.haigaiapp.cn

[C08] 闭包
来源：http://ul.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mk.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zr.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uq.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://md.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dl.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sl.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lk.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lc.bookmarksfly.cn

[C09] 递归
来源：http://js.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://db.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fv.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xn.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ml.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fh.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jq.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cy.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jc.asd995.cn

[C10] 变量作用域
来源：http://ay.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qw.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mm.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://po.huixiangedu.cn

TS:   同 JS
来源：http://zs.asd995.cn

Java: 方法内为块级作用域
来源：http://sr.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://sg.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nj.521024.cn

C#:   块级作用域
来源：http://wq.yuexingan06.cn

[C11] 模块导入与导出
来源：http://lr.shxzukj.cn

Py:   from module import func
来源：http://df.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qp.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jc.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vy.haigaiapp.cn

Java: import java.util.List;
来源：http://uc.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://im.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://hd.yuntaijiaju.cn

C#:   using System.Text;
来源：http://em.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://jw.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://jy.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://bh.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://dm.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://dh.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ok.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://sc.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://in.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://su.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://qx.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xd.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hq.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qt.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wf.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kp.shxzukj.cn

Go:   func add(a, b int) int
来源：http://wv.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ur.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oj.asd995.cn

[C14] 泛型函数
来源：http://sp.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ah.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://lu.521024.cn

JS:   // 无泛型
来源：http://ps.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://us.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aw.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ys.bookmarksfly.cn

Ruby: # 无泛型
来源：http://wk.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ov.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://es.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bc.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://pj.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lq.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zm.bookmarksfly.cn

Java: // 无解构
来源：http://kr.bookmarksfly.cn

Go:   // 无解构
来源：http://ju.lnxyls.cn

Ruby: a, b = pair
来源：http://iy.newstarts.cn

C#:   var (a, b) = pair;
来源：http://zi.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://gu.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lc.huixinmuqiang.cn

PHP:  // 无重载
来源：http://zp.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hv.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://aq.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ce.521024.cn

Go:   // 无重载：用不同函数名
来源：http://am.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://dg.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rd.huixiangedu.cn

================================================================================
来源：http://zy.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://uy.szxytkj.cn

================================================================================
来源：http://la.asd995.cn

[D01] 创建数组 / 列表
来源：http://bt.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zz.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zn.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ny.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ts.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eo.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://xf.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://xw.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://et.newstarts.cn

[D02] 追加元素到末尾
来源：http://vo.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fg.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ar.huixiangedu.cn

JS:   arr.push(4);
来源：http://mo.huanxung.cn

TS:   arr.push(4);
来源：http://ca.wgjwhj.cn

Java: list.add(4);
来源：http://ak.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://uj.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://cl.hahajie.cn

C#:   list.Add(4);
来源：http://aq.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://wf.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://vu.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://in.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hx.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://hp.wgjwhj.cn

Java: list.add(0, 0);
来源：http://az.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zq.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://po.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://dk.521024.cn

[D04] 删除元素
来源：http://pv.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fl.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bh.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zf.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://ob.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gn.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ei.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lq.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rr.chemitech.net.cn

[D05] 访问与修改元素
来源：http://bo.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ot.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xd.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nz.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://za.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://lm.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://jg.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jk.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nh.newstarts.cn

[D06] 数组长度
来源：http://rw.jianghongdianzi.cn


<!-- 参考信息 -->