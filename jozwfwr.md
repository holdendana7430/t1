代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fk.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://ft.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gr.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tp.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mm.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gc.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sd.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cb.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rs.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gw.shtwfgs.cn

[B07] while 循环
来源：http://of.newstarts.cn

Py:   while i < 10: i += 1
来源：http://vg.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pm.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://fl.521024.cn

TS:   while (i < 10) { i++; }
来源：http://km.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://uj.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pl.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://cd.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://ol.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://xk.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://kv.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yw.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://iu.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://hg.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://xp.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rz.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kw.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://jb.hahajie.cn

[B09] break 与 continue
来源：http://gb.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://va.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://id.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mq.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jb.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vp.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qi.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xn.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yw.colortex.cn

[B10] 遍历同时拿索引
来源：http://yl.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rj.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zx.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rr.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ae.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lx.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gi.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sz.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lq.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://se.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://fg.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://kr.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tg.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qb.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vl.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://jp.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://no.asd995.cn

[B12] 跳出多层循环
来源：http://lc.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://od.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vi.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ih.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pr.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tz.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rt.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qu.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wp.szsharing.cn

[B13] 判断是否为数字
来源：http://mr.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://tg.shxzskj.cn

PHP:  is_numeric($x)
来源：http://sm.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oi.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rg.yuntaijiaju.cn

Java: x instanceof Number
来源：http://rz.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ol.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://wz.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://ne.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://do.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://li.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ti.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://ol.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://qg.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gs.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dw.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fp.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nv.9csxet.cn

[B15] 布尔运算与取反
来源：http://om.wgjwhj.cn

Py:   a and b or not c
来源：http://vo.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://bi.nszjky.cn

JS:   a && b || !c
来源：http://ba.shxzskj.cn

TS:   a && b || !c
来源：http://qd.nicolike.cn

Java: a && b || !c
来源：http://xw.huixinmuqiang.cn

Go:   a && b || !c
来源：http://tz.newstarts.cn

Ruby: a && b || !c
来源：http://ko.chemitech.net.cn

C#:   a && b || !c
来源：http://ry.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gz.nszjky.cn

Py:   if not data: return
来源：http://mi.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://pc.nszjky.cn

JS:   if (!data) return;
来源：http://dc.shxzukj.cn

TS:   if (!data) return;
来源：http://yt.wgjwhj.cn

Java: if (data == null) return;
来源：http://da.shxzskj.cn

Go:   if data == nil { return }
来源：http://tr.szxytkj.cn

Ruby: return if data.nil?
来源：http://lq.hahajie.cn

C#:   if (data == null) return;
来源：http://fd.wgjwhj.cn

================================================================================
来源：http://wf.shxzukj.cn

C. 函数与作用域
来源：http://vn.shxzskj.cn

================================================================================
来源：http://ij.hahajie.cn

[C01] 定义函数
来源：http://um.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://tm.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ce.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://xf.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://md.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hd.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bb.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://lk.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cr.nicolike.cn

[C02] 默认参数
来源：http://qn.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ap.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ii.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://lj.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ok.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fg.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://os.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://zm.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://mn.szsharing.cn

[C03] 可变参数
来源：http://bb.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://el.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ii.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fy.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jb.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tb.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dg.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bq.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ng.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://qv.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pb.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hg.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yf.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tn.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://io.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://rz.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://ri.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://ul.newstarts.cn

[C05] 返回多个值
来源：http://ce.lnxyls.cn

Py:   return a, b
来源：http://ol.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://zl.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rk.bjjhwx.cn

TS:   return { a, b };
来源：http://at.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ex.asd995.cn

Go:   return a, b
来源：http://pc.huixiangedu.cn

Ruby: return a, b
来源：http://ll.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://ru.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://dy.nszjky.cn

Py:   square = lambda x: x * x
来源：http://he.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bn.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://hu.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://kq.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zr.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mn.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://jk.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gj.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://qz.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kf.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://es.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fz.wgjwhj.cn

TS:   arr.map(String)
来源：http://mn.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gg.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cv.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://vx.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xe.szxytkj.cn

[C08] 闭包
来源：http://bu.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uy.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nn.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qk.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jt.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cz.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yp.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qu.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tq.jctech888.com.cn

[C09] 递归
来源：http://hi.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vn.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vn.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fp.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dw.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sz.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xi.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://da.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rm.yuexingan06.cn

[C10] 变量作用域
来源：http://tm.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mx.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cd.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ax.9csxet.cn

TS:   同 JS
来源：http://ef.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ip.lnxyls.cn

Go:   花括号块级作用域
来源：http://tu.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wi.huanxung.cn

C#:   块级作用域
来源：http://xr.szxytkj.cn

[C11] 模块导入与导出
来源：http://dv.shxzukj.cn

Py:   from module import func
来源：http://np.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uz.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ms.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hs.huanxung.cn

Java: import java.util.List;
来源：http://ns.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hh.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://kc.huixinmuqiang.cn

C#:   using System.Text;
来源：http://kx.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://ig.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://lf.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://kl.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://hn.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://qv.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tz.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://eb.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://rg.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://aj.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://ur.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://po.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sa.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pl.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://la.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pl.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://at.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zt.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zz.nszjky.cn

[C14] 泛型函数
来源：http://xb.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tx.yuexingan06.cn

PHP:  // 无泛型
来源：http://sd.huixinmuqiang.cn

JS:   // 无泛型
来源：http://pw.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qd.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vu.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wu.yuexingan06.cn

Ruby: # 无泛型
来源：http://lg.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eo.huanxung.cn

[C15] 解构 / 展开参数
来源：http://qy.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mm.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://zc.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qh.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rc.9csxet.cn

Java: // 无解构
来源：http://rh.chemitech.net.cn

Go:   // 无解构
来源：http://wh.lnxyls.cn

Ruby: a, b = pair
来源：http://js.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://sy.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://bh.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xl.jianghongdianzi.cn

PHP:  // 无重载
来源：http://nb.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://co.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://at.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wg.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://ic.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://cs.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fg.yuntaijiaju.cn

================================================================================
来源：http://rf.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://re.colortex.cn

================================================================================
来源：http://do.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://br.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lo.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xu.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fk.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bz.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ox.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://qw.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://hv.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gv.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://wm.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://li.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yg.wgjwhj.cn

JS:   arr.push(4);
来源：http://go.bookmarksfly.cn

TS:   arr.push(4);
来源：http://ag.jctech888.com.cn

Java: list.add(4);
来源：http://xk.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://ui.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://it.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://yp.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://vl.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://xm.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lb.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fh.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://di.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://lx.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iz.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://py.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://xw.nszjky.cn

[D04] 删除元素
来源：http://od.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ud.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vj.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kt.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://no.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bb.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fn.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kc.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pv.newstarts.cn

[D05] 访问与修改元素
来源：http://dm.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lh.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iv.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gl.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://zl.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://uu.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://zn.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fh.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ta.bjjhwx.cn

[D06] 数组长度
来源：http://dr.bookmarksfly.cn

Py:   len(arr)
来源：http://ab.shtwfgs.cn

PHP:  count($arr);
来源：http://nb.521024.cn

JS:   arr.length
来源：http://kj.nszjky.cn

TS:   arr.length
来源：http://qa.hahajie.cn


<!-- 参考信息 -->