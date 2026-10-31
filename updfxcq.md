代发 wailian999

Py:   for i in range(10): print(i)
来源：http://ub.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://df.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ye.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qp.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ou.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hu.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://ea.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ay.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://qs.huanxung.cn

Py:   for item in arr: print(item)
来源：http://gr.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vt.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uw.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ga.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mj.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xk.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://pu.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tq.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://gg.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qo.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ym.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://at.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pj.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://we.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tf.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ww.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xk.hnjuh.cn

[B07] while 循环
来源：http://ar.nszjky.cn

Py:   while i < 10: i += 1
来源：http://yd.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zv.521024.cn

JS:   while (i < 10) { i++; }
来源：http://st.521024.cn

TS:   while (i < 10) { i++; }
来源：http://eg.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://fi.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nc.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://cz.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://hv.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://xl.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://jn.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qg.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://vw.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://yl.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://kd.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uv.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://an.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://tb.gzmigu.cn

[B09] break 与 continue
来源：http://ua.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fe.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kp.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://os.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cd.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ed.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zm.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://hh.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xo.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tb.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nv.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dp.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rk.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kr.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ud.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tu.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://pd.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://mz.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://je.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://go.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vv.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vd.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ey.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://lu.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sa.huanxung.cn

[B12] 跳出多层循环
来源：http://dt.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uq.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gj.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://np.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sd.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bs.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yk.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ej.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lb.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://kg.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://mi.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://ks.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yb.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zt.yuntaijiaju.cn

Java: x instanceof Number
来源：http://rw.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tc.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://wj.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://dh.colortex.cn

[B14] 判断值是否在集合内
来源：http://sz.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nz.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nu.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://nm.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://kl.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ju.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qk.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iw.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jd.szxytkj.cn

[B15] 布尔运算与取反
来源：http://mq.huanxung.cn

Py:   a and b or not c
来源：http://ol.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://ye.huanxung.cn

JS:   a && b || !c
来源：http://hh.yuexingan06.cn

TS:   a && b || !c
来源：http://mu.haigaiapp.cn

Java: a && b || !c
来源：http://lf.asd995.cn

Go:   a && b || !c
来源：http://yz.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://eq.521024.cn

C#:   a && b || !c
来源：http://gc.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eg.yuexingan06.cn

Py:   if not data: return
来源：http://ay.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://xf.bookmarksfly.cn

JS:   if (!data) return;
来源：http://mx.asd995.cn

TS:   if (!data) return;
来源：http://gt.hahajie.cn

Java: if (data == null) return;
来源：http://ko.521024.cn

Go:   if data == nil { return }
来源：http://ms.yuexingan06.cn

Ruby: return if data.nil?
来源：http://ce.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://do.lnxyls.cn

================================================================================
来源：http://yq.bjjhwx.cn

C. 函数与作用域
来源：http://hk.yuntaijiaju.cn

================================================================================
来源：http://pe.lnxyls.cn

[C01] 定义函数
来源：http://xk.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://qt.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ey.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://qh.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wg.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yt.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xr.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://ol.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pa.nszjky.cn

[C02] 默认参数
来源：http://cj.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://vb.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oq.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://cr.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xr.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zc.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ql.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://we.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://or.hnjuh.cn

[C03] 可变参数
来源：http://je.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://rx.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ib.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ab.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://km.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://te.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hd.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ii.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dh.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://ih.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tk.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gg.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lb.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gm.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://sq.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://ir.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://ff.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://ay.newstarts.cn

[C05] 返回多个值
来源：http://xg.nszjky.cn

Py:   return a, b
来源：http://de.9csxet.cn

PHP:  return [$a, $b];
来源：http://bh.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mz.hnjuh.cn

TS:   return { a, b };
来源：http://xm.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ck.yuntaijiaju.cn

Go:   return a, b
来源：http://wx.szsharing.cn

Ruby: return a, b
来源：http://qg.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://iu.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://ju.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://hj.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xu.nicolike.cn

JS:   const square = x => x * x;
来源：http://ce.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://av.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ss.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://za.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://rz.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://us.9csxet.cn

[C07] 把函数作为参数传入
来源：http://bh.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dc.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ok.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bv.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://zg.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qv.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sd.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://gp.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ha.jianghongdianzi.cn

[C08] 闭包
来源：http://ht.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mz.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://es.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qp.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kx.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hn.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pz.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ff.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vc.shxzukj.cn

[C09] 递归
来源：http://jm.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ww.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rc.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xj.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lj.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cw.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://og.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://od.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://js.szxytkj.cn

[C10] 变量作用域
来源：http://jn.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://up.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pu.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bn.newstarts.cn

TS:   同 JS
来源：http://tb.lnxyls.cn

Java: 方法内为块级作用域
来源：http://tx.huixiangedu.cn

Go:   花括号块级作用域
来源：http://tw.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xp.huixinmuqiang.cn

C#:   块级作用域
来源：http://pm.yuexingan06.cn

[C11] 模块导入与导出
来源：http://gt.jctech888.com.cn

Py:   from module import func
来源：http://vf.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nb.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://td.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fh.bjjhwx.cn

Java: import java.util.List;
来源：http://vz.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ut.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://pr.bookmarksfly.cn

C#:   using System.Text;
来源：http://ow.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://yi.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://ii.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://vr.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://qr.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://tm.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fo.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://yu.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://me.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xw.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://gs.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fv.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ak.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oo.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zy.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cf.shxzukj.cn

Go:   func add(a, b int) int
来源：http://ag.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bb.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zj.chemitech.net.cn

[C14] 泛型函数
来源：http://nn.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iv.haigaiapp.cn

PHP:  // 无泛型
来源：http://al.shtwfgs.cn

JS:   // 无泛型
来源：http://cn.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hu.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rz.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hg.hahajie.cn

Ruby: # 无泛型
来源：http://pt.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zq.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://mm.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dt.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://ew.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sv.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://te.huanxung.cn

Java: // 无解构
来源：http://ni.hahajie.cn

Go:   // 无解构
来源：http://ee.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://ud.newstarts.cn

C#:   var (a, b) = pair;
来源：http://kh.521024.cn

[C16] 函数 / 方法重载
来源：http://zn.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ek.panjiajie.cn

PHP:  // 无重载
来源：http://pu.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tp.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ni.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gl.521024.cn

Go:   // 无重载：用不同函数名
来源：http://dv.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://wd.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ib.lnxyls.cn

================================================================================
来源：http://kw.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://yd.yuntaijiaju.cn

================================================================================
来源：http://ij.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://ur.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dn.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://on.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eo.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zo.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oy.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://mp.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://pr.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vu.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://dj.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yx.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mu.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://re.huixiangedu.cn

TS:   arr.push(4);
来源：http://vt.chemitech.net.cn

Java: list.add(4);
来源：http://pr.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://mr.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://og.nszjky.cn

C#:   list.Add(4);
来源：http://ij.9csxet.cn

[D03] 在指定位置插入元素
来源：http://tv.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://pw.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ag.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ir.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://pt.huanxung.cn

Java: list.add(0, 0);
来源：http://km.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://my.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dx.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://he.huanxung.cn

[D04] 删除元素
来源：http://me.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mu.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nq.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kd.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://pa.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fz.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cr.chemitech.net.cn


<!-- 参考信息 -->