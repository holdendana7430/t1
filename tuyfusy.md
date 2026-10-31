代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ub.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://uy.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qw.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gw.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tz.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rn.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://is.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rn.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ml.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jh.shtwfgs.cn

[B07] while 循环
来源：http://ov.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://gb.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dy.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://qv.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://pg.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://ol.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pw.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://tm.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://lj.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://ea.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://ge.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lg.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://sb.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://zb.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://em.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fu.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fp.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://ct.bookmarksfly.cn

[B09] break 与 continue
来源：http://bh.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sz.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ib.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://na.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://av.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nc.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fk.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ln.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://te.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gw.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nh.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sp.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sp.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://au.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fs.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mg.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ds.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://et.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://ik.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://kh.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ap.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vm.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vn.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zy.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://qq.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xc.huixiangedu.cn

[B12] 跳出多层循环
来源：http://mj.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eh.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fx.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rh.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lz.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cj.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bq.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://es.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ks.chemitech.net.cn

[B13] 判断是否为数字
来源：http://ox.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://ok.gzmigu.cn

PHP:  is_numeric($x)
来源：http://pe.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://de.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mr.9csxet.cn

Java: x instanceof Number
来源：http://lk.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lv.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://qz.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://kn.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://eb.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pi.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kx.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://cg.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ki.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nd.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://me.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dn.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mi.asd995.cn

[B15] 布尔运算与取反
来源：http://yk.huixiangedu.cn

Py:   a and b or not c
来源：http://nv.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://se.szxytkj.cn

JS:   a && b || !c
来源：http://du.wgjwhj.cn

TS:   a && b || !c
来源：http://ce.chemitech.net.cn

Java: a && b || !c
来源：http://jo.huixinmuqiang.cn

Go:   a && b || !c
来源：http://hi.nszjky.cn

Ruby: a && b || !c
来源：http://yw.colortex.cn

C#:   a && b || !c
来源：http://hy.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oe.huixiangedu.cn

Py:   if not data: return
来源：http://bn.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://np.muxihuayi.cn

JS:   if (!data) return;
来源：http://xz.colortex.cn

TS:   if (!data) return;
来源：http://qc.gzmigu.cn

Java: if (data == null) return;
来源：http://hp.chemitech.net.cn

Go:   if data == nil { return }
来源：http://bc.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://xc.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://lf.bookmarksfly.cn

================================================================================
来源：http://gd.lnxyls.cn

C. 函数与作用域
来源：http://ys.bookmarksfly.cn

================================================================================
来源：http://gm.huanxung.cn

[C01] 定义函数
来源：http://mv.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://ad.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fp.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://kb.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iq.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yy.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ru.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://np.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ld.muxihuayi.cn

[C02] 默认参数
来源：http://mv.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://qn.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://td.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://ik.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gd.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cm.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ex.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://rk.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://qb.yuntaijiaju.cn

[C03] 可变参数
来源：http://wm.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://gj.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vu.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ya.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yj.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mu.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ix.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tg.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ok.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://pd.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zx.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dn.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kl.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xh.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://lc.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://sj.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://ct.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://fp.nszjky.cn

[C05] 返回多个值
来源：http://pt.yuntaijiaju.cn

Py:   return a, b
来源：http://vo.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://qa.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wb.jianghongdianzi.cn

TS:   return { a, b };
来源：http://mx.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bs.jctech888.com.cn

Go:   return a, b
来源：http://ra.chemitech.net.cn

Ruby: return a, b
来源：http://bi.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://gt.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://uo.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://rq.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nl.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://tg.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://gw.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ls.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gu.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://wc.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ms.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://cq.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://km.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ru.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wl.wgjwhj.cn

TS:   arr.map(String)
来源：http://ef.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ql.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ct.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://uy.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ym.9csxet.cn

[C08] 闭包
来源：http://fk.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rz.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ka.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://im.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xz.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fo.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jc.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vl.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ub.haigaiapp.cn

[C09] 递归
来源：http://qg.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lc.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yb.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cn.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ja.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ik.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uh.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kk.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://by.521024.cn

[C10] 变量作用域
来源：http://ix.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dl.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ki.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fw.haigaiapp.cn

TS:   同 JS
来源：http://ue.521024.cn

Java: 方法内为块级作用域
来源：http://og.colortex.cn

Go:   花括号块级作用域
来源：http://fg.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ug.lnxyls.cn

C#:   块级作用域
来源：http://qc.newstarts.cn

[C11] 模块导入与导出
来源：http://sq.colortex.cn

Py:   from module import func
来源：http://ok.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uj.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ae.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wv.chemitech.net.cn

Java: import java.util.List;
来源：http://wo.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ub.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://om.chemitech.net.cn

C#:   using System.Text;
来源：http://hb.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://bd.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://qg.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://oo.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://hm.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://vt.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nk.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://oi.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://df.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mt.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://zy.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ee.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qu.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wu.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bi.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ig.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://pa.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pr.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://js.bjjhwx.cn

[C14] 泛型函数
来源：http://gk.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rn.wgjwhj.cn

PHP:  // 无泛型
来源：http://nz.nicolike.cn

JS:   // 无泛型
来源：http://cf.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wj.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mp.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yj.chemitech.net.cn

Ruby: # 无泛型
来源：http://sg.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ke.szsharing.cn

[C15] 解构 / 展开参数
来源：http://up.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ge.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://ed.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xn.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hi.colortex.cn

Java: // 无解构
来源：http://sv.chemitech.net.cn

Go:   // 无解构
来源：http://jp.hahajie.cn

Ruby: a, b = pair
来源：http://oc.521024.cn

C#:   var (a, b) = pair;
来源：http://jo.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://mi.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tx.yuntaijiaju.cn

PHP:  // 无重载
来源：http://ih.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pb.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://gf.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nd.521024.cn

Go:   // 无重载：用不同函数名
来源：http://ey.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://yy.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sl.muxihuayi.cn

================================================================================
来源：http://ux.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://ei.huixiangedu.cn

================================================================================
来源：http://uy.huanxung.cn

[D01] 创建数组 / 列表
来源：http://bz.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ii.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ov.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://es.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gr.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vr.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://qw.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://dg.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ch.shxzskj.cn

[D02] 追加元素到末尾
来源：http://vp.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bp.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xv.hnjuh.cn

JS:   arr.push(4);
来源：http://oq.shxzskj.cn

TS:   arr.push(4);
来源：http://sk.gzmigu.cn

Java: list.add(4);
来源：http://ji.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://cf.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://qy.shxzskj.cn

C#:   list.Add(4);
来源：http://md.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://rh.colortex.cn

Py:   arr.insert(0, 0)
来源：http://hx.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ac.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jp.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://xp.yuexingan06.cn

Java: list.add(0, 0);
来源：http://yb.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vt.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hy.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://sq.muxihuayi.cn

[D04] 删除元素
来源：http://zp.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hc.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jz.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nl.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://ob.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nn.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cz.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bk.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://po.huixiangedu.cn

[D05] 访问与修改元素
来源：http://cd.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rp.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yg.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sx.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://fk.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://nk.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://hm.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yt.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kp.shxzukj.cn

[D06] 数组长度
来源：http://pl.wgjwhj.cn

Py:   len(arr)
来源：http://rm.huixiangedu.cn

PHP:  count($arr);
来源：http://pg.asd995.cn

JS:   arr.length
来源：http://ql.jianghongdianzi.cn

TS:   arr.length
来源：http://ri.nicolike.cn


<!-- 参考信息 -->