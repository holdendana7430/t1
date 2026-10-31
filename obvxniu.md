代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kt.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://na.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vq.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mj.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ff.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://er.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://in.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fc.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bo.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kl.szxytkj.cn

[B07] while 循环
来源：http://ck.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://gq.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fy.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://le.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://iq.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://ea.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kb.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://wk.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://yy.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://at.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://bm.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gd.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://ov.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://sv.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://gv.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yg.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ea.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://ft.bookmarksfly.cn

[B09] break 与 continue
来源：http://vt.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xk.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ee.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uw.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ts.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://be.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qu.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://za.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://xh.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nd.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yo.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xd.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zz.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kb.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hk.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tp.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hg.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://sq.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://yr.asd995.cn

PHP:  range(0, 10, 2);
来源：http://ri.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ug.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yo.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hw.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kz.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://wg.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ic.bjjhwx.cn

[B12] 跳出多层循环
来源：http://po.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zk.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pn.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yy.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dp.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ks.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pu.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ps.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zq.gzmigu.cn

[B13] 判断是否为数字
来源：http://ae.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://us.nszjky.cn

PHP:  is_numeric($x)
来源：http://tx.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jb.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xv.szsharing.cn

Java: x instanceof Number
来源：http://cw.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ua.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://tr.gzmigu.cn

C#:   x is int or double or decimal
来源：http://zn.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://kw.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rj.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hs.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://wa.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://pz.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ss.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pt.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://to.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fs.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://cc.hahajie.cn

Py:   a and b or not c
来源：http://tq.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://lx.shxzukj.cn

JS:   a && b || !c
来源：http://vn.hahajie.cn

TS:   a && b || !c
来源：http://mi.bookmarksfly.cn

Java: a && b || !c
来源：http://fd.shxzukj.cn

Go:   a && b || !c
来源：http://cr.yuexingan06.cn

Ruby: a && b || !c
来源：http://re.panjiajie.cn

C#:   a && b || !c
来源：http://cn.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hs.newstarts.cn

Py:   if not data: return
来源：http://he.colortex.cn

PHP:  if (!$data) { return; }
来源：http://hj.shtwfgs.cn

JS:   if (!data) return;
来源：http://qb.chemitech.net.cn

TS:   if (!data) return;
来源：http://jz.panjiajie.cn

Java: if (data == null) return;
来源：http://bw.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://nn.asd995.cn

Ruby: return if data.nil?
来源：http://sf.chemitech.net.cn

C#:   if (data == null) return;
来源：http://fb.huanxung.cn

================================================================================
来源：http://xf.yuexingan06.cn

C. 函数与作用域
来源：http://oe.jianghongdianzi.cn

================================================================================
来源：http://kw.huanxung.cn

[C01] 定义函数
来源：http://tm.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://wk.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wn.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://aa.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ib.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://us.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ts.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://po.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yw.nicolike.cn

[C02] 默认参数
来源：http://ls.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://tf.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://do.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://nd.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ze.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bj.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bx.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://hd.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://fi.nszjky.cn

[C03] 可变参数
来源：http://nf.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://em.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zp.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ql.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://co.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ly.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://al.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rj.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hg.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://wu.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vx.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gr.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wq.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vo.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://my.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://pl.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://xb.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://ew.nszjky.cn

[C05] 返回多个值
来源：http://zt.colortex.cn

Py:   return a, b
来源：http://dc.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://wc.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pi.nszjky.cn

TS:   return { a, b };
来源：http://qv.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://py.shxzukj.cn

Go:   return a, b
来源：http://le.shxzskj.cn

Ruby: return a, b
来源：http://xh.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://qq.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://tt.huanxung.cn

Py:   square = lambda x: x * x
来源：http://rr.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://be.shxzskj.cn

JS:   const square = x => x * x;
来源：http://oq.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://gu.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://af.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qx.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://oq.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xn.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://vv.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yk.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lm.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uk.muxihuayi.cn

TS:   arr.map(String)
来源：http://oq.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qw.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ui.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://zz.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lu.yuexingan06.cn

[C08] 闭包
来源：http://sj.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ar.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ka.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://td.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dc.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tc.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rp.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bt.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jt.521024.cn

[C09] 递归
来源：http://nc.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yf.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mf.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uq.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ks.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ob.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qy.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wi.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pm.jctech888.com.cn

[C10] 变量作用域
来源：http://cj.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cg.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iv.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yo.shtwfgs.cn

TS:   同 JS
来源：http://ot.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://ks.nicolike.cn

Go:   花括号块级作用域
来源：http://tp.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bz.gzmigu.cn

C#:   块级作用域
来源：http://sa.huanxung.cn

[C11] 模块导入与导出
来源：http://fd.yuntaijiaju.cn

Py:   from module import func
来源：http://az.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mn.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vw.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://me.lnxyls.cn

Java: import java.util.List;
来源：http://ol.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qp.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://vr.panjiajie.cn

C#:   using System.Text;
来源：http://bu.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://xh.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://dn.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://wt.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://ah.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://su.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ww.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://ho.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://df.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rm.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://wx.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dl.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://az.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xf.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ll.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mt.huanxung.cn

Go:   func add(a, b int) int
来源：http://qi.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://la.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://an.shxzukj.cn

[C14] 泛型函数
来源：http://ko.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ko.asd995.cn

PHP:  // 无泛型
来源：http://dp.hnjuh.cn

JS:   // 无泛型
来源：http://lb.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vt.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vy.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ug.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://ny.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yz.hahajie.cn

[C15] 解构 / 展开参数
来源：http://iq.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bd.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://nk.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xb.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ly.huanxung.cn

Java: // 无解构
来源：http://af.shtwfgs.cn

Go:   // 无解构
来源：http://nf.muxihuayi.cn

Ruby: a, b = pair
来源：http://yt.colortex.cn

C#:   var (a, b) = pair;
来源：http://zk.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://ah.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tj.chemitech.net.cn

PHP:  // 无重载
来源：http://xb.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xq.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ko.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hf.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://wr.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://ml.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zn.yuexingan06.cn

================================================================================
来源：http://xy.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://xe.9csxet.cn

================================================================================
来源：http://ge.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://zq.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jw.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gr.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ne.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ph.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kn.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://tr.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://im.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://km.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://jm.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eb.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ai.hahajie.cn

JS:   arr.push(4);
来源：http://op.newstarts.cn

TS:   arr.push(4);
来源：http://hb.9csxet.cn

Java: list.add(4);
来源：http://tf.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://mg.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://ue.521024.cn

C#:   list.Add(4);
来源：http://fp.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://iq.521024.cn

Py:   arr.insert(0, 0)
来源：http://hk.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ql.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kf.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://hr.asd995.cn

Java: list.add(0, 0);
来源：http://su.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zu.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qj.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ef.haigaiapp.cn

[D04] 删除元素
来源：http://xi.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dg.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://of.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ti.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://wx.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gv.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cd.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bs.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://at.chemitech.net.cn

[D05] 访问与修改元素
来源：http://of.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ph.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gk.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ts.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ty.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://uf.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://mz.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pi.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oy.bookmarksfly.cn

[D06] 数组长度
来源：http://pf.szxytkj.cn

Py:   len(arr)
来源：http://gr.asd995.cn

PHP:  count($arr);
来源：http://gl.yuntaijiaju.cn

JS:   arr.length
来源：http://hw.chemitech.net.cn

TS:   arr.length
来源：http://ye.9csxet.cn


<!-- 参考信息 -->