代发 wailian999

[B05] 遍历数组 / 列表
来源：http://fo.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://jx.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fs.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ol.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zw.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nq.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nu.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://ot.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ly.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://ld.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zy.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mq.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dj.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zg.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dz.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://co.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pb.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nt.szsharing.cn

[B07] while 循环
来源：http://ov.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://jv.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gy.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://ib.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://ec.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://ad.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pn.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://mt.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://uq.521024.cn

[B08] do-while（至少执行一次）
来源：http://wo.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://li.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rg.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://ek.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://ju.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://op.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tx.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dk.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://nc.nicolike.cn

[B09] break 与 continue
来源：http://oy.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ie.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rj.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://em.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://po.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yb.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jv.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kc.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gi.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://gf.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vr.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yq.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kv.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cb.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ca.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lh.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yt.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mz.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://pe.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://my.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://pm.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gm.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pl.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bq.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bq.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://wn.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://te.hnjuh.cn

[B12] 跳出多层循环
来源：http://qn.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://av.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oq.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dp.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wr.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ra.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qk.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uy.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qb.nszjky.cn

[B13] 判断是否为数字
来源：http://hu.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://ot.panjiajie.cn

PHP:  is_numeric($x)
来源：http://je.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hx.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sp.hnjuh.cn

Java: x instanceof Number
来源：http://lj.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zq.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://yb.shxzukj.cn

C#:   x is int or double or decimal
来源：http://ya.nicolike.cn

[B14] 判断值是否在集合内
来源：http://kq.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://la.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bf.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://gh.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ti.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fi.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yv.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dj.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sk.hnjuh.cn

[B15] 布尔运算与取反
来源：http://yf.shxzskj.cn

Py:   a and b or not c
来源：http://il.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://eg.colortex.cn

JS:   a && b || !c
来源：http://kd.panjiajie.cn

TS:   a && b || !c
来源：http://te.9csxet.cn

Java: a && b || !c
来源：http://xt.bookmarksfly.cn

Go:   a && b || !c
来源：http://ti.panjiajie.cn

Ruby: a && b || !c
来源：http://sd.shtwfgs.cn

C#:   a && b || !c
来源：http://al.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fb.haigaiapp.cn

Py:   if not data: return
来源：http://nt.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://sv.asd995.cn

JS:   if (!data) return;
来源：http://ta.szsharing.cn

TS:   if (!data) return;
来源：http://bf.newstarts.cn

Java: if (data == null) return;
来源：http://xl.shtwfgs.cn

Go:   if data == nil { return }
来源：http://xh.yuexingan06.cn

Ruby: return if data.nil?
来源：http://zq.haigaiapp.cn

C#:   if (data == null) return;
来源：http://kz.colortex.cn

================================================================================
来源：http://ak.panjiajie.cn

C. 函数与作用域
来源：http://ug.nicolike.cn

================================================================================
来源：http://au.hnjuh.cn

[C01] 定义函数
来源：http://yl.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://rq.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pl.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://xj.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pw.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vl.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fx.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://tf.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ej.nszjky.cn

[C02] 默认参数
来源：http://fe.521024.cn

Py:   def greet(name="World"): return name
来源：http://ii.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bi.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://qw.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mf.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vk.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ng.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://ve.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://zs.chemitech.net.cn

[C03] 可变参数
来源：http://ap.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://da.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://or.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lp.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kn.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kx.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://on.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ex.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ey.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://vz.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://re.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xs.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ps.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yo.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://np.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://bz.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://vq.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://lz.hahajie.cn

[C05] 返回多个值
来源：http://ya.huixinmuqiang.cn

Py:   return a, b
来源：http://br.hahajie.cn

PHP:  return [$a, $b];
来源：http://ul.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gg.nicolike.cn

TS:   return { a, b };
来源：http://kk.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cb.haigaiapp.cn

Go:   return a, b
来源：http://nh.shtwfgs.cn

Ruby: return a, b
来源：http://xp.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://yn.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://xe.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://li.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gc.521024.cn

JS:   const square = x => x * x;
来源：http://oc.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ev.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://em.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eu.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://cb.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mk.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://am.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ry.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ox.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ka.nszjky.cn

TS:   arr.map(String)
来源：http://ye.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jz.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://td.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://wf.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ip.nicolike.cn

[C08] 闭包
来源：http://qw.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rh.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vs.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://in.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mv.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uh.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xs.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ed.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pl.muxihuayi.cn

[C09] 递归
来源：http://gn.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lw.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ag.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ic.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oa.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mi.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ou.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xg.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hd.lnxyls.cn

[C10] 变量作用域
来源：http://rb.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xu.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fg.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tc.wgjwhj.cn

TS:   同 JS
来源：http://wt.szxytkj.cn

Java: 方法内为块级作用域
来源：http://eg.521024.cn

Go:   花括号块级作用域
来源：http://yo.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cs.jianghongdianzi.cn

C#:   块级作用域
来源：http://uy.muxihuayi.cn

[C11] 模块导入与导出
来源：http://ij.yuexingan06.cn

Py:   from module import func
来源：http://ju.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xk.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vw.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://za.lnxyls.cn

Java: import java.util.List;
来源：http://wh.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rz.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://na.newstarts.cn

C#:   using System.Text;
来源：http://zv.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://fs.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://iu.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://mq.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://bi.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://wf.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bl.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://oi.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://ca.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tu.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://mh.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zi.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://db.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ge.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xi.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pf.hnjuh.cn

Go:   func add(a, b int) int
来源：http://lb.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mx.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lg.szsharing.cn

[C14] 泛型函数
来源：http://ke.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bp.chemitech.net.cn

PHP:  // 无泛型
来源：http://ev.jianghongdianzi.cn

JS:   // 无泛型
来源：http://mx.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zl.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rn.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ee.nicolike.cn

Ruby: # 无泛型
来源：http://fg.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gr.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://jt.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xz.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://vk.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ao.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dw.muxihuayi.cn

Java: // 无解构
来源：http://vp.lnxyls.cn

Go:   // 无解构
来源：http://ph.szxytkj.cn

Ruby: a, b = pair
来源：http://rt.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://kq.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://me.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yq.jianghongdianzi.cn

PHP:  // 无重载
来源：http://cq.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vi.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://ud.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xf.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://cj.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://ba.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zc.jctech888.com.cn

================================================================================
来源：http://bh.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://pw.shxzukj.cn

================================================================================
来源：http://kj.szsharing.cn

[D01] 创建数组 / 列表
来源：http://xm.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cl.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vf.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wo.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cx.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jn.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://hj.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://zu.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://al.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://qh.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yt.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gc.shxzskj.cn

JS:   arr.push(4);
来源：http://rb.bjjhwx.cn

TS:   arr.push(4);
来源：http://ux.nszjky.cn

Java: list.add(4);
来源：http://zg.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://du.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://kz.panjiajie.cn

C#:   list.Add(4);
来源：http://yl.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://io.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://su.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lz.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sc.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://cl.wgjwhj.cn

Java: list.add(0, 0);
来源：http://jx.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qf.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ei.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://ay.yuexingan06.cn

[D04] 删除元素
来源：http://vo.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hn.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xk.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kq.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://mj.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sd.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dn.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dc.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qx.muxihuayi.cn

[D05] 访问与修改元素
来源：http://kv.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jz.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mg.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vz.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://qn.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://wx.yuntaijiaju.cn


<!-- 参考信息 -->