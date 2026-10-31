代发 wailian999

Py:   for i in range(10): print(i)
来源：http://uy.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jj.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xy.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qt.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://no.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://wz.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rx.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://cf.huanxung.cn

Py:   for item in arr: print(item)
来源：http://jb.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bb.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ax.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fi.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ao.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dc.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://eg.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bw.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://lo.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lz.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cq.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ed.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lh.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xo.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ee.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ip.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fb.yuntaijiaju.cn

[B07] while 循环
来源：http://li.521024.cn

Py:   while i < 10: i += 1
来源：http://uf.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gf.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://fs.521024.cn

TS:   while (i < 10) { i++; }
来源：http://gt.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://nd.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ic.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://uq.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://px.colortex.cn

[B08] do-while（至少执行一次）
来源：http://dt.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://kg.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ak.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://kw.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://os.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://tp.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yg.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gh.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://ox.shtwfgs.cn

[B09] break 与 continue
来源：http://nn.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nh.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://br.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qu.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oj.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://al.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://un.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ms.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zu.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://hp.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xx.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wz.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zd.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tq.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vh.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fx.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tb.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mu.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://kt.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://jb.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://wq.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://md.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hg.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rf.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zk.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://cx.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rx.szsharing.cn

[B12] 跳出多层循环
来源：http://ak.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dc.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://br.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dk.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dy.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://va.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vj.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lo.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qz.nicolike.cn

[B13] 判断是否为数字
来源：http://bc.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://hp.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://nj.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ad.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://it.nicolike.cn

Java: x instanceof Number
来源：http://gi.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dt.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://kp.hahajie.cn

C#:   x is int or double or decimal
来源：http://co.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ph.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://io.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pq.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://sy.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://fb.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xi.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kk.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yd.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sa.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://gv.haigaiapp.cn

Py:   a and b or not c
来源：http://zk.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://br.huixiangedu.cn

JS:   a && b || !c
来源：http://lm.bookmarksfly.cn

TS:   a && b || !c
来源：http://js.lnxyls.cn

Java: a && b || !c
来源：http://ze.nszjky.cn

Go:   a && b || !c
来源：http://yl.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://bf.huixiangedu.cn

C#:   a && b || !c
来源：http://op.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vs.shxzskj.cn

Py:   if not data: return
来源：http://eq.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://sa.lnxyls.cn

JS:   if (!data) return;
来源：http://jm.521024.cn

TS:   if (!data) return;
来源：http://fu.521024.cn

Java: if (data == null) return;
来源：http://ik.shxzukj.cn

Go:   if data == nil { return }
来源：http://az.panjiajie.cn

Ruby: return if data.nil?
来源：http://ap.521024.cn

C#:   if (data == null) return;
来源：http://ku.9csxet.cn

================================================================================
来源：http://ug.bjjhwx.cn

C. 函数与作用域
来源：http://pr.shtwfgs.cn

================================================================================
来源：http://ky.gzmigu.cn

[C01] 定义函数
来源：http://be.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://hm.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vp.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://iq.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ka.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pd.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dg.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://fp.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://is.nicolike.cn

[C02] 默认参数
来源：http://ui.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://ds.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vl.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://aw.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pr.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://to.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mn.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://yo.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://lz.panjiajie.cn

[C03] 可变参数
来源：http://jg.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://hm.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wf.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://og.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sw.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://if.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kl.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ve.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yz.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://km.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://la.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hj.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vu.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iq.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://rz.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://rx.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://bx.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://nu.lnxyls.cn

[C05] 返回多个值
来源：http://qg.asd995.cn

Py:   return a, b
来源：http://xy.huanxung.cn

PHP:  return [$a, $b];
来源：http://ni.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ts.huanxung.cn

TS:   return { a, b };
来源：http://pu.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ni.9csxet.cn

Go:   return a, b
来源：http://yg.521024.cn

Ruby: return a, b
来源：http://ht.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://tm.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://ff.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://vn.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ah.szsharing.cn

JS:   const square = x => x * x;
来源：http://fv.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ht.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qr.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://on.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://sq.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rw.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://zi.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tg.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ck.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nq.521024.cn

TS:   arr.map(String)
来源：http://ej.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gv.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qv.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://sq.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ey.lnxyls.cn

[C08] 闭包
来源：http://iy.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bt.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rm.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://id.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wr.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ou.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ls.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hb.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lm.huixiangedu.cn

[C09] 递归
来源：http://td.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xr.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ck.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://on.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ta.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ss.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ut.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sq.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mv.jianghongdianzi.cn

[C10] 变量作用域
来源：http://uz.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ep.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ct.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yv.colortex.cn

TS:   同 JS
来源：http://ze.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://el.shxzskj.cn

Go:   花括号块级作用域
来源：http://fh.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ax.huixiangedu.cn

C#:   块级作用域
来源：http://ny.huanxung.cn

[C11] 模块导入与导出
来源：http://iy.szxytkj.cn

Py:   from module import func
来源：http://um.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zn.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bq.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wl.jctech888.com.cn

Java: import java.util.List;
来源：http://dc.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ms.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ps.huixinmuqiang.cn

C#:   using System.Text;
来源：http://cd.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://js.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://nl.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://iu.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://kg.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ul.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vz.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://yy.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://gm.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ib.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://nh.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ca.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gk.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://md.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vs.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vd.shxzukj.cn

Go:   func add(a, b int) int
来源：http://dg.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zz.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sw.hnjuh.cn

[C14] 泛型函数
来源：http://kp.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tk.chemitech.net.cn

PHP:  // 无泛型
来源：http://il.szsharing.cn

JS:   // 无泛型
来源：http://yu.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vz.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pg.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bd.muxihuayi.cn

Ruby: # 无泛型
来源：http://dq.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ku.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://hi.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jm.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://ce.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fr.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://we.asd995.cn

Java: // 无解构
来源：http://xm.shtwfgs.cn

Go:   // 无解构
来源：http://gn.bjjhwx.cn

Ruby: a, b = pair
来源：http://kw.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://ya.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://th.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lo.colortex.cn

PHP:  // 无重载
来源：http://ja.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jv.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://jn.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://du.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://ak.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://pp.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aa.muxihuayi.cn

================================================================================
来源：http://li.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://ff.huixinmuqiang.cn

================================================================================
来源：http://ee.521024.cn

[D01] 创建数组 / 列表
来源：http://ro.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://py.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ra.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uf.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ng.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vq.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://uq.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://ee.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fb.nszjky.cn

[D02] 追加元素到末尾
来源：http://qc.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qw.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oa.muxihuayi.cn

JS:   arr.push(4);
来源：http://ch.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://cm.chemitech.net.cn

Java: list.add(4);
来源：http://in.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://ax.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://ij.asd995.cn

C#:   list.Add(4);
来源：http://vm.asd995.cn

[D03] 在指定位置插入元素
来源：http://rr.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://lw.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ir.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hf.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://my.haigaiapp.cn

Java: list.add(0, 0);
来源：http://pf.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dn.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pl.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://tw.huixiangedu.cn

[D04] 删除元素
来源：http://sh.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://er.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jl.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ai.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://dh.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ar.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://us.521024.cn


<!-- 参考信息 -->