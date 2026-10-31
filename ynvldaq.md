代发 wailian999

[B05] 遍历数组 / 列表
来源：http://kh.huanxung.cn

Py:   for item in arr: print(item)
来源：http://uw.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mu.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jg.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zn.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pn.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qo.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://ka.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://br.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://wn.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hs.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ov.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ae.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gg.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wz.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qe.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wk.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sk.bookmarksfly.cn

[B07] while 循环
来源：http://yz.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://oy.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nb.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://xu.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://al.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://qy.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oa.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://to.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://oo.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://vd.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://py.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ug.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://up.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://as.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://va.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iu.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://si.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://jp.wgjwhj.cn

[B09] break 与 continue
来源：http://qf.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zf.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sc.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tx.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://km.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ff.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jm.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uo.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fn.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://bi.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yy.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tx.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nj.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dp.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zb.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vb.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xo.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iy.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://oo.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://yy.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://mk.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zv.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pw.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ya.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://np.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://ph.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://df.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://sy.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iv.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lg.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cf.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lf.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qp.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lm.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://my.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oi.nszjky.cn

[B13] 判断是否为数字
来源：http://ry.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://ek.huanxung.cn

PHP:  is_numeric($x)
来源：http://gd.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sk.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yp.shtwfgs.cn

Java: x instanceof Number
来源：http://jh.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vq.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://vm.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://sp.nicolike.cn

[B14] 判断值是否在集合内
来源：http://vu.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yh.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zj.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://md.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ih.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ur.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://we.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tw.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ai.shxzukj.cn

[B15] 布尔运算与取反
来源：http://mm.bookmarksfly.cn

Py:   a and b or not c
来源：http://lv.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://ii.chemitech.net.cn

JS:   a && b || !c
来源：http://dp.asd995.cn

TS:   a && b || !c
来源：http://xz.colortex.cn

Java: a && b || !c
来源：http://mi.nszjky.cn

Go:   a && b || !c
来源：http://ay.521024.cn

Ruby: a && b || !c
来源：http://wm.yuexingan06.cn

C#:   a && b || !c
来源：http://dl.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gi.haigaiapp.cn

Py:   if not data: return
来源：http://qw.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://du.szxytkj.cn

JS:   if (!data) return;
来源：http://if.wgjwhj.cn

TS:   if (!data) return;
来源：http://qz.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://bx.521024.cn

Go:   if data == nil { return }
来源：http://gs.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://pq.muxihuayi.cn

C#:   if (data == null) return;
来源：http://qe.9csxet.cn

================================================================================
来源：http://fb.shtwfgs.cn

C. 函数与作用域
来源：http://qq.yuexingan06.cn

================================================================================
来源：http://zd.yuexingan06.cn

[C01] 定义函数
来源：http://zq.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://ra.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cn.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://wp.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ew.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xb.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oa.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://wa.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ey.wgjwhj.cn

[C02] 默认参数
来源：http://mw.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://hx.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mj.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://lv.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zj.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qh.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xm.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://bx.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://gk.huixiangedu.cn

[C03] 可变参数
来源：http://sq.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://jn.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zg.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qg.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://be.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://de.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tu.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oc.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yd.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://qk.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bb.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ub.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uv.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dz.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://hv.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://zk.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://au.521024.cn

C#:   f(a: 1, b: 2)
来源：http://pr.panjiajie.cn

[C05] 返回多个值
来源：http://km.huanxung.cn

Py:   return a, b
来源：http://zs.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://wp.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gf.newstarts.cn

TS:   return { a, b };
来源：http://jx.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kk.lnxyls.cn

Go:   return a, b
来源：http://yy.yuntaijiaju.cn

Ruby: return a, b
来源：http://tt.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://nh.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://tf.huanxung.cn

Py:   square = lambda x: x * x
来源：http://qd.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yg.shxzukj.cn

JS:   const square = x => x * x;
来源：http://fy.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://qs.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cv.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ne.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://gg.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pt.hahajie.cn

[C07] 把函数作为参数传入
来源：http://jk.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ks.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dx.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://in.yuexingan06.cn

TS:   arr.map(String)
来源：http://ux.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ug.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kz.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://mb.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lh.newstarts.cn

[C08] 闭包
来源：http://uh.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gg.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://os.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ul.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tl.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ro.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sw.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sw.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vu.jctech888.com.cn

[C09] 递归
来源：http://vp.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mg.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nq.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ax.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yv.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xx.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://va.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pd.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dp.panjiajie.cn

[C10] 变量作用域
来源：http://ws.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wp.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xk.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wy.521024.cn

TS:   同 JS
来源：http://ix.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://rj.bjjhwx.cn

Go:   花括号块级作用域
来源：http://wz.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://up.jctech888.com.cn

C#:   块级作用域
来源：http://ga.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://so.shtwfgs.cn

Py:   from module import func
来源：http://sa.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cc.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wh.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ch.huixiangedu.cn

Java: import java.util.List;
来源：http://yy.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sy.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://iu.asd995.cn

C#:   using System.Text;
来源：http://sa.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://ix.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://ki.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://es.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://if.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://uz.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ly.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://kx.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://qo.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bh.521024.cn

[C13] 类型声明 / 类型注解
来源：http://vu.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hf.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hc.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sh.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cx.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wk.9csxet.cn

Go:   func add(a, b int) int
来源：http://gb.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ry.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cb.huixiangedu.cn

[C14] 泛型函数
来源：http://ng.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sf.wgjwhj.cn

PHP:  // 无泛型
来源：http://yl.shxzukj.cn

JS:   // 无泛型
来源：http://as.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mr.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zt.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ga.hnjuh.cn

Ruby: # 无泛型
来源：http://hx.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cw.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://sf.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ox.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://jt.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hx.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ww.panjiajie.cn

Java: // 无解构
来源：http://cr.huixiangedu.cn

Go:   // 无解构
来源：http://av.lnxyls.cn

Ruby: a, b = pair
来源：http://qr.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://uc.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://bl.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ij.huixiangedu.cn

PHP:  // 无重载
来源：http://nq.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wy.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://gw.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sd.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://no.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://tx.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oh.colortex.cn

================================================================================
来源：http://yi.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://fe.wgjwhj.cn

================================================================================
来源：http://os.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://qo.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bs.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fz.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nd.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rb.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jk.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://qj.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://pg.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://la.hahajie.cn

[D02] 追加元素到末尾
来源：http://gm.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bi.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yx.yuexingan06.cn

JS:   arr.push(4);
来源：http://fk.shtwfgs.cn

TS:   arr.push(4);
来源：http://ck.yuexingan06.cn

Java: list.add(4);
来源：http://my.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://zx.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://sd.9csxet.cn

C#:   list.Add(4);
来源：http://wv.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://dv.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://zm.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://te.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tb.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://aj.colortex.cn

Java: list.add(0, 0);
来源：http://os.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tx.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://au.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://wn.521024.cn

[D04] 删除元素
来源：http://gx.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://us.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bf.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://we.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://km.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tq.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://om.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tv.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lv.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://ez.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gx.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fo.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yc.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://hb.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://da.jctech888.com.cn


<!-- 参考信息 -->