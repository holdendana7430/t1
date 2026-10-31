代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iu.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vx.szxytkj.cn

[B07] while 循环
来源：http://ux.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://ol.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ko.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://kj.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://yq.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://hx.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ol.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://aa.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://ue.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://kv.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://bo.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://we.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://ln.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://ve.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://ry.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tr.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ig.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://th.haigaiapp.cn

[B09] break 与 continue
来源：http://th.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cc.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ic.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gv.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wx.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ks.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gt.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yc.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://fb.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cq.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cs.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xp.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xn.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oe.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qy.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nz.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vf.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://mm.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://hh.colortex.cn

PHP:  range(0, 10, 2);
来源：http://tg.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fs.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gn.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://em.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uz.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://rv.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zv.nicolike.cn

[B12] 跳出多层循环
来源：http://lq.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dc.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gd.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ao.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oy.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dg.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ha.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bq.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gp.9csxet.cn

[B13] 判断是否为数字
来源：http://gs.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://zt.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://bn.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bf.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ey.szxytkj.cn

Java: x instanceof Number
来源：http://ii.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://py.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://lz.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://gb.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://fh.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tn.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nt.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://fg.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://kd.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xy.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ai.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gs.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tk.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://rj.chemitech.net.cn

Py:   a and b or not c
来源：http://yb.521024.cn

PHP:  $a && $b || !$c
来源：http://fy.huixiangedu.cn

JS:   a && b || !c
来源：http://vi.hnjuh.cn

TS:   a && b || !c
来源：http://iq.gzmigu.cn

Java: a && b || !c
来源：http://jr.shxzukj.cn

Go:   a && b || !c
来源：http://sd.colortex.cn

Ruby: a && b || !c
来源：http://be.hnjuh.cn

C#:   a && b || !c
来源：http://zb.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qr.521024.cn

Py:   if not data: return
来源：http://ir.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://re.szsharing.cn

JS:   if (!data) return;
来源：http://lk.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://ok.bookmarksfly.cn

Java: if (data == null) return;
来源：http://ph.asd995.cn

Go:   if data == nil { return }
来源：http://sj.szsharing.cn

Ruby: return if data.nil?
来源：http://kw.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://yu.nicolike.cn

================================================================================
来源：http://cc.521024.cn

C. 函数与作用域
来源：http://dm.asd995.cn

================================================================================
来源：http://jf.huixiangedu.cn

[C01] 定义函数
来源：http://ca.521024.cn

Py:   def add(a, b): return a + b
来源：http://zo.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://us.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://it.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://je.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xp.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vj.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://yp.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ah.shxzukj.cn

[C02] 默认参数
来源：http://kk.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://zo.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pj.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://rx.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://by.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ew.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://se.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://fk.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://te.wgjwhj.cn

[C03] 可变参数
来源：http://ix.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://bd.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cq.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sm.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yr.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rk.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ec.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sj.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ti.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://yt.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eu.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ko.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lf.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dx.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://rh.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://cg.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://kw.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://jx.jianghongdianzi.cn

[C05] 返回多个值
来源：http://uw.colortex.cn

Py:   return a, b
来源：http://yu.asd995.cn

PHP:  return [$a, $b];
来源：http://zg.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jp.yuexingan06.cn

TS:   return { a, b };
来源：http://tf.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ua.huanxung.cn

Go:   return a, b
来源：http://gp.nicolike.cn

Ruby: return a, b
来源：http://of.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://bs.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://iu.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://ap.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ad.shxzskj.cn

JS:   const square = x => x * x;
来源：http://jv.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://xh.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bo.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ki.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://br.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cf.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://bh.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dd.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xz.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://za.bjjhwx.cn

TS:   arr.map(String)
来源：http://na.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bj.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ul.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://at.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lh.asd995.cn

[C08] 闭包
来源：http://og.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://um.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wc.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hs.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xb.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sy.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sy.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://li.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yl.yuntaijiaju.cn

[C09] 递归
来源：http://ck.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qu.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cb.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wu.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kp.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ch.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ah.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://no.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gv.jctech888.com.cn

[C10] 变量作用域
来源：http://gb.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hk.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gw.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wa.yuntaijiaju.cn

TS:   同 JS
来源：http://mu.colortex.cn

Java: 方法内为块级作用域
来源：http://px.hnjuh.cn

Go:   花括号块级作用域
来源：http://is.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://km.colortex.cn

C#:   块级作用域
来源：http://rg.9csxet.cn

[C11] 模块导入与导出
来源：http://bh.colortex.cn

Py:   from module import func
来源：http://jp.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zw.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://em.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nu.szxytkj.cn

Java: import java.util.List;
来源：http://fq.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lw.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://ej.muxihuayi.cn

C#:   using System.Text;
来源：http://ok.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://oh.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://ow.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://eo.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://yk.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://qo.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lz.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://jr.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://mi.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oy.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://et.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ma.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ko.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ql.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pn.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zc.asd995.cn

Go:   func add(a, b int) int
来源：http://fo.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rq.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yi.hnjuh.cn

[C14] 泛型函数
来源：http://yz.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dv.chemitech.net.cn

PHP:  // 无泛型
来源：http://up.chemitech.net.cn

JS:   // 无泛型
来源：http://iq.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://br.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ob.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wo.huixiangedu.cn

Ruby: # 无泛型
来源：http://yp.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vu.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://qx.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://so.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://eh.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ij.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mc.haigaiapp.cn

Java: // 无解构
来源：http://pc.huanxung.cn

Go:   // 无解构
来源：http://zk.muxihuayi.cn

Ruby: a, b = pair
来源：http://md.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://jk.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://zd.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sx.bjjhwx.cn

PHP:  // 无重载
来源：http://uy.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bl.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://kx.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://do.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://sl.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://cn.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jp.newstarts.cn

================================================================================
来源：http://rf.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://te.haigaiapp.cn

================================================================================
来源：http://or.huanxung.cn

[D01] 创建数组 / 列表
来源：http://vh.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hi.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://at.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ua.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sf.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cg.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://qo.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://zl.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ka.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://fz.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ij.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ih.bookmarksfly.cn

JS:   arr.push(4);
来源：http://xi.521024.cn

TS:   arr.push(4);
来源：http://qv.lnxyls.cn

Java: list.add(4);
来源：http://sy.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://tc.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://sd.bookmarksfly.cn

C#:   list.Add(4);
来源：http://xg.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://ac.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://ke.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nt.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pf.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://oj.muxihuayi.cn

Java: list.add(0, 0);
来源：http://qk.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yi.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uv.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://bo.9csxet.cn

[D04] 删除元素
来源：http://po.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xp.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wj.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jb.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://ux.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uy.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gf.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zp.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://or.9csxet.cn

[D05] 访问与修改元素
来源：http://dn.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://me.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://db.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ty.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://sm.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://kz.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://id.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://za.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zg.szxytkj.cn

[D06] 数组长度
来源：http://bt.newstarts.cn

Py:   len(arr)
来源：http://vm.nicolike.cn

PHP:  count($arr);
来源：http://bf.lnxyls.cn

JS:   arr.length
来源：http://jb.szsharing.cn

TS:   arr.length
来源：http://cy.szxytkj.cn

Java: list.size();
来源：http://mr.521024.cn

Go:   len(arr)
来源：http://ve.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://rp.jctech888.com.cn

C#:   list.Count;
来源：http://mm.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://ex.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xs.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uq.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://uo.newstarts.cn


<!-- 参考信息 -->