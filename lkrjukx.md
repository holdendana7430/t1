代发 wailian999

Py:   for i in range(10): print(i)
来源：http://qc.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vz.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mw.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ia.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kz.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hg.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://xo.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sh.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://vs.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://jv.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ni.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xe.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fl.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wx.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xo.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://md.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bl.521024.cn

[B06] 遍历字典 / 对象
来源：http://mg.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kg.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tu.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cj.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xw.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mw.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hi.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jn.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tj.asd995.cn

[B07] while 循环
来源：http://jj.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://ew.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://un.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://gv.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ba.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://jo.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ri.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://za.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://al.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://ie.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://mh.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ud.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ol.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://rw.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://ww.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://le.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jy.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://ng.9csxet.cn

[B09] break 与 continue
来源：http://kx.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://et.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://io.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ra.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pb.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bx.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iw.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ey.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fs.newstarts.cn

[B10] 遍历同时拿索引
来源：http://tf.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lq.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ur.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jh.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fp.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nq.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bh.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vy.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rd.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://qp.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://zq.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://ff.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gq.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://po.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ay.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vu.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://ln.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ga.hnjuh.cn

[B12] 跳出多层循环
来源：http://zm.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rb.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ia.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iv.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nn.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xd.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dl.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xy.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lm.hahajie.cn

[B13] 判断是否为数字
来源：http://rv.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://lc.colortex.cn

PHP:  is_numeric($x)
来源：http://db.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ul.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vr.wgjwhj.cn

Java: x instanceof Number
来源：http://cf.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oj.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://px.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://tv.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://zy.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tu.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sn.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ek.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://ni.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nq.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://an.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dw.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bv.hnjuh.cn

[B15] 布尔运算与取反
来源：http://zl.haigaiapp.cn

Py:   a and b or not c
来源：http://tq.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://jt.nszjky.cn

JS:   a && b || !c
来源：http://ff.nicolike.cn

TS:   a && b || !c
来源：http://rz.newstarts.cn

Java: a && b || !c
来源：http://ak.shxzukj.cn

Go:   a && b || !c
来源：http://iw.szsharing.cn

Ruby: a && b || !c
来源：http://ar.chemitech.net.cn

C#:   a && b || !c
来源：http://vm.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sn.huixiangedu.cn

Py:   if not data: return
来源：http://oe.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://iz.hahajie.cn

JS:   if (!data) return;
来源：http://ex.szsharing.cn

TS:   if (!data) return;
来源：http://eh.9csxet.cn

Java: if (data == null) return;
来源：http://jg.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://at.shxzukj.cn

Ruby: return if data.nil?
来源：http://mz.huixiangedu.cn

C#:   if (data == null) return;
来源：http://yo.9csxet.cn

================================================================================
来源：http://in.huixinmuqiang.cn

C. 函数与作用域
来源：http://qf.hahajie.cn

================================================================================
来源：http://ur.szsharing.cn

[C01] 定义函数
来源：http://ll.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://rx.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gp.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://hi.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ou.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gf.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rd.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://pu.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ma.9csxet.cn

[C02] 默认参数
来源：http://hl.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://jl.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://em.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ft.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://by.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ai.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jq.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://id.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://be.huixiangedu.cn

[C03] 可变参数
来源：http://zg.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://oz.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lc.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fg.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ax.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ps.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dr.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hf.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cc.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://zl.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rt.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nw.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zb.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tr.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://rc.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://xx.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://cb.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://yl.hahajie.cn

[C05] 返回多个值
来源：http://nl.shxzukj.cn

Py:   return a, b
来源：http://er.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://pl.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fz.9csxet.cn

TS:   return { a, b };
来源：http://nd.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nn.huanxung.cn

Go:   return a, b
来源：http://bq.gzmigu.cn

Ruby: return a, b
来源：http://cw.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://zq.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://ei.asd995.cn

Py:   square = lambda x: x * x
来源：http://lt.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sk.shxzukj.cn

JS:   const square = x => x * x;
来源：http://gi.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://sa.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://di.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wb.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://ib.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sh.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://fp.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wf.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mr.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rl.lnxyls.cn

TS:   arr.map(String)
来源：http://qv.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ci.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yw.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://nj.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yt.hahajie.cn

[C08] 闭包
来源：http://mb.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fk.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zc.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mb.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ts.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mm.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nf.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pr.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://um.shxzukj.cn

[C09] 递归
来源：http://dv.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ft.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lq.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qg.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://we.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dm.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jr.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://la.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pz.huanxung.cn

[C10] 变量作用域
来源：http://ui.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zr.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qo.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hr.huixiangedu.cn

TS:   同 JS
来源：http://kh.szxytkj.cn

Java: 方法内为块级作用域
来源：http://kc.asd995.cn

Go:   花括号块级作用域
来源：http://ml.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wx.nicolike.cn

C#:   块级作用域
来源：http://pm.chemitech.net.cn

[C11] 模块导入与导出
来源：http://cs.hnjuh.cn

Py:   from module import func
来源：http://dk.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kw.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hp.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dk.newstarts.cn

Java: import java.util.List;
来源：http://fw.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tb.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://bq.shtwfgs.cn

C#:   using System.Text;
来源：http://pt.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://qg.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://tj.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://xk.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://iu.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://ds.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xv.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://in.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://ht.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ez.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://vf.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xe.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cs.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ko.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qf.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nh.hahajie.cn

Go:   func add(a, b int) int
来源：http://aw.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jp.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pe.huixinmuqiang.cn

[C14] 泛型函数
来源：http://qn.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://an.nszjky.cn

PHP:  // 无泛型
来源：http://uv.szxytkj.cn

JS:   // 无泛型
来源：http://rv.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wh.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ny.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xa.panjiajie.cn

Ruby: # 无泛型
来源：http://xh.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sx.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://lp.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kp.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://wn.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lv.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aw.muxihuayi.cn

Java: // 无解构
来源：http://cp.jianghongdianzi.cn

Go:   // 无解构
来源：http://pn.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://io.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://eg.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://hd.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ol.chemitech.net.cn

PHP:  // 无重载
来源：http://bh.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pv.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://hc.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ts.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://mj.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://kn.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wx.bookmarksfly.cn

================================================================================
来源：http://ia.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ra.521024.cn

================================================================================
来源：http://ei.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://as.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qa.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ll.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jm.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ji.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qb.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://to.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://tp.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vk.asd995.cn

[D02] 追加元素到末尾
来源：http://ck.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wy.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ou.bjjhwx.cn

JS:   arr.push(4);
来源：http://wj.jctech888.com.cn

TS:   arr.push(4);
来源：http://vv.haigaiapp.cn

Java: list.add(4);
来源：http://yx.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://py.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://jq.panjiajie.cn

C#:   list.Add(4);
来源：http://ro.asd995.cn

[D03] 在指定位置插入元素
来源：http://yl.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://bg.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qt.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vd.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://ha.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://co.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ct.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yj.521024.cn

C#:   list.Insert(0, 0);
来源：http://wk.colortex.cn

[D04] 删除元素
来源：http://wt.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lp.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hn.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fn.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://kk.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bz.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sa.hahajie.cn


<!-- 参考信息 -->