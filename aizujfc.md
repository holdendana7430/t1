代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://mp.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fb.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://th.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://kc.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ja.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://li.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://th.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yj.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rj.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zy.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iq.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ok.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yj.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oz.nicolike.cn

[B07] while 循环
来源：http://kt.szsharing.cn

Py:   while i < 10: i += 1
来源：http://ai.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ir.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://gr.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://qw.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://bm.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ba.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://rv.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://gv.521024.cn

[B08] do-while（至少执行一次）
来源：http://yk.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://no.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://me.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://xb.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://jy.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://wp.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ig.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eu.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://yd.nicolike.cn

[B09] break 与 continue
来源：http://cu.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fs.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uh.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ql.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://va.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xg.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rk.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hc.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://yd.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vf.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wd.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lc.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yv.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://li.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ky.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kw.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mo.521024.cn

[B11] 生成数字序列 / 区间
来源：http://wf.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://qo.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://vt.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yb.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sc.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ws.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mp.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://wr.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tq.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://ug.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rc.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pp.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kv.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://by.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tl.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cv.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ft.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xd.wgjwhj.cn

[B13] 判断是否为数字
来源：http://fw.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://pc.szsharing.cn

PHP:  is_numeric($x)
来源：http://wo.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://li.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iq.shxzskj.cn

Java: x instanceof Number
来源：http://cf.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aj.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://ql.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://am.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://av.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tl.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://um.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://tb.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://tm.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hq.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pk.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ip.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yq.lnxyls.cn

[B15] 布尔运算与取反
来源：http://ix.jianghongdianzi.cn

Py:   a and b or not c
来源：http://yn.asd995.cn

PHP:  $a && $b || !$c
来源：http://ze.nszjky.cn

JS:   a && b || !c
来源：http://gx.9csxet.cn

TS:   a && b || !c
来源：http://td.chemitech.net.cn

Java: a && b || !c
来源：http://td.huixinmuqiang.cn

Go:   a && b || !c
来源：http://ts.shxzukj.cn

Ruby: a && b || !c
来源：http://wr.chemitech.net.cn

C#:   a && b || !c
来源：http://sj.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://if.huixinmuqiang.cn

Py:   if not data: return
来源：http://zx.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://oj.wgjwhj.cn

JS:   if (!data) return;
来源：http://db.521024.cn

TS:   if (!data) return;
来源：http://aa.bjjhwx.cn

Java: if (data == null) return;
来源：http://fb.huanxung.cn

Go:   if data == nil { return }
来源：http://lt.bjjhwx.cn

Ruby: return if data.nil?
来源：http://iw.colortex.cn

C#:   if (data == null) return;
来源：http://hg.muxihuayi.cn

================================================================================
来源：http://cl.jctech888.com.cn

C. 函数与作用域
来源：http://ja.huixinmuqiang.cn

================================================================================
来源：http://ra.panjiajie.cn

[C01] 定义函数
来源：http://nb.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://km.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://by.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://bg.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qw.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://su.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gu.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://mu.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fx.521024.cn

[C02] 默认参数
来源：http://sg.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://pn.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vn.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://or.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ln.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mk.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lc.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://ik.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://fj.shxzukj.cn

[C03] 可变参数
来源：http://ot.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://cy.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qt.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qy.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cb.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yw.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lc.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zr.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sr.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://bt.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ce.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://su.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kb.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qh.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://oh.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://pj.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://dt.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://bc.szsharing.cn

[C05] 返回多个值
来源：http://dh.yuexingan06.cn

Py:   return a, b
来源：http://av.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://ze.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qd.bookmarksfly.cn

TS:   return { a, b };
来源：http://zd.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://js.shtwfgs.cn

Go:   return a, b
来源：http://ih.hahajie.cn

Ruby: return a, b
来源：http://ns.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://oz.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://od.newstarts.cn

Py:   square = lambda x: x * x
来源：http://fe.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gv.huanxung.cn

JS:   const square = x => x * x;
来源：http://bb.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://xd.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qr.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rv.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://ci.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pw.9csxet.cn

[C07] 把函数作为参数传入
来源：http://rx.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://il.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xh.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zp.panjiajie.cn

TS:   arr.map(String)
来源：http://eo.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sp.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vl.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://vw.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yq.szsharing.cn

[C08] 闭包
来源：http://vf.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ib.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jf.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ry.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uq.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nm.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jf.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ba.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pr.nicolike.cn

[C09] 递归
来源：http://jt.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mb.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oa.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dw.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://js.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://km.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bz.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://et.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sp.chemitech.net.cn

[C10] 变量作用域
来源：http://uu.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qu.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kp.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dy.jianghongdianzi.cn

TS:   同 JS
来源：http://hf.newstarts.cn

Java: 方法内为块级作用域
来源：http://di.shxzukj.cn

Go:   花括号块级作用域
来源：http://as.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://of.nicolike.cn

C#:   块级作用域
来源：http://cw.panjiajie.cn

[C11] 模块导入与导出
来源：http://ra.lnxyls.cn

Py:   from module import func
来源：http://qt.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hy.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zg.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ua.chemitech.net.cn

Java: import java.util.List;
来源：http://cx.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wq.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://yl.shtwfgs.cn

C#:   using System.Text;
来源：http://ol.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://dq.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://td.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://eh.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://vm.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://zd.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eb.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://qe.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://nf.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ae.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://af.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kd.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xk.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sh.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nu.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hq.colortex.cn

Go:   func add(a, b int) int
来源：http://zb.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mh.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ef.hahajie.cn

[C14] 泛型函数
来源：http://dm.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iy.nszjky.cn

PHP:  // 无泛型
来源：http://ow.szsharing.cn

JS:   // 无泛型
来源：http://sv.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dd.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ti.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jj.hahajie.cn

Ruby: # 无泛型
来源：http://gu.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fd.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://bn.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oj.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://hc.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://er.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zx.newstarts.cn

Java: // 无解构
来源：http://wc.haigaiapp.cn

Go:   // 无解构
来源：http://ah.nszjky.cn

Ruby: a, b = pair
来源：http://dv.newstarts.cn

C#:   var (a, b) = pair;
来源：http://bf.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://wp.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ie.bjjhwx.cn

PHP:  // 无重载
来源：http://uw.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tl.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://wt.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wd.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://rb.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://jd.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sc.yuexingan06.cn

================================================================================
来源：http://vd.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://vd.hahajie.cn

================================================================================
来源：http://ot.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://wk.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oj.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bx.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pw.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://an.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xc.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://vo.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://dx.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wr.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://dw.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vu.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xy.colortex.cn

JS:   arr.push(4);
来源：http://me.nicolike.cn

TS:   arr.push(4);
来源：http://wp.nszjky.cn

Java: list.add(4);
来源：http://jv.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://tt.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://lg.wgjwhj.cn

C#:   list.Add(4);
来源：http://zr.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://ek.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://ks.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yp.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ce.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://fr.panjiajie.cn

Java: list.add(0, 0);
来源：http://yu.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://id.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qy.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://sm.jianghongdianzi.cn

[D04] 删除元素
来源：http://sv.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ps.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xj.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wb.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://on.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iq.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xv.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ji.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jv.gzmigu.cn

[D05] 访问与修改元素
来源：http://mx.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://og.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uk.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://io.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://ax.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://uq.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://wy.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dd.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gx.colortex.cn

[D06] 数组长度
来源：http://lp.gzmigu.cn


<!-- 参考信息 -->