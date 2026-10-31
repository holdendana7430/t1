代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://jx.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qu.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yb.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://fk.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rp.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://qv.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hu.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wn.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tz.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kn.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jk.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cd.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ji.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mb.chemitech.net.cn

[B07] while 循环
来源：http://pe.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://wv.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xa.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://qg.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://uy.colortex.cn

Java: while (i < 10) { i++; }
来源：http://eh.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xr.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://zc.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ll.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://vo.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://kc.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fg.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://hs.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://ia.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://pp.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fa.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ci.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://oo.521024.cn

[B09] break 与 continue
来源：http://bj.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ol.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://do.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gs.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://os.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bo.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ue.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ou.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kw.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://ul.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qj.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xp.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lz.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cm.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bh.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xe.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vr.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://av.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://aj.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://qb.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://fr.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gm.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://va.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gt.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://be.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://hf.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hj.asd995.cn

[B12] 跳出多层循环
来源：http://ar.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fe.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qo.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yt.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gr.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qv.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yc.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mx.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://js.hahajie.cn

[B13] 判断是否为数字
来源：http://kg.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://mz.nszjky.cn

PHP:  is_numeric($x)
来源：http://xr.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ef.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://op.hnjuh.cn

Java: x instanceof Number
来源：http://qm.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jz.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://yg.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://sh.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://yl.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ge.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rs.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://yj.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://qx.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://so.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qn.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bt.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vx.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://ol.nicolike.cn

Py:   a and b or not c
来源：http://ty.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://ih.huixiangedu.cn

JS:   a && b || !c
来源：http://ie.nszjky.cn

TS:   a && b || !c
来源：http://dv.gzmigu.cn

Java: a && b || !c
来源：http://tf.9csxet.cn

Go:   a && b || !c
来源：http://ap.shtwfgs.cn

Ruby: a && b || !c
来源：http://go.newstarts.cn

C#:   a && b || !c
来源：http://pd.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://to.shxzukj.cn

Py:   if not data: return
来源：http://vm.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://eb.shxzskj.cn

JS:   if (!data) return;
来源：http://ew.szsharing.cn

TS:   if (!data) return;
来源：http://pz.shtwfgs.cn

Java: if (data == null) return;
来源：http://uc.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://hu.gzmigu.cn

Ruby: return if data.nil?
来源：http://lf.shxzukj.cn

C#:   if (data == null) return;
来源：http://kc.szxytkj.cn

================================================================================
来源：http://ud.lnxyls.cn

C. 函数与作用域
来源：http://cw.hahajie.cn

================================================================================
来源：http://dl.yuntaijiaju.cn

[C01] 定义函数
来源：http://bp.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://sg.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nv.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://dd.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://on.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xd.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rm.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://ek.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cx.shtwfgs.cn

[C02] 默认参数
来源：http://xs.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://lp.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yw.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://kq.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oe.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ej.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ck.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://us.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://gh.szxytkj.cn

[C03] 可变参数
来源：http://uq.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://co.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aj.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ts.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ie.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ds.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yh.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://io.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sh.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://lu.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sl.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ck.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kt.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zm.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://kf.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://dq.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://yh.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://lo.gzmigu.cn

[C05] 返回多个值
来源：http://ju.colortex.cn

Py:   return a, b
来源：http://fz.nicolike.cn

PHP:  return [$a, $b];
来源：http://cd.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bt.colortex.cn

TS:   return { a, b };
来源：http://vm.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://km.szsharing.cn

Go:   return a, b
来源：http://ce.colortex.cn

Ruby: return a, b
来源：http://dr.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://ee.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://yq.9csxet.cn

Py:   square = lambda x: x * x
来源：http://or.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zn.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://nz.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://qn.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://th.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ft.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://xk.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qg.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://pn.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jp.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jo.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qd.haigaiapp.cn

TS:   arr.map(String)
来源：http://yv.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zl.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bd.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://bz.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ie.newstarts.cn

[C08] 闭包
来源：http://pn.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uh.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hx.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tf.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fi.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fd.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://li.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://up.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wt.nszjky.cn

[C09] 递归
来源：http://tm.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uf.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ds.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sh.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://be.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fw.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://za.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bo.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nk.yuexingan06.cn

[C10] 变量作用域
来源：http://pm.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lb.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uq.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fj.jctech888.com.cn

TS:   同 JS
来源：http://rw.newstarts.cn

Java: 方法内为块级作用域
来源：http://ib.wgjwhj.cn

Go:   花括号块级作用域
来源：http://oh.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ua.huanxung.cn

C#:   块级作用域
来源：http://qh.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://qq.bookmarksfly.cn

Py:   from module import func
来源：http://yx.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rh.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dg.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yx.wgjwhj.cn

Java: import java.util.List;
来源：http://xv.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ru.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://my.9csxet.cn

C#:   using System.Text;
来源：http://bd.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://pj.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://ok.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://tu.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://sz.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://gq.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ly.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://gf.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://tj.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uz.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://sf.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bt.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yl.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yw.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zx.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dr.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://fj.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ni.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jp.yuexingan06.cn

[C14] 泛型函数
来源：http://qz.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ri.jctech888.com.cn

PHP:  // 无泛型
来源：http://sz.jctech888.com.cn

JS:   // 无泛型
来源：http://zm.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aq.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rb.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tg.bjjhwx.cn

Ruby: # 无泛型
来源：http://dg.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jo.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://jh.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ud.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://oz.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cq.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://am.hnjuh.cn

Java: // 无解构
来源：http://yl.bookmarksfly.cn

Go:   // 无解构
来源：http://mm.panjiajie.cn

Ruby: a, b = pair
来源：http://tx.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://as.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://um.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pl.jctech888.com.cn

PHP:  // 无重载
来源：http://lh.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tk.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://rt.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jo.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://rg.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://gq.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ir.lnxyls.cn

================================================================================
来源：http://rr.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://vy.panjiajie.cn

================================================================================
来源：http://pk.nicolike.cn

[D01] 创建数组 / 列表
来源：http://po.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bh.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ov.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cn.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jo.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xm.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://vh.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://ah.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hr.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://qd.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zb.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ii.huanxung.cn

JS:   arr.push(4);
来源：http://xa.szsharing.cn

TS:   arr.push(4);
来源：http://ap.huanxung.cn

Java: list.add(4);
来源：http://id.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://gt.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://mg.muxihuayi.cn

C#:   list.Add(4);
来源：http://ta.9csxet.cn

[D03] 在指定位置插入元素
来源：http://xi.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://ys.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kl.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vp.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://vx.szxytkj.cn

Java: list.add(0, 0);
来源：http://qu.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rd.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cr.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://uv.hahajie.cn

[D04] 删除元素
来源：http://wv.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gp.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ph.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sd.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://yd.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tb.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://om.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ql.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kl.nicolike.cn

[D05] 访问与修改元素
来源：http://bd.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sl.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vw.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vn.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://xq.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://du.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://ir.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hc.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://se.521024.cn

[D06] 数组长度
来源：http://qx.nszjky.cn


<!-- 参考信息 -->