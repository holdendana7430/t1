代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iz.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xq.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://nx.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zb.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://iq.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://le.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jz.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lr.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xh.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vi.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mh.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://un.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sn.asd995.cn

[B06] 遍历字典 / 对象
来源：http://ik.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ok.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fz.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ql.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vo.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bj.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dy.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jw.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xg.lnxyls.cn

[B07] while 循环
来源：http://cd.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://qi.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ag.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://kg.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://td.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://nw.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vz.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://mg.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://lz.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://le.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://fl.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jn.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://tv.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://xs.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://qn.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ac.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zw.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://rh.chemitech.net.cn

[B09] break 与 continue
来源：http://bh.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ql.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xo.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gc.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yq.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://by.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ig.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cd.hahajie.cn

[B10] 遍历同时拿索引
来源：http://bo.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pw.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ed.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ht.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rj.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wt.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gh.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nn.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dk.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://wx.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://ct.521024.cn

PHP:  range(0, 10, 2);
来源：http://uq.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ko.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bv.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zu.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dw.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://we.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lx.nicolike.cn

[B12] 跳出多层循环
来源：http://yi.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ig.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nc.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ub.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qc.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cc.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bb.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sd.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wv.szxytkj.cn

[B13] 判断是否为数字
来源：http://ap.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://zv.lnxyls.cn

PHP:  is_numeric($x)
来源：http://zn.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mo.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bw.lnxyls.cn

Java: x instanceof Number
来源：http://kv.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xm.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://dr.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://ai.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://tc.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oj.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ej.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://uj.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://ab.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ej.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dh.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qp.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wo.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://ao.szxytkj.cn

Py:   a and b or not c
来源：http://xq.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://ef.colortex.cn

JS:   a && b || !c
来源：http://gc.hahajie.cn

TS:   a && b || !c
来源：http://kl.chemitech.net.cn

Java: a && b || !c
来源：http://gf.nicolike.cn

Go:   a && b || !c
来源：http://ix.gzmigu.cn

Ruby: a && b || !c
来源：http://ao.colortex.cn

C#:   a && b || !c
来源：http://gq.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zv.bookmarksfly.cn

Py:   if not data: return
来源：http://qq.521024.cn

PHP:  if (!$data) { return; }
来源：http://gj.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://nm.nicolike.cn

TS:   if (!data) return;
来源：http://df.bjjhwx.cn

Java: if (data == null) return;
来源：http://bt.asd995.cn

Go:   if data == nil { return }
来源：http://vk.newstarts.cn

Ruby: return if data.nil?
来源：http://wo.newstarts.cn

C#:   if (data == null) return;
来源：http://cx.bjjhwx.cn

================================================================================
来源：http://xl.huixiangedu.cn

C. 函数与作用域
来源：http://fy.wgjwhj.cn

================================================================================
来源：http://pf.yuexingan06.cn

[C01] 定义函数
来源：http://qk.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://dl.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zc.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://dh.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://og.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eo.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mm.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://yb.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ul.yuexingan06.cn

[C02] 默认参数
来源：http://oh.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://gt.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rr.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://ie.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pq.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yx.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tw.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://un.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ca.shxzukj.cn

[C03] 可变参数
来源：http://kw.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://nw.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ng.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yd.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gu.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zf.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gw.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zl.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rm.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://ed.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dl.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://np.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hp.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gm.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://vm.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://yq.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://fd.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://oa.hnjuh.cn

[C05] 返回多个值
来源：http://po.haigaiapp.cn

Py:   return a, b
来源：http://hy.colortex.cn

PHP:  return [$a, $b];
来源：http://iq.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://al.huixiangedu.cn

TS:   return { a, b };
来源：http://we.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://or.bookmarksfly.cn

Go:   return a, b
来源：http://hb.nicolike.cn

Ruby: return a, b
来源：http://yt.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://cg.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://to.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://wv.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://un.lnxyls.cn

JS:   const square = x => x * x;
来源：http://jj.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://zm.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pk.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hw.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://at.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tb.colortex.cn

[C07] 把函数作为参数传入
来源：http://af.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://im.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://su.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vi.nszjky.cn

TS:   arr.map(String)
来源：http://ff.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yv.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kp.521024.cn

Ruby: arr.map(&:upcase)
来源：http://za.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sd.yuexingan06.cn

[C08] 闭包
来源：http://qu.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rk.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sj.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://en.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zx.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ex.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vj.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bk.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oy.gzmigu.cn

[C09] 递归
来源：http://kt.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qo.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bp.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mu.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fw.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jp.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kv.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vy.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pb.hnjuh.cn

[C10] 变量作用域
来源：http://ro.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cm.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://af.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ie.panjiajie.cn

TS:   同 JS
来源：http://bl.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://ns.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://gw.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hp.521024.cn

C#:   块级作用域
来源：http://rx.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://rx.huanxung.cn

Py:   from module import func
来源：http://no.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fu.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gf.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tb.muxihuayi.cn

Java: import java.util.List;
来源：http://bj.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fy.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://eh.huixiangedu.cn

C#:   using System.Text;
来源：http://qu.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://wp.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://uj.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://ty.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://sh.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://zh.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ns.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://nr.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://mj.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cy.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://fk.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dk.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jw.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ej.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xk.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vu.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://zd.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wp.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jd.shtwfgs.cn

[C14] 泛型函数
来源：http://gz.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cz.shxzskj.cn

PHP:  // 无泛型
来源：http://uw.jianghongdianzi.cn

JS:   // 无泛型
来源：http://yl.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ip.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ij.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mg.nicolike.cn

Ruby: # 无泛型
来源：http://nb.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qc.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://py.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://du.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://sw.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ii.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gk.jctech888.com.cn

Java: // 无解构
来源：http://kb.jianghongdianzi.cn

Go:   // 无解构
来源：http://ah.huanxung.cn

Ruby: a, b = pair
来源：http://ou.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://kw.9csxet.cn

[C16] 函数 / 方法重载
来源：http://wf.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bq.shxzukj.cn

PHP:  // 无重载
来源：http://ur.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://se.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ej.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qt.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://fb.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://yy.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pd.521024.cn

================================================================================
来源：http://dr.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://sv.shxzukj.cn

================================================================================
来源：http://ax.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://zy.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vo.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kc.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lr.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ln.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://th.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://aa.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://to.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bs.szsharing.cn

[D02] 追加元素到末尾
来源：http://jr.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://co.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tf.szsharing.cn

JS:   arr.push(4);
来源：http://ws.wgjwhj.cn

TS:   arr.push(4);
来源：http://er.szsharing.cn

Java: list.add(4);
来源：http://dv.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://cb.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://tg.hnjuh.cn

C#:   list.Add(4);
来源：http://fk.newstarts.cn

[D03] 在指定位置插入元素
来源：http://rh.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://me.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tz.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yz.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://rz.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://lt.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xm.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bp.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://vi.hnjuh.cn

[D04] 删除元素
来源：http://de.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zt.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kf.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zo.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://kw.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ga.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ww.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wy.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ax.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://qs.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://be.gzmigu.cn


<!-- 参考信息 -->