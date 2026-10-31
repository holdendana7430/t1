代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rr.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lz.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://da.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jx.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://lo.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://ey.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zt.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wi.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gb.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rt.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cm.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://bk.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sw.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://hd.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ke.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ef.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bv.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://it.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tv.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ve.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://co.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iq.muxihuayi.cn

[B07] while 循环
来源：http://zw.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://tj.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wn.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://pc.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://rz.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://xy.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://is.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://kv.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://zb.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://sm.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://ro.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mh.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://xy.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://ii.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://mj.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://au.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lg.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://mf.huixiangedu.cn

[B09] break 与 continue
来源：http://am.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pc.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ky.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rl.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uf.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wv.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zw.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ly.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fg.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://se.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qr.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cj.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bw.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qg.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lc.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ob.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://dd.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://gz.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://wr.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bj.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zy.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://np.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ok.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://dx.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bl.hahajie.cn

[B12] 跳出多层循环
来源：http://uz.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xf.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pw.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uu.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ni.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ym.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yv.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fh.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cu.shxzskj.cn

[B13] 判断是否为数字
来源：http://ur.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://nb.nszjky.cn

PHP:  is_numeric($x)
来源：http://rx.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pm.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zb.huixinmuqiang.cn

Java: x instanceof Number
来源：http://tk.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ui.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://cl.nicolike.cn

C#:   x is int or double or decimal
来源：http://tk.newstarts.cn

[B14] 判断值是否在集合内
来源：http://md.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yx.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dx.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://iq.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://gi.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ln.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wo.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kv.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ya.nszjky.cn

[B15] 布尔运算与取反
来源：http://rn.szsharing.cn

Py:   a and b or not c
来源：http://uf.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://by.chemitech.net.cn

JS:   a && b || !c
来源：http://ls.shxzukj.cn

TS:   a && b || !c
来源：http://fd.muxihuayi.cn

Java: a && b || !c
来源：http://ve.shxzskj.cn

Go:   a && b || !c
来源：http://cw.521024.cn

Ruby: a && b || !c
来源：http://fx.szxytkj.cn

C#:   a && b || !c
来源：http://fn.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jl.521024.cn

Py:   if not data: return
来源：http://zv.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://it.hahajie.cn

JS:   if (!data) return;
来源：http://ko.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://ey.shtwfgs.cn

Java: if (data == null) return;
来源：http://ug.panjiajie.cn

Go:   if data == nil { return }
来源：http://xy.wgjwhj.cn

Ruby: return if data.nil?
来源：http://cv.colortex.cn

C#:   if (data == null) return;
来源：http://em.shtwfgs.cn

================================================================================
来源：http://fu.9csxet.cn

C. 函数与作用域
来源：http://xu.szsharing.cn

================================================================================
来源：http://bg.yuntaijiaju.cn

[C01] 定义函数
来源：http://hz.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://jb.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hx.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://uz.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sn.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bc.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tj.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://pt.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zg.shtwfgs.cn

[C02] 默认参数
来源：http://un.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://ss.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fy.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://hs.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oq.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fo.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wg.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://yi.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://wy.huixiangedu.cn

[C03] 可变参数
来源：http://zm.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://un.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://al.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ur.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jy.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ig.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bj.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dp.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sx.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ti.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rl.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zd.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zr.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dv.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://zo.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://lz.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://lx.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://cx.nicolike.cn

[C05] 返回多个值
来源：http://dz.hnjuh.cn

Py:   return a, b
来源：http://wz.shxzskj.cn

PHP:  return [$a, $b];
来源：http://da.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oj.shxzskj.cn

TS:   return { a, b };
来源：http://rk.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://db.szsharing.cn

Go:   return a, b
来源：http://az.nicolike.cn

Ruby: return a, b
来源：http://dw.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://yg.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://cb.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://hf.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sn.asd995.cn

JS:   const square = x => x * x;
来源：http://it.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://kc.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xw.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qg.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://gu.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oa.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://sb.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yh.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ct.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://to.nszjky.cn

TS:   arr.map(String)
来源：http://em.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bz.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dg.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://sj.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ja.muxihuayi.cn

[C08] 闭包
来源：http://di.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mo.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mv.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ou.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yb.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://te.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://je.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ti.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rl.panjiajie.cn

[C09] 递归
来源：http://fu.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vn.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://el.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rn.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sc.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yn.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iu.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ak.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xq.yuexingan06.cn

[C10] 变量作用域
来源：http://fd.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qm.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jz.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shtwfgs.cn

TS:   同 JS
来源：http://bi.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://gv.9csxet.cn

Go:   花括号块级作用域
来源：http://bg.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tl.nszjky.cn

C#:   块级作用域
来源：http://wo.muxihuayi.cn

[C11] 模块导入与导出
来源：http://yf.521024.cn

Py:   from module import func
来源：http://vt.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rn.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sp.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kw.szxytkj.cn

Java: import java.util.List;
来源：http://zm.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sj.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://nu.asd995.cn

C#:   using System.Text;
来源：http://vx.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://pb.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://ht.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://ir.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://pp.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://ep.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xh.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://wz.521024.cn

Ruby: -> { puts "run" }.call
来源：http://xe.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://km.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://fr.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vf.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pc.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jy.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dx.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pm.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://bx.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hv.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jz.colortex.cn

[C14] 泛型函数
来源：http://em.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zi.shtwfgs.cn

PHP:  // 无泛型
来源：http://lb.shxzskj.cn

JS:   // 无泛型
来源：http://we.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rz.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ts.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wr.haigaiapp.cn

Ruby: # 无泛型
来源：http://dx.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kq.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://nj.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rz.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://zq.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sq.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rn.jianghongdianzi.cn

Java: // 无解构
来源：http://kn.huanxung.cn

Go:   // 无解构
来源：http://bu.huanxung.cn

Ruby: a, b = pair
来源：http://zu.asd995.cn

C#:   var (a, b) = pair;
来源：http://cy.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://yc.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hw.muxihuayi.cn

PHP:  // 无重载
来源：http://nk.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ok.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://nw.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yl.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://sp.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://nu.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://py.yuntaijiaju.cn

================================================================================
来源：http://ll.521024.cn

D. 数组 / 列表 / 集合
来源：http://kw.huixinmuqiang.cn

================================================================================
来源：http://nf.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://xr.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lx.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ok.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://le.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hr.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ag.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://ia.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://kl.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pc.szsharing.cn

[D02] 追加元素到末尾
来源：http://hy.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wf.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pu.hahajie.cn

JS:   arr.push(4);
来源：http://xl.chemitech.net.cn

TS:   arr.push(4);
来源：http://sg.hahajie.cn

Java: list.add(4);
来源：http://te.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://oi.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://ao.gzmigu.cn

C#:   list.Add(4);
来源：http://en.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://mt.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://gk.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rk.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zv.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://uy.yuexingan06.cn

Java: list.add(0, 0);
来源：http://gm.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ix.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sc.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://ib.shxzskj.cn

[D04] 删除元素
来源：http://dh.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gi.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ow.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fi.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://te.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vl.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xo.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vf.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ug.nszjky.cn

[D05] 访问与修改元素
来源：http://rk.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kw.521024.cn


<!-- 参考信息 -->