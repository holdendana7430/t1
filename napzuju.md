代发 wailian999

Py:   for i in range(10): print(i)
来源：http://ql.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gm.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lr.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ec.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ux.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bp.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://tw.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hb.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://pb.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://yv.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gv.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gi.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sw.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ia.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ls.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://tu.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bq.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://rl.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rb.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ps.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ep.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hg.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fl.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sa.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nh.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nd.huanxung.cn

[B07] while 循环
来源：http://ew.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://fh.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lt.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://do.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://qv.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://so.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://po.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://hm.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://zf.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://hz.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://rq.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wm.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://wz.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://dj.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://vx.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kf.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ag.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://wb.newstarts.cn

[B09] break 与 continue
来源：http://pm.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pz.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tl.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cy.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gi.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eg.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nr.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fq.nicolike.cn

[B10] 遍历同时拿索引
来源：http://pc.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nv.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://me.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zg.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sk.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yn.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hm.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ha.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fl.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://vn.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://rq.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://rn.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cr.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://in.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ur.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dt.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://sd.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hq.hnjuh.cn

[B12] 跳出多层循环
来源：http://as.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yv.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wk.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vl.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wa.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bs.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zk.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lz.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nc.haigaiapp.cn

[B13] 判断是否为数字
来源：http://ei.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://ie.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://qy.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ve.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iy.haigaiapp.cn

Java: x instanceof Number
来源：http://kb.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zq.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://fm.asd995.cn

C#:   x is int or double or decimal
来源：http://or.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://ti.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iu.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xd.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://cv.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://dx.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mg.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qo.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sw.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qm.newstarts.cn

[B15] 布尔运算与取反
来源：http://ip.nszjky.cn

Py:   a and b or not c
来源：http://em.colortex.cn

PHP:  $a && $b || !$c
来源：http://jk.shxzskj.cn

JS:   a && b || !c
来源：http://be.yuntaijiaju.cn

TS:   a && b || !c
来源：http://vd.huanxung.cn

Java: a && b || !c
来源：http://nm.shxzukj.cn

Go:   a && b || !c
来源：http://gy.521024.cn

Ruby: a && b || !c
来源：http://qv.panjiajie.cn

C#:   a && b || !c
来源：http://us.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gj.nszjky.cn

Py:   if not data: return
来源：http://sc.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://to.nszjky.cn

JS:   if (!data) return;
来源：http://ob.521024.cn

TS:   if (!data) return;
来源：http://li.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://mj.gzmigu.cn

Go:   if data == nil { return }
来源：http://ww.panjiajie.cn

Ruby: return if data.nil?
来源：http://gk.colortex.cn

C#:   if (data == null) return;
来源：http://at.newstarts.cn

================================================================================
来源：http://qt.chemitech.net.cn

C. 函数与作用域
来源：http://gr.panjiajie.cn

================================================================================
来源：http://ce.gzmigu.cn

[C01] 定义函数
来源：http://ev.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://bx.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://km.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ya.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fh.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fb.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qm.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://op.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uq.jctech888.com.cn

[C02] 默认参数
来源：http://el.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://xo.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mu.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://tk.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zc.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://br.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mw.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://pb.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://da.huixinmuqiang.cn

[C03] 可变参数
来源：http://rf.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://dg.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nw.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://et.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ki.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tc.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cu.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zo.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qv.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://tc.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pw.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ka.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ei.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ub.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://zz.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://li.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://wq.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://cx.szsharing.cn

[C05] 返回多个值
来源：http://ex.nicolike.cn

Py:   return a, b
来源：http://ol.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://vk.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cz.huanxung.cn

TS:   return { a, b };
来源：http://zb.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://du.huixinmuqiang.cn

Go:   return a, b
来源：http://to.szxytkj.cn

Ruby: return a, b
来源：http://ik.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://sn.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://zo.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://rf.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tn.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://op.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ak.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fo.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://th.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://qi.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://am.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://ma.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sr.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uk.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uk.szxytkj.cn

TS:   arr.map(String)
来源：http://tf.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iv.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lo.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://ga.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zu.newstarts.cn

[C08] 闭包
来源：http://nb.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vb.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oi.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rl.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ry.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://na.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ri.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tj.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jt.shtwfgs.cn

[C09] 递归
来源：http://we.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ar.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dz.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iu.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ep.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ez.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://og.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jw.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rl.nicolike.cn

[C10] 变量作用域
来源：http://hz.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zb.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zf.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wu.asd995.cn

TS:   同 JS
来源：http://uz.huanxung.cn

Java: 方法内为块级作用域
来源：http://ur.wgjwhj.cn

Go:   花括号块级作用域
来源：http://ay.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gl.nszjky.cn

C#:   块级作用域
来源：http://pi.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://bz.shtwfgs.cn

Py:   from module import func
来源：http://ao.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aa.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vw.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yy.jctech888.com.cn

Java: import java.util.List;
来源：http://uy.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nu.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://nx.hnjuh.cn

C#:   using System.Text;
来源：http://jt.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://gi.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://ml.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://ce.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ga.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://qv.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vn.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://yo.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://sy.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://an.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://zg.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jd.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://um.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cx.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mz.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://af.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://rc.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rl.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ko.jctech888.com.cn

[C14] 泛型函数
来源：http://xv.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kx.wgjwhj.cn

PHP:  // 无泛型
来源：http://rn.jianghongdianzi.cn

JS:   // 无泛型
来源：http://zv.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lx.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bt.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dl.szsharing.cn

Ruby: # 无泛型
来源：http://ac.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ue.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://so.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://it.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://lj.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ku.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://td.asd995.cn

Java: // 无解构
来源：http://qf.bookmarksfly.cn

Go:   // 无解构
来源：http://gh.lnxyls.cn

Ruby: a, b = pair
来源：http://dj.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://hv.newstarts.cn

[C16] 函数 / 方法重载
来源：http://dt.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ix.jctech888.com.cn

PHP:  // 无重载
来源：http://hg.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cz.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://ha.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pm.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://ux.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://yp.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kr.chemitech.net.cn

================================================================================
来源：http://ba.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://ao.huixiangedu.cn

================================================================================
来源：http://ax.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://pr.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://np.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nl.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hi.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rj.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qo.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://fu.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://tk.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ih.521024.cn

[D02] 追加元素到末尾
来源：http://rb.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uh.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vj.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://sd.asd995.cn

TS:   arr.push(4);
来源：http://us.bookmarksfly.cn

Java: list.add(4);
来源：http://na.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://ek.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://tx.haigaiapp.cn

C#:   list.Add(4);
来源：http://wz.nicolike.cn

[D03] 在指定位置插入元素
来源：http://fu.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://ls.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jk.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eb.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://gz.gzmigu.cn

Java: list.add(0, 0);
来源：http://rl.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ch.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://js.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://hq.szxytkj.cn

[D04] 删除元素
来源：http://dh.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bo.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jb.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sb.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://oe.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ix.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fa.asd995.cn


<!-- 参考信息 -->