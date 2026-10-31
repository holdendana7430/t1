代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vm.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://me.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bw.shxzskj.cn

[B04] for 计数循环
来源：http://pv.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://lw.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nk.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yw.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lk.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kl.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nm.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://ov.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cs.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://hm.huanxung.cn

Py:   for item in arr: print(item)
来源：http://pk.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hw.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://md.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ki.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pd.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sy.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://hw.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://no.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://fd.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vx.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oc.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ym.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ve.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mz.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cc.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lx.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pv.jianghongdianzi.cn

[B07] while 循环
来源：http://fn.hahajie.cn

Py:   while i < 10: i += 1
来源：http://va.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eb.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://rx.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://al.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://wg.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mc.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://gn.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://wt.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://te.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://wj.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vw.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://mp.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://vb.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://rx.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oa.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wa.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://zq.panjiajie.cn

[B09] break 与 continue
来源：http://vf.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qo.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ka.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ds.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ba.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lt.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ho.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wq.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://th.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://gb.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pr.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yz.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rb.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cl.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jx.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lf.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hr.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zu.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://bs.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://jy.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://tp.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zp.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fu.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rr.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vi.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://oy.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nu.9csxet.cn

[B12] 跳出多层循环
来源：http://qd.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ym.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uk.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xl.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aw.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pf.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wd.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yd.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gt.asd995.cn

[B13] 判断是否为数字
来源：http://yv.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://bg.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://vf.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wl.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zc.nszjky.cn

Java: x instanceof Number
来源：http://qv.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vp.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://hy.asd995.cn

C#:   x is int or double or decimal
来源：http://ll.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://zc.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pd.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ma.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://dp.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://qy.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xq.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gu.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xq.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pf.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://qq.newstarts.cn

Py:   a and b or not c
来源：http://ye.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://es.asd995.cn

JS:   a && b || !c
来源：http://hd.asd995.cn

TS:   a && b || !c
来源：http://dq.9csxet.cn

Java: a && b || !c
来源：http://np.colortex.cn

Go:   a && b || !c
来源：http://ea.szsharing.cn

Ruby: a && b || !c
来源：http://ed.huixinmuqiang.cn

C#:   a && b || !c
来源：http://on.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tt.jianghongdianzi.cn

Py:   if not data: return
来源：http://wq.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://do.newstarts.cn

JS:   if (!data) return;
来源：http://hi.shtwfgs.cn

TS:   if (!data) return;
来源：http://jl.hahajie.cn

Java: if (data == null) return;
来源：http://gh.asd995.cn

Go:   if data == nil { return }
来源：http://po.jctech888.com.cn

Ruby: return if data.nil?
来源：http://vi.szxytkj.cn

C#:   if (data == null) return;
来源：http://rr.chemitech.net.cn

================================================================================
来源：http://tp.asd995.cn

C. 函数与作用域
来源：http://mx.panjiajie.cn

================================================================================
来源：http://ih.gzmigu.cn

[C01] 定义函数
来源：http://gz.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://fe.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bd.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://mz.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pl.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gp.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wz.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://ql.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vy.asd995.cn

[C02] 默认参数
来源：http://mb.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://qf.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wd.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://yv.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://on.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ux.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qp.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://nr.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://up.hnjuh.cn

[C03] 可变参数
来源：http://hs.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://ep.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://re.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bd.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ki.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gc.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://du.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uv.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yp.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://wa.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lc.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vl.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gv.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vm.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://bo.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://mx.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://jq.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://tg.colortex.cn

[C05] 返回多个值
来源：http://fh.colortex.cn

Py:   return a, b
来源：http://uj.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://dk.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://al.9csxet.cn

TS:   return { a, b };
来源：http://wz.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mu.lnxyls.cn

Go:   return a, b
来源：http://pb.nszjky.cn

Ruby: return a, b
来源：http://rf.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ol.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://ip.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://yi.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tv.shxzukj.cn

JS:   const square = x => x * x;
来源：http://ph.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://ya.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ae.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ug.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://bv.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bk.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://dh.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jq.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sn.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hx.shtwfgs.cn

TS:   arr.map(String)
来源：http://jr.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cs.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dw.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://jn.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ku.szsharing.cn

[C08] 闭包
来源：http://wl.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oi.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://br.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ay.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fr.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ry.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yr.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qv.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tc.newstarts.cn

[C09] 递归
来源：http://qj.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bj.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pf.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fs.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bd.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dy.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rm.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qk.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fx.hnjuh.cn

[C10] 变量作用域
来源：http://gw.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://st.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hi.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vp.szsharing.cn

TS:   同 JS
来源：http://im.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://vg.colortex.cn

Go:   花括号块级作用域
来源：http://iw.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gw.huixiangedu.cn

C#:   块级作用域
来源：http://kg.lnxyls.cn

[C11] 模块导入与导出
来源：http://yw.newstarts.cn

Py:   from module import func
来源：http://vt.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gv.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wj.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xe.asd995.cn

Java: import java.util.List;
来源：http://hh.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iq.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://up.szsharing.cn

C#:   using System.Text;
来源：http://zq.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://xe.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://nb.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://po.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://qo.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://wo.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://br.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://nq.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://zp.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kc.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://xc.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bp.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sy.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ly.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jf.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iv.szxytkj.cn

Go:   func add(a, b int) int
来源：http://qi.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xu.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kl.jctech888.com.cn

[C14] 泛型函数
来源：http://hk.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ua.9csxet.cn

PHP:  // 无泛型
来源：http://tr.huixiangedu.cn

JS:   // 无泛型
来源：http://sa.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fb.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xo.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://za.asd995.cn

Ruby: # 无泛型
来源：http://ok.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ju.nszjky.cn

[C15] 解构 / 展开参数
来源：http://ej.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ve.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://tu.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eo.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sf.hnjuh.cn

Java: // 无解构
来源：http://aq.muxihuayi.cn

Go:   // 无解构
来源：http://ii.shxzukj.cn

Ruby: a, b = pair
来源：http://rg.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://ox.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ww.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ip.chemitech.net.cn

PHP:  // 无重载
来源：http://md.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://no.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://pf.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zz.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://mr.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://sb.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wc.szxytkj.cn

================================================================================
来源：http://wo.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://sa.bjjhwx.cn

================================================================================
来源：http://jl.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://dc.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rc.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zg.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://je.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://js.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sm.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://fz.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://pw.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tt.nszjky.cn

[D02] 追加元素到末尾
来源：http://sa.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iz.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://br.colortex.cn

JS:   arr.push(4);
来源：http://am.szsharing.cn

TS:   arr.push(4);
来源：http://fa.hnjuh.cn

Java: list.add(4);
来源：http://wf.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://zn.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://di.newstarts.cn

C#:   list.Add(4);
来源：http://yg.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://gq.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://ws.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qp.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lw.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ao.newstarts.cn

Java: list.add(0, 0);
来源：http://hw.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zw.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://be.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://py.colortex.cn

[D04] 删除元素
来源：http://or.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yg.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ae.szxytkj.cn


<!-- 参考信息 -->