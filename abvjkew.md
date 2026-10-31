代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ua.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://fy.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://do.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qo.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nz.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://al.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hj.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zk.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sc.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bw.jctech888.com.cn

[B07] while 循环
来源：http://wr.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://us.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ez.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://fs.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://za.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://zy.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ky.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://il.521024.cn

C#:   while (i < 10) { i++; }
来源：http://fx.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://bq.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ye.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pt.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://gn.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://mh.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://ka.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jg.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cy.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://tk.haigaiapp.cn

[B09] break 与 continue
来源：http://jg.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ee.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ys.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uu.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pw.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ol.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qs.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ik.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tl.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://mx.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://li.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uj.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hy.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://on.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gh.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tp.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fv.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ji.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://fu.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://kc.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://yz.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wm.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bx.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hm.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://re.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://kr.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hk.shxzukj.cn

[B12] 跳出多层循环
来源：http://yl.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vy.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uz.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dl.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dq.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vz.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zv.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iq.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nz.newstarts.cn

[B13] 判断是否为数字
来源：http://ou.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://vs.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://js.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fi.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pm.bjjhwx.cn

Java: x instanceof Number
来源：http://lc.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://au.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://ta.nszjky.cn

C#:   x is int or double or decimal
来源：http://sm.521024.cn

[B14] 判断值是否在集合内
来源：http://ua.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jq.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://re.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://bl.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://dc.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mg.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wb.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zv.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mv.newstarts.cn

[B15] 布尔运算与取反
来源：http://ka.huanxung.cn

Py:   a and b or not c
来源：http://ag.newstarts.cn

PHP:  $a && $b || !$c
来源：http://uq.szsharing.cn

JS:   a && b || !c
来源：http://bu.yuntaijiaju.cn

TS:   a && b || !c
来源：http://tt.jianghongdianzi.cn

Java: a && b || !c
来源：http://ba.yuexingan06.cn

Go:   a && b || !c
来源：http://jf.huanxung.cn

Ruby: a && b || !c
来源：http://si.colortex.cn

C#:   a && b || !c
来源：http://sh.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uz.yuntaijiaju.cn

Py:   if not data: return
来源：http://ja.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://ro.9csxet.cn

JS:   if (!data) return;
来源：http://xk.colortex.cn

TS:   if (!data) return;
来源：http://bb.hnjuh.cn

Java: if (data == null) return;
来源：http://iq.shtwfgs.cn

Go:   if data == nil { return }
来源：http://al.gzmigu.cn

Ruby: return if data.nil?
来源：http://mq.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://om.nszjky.cn

================================================================================
来源：http://pp.lnxyls.cn

C. 函数与作用域
来源：http://sn.shxzskj.cn

================================================================================
来源：http://mm.asd995.cn

[C01] 定义函数
来源：http://ra.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://yj.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sn.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://oe.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xy.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://um.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zb.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://sx.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://si.jianghongdianzi.cn

[C02] 默认参数
来源：http://xl.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://ia.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tw.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://va.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jl.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bf.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fh.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://to.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://xz.chemitech.net.cn

[C03] 可变参数
来源：http://cg.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://op.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dj.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qj.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jy.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://do.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jk.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fs.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dc.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://ub.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sy.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nk.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://us.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ua.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://hk.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://cp.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://vs.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://nm.bjjhwx.cn

[C05] 返回多个值
来源：http://xe.asd995.cn

Py:   return a, b
来源：http://aa.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://lp.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hs.jctech888.com.cn

TS:   return { a, b };
来源：http://cs.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ar.lnxyls.cn

Go:   return a, b
来源：http://yc.nicolike.cn

Ruby: return a, b
来源：http://nb.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://wb.asd995.cn

[C06] 匿名函数 / lambda
来源：http://jp.nszjky.cn

Py:   square = lambda x: x * x
来源：http://le.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dh.shxzskj.cn

JS:   const square = x => x * x;
来源：http://th.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ob.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dv.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://po.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://ea.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pe.nszjky.cn

[C07] 把函数作为参数传入
来源：http://oc.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hl.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ji.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://su.huixiangedu.cn

TS:   arr.map(String)
来源：http://mc.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://me.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xt.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://ni.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tx.9csxet.cn

[C08] 闭包
来源：http://gw.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://le.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zb.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nh.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fg.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tq.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lo.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yq.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sd.bjjhwx.cn

[C09] 递归
来源：http://kb.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sv.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mr.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rj.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gs.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://af.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://og.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xx.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nm.muxihuayi.cn

[C10] 变量作用域
来源：http://mq.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ug.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lw.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rc.szsharing.cn

TS:   同 JS
来源：http://ad.szsharing.cn

Java: 方法内为块级作用域
来源：http://lp.gzmigu.cn

Go:   花括号块级作用域
来源：http://yd.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lq.huanxung.cn

C#:   块级作用域
来源：http://jj.szsharing.cn

[C11] 模块导入与导出
来源：http://tt.jctech888.com.cn

Py:   from module import func
来源：http://hf.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jx.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://et.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rg.szxytkj.cn

Java: import java.util.List;
来源：http://oo.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lc.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://lu.nszjky.cn

C#:   using System.Text;
来源：http://uk.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://nd.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://pd.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://kp.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://ei.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://eo.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ny.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://qr.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://fm.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://va.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://mf.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hr.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ag.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://up.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vs.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rh.colortex.cn

Go:   func add(a, b int) int
来源：http://gu.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tn.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tj.jianghongdianzi.cn

[C14] 泛型函数
来源：http://sr.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zj.asd995.cn

PHP:  // 无泛型
来源：http://lt.hahajie.cn

JS:   // 无泛型
来源：http://hk.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vn.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://da.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ni.hahajie.cn

Ruby: # 无泛型
来源：http://ow.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zq.521024.cn

[C15] 解构 / 展开参数
来源：http://vv.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tu.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://uw.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://en.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iz.colortex.cn

Java: // 无解构
来源：http://vl.shxzukj.cn

Go:   // 无解构
来源：http://al.hahajie.cn

Ruby: a, b = pair
来源：http://tg.szsharing.cn

C#:   var (a, b) = pair;
来源：http://uq.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://jw.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ce.yuntaijiaju.cn

PHP:  // 无重载
来源：http://bd.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eb.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://wt.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xl.521024.cn

Go:   // 无重载：用不同函数名
来源：http://xk.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://cz.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lv.asd995.cn

================================================================================
来源：http://mp.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://yz.newstarts.cn

================================================================================
来源：http://nk.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://yh.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wu.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iv.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vo.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sx.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gd.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://ey.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://ux.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sg.newstarts.cn

[D02] 追加元素到末尾
来源：http://ew.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sg.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sw.9csxet.cn

JS:   arr.push(4);
来源：http://lu.haigaiapp.cn

TS:   arr.push(4);
来源：http://lo.huixiangedu.cn

Java: list.add(4);
来源：http://ck.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://au.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://op.huanxung.cn

C#:   list.Add(4);
来源：http://hs.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://oc.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://ez.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fe.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://it.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://vk.hnjuh.cn

Java: list.add(0, 0);
来源：http://ej.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pe.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yi.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://pp.yuexingan06.cn

[D04] 删除元素
来源：http://fn.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pt.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://me.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://py.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://rx.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xl.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wq.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ex.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fn.nicolike.cn

[D05] 访问与修改元素
来源：http://ya.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://os.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cb.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ey.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://tb.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://lf.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://xm.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qa.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eb.hnjuh.cn

[D06] 数组长度
来源：http://hk.9csxet.cn

Py:   len(arr)
来源：http://rc.huixinmuqiang.cn

PHP:  count($arr);
来源：http://jd.lnxyls.cn

JS:   arr.length
来源：http://zs.huixiangedu.cn

TS:   arr.length
来源：http://zp.huixiangedu.cn


<!-- 参考信息 -->