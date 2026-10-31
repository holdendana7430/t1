代发 wailian999

[B05] 遍历数组 / 列表
来源：http://ej.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://vb.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zr.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tc.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tr.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ft.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gr.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://dt.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yo.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://si.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fu.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ac.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qm.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xb.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pq.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xl.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ol.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mx.bjjhwx.cn

[B07] while 循环
来源：http://gd.nszjky.cn

Py:   while i < 10: i += 1
来源：http://ke.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://np.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://qk.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://wc.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://vf.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xo.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://hg.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ts.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://ep.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://mt.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ab.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://wi.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://lx.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://tz.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wl.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yb.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://jk.szxytkj.cn

[B09] break 与 continue
来源：http://wh.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zm.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ph.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lj.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wh.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qt.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fr.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lf.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://sm.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mz.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ie.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yx.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xg.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ir.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fs.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xf.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ju.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://xn.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://lv.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://ub.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yp.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fw.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rr.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tj.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://mu.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jb.hahajie.cn

[B12] 跳出多层循环
来源：http://xo.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://in.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gn.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dv.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ea.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vw.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pp.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pm.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dg.bjjhwx.cn

[B13] 判断是否为数字
来源：http://vg.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://lu.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://cb.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ka.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zl.panjiajie.cn

Java: x instanceof Number
来源：http://ow.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vr.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://rq.9csxet.cn

C#:   x is int or double or decimal
来源：http://yf.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://op.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ko.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ii.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://yd.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://vi.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zf.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sp.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xp.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gx.asd995.cn

[B15] 布尔运算与取反
来源：http://wv.jctech888.com.cn

Py:   a and b or not c
来源：http://hu.hahajie.cn

PHP:  $a && $b || !$c
来源：http://uu.huanxung.cn

JS:   a && b || !c
来源：http://ds.hnjuh.cn

TS:   a && b || !c
来源：http://mw.huanxung.cn

Java: a && b || !c
来源：http://eg.huanxung.cn

Go:   a && b || !c
来源：http://hd.gzmigu.cn

Ruby: a && b || !c
来源：http://jl.szxytkj.cn

C#:   a && b || !c
来源：http://aq.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wl.hnjuh.cn

Py:   if not data: return
来源：http://wx.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://jy.nicolike.cn

JS:   if (!data) return;
来源：http://br.panjiajie.cn

TS:   if (!data) return;
来源：http://ul.huixiangedu.cn

Java: if (data == null) return;
来源：http://ig.nicolike.cn

Go:   if data == nil { return }
来源：http://vi.shtwfgs.cn

Ruby: return if data.nil?
来源：http://la.hahajie.cn

C#:   if (data == null) return;
来源：http://cg.nicolike.cn

================================================================================
来源：http://od.panjiajie.cn

C. 函数与作用域
来源：http://qb.haigaiapp.cn

================================================================================
来源：http://le.jctech888.com.cn

[C01] 定义函数
来源：http://np.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://nl.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xo.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://wc.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xv.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mj.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dw.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://jb.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yu.nicolike.cn

[C02] 默认参数
来源：http://ae.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://xz.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yt.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://ri.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dk.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jz.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qd.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://jl.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://fg.9csxet.cn

[C03] 可变参数
来源：http://uy.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://hf.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dl.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nt.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qu.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dr.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dg.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tq.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ne.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://sy.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bj.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qv.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ha.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fj.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://vb.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://it.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://ei.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://bk.nicolike.cn

[C05] 返回多个值
来源：http://yf.bjjhwx.cn

Py:   return a, b
来源：http://dl.newstarts.cn

PHP:  return [$a, $b];
来源：http://ke.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ax.newstarts.cn

TS:   return { a, b };
来源：http://ee.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://re.gzmigu.cn

Go:   return a, b
来源：http://qf.newstarts.cn

Ruby: return a, b
来源：http://rp.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://nt.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://dj.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://ve.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://um.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://qg.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://nq.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ls.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ik.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://cz.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hm.newstarts.cn

[C07] 把函数作为参数传入
来源：http://vm.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jc.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sf.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gq.gzmigu.cn

TS:   arr.map(String)
来源：http://cb.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xq.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xs.521024.cn

Ruby: arr.map(&:upcase)
来源：http://bo.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sm.hahajie.cn

[C08] 闭包
来源：http://fa.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lg.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jz.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lg.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ib.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sz.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://op.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://px.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yp.nszjky.cn

[C09] 递归
来源：http://vf.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zp.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wc.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cw.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uv.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yc.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fp.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qk.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://od.jctech888.com.cn

[C10] 变量作用域
来源：http://bg.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nq.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jc.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dr.haigaiapp.cn

TS:   同 JS
来源：http://dh.szsharing.cn

Java: 方法内为块级作用域
来源：http://gs.newstarts.cn

Go:   花括号块级作用域
来源：http://bf.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jc.yuntaijiaju.cn

C#:   块级作用域
来源：http://tt.9csxet.cn

[C11] 模块导入与导出
来源：http://gn.huanxung.cn

Py:   from module import func
来源：http://cl.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wq.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://so.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gh.shxzukj.cn

Java: import java.util.List;
来源：http://fo.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vy.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://ti.asd995.cn

C#:   using System.Text;
来源：http://js.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://kl.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://cn.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://di.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://xo.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://pl.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aq.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://sz.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://hr.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zo.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://je.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://it.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gf.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vj.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yu.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ba.huanxung.cn

Go:   func add(a, b int) int
来源：http://wt.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://si.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qt.huanxung.cn

[C14] 泛型函数
来源：http://er.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ua.chemitech.net.cn

PHP:  // 无泛型
来源：http://ck.hnjuh.cn

JS:   // 无泛型
来源：http://aw.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yy.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vc.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pw.shxzskj.cn

Ruby: # 无泛型
来源：http://oz.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bx.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://cm.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oq.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://fv.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://be.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jc.muxihuayi.cn

Java: // 无解构
来源：http://mf.haigaiapp.cn

Go:   // 无解构
来源：http://zt.muxihuayi.cn

Ruby: a, b = pair
来源：http://oh.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://ec.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://ui.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yu.yuexingan06.cn

PHP:  // 无重载
来源：http://rg.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://za.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://ni.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ew.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://te.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://zm.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://so.shtwfgs.cn

================================================================================
来源：http://pe.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://mh.newstarts.cn

================================================================================
来源：http://bx.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://mr.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://np.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://au.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tp.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tw.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lg.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://kq.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://gg.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jt.521024.cn

[D02] 追加元素到末尾
来源：http://ce.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ha.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rm.szsharing.cn

JS:   arr.push(4);
来源：http://ho.bjjhwx.cn

TS:   arr.push(4);
来源：http://ko.szxytkj.cn

Java: list.add(4);
来源：http://ke.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://ri.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://ea.colortex.cn

C#:   list.Add(4);
来源：http://oo.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://xn.521024.cn

Py:   arr.insert(0, 0)
来源：http://ws.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bf.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zj.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://ih.hahajie.cn

Java: list.add(0, 0);
来源：http://gp.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://py.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://km.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://mg.colortex.cn

[D04] 删除元素
来源：http://qz.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ws.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://az.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yq.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://gd.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uy.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bd.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jy.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nd.nicolike.cn

[D05] 访问与修改元素
来源：http://oy.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xv.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ei.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sg.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://ob.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://wv.yuntaijiaju.cn


<!-- 参考信息 -->