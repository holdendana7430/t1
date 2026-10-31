代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://wf.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jr.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kh.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://zd.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iy.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://zr.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zm.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sg.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ve.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nk.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jb.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vg.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qi.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lj.szsharing.cn

[B07] while 循环
来源：http://ms.hahajie.cn

Py:   while i < 10: i += 1
来源：http://pn.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://su.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://eo.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://ft.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://ko.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ou.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://xe.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://rj.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://iw.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://tu.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cj.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://jg.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://sz.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://xc.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uu.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sd.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://dn.panjiajie.cn

[B09] break 与 continue
来源：http://ep.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://in.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ys.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tt.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wg.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ye.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mq.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gt.nszjky.cn

[B10] 遍历同时拿索引
来源：http://uo.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bh.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lt.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wn.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jx.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ot.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://he.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rn.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ic.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://af.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://gv.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://bo.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jv.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wl.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gs.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nc.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://jk.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lu.hnjuh.cn

[B12] 跳出多层循环
来源：http://ke.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xw.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qe.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xs.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ra.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jt.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hi.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ur.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ix.521024.cn

[B13] 判断是否为数字
来源：http://it.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://gv.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://lc.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ud.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uc.huanxung.cn

Java: x instanceof Number
来源：http://sy.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bp.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://pw.hahajie.cn

C#:   x is int or double or decimal
来源：http://uj.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://cv.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tz.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gl.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://gz.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://ry.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tk.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gl.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cz.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rk.asd995.cn

[B15] 布尔运算与取反
来源：http://af.muxihuayi.cn

Py:   a and b or not c
来源：http://jv.huanxung.cn

PHP:  $a && $b || !$c
来源：http://ze.nicolike.cn

JS:   a && b || !c
来源：http://fg.haigaiapp.cn

TS:   a && b || !c
来源：http://cp.jctech888.com.cn

Java: a && b || !c
来源：http://km.bookmarksfly.cn

Go:   a && b || !c
来源：http://ld.nszjky.cn

Ruby: a && b || !c
来源：http://ng.shxzskj.cn

C#:   a && b || !c
来源：http://fk.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jq.muxihuayi.cn

Py:   if not data: return
来源：http://ac.colortex.cn

PHP:  if (!$data) { return; }
来源：http://hn.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://oa.gzmigu.cn

TS:   if (!data) return;
来源：http://ek.colortex.cn

Java: if (data == null) return;
来源：http://cl.haigaiapp.cn

Go:   if data == nil { return }
来源：http://gv.9csxet.cn

Ruby: return if data.nil?
来源：http://ip.newstarts.cn

C#:   if (data == null) return;
来源：http://oh.bookmarksfly.cn

================================================================================
来源：http://vl.hnjuh.cn

C. 函数与作用域
来源：http://le.nicolike.cn

================================================================================
来源：http://rk.huanxung.cn

[C01] 定义函数
来源：http://hk.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://un.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lr.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://my.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://el.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qt.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kb.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://wd.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ym.nicolike.cn

[C02] 默认参数
来源：http://zo.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://yk.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gv.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://fw.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nl.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ik.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ks.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://gg.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://vz.muxihuayi.cn

[C03] 可变参数
来源：http://yv.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://cv.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rc.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zv.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cn.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zw.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wc.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mm.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://ux.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fe.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yp.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uu.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hh.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://qv.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://sf.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://lj.521024.cn

C#:   f(a: 1, b: 2)
来源：http://ve.szxytkj.cn

[C05] 返回多个值
来源：http://nz.szxytkj.cn

Py:   return a, b
来源：http://ws.hnjuh.cn

PHP:  return [$a, $b];
来源：http://so.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ta.9csxet.cn

TS:   return { a, b };
来源：http://pz.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://as.chemitech.net.cn

Go:   return a, b
来源：http://lk.szsharing.cn

Ruby: return a, b
来源：http://eb.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://yf.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://cl.szsharing.cn

Py:   square = lambda x: x * x
来源：http://dq.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ef.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://jq.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://uz.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ni.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://en.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://rd.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zz.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://jd.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xu.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ov.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://up.jctech888.com.cn

TS:   arr.map(String)
来源：http://kg.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sq.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hp.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://gw.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cd.bjjhwx.cn

[C08] 闭包
来源：http://oc.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gb.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zj.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cj.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dr.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oq.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fp.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tp.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ob.szsharing.cn

[C09] 递归
来源：http://vy.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ar.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jd.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gk.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ab.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fx.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mi.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nr.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fn.asd995.cn

[C10] 变量作用域
来源：http://az.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nw.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sl.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tv.shtwfgs.cn

TS:   同 JS
来源：http://ab.szxytkj.cn

Java: 方法内为块级作用域
来源：http://jr.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://hk.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zs.szxytkj.cn

C#:   块级作用域
来源：http://oj.bjjhwx.cn

[C11] 模块导入与导出
来源：http://ce.colortex.cn

Py:   from module import func
来源：http://ah.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://de.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yg.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fu.szsharing.cn

Java: import java.util.List;
来源：http://cq.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pr.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://rp.yuexingan06.cn

C#:   using System.Text;
来源：http://yh.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://fk.colortex.cn

Py:   (lambda: print("run"))()
来源：http://hk.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://jp.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://fs.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://vf.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rb.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://vr.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://ii.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gn.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://xq.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jk.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eb.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gv.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zs.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mq.521024.cn

Go:   func add(a, b int) int
来源：http://ey.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gr.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ij.yuexingan06.cn

[C14] 泛型函数
来源：http://wh.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eo.huixiangedu.cn

PHP:  // 无泛型
来源：http://dn.nszjky.cn

JS:   // 无泛型
来源：http://tk.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://to.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dp.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kx.hnjuh.cn

Ruby: # 无泛型
来源：http://xi.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pf.nicolike.cn

[C15] 解构 / 展开参数
来源：http://qg.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lc.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://ax.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mj.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yf.panjiajie.cn

Java: // 无解构
来源：http://li.hahajie.cn

Go:   // 无解构
来源：http://as.hahajie.cn

Ruby: a, b = pair
来源：http://lw.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://yn.nicolike.cn

[C16] 函数 / 方法重载
来源：http://fl.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ct.hahajie.cn

PHP:  // 无重载
来源：http://xh.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yi.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ue.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tj.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://ec.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://zj.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fi.szxytkj.cn

================================================================================
来源：http://oj.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://aw.wgjwhj.cn

================================================================================
来源：http://jn.hahajie.cn

[D01] 创建数组 / 列表
来源：http://vg.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sh.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://os.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jg.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://up.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fe.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://eh.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://fp.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kg.shxzukj.cn

[D02] 追加元素到末尾
来源：http://hr.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ae.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://df.521024.cn

JS:   arr.push(4);
来源：http://do.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://ot.chemitech.net.cn

Java: list.add(4);
来源：http://td.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://vl.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://lj.haigaiapp.cn

C#:   list.Add(4);
来源：http://hy.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://na.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://ms.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ww.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rq.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://ro.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://xz.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qt.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vr.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://pa.bjjhwx.cn

[D04] 删除元素
来源：http://kf.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gj.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://on.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://sj.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zm.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qy.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://la.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ba.nszjky.cn

[D05] 访问与修改元素
来源：http://mv.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sx.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tv.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lr.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://ol.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://sc.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ug.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nm.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fc.bookmarksfly.cn

[D06] 数组长度
来源：http://ak.hnjuh.cn


<!-- 参考信息 -->