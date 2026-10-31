代发 wailian999

[B05] 遍历数组 / 列表
来源：http://gk.newstarts.cn

Py:   for item in arr: print(item)
来源：http://sx.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pv.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yu.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wz.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ln.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qf.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://ob.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zt.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://ww.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bl.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mv.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mq.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://we.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gf.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wa.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xo.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uf.shxzskj.cn

[B07] while 循环
来源：http://rd.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://wm.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kt.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://lj.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://je.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://wb.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://be.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://cn.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://ex.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://hp.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://dl.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ee.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://nu.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://fk.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://ew.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://al.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tv.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://sw.asd995.cn

[B09] break 与 continue
来源：http://bq.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://li.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ts.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sv.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gp.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tw.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ut.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://id.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xk.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://dz.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xl.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yg.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rk.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bw.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qg.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xp.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lt.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jk.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://oj.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://ji.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://mc.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://di.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qz.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nb.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zm.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://qd.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dt.yuexingan06.cn

[B12] 跳出多层循环
来源：http://ku.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ra.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bo.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qh.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hm.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qf.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bu.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nd.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yh.yuexingan06.cn

[B13] 判断是否为数字
来源：http://cz.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://yn.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://vn.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ng.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ek.panjiajie.cn

Java: x instanceof Number
来源：http://hq.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jm.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://cx.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://qm.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://zf.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cu.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sf.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://bn.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ok.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qm.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cx.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wv.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yo.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://uz.yuntaijiaju.cn

Py:   a and b or not c
来源：http://ao.szsharing.cn

PHP:  $a && $b || !$c
来源：http://dz.shxzukj.cn

JS:   a && b || !c
来源：http://kh.chemitech.net.cn

TS:   a && b || !c
来源：http://zz.jctech888.com.cn

Java: a && b || !c
来源：http://bb.nszjky.cn

Go:   a && b || !c
来源：http://hc.newstarts.cn

Ruby: a && b || !c
来源：http://sp.bookmarksfly.cn

C#:   a && b || !c
来源：http://te.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dt.shxzskj.cn

Py:   if not data: return
来源：http://km.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://oq.huixiangedu.cn

JS:   if (!data) return;
来源：http://se.lnxyls.cn

TS:   if (!data) return;
来源：http://gc.lnxyls.cn

Java: if (data == null) return;
来源：http://ap.shxzskj.cn

Go:   if data == nil { return }
来源：http://ty.shtwfgs.cn

Ruby: return if data.nil?
来源：http://yg.szxytkj.cn

C#:   if (data == null) return;
来源：http://ox.huanxung.cn

================================================================================
来源：http://bv.huixiangedu.cn

C. 函数与作用域
来源：http://rs.szxytkj.cn

================================================================================
来源：http://cd.yuntaijiaju.cn

[C01] 定义函数
来源：http://bx.asd995.cn

Py:   def add(a, b): return a + b
来源：http://xk.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dm.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://bo.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://es.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ae.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bl.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://ee.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://is.huanxung.cn

[C02] 默认参数
来源：http://jt.521024.cn

Py:   def greet(name="World"): return name
来源：http://ll.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://th.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://nr.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://md.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zf.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://md.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://lv.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://jx.hahajie.cn

[C03] 可变参数
来源：http://uj.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://be.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ff.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bi.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ee.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pp.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bd.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tl.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://su.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://jp.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tq.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pg.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ja.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sb.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://ia.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://uh.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://nk.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://xr.chemitech.net.cn

[C05] 返回多个值
来源：http://no.bookmarksfly.cn

Py:   return a, b
来源：http://fo.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://lp.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zl.wgjwhj.cn

TS:   return { a, b };
来源：http://hj.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://em.panjiajie.cn

Go:   return a, b
来源：http://zk.jctech888.com.cn

Ruby: return a, b
来源：http://yc.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://cq.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://xw.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://gq.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lg.gzmigu.cn

JS:   const square = x => x * x;
来源：http://ez.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://oe.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://en.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ns.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://zf.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nm.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://sg.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ba.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ou.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cm.gzmigu.cn

TS:   arr.map(String)
来源：http://zn.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kj.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zc.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://hf.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zl.nicolike.cn

[C08] 闭包
来源：http://bv.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wo.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oq.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eh.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uo.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cw.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ts.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oy.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rf.haigaiapp.cn

[C09] 递归
来源：http://mn.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tt.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hy.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vx.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ps.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://za.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cc.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://od.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wh.521024.cn

[C10] 变量作用域
来源：http://kt.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nb.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rb.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qy.szsharing.cn

TS:   同 JS
来源：http://sh.szxytkj.cn

Java: 方法内为块级作用域
来源：http://zu.shxzskj.cn

Go:   花括号块级作用域
来源：http://fw.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://in.hnjuh.cn

C#:   块级作用域
来源：http://qo.gzmigu.cn

[C11] 模块导入与导出
来源：http://uk.hnjuh.cn

Py:   from module import func
来源：http://bh.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://co.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://if.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lo.gzmigu.cn

Java: import java.util.List;
来源：http://mk.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fx.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://md.huanxung.cn

C#:   using System.Text;
来源：http://rw.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://ac.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://zk.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://ia.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://uo.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://qh.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pa.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://iu.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://pd.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hn.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://ko.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ia.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mn.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://my.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zb.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cu.nicolike.cn

Go:   func add(a, b int) int
来源：http://fi.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vo.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ib.gzmigu.cn

[C14] 泛型函数
来源：http://vl.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dd.panjiajie.cn

PHP:  // 无泛型
来源：http://hz.521024.cn

JS:   // 无泛型
来源：http://fh.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oh.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mv.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://px.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://ek.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tv.hahajie.cn

[C15] 解构 / 展开参数
来源：http://do.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gh.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://ge.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lo.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xj.bjjhwx.cn

Java: // 无解构
来源：http://qj.gzmigu.cn

Go:   // 无解构
来源：http://ye.panjiajie.cn

Ruby: a, b = pair
来源：http://kp.newstarts.cn

C#:   var (a, b) = pair;
来源：http://dj.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://yl.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nt.shtwfgs.cn

PHP:  // 无重载
来源：http://mx.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yo.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://gx.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ox.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://pu.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://se.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ov.bjjhwx.cn

================================================================================
来源：http://gs.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://ng.hahajie.cn

================================================================================
来源：http://gp.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://cv.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hn.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xu.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lw.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iu.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ug.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://tx.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://ay.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jj.521024.cn

[D02] 追加元素到末尾
来源：http://wm.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ko.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xz.jctech888.com.cn

JS:   arr.push(4);
来源：http://fv.shxzskj.cn

TS:   arr.push(4);
来源：http://yk.huixiangedu.cn

Java: list.add(4);
来源：http://qf.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://hm.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://pv.colortex.cn

C#:   list.Add(4);
来源：http://vo.huanxung.cn

[D03] 在指定位置插入元素
来源：http://qw.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://on.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wn.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yl.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://zk.huanxung.cn

Java: list.add(0, 0);
来源：http://cs.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qi.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hr.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://jy.huixinmuqiang.cn

[D04] 删除元素
来源：http://uv.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://of.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sp.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xo.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://oa.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://np.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fu.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wd.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://il.szxytkj.cn

[D05] 访问与修改元素
来源：http://wm.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://go.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xe.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gj.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://sh.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://yz.bjjhwx.cn


<!-- 参考信息 -->