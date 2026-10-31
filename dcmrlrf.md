代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://er.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vs.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://tt.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gn.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://tt.nszjky.cn

Py:   for item in arr: print(item)
来源：http://nh.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gz.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mv.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zf.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qf.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://te.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://jf.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ik.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://de.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ou.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bg.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fz.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xx.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vx.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qn.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hc.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rc.chemitech.net.cn

[B07] while 循环
来源：http://hj.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://fw.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yu.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://ua.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://wi.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://jd.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nk.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://np.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://wc.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://jn.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://os.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fu.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://vh.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://zy.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://xr.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vb.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zp.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://qe.szsharing.cn

[B09] break 与 continue
来源：http://mx.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ni.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zj.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qn.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ib.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tg.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gm.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gv.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vf.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://wc.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://at.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rw.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pn.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mz.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eo.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bw.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wz.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kw.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://rq.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://oq.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://le.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ml.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tp.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sr.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hh.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://po.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yw.521024.cn

[B12] 跳出多层循环
来源：http://wk.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://on.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pd.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sw.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://br.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xf.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wz.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://of.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rf.colortex.cn

[B13] 判断是否为数字
来源：http://nc.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://fg.szxytkj.cn

PHP:  is_numeric($x)
来源：http://my.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iv.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bp.huanxung.cn

Java: x instanceof Number
来源：http://rd.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://at.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://wx.hahajie.cn

C#:   x is int or double or decimal
来源：http://ia.521024.cn

[B14] 判断值是否在集合内
来源：http://ku.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fz.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pz.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://fj.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://dr.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ar.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wp.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ja.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oi.lnxyls.cn

[B15] 布尔运算与取反
来源：http://sq.panjiajie.cn

Py:   a and b or not c
来源：http://js.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://sf.yuexingan06.cn

JS:   a && b || !c
来源：http://xu.shtwfgs.cn

TS:   a && b || !c
来源：http://bj.lnxyls.cn

Java: a && b || !c
来源：http://ny.nszjky.cn

Go:   a && b || !c
来源：http://mj.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://wg.shtwfgs.cn

C#:   a && b || !c
来源：http://aw.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pv.wgjwhj.cn

Py:   if not data: return
来源：http://er.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://la.huanxung.cn

JS:   if (!data) return;
来源：http://pa.bjjhwx.cn

TS:   if (!data) return;
来源：http://sk.9csxet.cn

Java: if (data == null) return;
来源：http://zw.huixiangedu.cn

Go:   if data == nil { return }
来源：http://eu.shxzskj.cn

Ruby: return if data.nil?
来源：http://nr.huixiangedu.cn

C#:   if (data == null) return;
来源：http://ku.lnxyls.cn

================================================================================
来源：http://rz.hnjuh.cn

C. 函数与作用域
来源：http://rl.szsharing.cn

================================================================================
来源：http://fe.yuntaijiaju.cn

[C01] 定义函数
来源：http://ev.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://cv.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yr.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://kv.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://or.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://em.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yf.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://tm.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xg.newstarts.cn

[C02] 默认参数
来源：http://ou.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://ln.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mp.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://tp.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ln.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://co.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xm.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://zm.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://kf.haigaiapp.cn

[C03] 可变参数
来源：http://nu.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://nh.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://td.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zq.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ds.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dy.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ir.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hv.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pu.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://nm.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dl.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ev.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fe.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xd.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://el.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://xy.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://qz.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://ah.wgjwhj.cn

[C05] 返回多个值
来源：http://ss.gzmigu.cn

Py:   return a, b
来源：http://yu.szxytkj.cn

PHP:  return [$a, $b];
来源：http://ye.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tm.muxihuayi.cn

TS:   return { a, b };
来源：http://fm.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ag.bjjhwx.cn

Go:   return a, b
来源：http://hm.shtwfgs.cn

Ruby: return a, b
来源：http://xx.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://uy.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://is.colortex.cn

Py:   square = lambda x: x * x
来源：http://uy.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ls.9csxet.cn

JS:   const square = x => x * x;
来源：http://zz.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://dm.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vy.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iw.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://mx.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://te.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://al.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kn.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pd.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://le.bookmarksfly.cn

TS:   arr.map(String)
来源：http://jv.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://je.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ym.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://ru.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lo.lnxyls.cn

[C08] 闭包
来源：http://jb.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hx.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xc.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xs.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://si.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qg.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jp.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vq.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gc.chemitech.net.cn

[C09] 递归
来源：http://pr.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://se.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dc.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fp.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hf.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vp.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ma.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vu.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zf.shxzukj.cn

[C10] 变量作用域
来源：http://dr.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://km.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jx.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wt.colortex.cn

TS:   同 JS
来源：http://pf.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://ew.asd995.cn

Go:   花括号块级作用域
来源：http://gz.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ql.muxihuayi.cn

C#:   块级作用域
来源：http://kw.nicolike.cn

[C11] 模块导入与导出
来源：http://sf.huixiangedu.cn

Py:   from module import func
来源：http://qk.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hg.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ek.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vj.lnxyls.cn

Java: import java.util.List;
来源：http://wk.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aa.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://gn.jctech888.com.cn

C#:   using System.Text;
来源：http://dq.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://im.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://yv.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://vu.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://vx.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://kd.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pi.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://dw.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://rt.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gx.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://pa.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fy.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yo.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kb.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oo.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jf.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://kf.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qm.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ck.yuntaijiaju.cn

[C14] 泛型函数
来源：http://al.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bn.huixiangedu.cn

PHP:  // 无泛型
来源：http://qu.shxzskj.cn

JS:   // 无泛型
来源：http://ir.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qp.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mj.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qh.yuexingan06.cn

Ruby: # 无泛型
来源：http://ue.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qt.szsharing.cn

[C15] 解构 / 展开参数
来源：http://kj.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://es.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://mb.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yg.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qs.yuntaijiaju.cn

Java: // 无解构
来源：http://kv.9csxet.cn

Go:   // 无解构
来源：http://cw.9csxet.cn

Ruby: a, b = pair
来源：http://gz.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://uw.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://sh.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fp.newstarts.cn

PHP:  // 无重载
来源：http://ot.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hx.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://cd.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xc.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://sp.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://be.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zc.wgjwhj.cn

================================================================================
来源：http://he.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://ie.gzmigu.cn

================================================================================
来源：http://xp.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://xe.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iz.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bi.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vz.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xz.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://il.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://bh.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://dj.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ph.szsharing.cn

[D02] 追加元素到末尾
来源：http://iu.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lz.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xh.shxzukj.cn

JS:   arr.push(4);
来源：http://ss.huixiangedu.cn

TS:   arr.push(4);
来源：http://kl.newstarts.cn

Java: list.add(4);
来源：http://at.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://sr.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://rd.chemitech.net.cn

C#:   list.Add(4);
来源：http://vs.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://tm.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://pz.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xd.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pv.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://jn.colortex.cn

Java: list.add(0, 0);
来源：http://rk.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rk.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tm.asd995.cn

C#:   list.Insert(0, 0);
来源：http://ra.huixiangedu.cn

[D04] 删除元素
来源：http://xb.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fi.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nn.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jb.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://qi.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ye.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lc.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lc.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nb.newstarts.cn

[D05] 访问与修改元素
来源：http://gp.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bv.shxzukj.cn


<!-- 参考信息 -->