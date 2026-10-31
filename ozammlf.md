代发 wailian999

[B05] 遍历数组 / 列表
来源：http://yz.521024.cn

Py:   for item in arr: print(item)
来源：http://lg.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xf.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yw.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cc.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ni.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ef.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://cf.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://et.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://cy.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ck.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xb.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://id.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wa.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://re.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kl.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ud.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qa.lnxyls.cn

[B07] while 循环
来源：http://dl.521024.cn

Py:   while i < 10: i += 1
来源：http://si.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qm.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://xt.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://pp.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://xp.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://si.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://ab.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://fb.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://gi.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://bf.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://op.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://vn.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://ye.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://xo.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rs.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bs.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://oo.bookmarksfly.cn

[B09] break 与 continue
来源：http://uj.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cb.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ob.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jo.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mg.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xf.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zl.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qf.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qv.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://zu.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ju.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ul.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ko.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kn.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nt.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cr.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qn.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jt.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://yx.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://jh.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://ev.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qy.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yf.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fl.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bl.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://lr.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vv.lnxyls.cn

[B12] 跳出多层循环
来源：http://oq.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pp.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ph.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kg.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tl.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ab.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ta.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pl.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fl.521024.cn

[B13] 判断是否为数字
来源：http://xv.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://tb.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://sa.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cy.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gm.gzmigu.cn

Java: x instanceof Number
来源：http://gg.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uv.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://yf.521024.cn

C#:   x is int or double or decimal
来源：http://cr.9csxet.cn

[B14] 判断值是否在集合内
来源：http://gi.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xy.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tx.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ax.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://sf.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tp.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xa.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hm.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pl.shxzskj.cn

[B15] 布尔运算与取反
来源：http://us.9csxet.cn

Py:   a and b or not c
来源：http://vj.9csxet.cn

PHP:  $a && $b || !$c
来源：http://ac.521024.cn

JS:   a && b || !c
来源：http://fr.chemitech.net.cn

TS:   a && b || !c
来源：http://gc.lnxyls.cn

Java: a && b || !c
来源：http://sc.wgjwhj.cn

Go:   a && b || !c
来源：http://ih.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://ws.huixinmuqiang.cn

C#:   a && b || !c
来源：http://lk.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fr.szsharing.cn

Py:   if not data: return
来源：http://bn.asd995.cn

PHP:  if (!$data) { return; }
来源：http://qe.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://ko.bookmarksfly.cn

TS:   if (!data) return;
来源：http://aq.lnxyls.cn

Java: if (data == null) return;
来源：http://gp.yuexingan06.cn

Go:   if data == nil { return }
来源：http://vg.szsharing.cn

Ruby: return if data.nil?
来源：http://ed.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://fh.haigaiapp.cn

================================================================================
来源：http://hl.colortex.cn

C. 函数与作用域
来源：http://an.521024.cn

================================================================================
来源：http://nd.nicolike.cn

[C01] 定义函数
来源：http://ty.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://kv.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://no.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://zg.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ud.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ra.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ev.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://lh.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bp.nicolike.cn

[C02] 默认参数
来源：http://er.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://lj.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oy.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://is.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eu.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mg.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zj.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://xg.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://jg.yuexingan06.cn

[C03] 可变参数
来源：http://az.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://uu.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dn.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ed.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dv.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mc.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://su.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qx.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oq.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://yj.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kq.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xa.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dn.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bh.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://iw.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://vr.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://ih.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://dm.yuexingan06.cn

[C05] 返回多个值
来源：http://ju.huixiangedu.cn

Py:   return a, b
来源：http://mo.gzmigu.cn

PHP:  return [$a, $b];
来源：http://jd.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kn.huanxung.cn

TS:   return { a, b };
来源：http://ne.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ts.shxzukj.cn

Go:   return a, b
来源：http://dm.asd995.cn

Ruby: return a, b
来源：http://ez.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://yp.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://bh.newstarts.cn

Py:   square = lambda x: x * x
来源：http://lg.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eh.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://vi.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://dv.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qt.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://aq.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://ct.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xz.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://vx.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qm.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lo.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kr.nszjky.cn

TS:   arr.map(String)
来源：http://gu.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ih.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wl.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://zy.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ts.yuntaijiaju.cn

[C08] 闭包
来源：http://mj.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ky.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vd.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hj.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ag.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rf.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cj.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ru.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://et.colortex.cn

[C09] 递归
来源：http://hi.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jb.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hn.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ee.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eq.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ca.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qq.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mq.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ap.hahajie.cn

[C10] 变量作用域
来源：http://vm.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oi.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zg.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lx.bookmarksfly.cn

TS:   同 JS
来源：http://ud.gzmigu.cn

Java: 方法内为块级作用域
来源：http://ub.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://yg.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ml.colortex.cn

C#:   块级作用域
来源：http://dr.hahajie.cn

[C11] 模块导入与导出
来源：http://iy.jctech888.com.cn

Py:   from module import func
来源：http://sl.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ua.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rr.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ci.huixiangedu.cn

Java: import java.util.List;
来源：http://ux.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://at.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://ca.muxihuayi.cn

C#:   using System.Text;
来源：http://ga.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://xd.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://rb.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://jc.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://sh.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ik.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bx.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://ux.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://ks.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gx.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://ps.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zz.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xm.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oq.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://my.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oc.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://mk.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aa.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gl.huixinmuqiang.cn

[C14] 泛型函数
来源：http://ig.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ei.chemitech.net.cn

PHP:  // 无泛型
来源：http://xf.bookmarksfly.cn

JS:   // 无泛型
来源：http://qn.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fh.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vc.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rv.newstarts.cn

Ruby: # 无泛型
来源：http://bg.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ov.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://qw.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wv.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://ed.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://td.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ae.szsharing.cn

Java: // 无解构
来源：http://sg.521024.cn

Go:   // 无解构
来源：http://nq.yuexingan06.cn

Ruby: a, b = pair
来源：http://ob.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://in.colortex.cn

[C16] 函数 / 方法重载
来源：http://js.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zq.asd995.cn

PHP:  // 无重载
来源：http://xb.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ov.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://vp.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uj.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://qr.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://um.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ug.haigaiapp.cn

================================================================================
来源：http://ro.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://vz.huanxung.cn

================================================================================
来源：http://to.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://nn.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ys.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ld.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rr.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rq.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pu.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://zf.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://ng.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hv.szxytkj.cn

[D02] 追加元素到末尾
来源：http://zp.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tu.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lh.shxzukj.cn

JS:   arr.push(4);
来源：http://ia.gzmigu.cn

TS:   arr.push(4);
来源：http://tx.yuntaijiaju.cn

Java: list.add(4);
来源：http://mc.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://vr.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://ch.colortex.cn

C#:   list.Add(4);
来源：http://az.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://px.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://os.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://li.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cr.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://iq.colortex.cn

Java: list.add(0, 0);
来源：http://yx.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dz.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://an.colortex.cn

C#:   list.Insert(0, 0);
来源：http://iw.wgjwhj.cn

[D04] 删除元素
来源：http://fy.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kg.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gw.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pd.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://wj.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jw.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://se.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://en.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rg.szxytkj.cn

[D05] 访问与修改元素
来源：http://xq.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qf.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rl.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yo.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://im.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://bs.bookmarksfly.cn


<!-- 参考信息 -->