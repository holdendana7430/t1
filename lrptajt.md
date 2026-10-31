代发 wailian999

[B05] 遍历数组 / 列表
来源：http://cy.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://qj.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yd.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dl.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ml.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dk.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mx.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://qd.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lk.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://gz.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ed.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oo.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vv.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://as.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://if.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pw.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wz.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://im.bookmarksfly.cn

[B07] while 循环
来源：http://hb.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://qm.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kh.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://gh.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://fq.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://er.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ln.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://us.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://jt.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://vs.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://gn.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://so.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://fc.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://lh.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://qs.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vz.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cs.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://ga.szxytkj.cn

[B09] break 与 continue
来源：http://jx.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://za.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iz.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://np.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oc.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wx.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gk.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ae.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lz.asd995.cn

[B10] 遍历同时拿索引
来源：http://kj.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mr.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ej.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://il.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dz.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://my.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ab.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dl.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rl.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://rp.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://rq.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://mx.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pc.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ag.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ik.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yr.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://ev.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ni.521024.cn

[B12] 跳出多层循环
来源：http://va.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mc.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gl.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rd.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wh.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gm.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ix.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pu.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vs.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://sq.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://me.colortex.cn

PHP:  is_numeric($x)
来源：http://xx.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://st.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yq.yuntaijiaju.cn

Java: x instanceof Number
来源：http://fa.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pm.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://dn.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://tw.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://dl.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vh.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sw.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://yz.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://by.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bx.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xf.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gx.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ub.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://yi.szxytkj.cn

Py:   a and b or not c
来源：http://rl.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://nh.panjiajie.cn

JS:   a && b || !c
来源：http://oi.wgjwhj.cn

TS:   a && b || !c
来源：http://kx.szsharing.cn

Java: a && b || !c
来源：http://ub.lnxyls.cn

Go:   a && b || !c
来源：http://sc.bookmarksfly.cn

Ruby: a && b || !c
来源：http://zt.bookmarksfly.cn

C#:   a && b || !c
来源：http://jn.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fy.yuexingan06.cn

Py:   if not data: return
来源：http://hw.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://ga.yuexingan06.cn

JS:   if (!data) return;
来源：http://mz.shxzukj.cn

TS:   if (!data) return;
来源：http://ba.panjiajie.cn

Java: if (data == null) return;
来源：http://ea.panjiajie.cn

Go:   if data == nil { return }
来源：http://jl.9csxet.cn

Ruby: return if data.nil?
来源：http://ii.colortex.cn

C#:   if (data == null) return;
来源：http://sb.521024.cn

================================================================================
来源：http://za.huanxung.cn

C. 函数与作用域
来源：http://tm.newstarts.cn

================================================================================
来源：http://hh.yuexingan06.cn

[C01] 定义函数
来源：http://ol.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://vv.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tp.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ci.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tl.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zi.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fn.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://bu.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kc.wgjwhj.cn

[C02] 默认参数
来源：http://ft.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://mc.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ja.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://yz.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tw.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kt.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mm.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://cn.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://fa.gzmigu.cn

[C03] 可变参数
来源：http://tz.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://st.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bu.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sf.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oo.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iy.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mb.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jk.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bk.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://bi.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fp.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gu.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pp.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tu.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ck.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://qr.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://nx.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://uf.bjjhwx.cn

[C05] 返回多个值
来源：http://qd.wgjwhj.cn

Py:   return a, b
来源：http://cf.asd995.cn

PHP:  return [$a, $b];
来源：http://dc.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ad.newstarts.cn

TS:   return { a, b };
来源：http://bi.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hg.nicolike.cn

Go:   return a, b
来源：http://um.nszjky.cn

Ruby: return a, b
来源：http://ev.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://cj.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://pm.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://ql.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nx.lnxyls.cn

JS:   const square = x => x * x;
来源：http://fo.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://tm.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jd.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kn.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://yo.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ki.huanxung.cn

[C07] 把函数作为参数传入
来源：http://iw.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aw.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dt.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xd.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://wv.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://as.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tj.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://fm.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sy.yuntaijiaju.cn

[C08] 闭包
来源：http://xy.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ak.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://be.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bc.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yb.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fq.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ia.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gw.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eo.gzmigu.cn

[C09] 递归
来源：http://pk.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yr.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ub.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hy.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://as.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fv.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vp.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vn.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hp.521024.cn

[C10] 变量作用域
来源：http://zg.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qy.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hq.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fb.hnjuh.cn

TS:   同 JS
来源：http://ra.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://xq.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://nd.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hp.shtwfgs.cn

C#:   块级作用域
来源：http://ai.lnxyls.cn

[C11] 模块导入与导出
来源：http://bu.colortex.cn

Py:   from module import func
来源：http://ex.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ef.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qt.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kj.szsharing.cn

Java: import java.util.List;
来源：http://wl.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://un.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://eh.chemitech.net.cn

C#:   using System.Text;
来源：http://jh.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://lk.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://mt.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://ys.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://pm.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://ye.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kj.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ak.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://cg.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://il.521024.cn

[C13] 类型声明 / 类型注解
来源：http://lg.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://je.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ro.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ia.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wx.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qx.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://ji.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eh.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dr.haigaiapp.cn

[C14] 泛型函数
来源：http://db.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eu.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://sb.nszjky.cn

JS:   // 无泛型
来源：http://be.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://el.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wr.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bh.colortex.cn

Ruby: # 无泛型
来源：http://ue.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bu.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://tp.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tt.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://ch.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qd.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ou.muxihuayi.cn

Java: // 无解构
来源：http://th.muxihuayi.cn

Go:   // 无解构
来源：http://np.chemitech.net.cn

Ruby: a, b = pair
来源：http://nh.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://tc.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://su.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aw.nszjky.cn

PHP:  // 无重载
来源：http://mz.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xv.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://db.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wq.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://vd.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://wu.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shxzukj.cn

================================================================================
来源：http://bw.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://lx.9csxet.cn

================================================================================
来源：http://lw.nicolike.cn

[D01] 创建数组 / 列表
来源：http://dc.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ur.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gb.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bj.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ed.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tp.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://dy.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://hk.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://br.szsharing.cn

[D02] 追加元素到末尾
来源：http://ut.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sm.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://us.asd995.cn

JS:   arr.push(4);
来源：http://im.nicolike.cn

TS:   arr.push(4);
来源：http://bp.lnxyls.cn

Java: list.add(4);
来源：http://yy.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://ge.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://na.bjjhwx.cn

C#:   list.Add(4);
来源：http://bk.szsharing.cn

[D03] 在指定位置插入元素
来源：http://gb.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://pd.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qs.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lk.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://kc.szxytkj.cn

Java: list.add(0, 0);
来源：http://kd.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mp.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fy.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://bs.nicolike.cn

[D04] 删除元素
来源：http://hn.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gn.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pn.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ya.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://tp.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wx.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fl.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fm.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yb.shxzskj.cn

[D05] 访问与修改元素
来源：http://qq.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ra.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ib.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fv.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://qj.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://hz.jctech888.com.cn


<!-- 参考信息 -->