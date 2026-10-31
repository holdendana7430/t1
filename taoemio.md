代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kr.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wt.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://zk.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://az.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://ly.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://tp.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fm.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wi.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kv.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ra.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yh.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://jm.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ff.asd995.cn

[B06] 遍历字典 / 对象
来源：http://tu.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cy.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hn.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wx.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vt.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kv.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bx.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xt.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pb.nszjky.cn

[B07] while 循环
来源：http://nz.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://ql.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bl.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://xe.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://gp.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://bu.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ei.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://ju.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://oa.colortex.cn

[B08] do-while（至少执行一次）
来源：http://gx.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://po.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lf.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://nd.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://kv.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://xy.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xu.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ox.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://bw.szxytkj.cn

[B09] break 与 continue
来源：http://cv.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xg.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cl.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vu.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xe.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ge.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://at.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ao.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tc.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://ve.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qd.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oa.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bq.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qy.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://px.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dr.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qr.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uk.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://rr.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://mk.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://wa.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://es.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zu.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wy.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ez.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://bx.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kj.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://og.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ag.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cc.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ii.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gs.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ep.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ue.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eu.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jy.gzmigu.cn

[B13] 判断是否为数字
来源：http://kw.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://hy.521024.cn

PHP:  is_numeric($x)
来源：http://lt.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ta.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bd.bookmarksfly.cn

Java: x instanceof Number
来源：http://ry.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gi.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://rx.gzmigu.cn

C#:   x is int or double or decimal
来源：http://md.9csxet.cn

[B14] 判断值是否在集合内
来源：http://fo.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vy.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wb.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://ap.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://jo.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wo.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xp.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cl.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cd.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://zb.haigaiapp.cn

Py:   a and b or not c
来源：http://er.nszjky.cn

PHP:  $a && $b || !$c
来源：http://ai.szsharing.cn

JS:   a && b || !c
来源：http://mv.muxihuayi.cn

TS:   a && b || !c
来源：http://ur.huixiangedu.cn

Java: a && b || !c
来源：http://ea.haigaiapp.cn

Go:   a && b || !c
来源：http://ha.bjjhwx.cn

Ruby: a && b || !c
来源：http://sr.hnjuh.cn

C#:   a && b || !c
来源：http://nu.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kq.szxytkj.cn

Py:   if not data: return
来源：http://yb.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://ks.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://wl.muxihuayi.cn

TS:   if (!data) return;
来源：http://ap.lnxyls.cn

Java: if (data == null) return;
来源：http://yr.lnxyls.cn

Go:   if data == nil { return }
来源：http://ng.asd995.cn

Ruby: return if data.nil?
来源：http://dn.lnxyls.cn

C#:   if (data == null) return;
来源：http://av.huanxung.cn

================================================================================
来源：http://jx.jianghongdianzi.cn

C. 函数与作用域
来源：http://cg.shxzukj.cn

================================================================================
来源：http://vb.haigaiapp.cn

[C01] 定义函数
来源：http://pa.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://oq.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://og.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://uj.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gt.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tr.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yl.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://uk.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ir.wgjwhj.cn

[C02] 默认参数
来源：http://rp.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://bp.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fd.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://ik.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bw.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jw.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oa.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://jx.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://bx.gzmigu.cn

[C03] 可变参数
来源：http://vf.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://av.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zn.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://op.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mw.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nz.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qq.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xj.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nl.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://tm.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aq.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iz.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sw.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sp.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://eh.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://rv.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://px.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://ls.nszjky.cn

[C05] 返回多个值
来源：http://ox.colortex.cn

Py:   return a, b
来源：http://jx.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://yq.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ky.bjjhwx.cn

TS:   return { a, b };
来源：http://qb.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mv.hnjuh.cn

Go:   return a, b
来源：http://oe.shxzukj.cn

Ruby: return a, b
来源：http://tv.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://ux.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://pi.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ss.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rs.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://lh.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://qm.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wm.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wv.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://ua.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tt.hahajie.cn

[C07] 把函数作为参数传入
来源：http://qv.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://by.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hk.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dn.yuexingan06.cn

TS:   arr.map(String)
来源：http://kj.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wo.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ik.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://oo.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yy.nszjky.cn

[C08] 闭包
来源：http://fp.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ub.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mm.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iy.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ct.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tq.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fi.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ts.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jw.hnjuh.cn

[C09] 递归
来源：http://sc.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://um.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jz.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yk.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hx.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lk.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tp.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zr.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://go.szsharing.cn

[C10] 变量作用域
来源：http://fj.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kw.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ff.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lq.haigaiapp.cn

TS:   同 JS
来源：http://ob.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://wr.521024.cn

Go:   花括号块级作用域
来源：http://eg.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pd.yuexingan06.cn

C#:   块级作用域
来源：http://aq.newstarts.cn

[C11] 模块导入与导出
来源：http://wf.newstarts.cn

Py:   from module import func
来源：http://lg.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zf.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zx.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lj.nszjky.cn

Java: import java.util.List;
来源：http://he.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ob.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://mx.wgjwhj.cn

C#:   using System.Text;
来源：http://zv.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://pr.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://gt.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://lr.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://bi.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://da.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wy.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://da.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://im.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pn.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://uo.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://de.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ci.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ol.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ug.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lj.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://jy.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uw.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gs.hnjuh.cn

[C14] 泛型函数
来源：http://ut.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ds.yuexingan06.cn

PHP:  // 无泛型
来源：http://xz.huixinmuqiang.cn

JS:   // 无泛型
来源：http://gu.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hk.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ys.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lh.hnjuh.cn

Ruby: # 无泛型
来源：http://ag.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zf.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://hx.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wh.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://fw.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uu.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xt.jctech888.com.cn

Java: // 无解构
来源：http://am.521024.cn

Go:   // 无解构
来源：http://zl.haigaiapp.cn

Ruby: a, b = pair
来源：http://ak.521024.cn

C#:   var (a, b) = pair;
来源：http://ar.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://qz.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fq.hahajie.cn

PHP:  // 无重载
来源：http://ze.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zk.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://wz.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pr.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://js.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://ug.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hm.panjiajie.cn

================================================================================
来源：http://hq.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://gt.bookmarksfly.cn

================================================================================
来源：http://yp.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://ha.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qw.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://we.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mx.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fy.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xd.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ha.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://tr.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zb.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://kl.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qw.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://up.9csxet.cn

JS:   arr.push(4);
来源：http://ff.wgjwhj.cn

TS:   arr.push(4);
来源：http://ee.chemitech.net.cn

Java: list.add(4);
来源：http://ad.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://us.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://qj.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://on.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://pd.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://ke.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tt.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ha.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://oo.nicolike.cn

Java: list.add(0, 0);
来源：http://cn.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yx.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hl.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://vk.wgjwhj.cn

[D04] 删除元素
来源：http://pg.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://co.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://on.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wq.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://ea.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://am.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ty.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pk.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nf.9csxet.cn

[D05] 访问与修改元素
来源：http://eu.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zg.jctech888.com.cn


<!-- 参考信息 -->