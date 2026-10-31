代发 wailian999

Py:   for i in range(10): print(i)
来源：http://ki.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nd.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rj.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iq.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hl.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ey.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://qf.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qp.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://vm.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://vh.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eh.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yw.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fy.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cl.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vv.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://st.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lx.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://hs.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pl.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bj.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://em.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zk.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fg.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://np.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://po.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pw.jianghongdianzi.cn

[B07] while 循环
来源：http://yc.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://ky.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cz.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://sj.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://og.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://xh.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wr.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://mu.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://vy.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://fe.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://cr.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yg.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ds.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://wg.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://ba.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sv.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://il.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://ot.yuexingan06.cn

[B09] break 与 continue
来源：http://uo.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xl.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ot.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nz.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yy.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tv.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vd.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fa.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wu.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://vr.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://io.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wq.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jw.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ay.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yk.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dk.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gl.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sh.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://ht.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://of.521024.cn

PHP:  range(0, 10, 2);
来源：http://yn.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xd.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yh.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ku.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zp.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://ft.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pv.hnjuh.cn

[B12] 跳出多层循环
来源：http://gj.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oh.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lh.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pr.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://da.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://je.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kk.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pt.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fn.muxihuayi.cn

[B13] 判断是否为数字
来源：http://hn.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://ww.gzmigu.cn

PHP:  is_numeric($x)
来源：http://vu.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gv.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qv.hnjuh.cn

Java: x instanceof Number
来源：http://wf.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yx.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://uz.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://bi.asd995.cn

[B14] 判断值是否在集合内
来源：http://hq.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kc.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fu.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://rq.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ru.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hv.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vj.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qq.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qu.shxzskj.cn

[B15] 布尔运算与取反
来源：http://jy.hahajie.cn

Py:   a and b or not c
来源：http://ud.colortex.cn

PHP:  $a && $b || !$c
来源：http://gg.szsharing.cn

JS:   a && b || !c
来源：http://lw.asd995.cn

TS:   a && b || !c
来源：http://wj.chemitech.net.cn

Java: a && b || !c
来源：http://ji.shxzskj.cn

Go:   a && b || !c
来源：http://jh.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://mx.szxytkj.cn

C#:   a && b || !c
来源：http://oh.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hi.yuntaijiaju.cn

Py:   if not data: return
来源：http://am.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://ll.nicolike.cn

JS:   if (!data) return;
来源：http://vc.shtwfgs.cn

TS:   if (!data) return;
来源：http://xc.jctech888.com.cn

Java: if (data == null) return;
来源：http://xu.nicolike.cn

Go:   if data == nil { return }
来源：http://mj.huanxung.cn

Ruby: return if data.nil?
来源：http://az.nicolike.cn

C#:   if (data == null) return;
来源：http://to.521024.cn

================================================================================
来源：http://zt.panjiajie.cn

C. 函数与作用域
来源：http://li.shxzukj.cn

================================================================================
来源：http://rg.panjiajie.cn

[C01] 定义函数
来源：http://nt.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://lr.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lt.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://bx.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lk.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jp.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hi.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://fe.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yb.shxzskj.cn

[C02] 默认参数
来源：http://rt.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://gr.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://po.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://ob.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ql.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mo.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dt.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ek.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://ay.gzmigu.cn

[C03] 可变参数
来源：http://no.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://ux.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ai.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yd.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rq.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dn.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tv.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://si.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ed.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://no.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ui.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wy.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dj.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://or.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://dt.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://hn.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://pu.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://cl.hnjuh.cn

[C05] 返回多个值
来源：http://si.bookmarksfly.cn

Py:   return a, b
来源：http://hc.lnxyls.cn

PHP:  return [$a, $b];
来源：http://lk.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ck.bjjhwx.cn

TS:   return { a, b };
来源：http://jx.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gn.521024.cn

Go:   return a, b
来源：http://lf.hahajie.cn

Ruby: return a, b
来源：http://kn.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://so.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://ti.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://ds.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ar.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://pd.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ak.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ir.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mu.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://ki.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://we.huanxung.cn

[C07] 把函数作为参数传入
来源：http://zc.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aj.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wk.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://if.9csxet.cn

TS:   arr.map(String)
来源：http://fy.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fe.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wd.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://az.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wc.gzmigu.cn

[C08] 闭包
来源：http://xf.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bf.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ax.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uo.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xt.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nc.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zt.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hk.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iv.shtwfgs.cn

[C09] 递归
来源：http://kn.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zv.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yx.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wx.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nr.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yq.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pf.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zn.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hm.gzmigu.cn

[C10] 变量作用域
来源：http://cv.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yk.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xv.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hq.hnjuh.cn

TS:   同 JS
来源：http://az.nszjky.cn

Java: 方法内为块级作用域
来源：http://wd.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://lj.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jz.wgjwhj.cn

C#:   块级作用域
来源：http://xq.gzmigu.cn

[C11] 模块导入与导出
来源：http://jp.lnxyls.cn

Py:   from module import func
来源：http://we.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ea.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://id.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gf.wgjwhj.cn

Java: import java.util.List;
来源：http://ge.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zz.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://wt.nszjky.cn

C#:   using System.Text;
来源：http://ov.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://vg.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://fw.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://dl.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://in.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://rc.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ae.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://pm.521024.cn

Ruby: -> { puts "run" }.call
来源：http://im.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uo.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://ja.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fg.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kt.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rr.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ky.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mf.huanxung.cn

Go:   func add(a, b int) int
来源：http://by.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iy.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qy.szsharing.cn

[C14] 泛型函数
来源：http://sz.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://al.yuexingan06.cn

PHP:  // 无泛型
来源：http://td.shtwfgs.cn

JS:   // 无泛型
来源：http://bg.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oc.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zk.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qu.lnxyls.cn

Ruby: # 无泛型
来源：http://oy.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oq.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://ol.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ep.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://yg.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iu.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sp.szxytkj.cn

Java: // 无解构
来源：http://io.huanxung.cn

Go:   // 无解构
来源：http://vf.nicolike.cn

Ruby: a, b = pair
来源：http://og.colortex.cn

C#:   var (a, b) = pair;
来源：http://cq.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://il.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://do.huixinmuqiang.cn

PHP:  // 无重载
来源：http://so.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dg.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://qt.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ti.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://gp.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://pe.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pm.szxytkj.cn

================================================================================
来源：http://jd.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://ey.huixinmuqiang.cn

================================================================================
来源：http://gw.521024.cn

[D01] 创建数组 / 列表
来源：http://nv.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vv.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wq.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://co.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wg.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xb.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://yd.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://ew.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hr.hnjuh.cn

[D02] 追加元素到末尾
来源：http://ur.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sy.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gb.nszjky.cn

JS:   arr.push(4);
来源：http://jq.521024.cn

TS:   arr.push(4);
来源：http://qa.bookmarksfly.cn

Java: list.add(4);
来源：http://wl.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://wb.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://nl.lnxyls.cn

C#:   list.Add(4);
来源：http://hx.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://ug.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://pq.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bl.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jy.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://yp.lnxyls.cn

Java: list.add(0, 0);
来源：http://jx.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ds.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qt.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://tc.gzmigu.cn

[D04] 删除元素
来源：http://aj.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jn.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uh.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gd.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://bk.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kr.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ec.shxzskj.cn


<!-- 参考信息 -->