代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://jn.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cu.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hk.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://ul.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ma.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://qy.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yv.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nx.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yv.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tk.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pc.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vs.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nf.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eg.bjjhwx.cn

[B07] while 循环
来源：http://ui.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://aa.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ge.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://su.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://jk.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://og.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fd.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://ma.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://eu.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://qi.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://rj.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://il.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://pf.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://ad.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://ff.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iz.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uw.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://th.bookmarksfly.cn

[B09] break 与 continue
来源：http://dv.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lu.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cl.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gr.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://az.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ib.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bb.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://di.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ja.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://mx.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://md.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wa.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lj.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fu.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ll.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ag.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ox.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tg.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ib.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://ks.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://ei.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mg.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vv.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mh.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gl.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://zp.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hc.hnjuh.cn

[B12] 跳出多层循环
来源：http://nc.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tt.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lv.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fa.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sl.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sf.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xh.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bc.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xo.panjiajie.cn

[B13] 判断是否为数字
来源：http://hc.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://pa.gzmigu.cn

PHP:  is_numeric($x)
来源：http://jl.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zh.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dy.521024.cn

Java: x instanceof Number
来源：http://fj.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hl.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://ju.521024.cn

C#:   x is int or double or decimal
来源：http://mn.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://bv.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gv.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://id.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://uu.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://cg.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fr.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cn.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kl.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ta.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://dq.yuexingan06.cn

Py:   a and b or not c
来源：http://fl.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://ui.wgjwhj.cn

JS:   a && b || !c
来源：http://vz.jctech888.com.cn

TS:   a && b || !c
来源：http://im.jctech888.com.cn

Java: a && b || !c
来源：http://nb.jianghongdianzi.cn

Go:   a && b || !c
来源：http://tm.wgjwhj.cn

Ruby: a && b || !c
来源：http://ua.wgjwhj.cn

C#:   a && b || !c
来源：http://ju.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ur.nicolike.cn

Py:   if not data: return
来源：http://fn.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://yp.shxzskj.cn

JS:   if (!data) return;
来源：http://ru.panjiajie.cn

TS:   if (!data) return;
来源：http://gd.521024.cn

Java: if (data == null) return;
来源：http://el.521024.cn

Go:   if data == nil { return }
来源：http://yo.jctech888.com.cn

Ruby: return if data.nil?
来源：http://zf.colortex.cn

C#:   if (data == null) return;
来源：http://ne.asd995.cn

================================================================================
来源：http://tl.nszjky.cn

C. 函数与作用域
来源：http://mh.haigaiapp.cn

================================================================================
来源：http://ja.bookmarksfly.cn

[C01] 定义函数
来源：http://yz.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://yt.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cz.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ku.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kz.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://df.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xt.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://rl.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ez.wgjwhj.cn

[C02] 默认参数
来源：http://lp.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://nd.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://is.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://gt.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tu.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://li.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://er.521024.cn

Ruby: def greet(name = "World") = name
来源：http://cr.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://va.wgjwhj.cn

[C03] 可变参数
来源：http://bx.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://km.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mj.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bq.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wm.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ae.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bx.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yo.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fq.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://tb.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wp.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mb.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gl.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ou.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://qe.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://rr.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://tw.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://hv.szsharing.cn

[C05] 返回多个值
来源：http://my.jctech888.com.cn

Py:   return a, b
来源：http://id.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://ha.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kt.lnxyls.cn

TS:   return { a, b };
来源：http://bg.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hi.chemitech.net.cn

Go:   return a, b
来源：http://hv.jianghongdianzi.cn

Ruby: return a, b
来源：http://wz.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://ay.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://qd.asd995.cn

Py:   square = lambda x: x * x
来源：http://fl.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yw.panjiajie.cn

JS:   const square = x => x * x;
来源：http://sm.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://wg.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gb.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qd.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://bs.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vp.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://rb.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mn.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hk.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lh.gzmigu.cn

TS:   arr.map(String)
来源：http://to.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wf.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bt.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://jq.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fs.shtwfgs.cn

[C08] 闭包
来源：http://te.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://if.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ci.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qj.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pd.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eq.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tn.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mi.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://su.szxytkj.cn

[C09] 递归
来源：http://yb.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lb.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wo.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sr.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ii.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iv.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sn.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vk.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iu.hahajie.cn

[C10] 变量作用域
来源：http://ve.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xu.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ws.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://md.wgjwhj.cn

TS:   同 JS
来源：http://mw.9csxet.cn

Java: 方法内为块级作用域
来源：http://fh.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://sm.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sy.asd995.cn

C#:   块级作用域
来源：http://px.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://cl.hnjuh.cn

Py:   from module import func
来源：http://qz.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hx.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uv.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nq.521024.cn

Java: import java.util.List;
来源：http://cm.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dr.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://qn.yuexingan06.cn

C#:   using System.Text;
来源：http://we.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://ys.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://sw.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://ik.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://cb.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://ug.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fb.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://ac.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://bd.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uy.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://mn.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oy.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ev.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ed.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hp.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://av.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://se.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qe.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rd.huixinmuqiang.cn

[C14] 泛型函数
来源：http://xf.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ml.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://lx.colortex.cn

JS:   // 无泛型
来源：http://bw.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tf.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gg.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ew.muxihuayi.cn

Ruby: # 无泛型
来源：http://mw.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://na.asd995.cn

[C15] 解构 / 展开参数
来源：http://kb.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zz.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://sv.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vw.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kl.nszjky.cn

Java: // 无解构
来源：http://kx.9csxet.cn

Go:   // 无解构
来源：http://xq.gzmigu.cn

Ruby: a, b = pair
来源：http://oh.9csxet.cn

C#:   var (a, b) = pair;
来源：http://yw.521024.cn

[C16] 函数 / 方法重载
来源：http://tx.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oc.yuntaijiaju.cn

PHP:  // 无重载
来源：http://ry.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ps.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://el.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://do.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://uu.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://yo.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dj.9csxet.cn

================================================================================
来源：http://sz.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://vy.nszjky.cn

================================================================================
来源：http://hv.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://ty.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hk.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gy.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ah.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pi.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cb.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://pd.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://xx.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ph.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://px.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rd.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wm.haigaiapp.cn

JS:   arr.push(4);
来源：http://yi.jctech888.com.cn

TS:   arr.push(4);
来源：http://gv.jctech888.com.cn

Java: list.add(4);
来源：http://bx.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://ew.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://ct.muxihuayi.cn

C#:   list.Add(4);
来源：http://tr.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://ds.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://bn.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nj.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ze.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://oc.nszjky.cn

Java: list.add(0, 0);
来源：http://zu.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zp.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mt.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://kj.asd995.cn

[D04] 删除元素
来源：http://fs.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ai.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rb.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eu.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://wj.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bo.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pj.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qx.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sf.9csxet.cn

[D05] 访问与修改元素
来源：http://ts.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qr.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lx.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zu.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://ms.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://yv.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://py.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fk.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cb.panjiajie.cn

[D06] 数组长度
来源：http://bt.huixinmuqiang.cn


<!-- 参考信息 -->