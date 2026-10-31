代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hh.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://do.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jw.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lx.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://te.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oy.huixinmuqiang.cn

[B07] while 循环
来源：http://ms.colortex.cn

Py:   while i < 10: i += 1
来源：http://gm.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dz.521024.cn

JS:   while (i < 10) { i++; }
来源：http://mk.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://mb.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://bm.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yc.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://ng.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://uy.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://px.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://jy.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zg.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://jj.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://qs.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://rp.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ai.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bt.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://eo.huixinmuqiang.cn

[B09] break 与 continue
来源：http://ga.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rl.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://la.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iu.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bk.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://og.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lh.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rx.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ze.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://wh.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sw.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ms.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oi.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mn.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hx.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://px.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vf.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ae.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://ue.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://zq.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://dp.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gl.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ck.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://or.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qa.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://gy.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ji.chemitech.net.cn

[B12] 跳出多层循环
来源：http://yb.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xf.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ct.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uk.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fk.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xt.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ra.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jb.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sa.lnxyls.cn

[B13] 判断是否为数字
来源：http://hz.521024.cn

Py:   isinstance(x, (int, float))
来源：http://jx.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://ml.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mu.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nh.hahajie.cn

Java: x instanceof Number
来源：http://vk.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cn.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://lr.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://dj.521024.cn

[B14] 判断值是否在集合内
来源：http://qp.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mu.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vd.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://uz.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://gj.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zz.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nh.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rs.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eo.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://lv.shtwfgs.cn

Py:   a and b or not c
来源：http://rw.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://yt.9csxet.cn

JS:   a && b || !c
来源：http://hq.9csxet.cn

TS:   a && b || !c
来源：http://tb.hnjuh.cn

Java: a && b || !c
来源：http://rj.hahajie.cn

Go:   a && b || !c
来源：http://ke.colortex.cn

Ruby: a && b || !c
来源：http://ji.bookmarksfly.cn

C#:   a && b || !c
来源：http://hi.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ed.shxzukj.cn

Py:   if not data: return
来源：http://ua.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://ey.nszjky.cn

JS:   if (!data) return;
来源：http://jw.521024.cn

TS:   if (!data) return;
来源：http://ty.nszjky.cn

Java: if (data == null) return;
来源：http://sj.hnjuh.cn

Go:   if data == nil { return }
来源：http://yg.shxzukj.cn

Ruby: return if data.nil?
来源：http://xl.lnxyls.cn

C#:   if (data == null) return;
来源：http://ec.szsharing.cn

================================================================================
来源：http://yu.haigaiapp.cn

C. 函数与作用域
来源：http://nh.nszjky.cn

================================================================================
来源：http://ok.szsharing.cn

[C01] 定义函数
来源：http://sm.asd995.cn

Py:   def add(a, b): return a + b
来源：http://qd.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zg.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://xp.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ek.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cd.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tg.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://gy.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ll.szxytkj.cn

[C02] 默认参数
来源：http://ph.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://hn.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dw.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ve.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bl.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jz.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fk.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://ui.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ns.shtwfgs.cn

[C03] 可变参数
来源：http://xx.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://vk.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hw.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dv.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lt.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xm.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://na.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ge.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qk.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://lk.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ki.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vu.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rt.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yf.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://aw.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://zz.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ci.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://gd.chemitech.net.cn

[C05] 返回多个值
来源：http://oa.shtwfgs.cn

Py:   return a, b
来源：http://qm.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://rh.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ps.wgjwhj.cn

TS:   return { a, b };
来源：http://gx.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://on.szsharing.cn

Go:   return a, b
来源：http://ku.yuexingan06.cn

Ruby: return a, b
来源：http://qy.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://po.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://xr.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://fp.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iy.shxzskj.cn

JS:   const square = x => x * x;
来源：http://la.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://we.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xs.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mj.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://ib.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ts.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://fp.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pn.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://do.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xd.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://vf.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://op.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ar.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://oo.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ab.bjjhwx.cn

[C08] 闭包
来源：http://fm.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xs.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rh.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gq.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://to.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zg.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ld.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jo.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ry.jianghongdianzi.cn

[C09] 递归
来源：http://dp.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://od.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://by.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vn.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qu.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://an.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jg.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vf.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rk.yuexingan06.cn

[C10] 变量作用域
来源：http://jg.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jj.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uj.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lr.shxzskj.cn

TS:   同 JS
来源：http://jb.lnxyls.cn

Java: 方法内为块级作用域
来源：http://go.panjiajie.cn

Go:   花括号块级作用域
来源：http://pv.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mq.szxytkj.cn

C#:   块级作用域
来源：http://ff.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://nq.huixiangedu.cn

Py:   from module import func
来源：http://nz.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uf.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bn.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ib.bjjhwx.cn

Java: import java.util.List;
来源：http://og.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dl.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://mn.huanxung.cn

C#:   using System.Text;
来源：http://ao.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://kh.521024.cn

Py:   (lambda: print("run"))()
来源：http://ra.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://yi.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://tj.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://wd.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hx.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://gx.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://cq.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pw.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://iw.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lk.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://je.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eh.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dv.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rv.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://xi.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hf.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xz.haigaiapp.cn

[C14] 泛型函数
来源：http://aj.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://te.jctech888.com.cn

PHP:  // 无泛型
来源：http://lr.colortex.cn

JS:   // 无泛型
来源：http://lp.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kz.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bh.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qu.huixiangedu.cn

Ruby: # 无泛型
来源：http://bp.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tx.colortex.cn

[C15] 解构 / 展开参数
来源：http://cs.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pn.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://vj.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://au.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pn.yuexingan06.cn

Java: // 无解构
来源：http://si.nicolike.cn

Go:   // 无解构
来源：http://ov.hnjuh.cn

Ruby: a, b = pair
来源：http://ix.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://wv.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://rq.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tl.521024.cn

PHP:  // 无重载
来源：http://no.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cw.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://hc.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ao.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://gx.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://oe.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ws.newstarts.cn

================================================================================
来源：http://us.asd995.cn

D. 数组 / 列表 / 集合
来源：http://zq.szsharing.cn

================================================================================
来源：http://nf.huanxung.cn

[D01] 创建数组 / 列表
来源：http://fi.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ft.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ex.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vl.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zs.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xl.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://et.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://fj.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bk.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://mo.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wp.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cz.haigaiapp.cn

JS:   arr.push(4);
来源：http://ya.nszjky.cn

TS:   arr.push(4);
来源：http://jq.shxzskj.cn

Java: list.add(4);
来源：http://gd.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://cn.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://dk.hnjuh.cn

C#:   list.Add(4);
来源：http://uv.huanxung.cn

[D03] 在指定位置插入元素
来源：http://qd.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://ny.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eh.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ye.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://hq.shtwfgs.cn

Java: list.add(0, 0);
来源：http://yv.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gt.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ux.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://bl.yuexingan06.cn

[D04] 删除元素
来源：http://uk.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nq.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ph.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://if.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://dp.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sg.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sx.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vu.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cu.huanxung.cn

[D05] 访问与修改元素
来源：http://wt.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fn.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://re.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nh.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://vj.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://fl.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://tc.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kx.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xr.chemitech.net.cn

[D06] 数组长度
来源：http://zk.haigaiapp.cn

Py:   len(arr)
来源：http://yl.jianghongdianzi.cn

PHP:  count($arr);
来源：http://hu.colortex.cn

JS:   arr.length
来源：http://dk.szsharing.cn

TS:   arr.length
来源：http://bd.huixinmuqiang.cn

Java: list.size();
来源：http://bk.colortex.cn

Go:   len(arr)
来源：http://hz.colortex.cn

Ruby: arr.length; arr.size
来源：http://si.lnxyls.cn

C#:   list.Count;
来源：http://hz.jianghongdianzi.cn


<!-- 参考信息 -->