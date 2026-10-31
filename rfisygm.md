代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ah.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qx.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zz.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ec.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://no.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ei.muxihuayi.cn

[B07] while 循环
来源：http://qa.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://xf.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://be.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://hd.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://zf.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://lv.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fy.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://or.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://py.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://ib.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://gy.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jp.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://pa.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://qh.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://jw.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ys.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vb.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://bf.bjjhwx.cn

[B09] break 与 continue
来源：http://ur.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yq.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vf.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tg.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oj.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hc.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cj.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qp.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://ht.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hl.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cj.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aw.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fs.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xu.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vj.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ib.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ir.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://nb.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://dl.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://dh.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fn.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wf.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dz.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://be.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://xz.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zs.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://tw.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hf.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dq.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xb.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pa.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ej.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ss.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ng.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pq.szxytkj.cn

[B13] 判断是否为数字
来源：http://kj.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://jc.panjiajie.cn

PHP:  is_numeric($x)
来源：http://pw.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cc.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rb.shxzskj.cn

Java: x instanceof Number
来源：http://vu.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kx.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://ow.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://ru.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://kv.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qs.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bx.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://yp.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://fz.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tz.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://is.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ai.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oq.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://gz.jctech888.com.cn

Py:   a and b or not c
来源：http://kk.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://kt.lnxyls.cn

JS:   a && b || !c
来源：http://mq.nszjky.cn

TS:   a && b || !c
来源：http://xw.haigaiapp.cn

Java: a && b || !c
来源：http://ck.szsharing.cn

Go:   a && b || !c
来源：http://mb.nicolike.cn

Ruby: a && b || !c
来源：http://ir.wgjwhj.cn

C#:   a && b || !c
来源：http://wn.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://df.shxzskj.cn

Py:   if not data: return
来源：http://jx.521024.cn

PHP:  if (!$data) { return; }
来源：http://ou.lnxyls.cn

JS:   if (!data) return;
来源：http://bu.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://uq.nszjky.cn

Java: if (data == null) return;
来源：http://bl.chemitech.net.cn

Go:   if data == nil { return }
来源：http://di.yuexingan06.cn

Ruby: return if data.nil?
来源：http://ri.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://jc.nszjky.cn

================================================================================
来源：http://yz.hnjuh.cn

C. 函数与作用域
来源：http://cw.521024.cn

================================================================================
来源：http://qo.shxzskj.cn

[C01] 定义函数
来源：http://nq.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://mm.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rf.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://fy.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mr.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wz.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xj.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://iy.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gr.yuexingan06.cn

[C02] 默认参数
来源：http://lz.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://vy.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nb.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://zk.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yw.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ir.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bz.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://yh.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://cl.colortex.cn

[C03] 可变参数
来源：http://wb.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://oy.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zc.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jd.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://do.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vj.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ph.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://en.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lz.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://ej.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bu.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dc.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fz.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fx.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ct.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://kf.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://gr.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://fd.newstarts.cn

[C05] 返回多个值
来源：http://nh.shtwfgs.cn

Py:   return a, b
来源：http://vz.521024.cn

PHP:  return [$a, $b];
来源：http://gs.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lz.shxzukj.cn

TS:   return { a, b };
来源：http://um.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fh.jctech888.com.cn

Go:   return a, b
来源：http://ic.chemitech.net.cn

Ruby: return a, b
来源：http://ct.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://eg.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://is.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://bu.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pp.szsharing.cn

JS:   const square = x => x * x;
来源：http://ph.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://mc.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qf.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ip.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://au.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gn.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://ou.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oy.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mp.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bz.bookmarksfly.cn

TS:   arr.map(String)
来源：http://ys.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bz.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fx.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://ck.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ty.haigaiapp.cn

[C08] 闭包
来源：http://th.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jp.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pc.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vd.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mc.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://so.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yb.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ou.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://it.huanxung.cn

[C09] 递归
来源：http://zx.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kh.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qz.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mf.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dd.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rn.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kn.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tz.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yk.colortex.cn

[C10] 变量作用域
来源：http://ru.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yt.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vj.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://om.colortex.cn

TS:   同 JS
来源：http://yt.nszjky.cn

Java: 方法内为块级作用域
来源：http://rm.colortex.cn

Go:   花括号块级作用域
来源：http://lg.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://le.huixiangedu.cn

C#:   块级作用域
来源：http://ic.nszjky.cn

[C11] 模块导入与导出
来源：http://xa.9csxet.cn

Py:   from module import func
来源：http://wa.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hd.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sq.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gn.nicolike.cn

Java: import java.util.List;
来源：http://rw.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://na.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ax.szxytkj.cn

C#:   using System.Text;
来源：http://on.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://rq.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://ps.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://rl.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://pg.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://gx.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ok.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://hz.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://uc.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://on.521024.cn

[C13] 类型声明 / 类型注解
来源：http://nr.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mx.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yi.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fn.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://me.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pd.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://ia.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ih.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dh.muxihuayi.cn

[C14] 泛型函数
来源：http://xi.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fx.panjiajie.cn

PHP:  // 无泛型
来源：http://na.szxytkj.cn

JS:   // 无泛型
来源：http://yx.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wt.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xk.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uw.shxzukj.cn

Ruby: # 无泛型
来源：http://rh.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zg.hahajie.cn

[C15] 解构 / 展开参数
来源：http://iy.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jg.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://ei.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gg.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aj.huixiangedu.cn

Java: // 无解构
来源：http://wz.newstarts.cn

Go:   // 无解构
来源：http://vf.yuexingan06.cn

Ruby: a, b = pair
来源：http://ht.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://dq.521024.cn

[C16] 函数 / 方法重载
来源：http://xz.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tu.colortex.cn

PHP:  // 无重载
来源：http://lf.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ag.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://re.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dy.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://qq.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://mc.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ez.hahajie.cn

================================================================================
来源：http://pn.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://wt.9csxet.cn

================================================================================
来源：http://yl.nszjky.cn

[D01] 创建数组 / 列表
来源：http://iq.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uv.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rg.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://db.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bx.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://st.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://eq.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://pp.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ax.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://km.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xs.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ck.wgjwhj.cn

JS:   arr.push(4);
来源：http://vd.yuexingan06.cn

TS:   arr.push(4);
来源：http://vu.wgjwhj.cn

Java: list.add(4);
来源：http://op.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://et.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://ed.jctech888.com.cn

C#:   list.Add(4);
来源：http://xk.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://hp.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://iy.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tj.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://op.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://yv.shxzskj.cn

Java: list.add(0, 0);
来源：http://tr.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ab.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rs.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://vy.shtwfgs.cn

[D04] 删除元素
来源：http://cb.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fy.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oh.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lq.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://bf.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zj.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cq.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bb.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tg.shtwfgs.cn

[D05] 访问与修改元素
来源：http://gn.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ex.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jn.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ai.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://pr.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://oj.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://dl.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sb.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xv.wgjwhj.cn

[D06] 数组长度
来源：http://or.9csxet.cn

Py:   len(arr)
来源：http://nw.wgjwhj.cn

PHP:  count($arr);
来源：http://jo.shxzskj.cn

JS:   arr.length
来源：http://tc.hnjuh.cn

TS:   arr.length
来源：http://ig.521024.cn

Java: list.size();
来源：http://gf.hnjuh.cn

Go:   len(arr)
来源：http://fr.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://qk.asd995.cn

C#:   list.Count;
来源：http://ai.gzmigu.cn


<!-- 参考信息 -->