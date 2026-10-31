代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sg.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://re.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dt.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uw.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dp.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vu.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mk.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://on.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pg.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vl.bookmarksfly.cn

[B07] while 循环
来源：http://gp.colortex.cn

Py:   while i < 10: i += 1
来源：http://hd.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ja.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://yu.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://ez.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://fi.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bo.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://xw.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://jc.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://re.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://oy.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rw.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://ze.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://ai.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://mx.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oo.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uv.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://kd.yuexingan06.cn

[B09] break 与 continue
来源：http://kj.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ij.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nc.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xa.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bf.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mk.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pu.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sh.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mt.colortex.cn

[B10] 遍历同时拿索引
来源：http://gj.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hv.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yd.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hq.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qc.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qj.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lv.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pc.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bf.521024.cn

[B11] 生成数字序列 / 区间
来源：http://kh.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://sd.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://zw.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://id.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nb.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qh.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cv.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://ih.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pw.shxzskj.cn

[B12] 跳出多层循环
来源：http://ge.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gp.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tp.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sc.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xp.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xe.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xd.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gw.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wc.asd995.cn

[B13] 判断是否为数字
来源：http://nt.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://zu.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://wy.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uy.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sa.yuntaijiaju.cn

Java: x instanceof Number
来源：http://zm.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yb.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://el.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://xk.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://xt.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bc.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pg.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://yb.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://gb.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zm.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://al.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ng.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gd.panjiajie.cn

[B15] 布尔运算与取反
来源：http://nu.lnxyls.cn

Py:   a and b or not c
来源：http://um.colortex.cn

PHP:  $a && $b || !$c
来源：http://vs.szsharing.cn

JS:   a && b || !c
来源：http://hy.hnjuh.cn

TS:   a && b || !c
来源：http://iy.yuntaijiaju.cn

Java: a && b || !c
来源：http://jk.huanxung.cn

Go:   a && b || !c
来源：http://tf.nicolike.cn

Ruby: a && b || !c
来源：http://yi.9csxet.cn

C#:   a && b || !c
来源：http://wl.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tj.szsharing.cn

Py:   if not data: return
来源：http://mb.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://zm.shtwfgs.cn

JS:   if (!data) return;
来源：http://he.shtwfgs.cn

TS:   if (!data) return;
来源：http://ar.shtwfgs.cn

Java: if (data == null) return;
来源：http://ba.nicolike.cn

Go:   if data == nil { return }
来源：http://lq.colortex.cn

Ruby: return if data.nil?
来源：http://fx.9csxet.cn

C#:   if (data == null) return;
来源：http://bc.chemitech.net.cn

================================================================================
来源：http://ds.9csxet.cn

C. 函数与作用域
来源：http://bd.521024.cn

================================================================================
来源：http://nh.yuntaijiaju.cn

[C01] 定义函数
来源：http://ax.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://rs.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bj.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://yr.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vt.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://le.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vs.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://tt.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ln.nszjky.cn

[C02] 默认参数
来源：http://yr.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://ou.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://od.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://su.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fi.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://is.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gv.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://ou.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://gk.521024.cn

[C03] 可变参数
来源：http://ex.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://go.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mw.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xa.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mr.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iz.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ho.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qk.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ut.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://qk.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hx.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lc.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ap.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eq.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://sp.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://pn.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://af.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://qk.9csxet.cn

[C05] 返回多个值
来源：http://dy.wgjwhj.cn

Py:   return a, b
来源：http://uj.9csxet.cn

PHP:  return [$a, $b];
来源：http://bq.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ix.nicolike.cn

TS:   return { a, b };
来源：http://bs.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sx.haigaiapp.cn

Go:   return a, b
来源：http://uv.yuexingan06.cn

Ruby: return a, b
来源：http://yb.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://vm.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://ez.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://pv.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wm.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://gg.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://vc.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yc.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pd.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://cu.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ws.huanxung.cn

[C07] 把函数作为参数传入
来源：http://jd.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oa.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zc.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qu.9csxet.cn

TS:   arr.map(String)
来源：http://wb.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tg.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xr.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://yg.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zq.yuntaijiaju.cn

[C08] 闭包
来源：http://bz.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wi.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ph.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://av.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mq.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uf.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jv.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ay.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ma.nicolike.cn

[C09] 递归
来源：http://kd.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://di.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oy.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rv.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ue.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ib.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gf.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jo.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tq.panjiajie.cn

[C10] 变量作用域
来源：http://qr.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://za.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://el.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fx.chemitech.net.cn

TS:   同 JS
来源：http://ti.521024.cn

Java: 方法内为块级作用域
来源：http://ql.chemitech.net.cn

Go:   花括号块级作用域
来源：http://zm.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kl.jianghongdianzi.cn

C#:   块级作用域
来源：http://xn.colortex.cn

[C11] 模块导入与导出
来源：http://lw.hnjuh.cn

Py:   from module import func
来源：http://pr.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sq.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ig.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sm.hahajie.cn

Java: import java.util.List;
来源：http://ow.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ux.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://pl.lnxyls.cn

C#:   using System.Text;
来源：http://mv.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://mr.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://ww.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://xv.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://de.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://qt.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ua.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://nd.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://yz.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bp.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://ct.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fu.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bc.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hk.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ug.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cj.colortex.cn

Go:   func add(a, b int) int
来源：http://sj.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vo.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wn.hnjuh.cn

[C14] 泛型函数
来源：http://ry.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ir.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://pe.colortex.cn

JS:   // 无泛型
来源：http://sg.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vo.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://od.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pk.szsharing.cn

Ruby: # 无泛型
来源：http://ac.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nm.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://cw.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kk.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://sx.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gp.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qc.shxzukj.cn

Java: // 无解构
来源：http://at.yuexingan06.cn

Go:   // 无解构
来源：http://by.521024.cn

Ruby: a, b = pair
来源：http://fn.hahajie.cn

C#:   var (a, b) = pair;
来源：http://ui.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://vb.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fs.huanxung.cn

PHP:  // 无重载
来源：http://ag.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qt.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://xf.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ql.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://ht.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://aq.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jl.wgjwhj.cn

================================================================================
来源：http://bz.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://mj.shxzskj.cn

================================================================================
来源：http://xm.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://jj.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dv.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xe.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gr.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ml.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nj.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://xo.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://lc.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fl.asd995.cn

[D02] 追加元素到末尾
来源：http://sb.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tf.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zn.nicolike.cn

JS:   arr.push(4);
来源：http://zk.521024.cn

TS:   arr.push(4);
来源：http://rn.asd995.cn

Java: list.add(4);
来源：http://vs.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://pl.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://eu.shxzskj.cn

C#:   list.Add(4);
来源：http://hb.nszjky.cn

[D03] 在指定位置插入元素
来源：http://qn.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://is.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jw.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dn.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://av.haigaiapp.cn

Java: list.add(0, 0);
来源：http://ik.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qh.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ql.521024.cn

C#:   list.Insert(0, 0);
来源：http://un.szxytkj.cn

[D04] 删除元素
来源：http://fd.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vl.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jt.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://st.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://fr.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ug.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wt.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ou.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xk.panjiajie.cn

[D05] 访问与修改元素
来源：http://ys.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wc.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hw.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vs.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ur.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://xf.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://lg.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hr.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vq.jianghongdianzi.cn

[D06] 数组长度
来源：http://me.huixiangedu.cn

Py:   len(arr)
来源：http://ky.shxzukj.cn

PHP:  count($arr);
来源：http://ws.newstarts.cn

JS:   arr.length
来源：http://eo.bjjhwx.cn

TS:   arr.length
来源：http://xo.huanxung.cn


<!-- 参考信息 -->