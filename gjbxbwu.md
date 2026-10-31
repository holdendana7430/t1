代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://db.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ux.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ht.huanxung.cn

[B04] for 计数循环
来源：http://yf.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://fm.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lh.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zr.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zz.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sd.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rb.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://sr.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wf.521024.cn

[B05] 遍历数组 / 列表
来源：http://zn.hahajie.cn

Py:   for item in arr: print(item)
来源：http://nq.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dy.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yg.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ou.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bt.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://en.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://wm.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gg.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://as.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pw.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wl.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ak.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xr.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gt.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rb.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fs.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dj.bookmarksfly.cn

[B07] while 循环
来源：http://qw.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://mj.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zi.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://he.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://sq.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://xu.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gl.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://ls.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://ux.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://dl.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://fg.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pz.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://jn.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://mq.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://ri.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://th.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ug.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://pg.hahajie.cn

[B09] break 与 continue
来源：http://gk.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ud.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hl.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wh.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zf.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://as.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gk.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xt.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gr.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://aj.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cc.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hb.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ho.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fa.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wi.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gy.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mz.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jk.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://yg.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://zw.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://qb.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iu.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://my.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ia.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ac.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://zr.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sw.9csxet.cn

[B12] 跳出多层循环
来源：http://xf.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rr.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pr.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mh.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pw.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gp.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mm.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://im.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fz.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://jt.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://ce.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://wv.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://me.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ug.haigaiapp.cn

Java: x instanceof Number
来源：http://re.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xg.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://qy.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://ek.newstarts.cn

[B14] 判断值是否在集合内
来源：http://te.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://if.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ce.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://tq.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://sb.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wz.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dq.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hn.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://se.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://ye.hnjuh.cn

Py:   a and b or not c
来源：http://pz.nszjky.cn

PHP:  $a && $b || !$c
来源：http://xj.bjjhwx.cn

JS:   a && b || !c
来源：http://ry.colortex.cn

TS:   a && b || !c
来源：http://qc.hahajie.cn

Java: a && b || !c
来源：http://ph.jianghongdianzi.cn

Go:   a && b || !c
来源：http://ci.haigaiapp.cn

Ruby: a && b || !c
来源：http://ws.gzmigu.cn

C#:   a && b || !c
来源：http://gh.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ej.muxihuayi.cn

Py:   if not data: return
来源：http://zk.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://dq.szxytkj.cn

JS:   if (!data) return;
来源：http://tx.gzmigu.cn

TS:   if (!data) return;
来源：http://sd.newstarts.cn

Java: if (data == null) return;
来源：http://pd.shxzukj.cn

Go:   if data == nil { return }
来源：http://yc.asd995.cn

Ruby: return if data.nil?
来源：http://yx.chemitech.net.cn

C#:   if (data == null) return;
来源：http://nc.jctech888.com.cn

================================================================================
来源：http://gi.bjjhwx.cn

C. 函数与作用域
来源：http://bw.jianghongdianzi.cn

================================================================================
来源：http://fj.shxzukj.cn

[C01] 定义函数
来源：http://dt.asd995.cn

Py:   def add(a, b): return a + b
来源：http://as.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mz.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://hv.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://id.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://no.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://me.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://kf.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dl.shxzskj.cn

[C02] 默认参数
来源：http://gy.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://hu.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ci.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://yf.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://da.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wc.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fx.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://ud.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://hr.9csxet.cn

[C03] 可变参数
来源：http://ir.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://im.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ss.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ip.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://my.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ld.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nv.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tr.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yi.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ta.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://up.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ef.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gx.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://be.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://lq.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://pg.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://ip.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://eb.gzmigu.cn

[C05] 返回多个值
来源：http://cf.jctech888.com.cn

Py:   return a, b
来源：http://kw.shxzukj.cn

PHP:  return [$a, $b];
来源：http://dj.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wz.nszjky.cn

TS:   return { a, b };
来源：http://gz.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lj.chemitech.net.cn

Go:   return a, b
来源：http://zt.szxytkj.cn

Ruby: return a, b
来源：http://co.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://lo.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://pv.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://ew.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rv.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://cy.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://qv.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oa.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sz.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ln.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tq.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://uk.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cr.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tr.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://af.huanxung.cn

TS:   arr.map(String)
来源：http://fl.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ua.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jy.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://ec.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ym.szsharing.cn

[C08] 闭包
来源：http://cj.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vo.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fv.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dp.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://he.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nd.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gb.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gl.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pm.nszjky.cn

[C09] 递归
来源：http://ys.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ew.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://li.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nr.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ug.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pn.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fm.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vd.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sj.shxzukj.cn

[C10] 变量作用域
来源：http://ua.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ad.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cd.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wa.jianghongdianzi.cn

TS:   同 JS
来源：http://qp.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://kk.wgjwhj.cn

Go:   花括号块级作用域
来源：http://uw.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cl.huixinmuqiang.cn

C#:   块级作用域
来源：http://jm.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://ix.nszjky.cn

Py:   from module import func
来源：http://eg.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lf.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yi.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uk.hnjuh.cn

Java: import java.util.List;
来源：http://nj.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yi.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://vg.wgjwhj.cn

C#:   using System.Text;
来源：http://yq.521024.cn

[C12] 立即执行函数 IIFE
来源：http://ef.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://ob.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://ls.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://zd.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://aj.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yx.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://hy.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://zg.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pn.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://dr.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qf.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ui.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cf.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rz.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bh.shxzukj.cn

Go:   func add(a, b int) int
来源：http://cc.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ch.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ii.nicolike.cn

[C14] 泛型函数
来源：http://gi.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zt.szxytkj.cn

PHP:  // 无泛型
来源：http://my.521024.cn

JS:   // 无泛型
来源：http://kz.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lw.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ji.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hl.panjiajie.cn

Ruby: # 无泛型
来源：http://ho.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ir.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://dp.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sv.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://fv.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fh.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ka.hahajie.cn

Java: // 无解构
来源：http://ln.bookmarksfly.cn

Go:   // 无解构
来源：http://vv.bookmarksfly.cn

Ruby: a, b = pair
来源：http://ll.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://zm.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://os.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sg.bookmarksfly.cn

PHP:  // 无重载
来源：http://dk.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cn.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://yf.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ts.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://nw.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://xg.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://po.newstarts.cn

================================================================================
来源：http://pm.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ho.chemitech.net.cn

================================================================================
来源：http://lx.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://pk.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mf.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qg.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mj.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yh.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://py.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://kt.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://yk.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xp.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://hm.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pb.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ji.colortex.cn

JS:   arr.push(4);
来源：http://jw.yuexingan06.cn

TS:   arr.push(4);
来源：http://gb.nicolike.cn

Java: list.add(4);
来源：http://ny.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://vb.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://ri.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://vj.hahajie.cn

[D03] 在指定位置插入元素
来源：http://ws.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://db.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eb.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xf.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://lm.huanxung.cn

Java: list.add(0, 0);
来源：http://cw.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fq.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pb.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://ti.9csxet.cn

[D04] 删除元素
来源：http://cg.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://at.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cz.szsharing.cn


<!-- 参考信息 -->