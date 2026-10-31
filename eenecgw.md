代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xm.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://da.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://gu.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://km.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://eh.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://pg.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rx.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hh.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yw.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cc.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zq.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://hf.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kc.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://lg.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gz.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wx.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uu.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sx.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yo.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ca.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pi.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ng.bjjhwx.cn

[B07] while 循环
来源：http://qm.szsharing.cn

Py:   while i < 10: i += 1
来源：http://uf.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nx.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://vp.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://ej.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://cz.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bf.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://ct.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://cs.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ub.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://if.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vm.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://ie.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://sj.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://qx.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://th.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dt.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://og.521024.cn

[B09] break 与 continue
来源：http://vo.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vf.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fa.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bm.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sz.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cp.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ib.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zb.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yy.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ne.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uc.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jz.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://su.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bi.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ie.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ut.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ir.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pl.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://kj.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://pn.colortex.cn

PHP:  range(0, 10, 2);
来源：http://ha.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mk.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gv.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fd.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ao.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://pv.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bf.huixiangedu.cn

[B12] 跳出多层循环
来源：http://vm.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ih.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mb.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xs.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yu.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cn.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ed.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ku.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uz.nicolike.cn

[B13] 判断是否为数字
来源：http://lb.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ts.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://rb.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rk.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kb.bjjhwx.cn

Java: x instanceof Number
来源：http://yn.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dl.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://go.9csxet.cn

C#:   x is int or double or decimal
来源：http://xk.newstarts.cn

[B14] 判断值是否在集合内
来源：http://kp.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://be.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fv.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://vm.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://da.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jw.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ji.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ew.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jq.gzmigu.cn

[B15] 布尔运算与取反
来源：http://qy.huixinmuqiang.cn

Py:   a and b or not c
来源：http://pn.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://ie.gzmigu.cn

JS:   a && b || !c
来源：http://cm.521024.cn

TS:   a && b || !c
来源：http://bv.jctech888.com.cn

Java: a && b || !c
来源：http://rr.hahajie.cn

Go:   a && b || !c
来源：http://nz.9csxet.cn

Ruby: a && b || !c
来源：http://oi.newstarts.cn

C#:   a && b || !c
来源：http://zn.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xm.yuexingan06.cn

Py:   if not data: return
来源：http://tf.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://ol.nszjky.cn

JS:   if (!data) return;
来源：http://dq.9csxet.cn

TS:   if (!data) return;
来源：http://ms.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://to.jctech888.com.cn

Go:   if data == nil { return }
来源：http://ow.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://hw.asd995.cn

C#:   if (data == null) return;
来源：http://qe.shtwfgs.cn

================================================================================
来源：http://pm.asd995.cn

C. 函数与作用域
来源：http://uc.szxytkj.cn

================================================================================
来源：http://ao.asd995.cn

[C01] 定义函数
来源：http://rq.colortex.cn

Py:   def add(a, b): return a + b
来源：http://vv.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bs.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://nz.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jh.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rn.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iu.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://fw.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fe.nicolike.cn

[C02] 默认参数
来源：http://kt.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://pz.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ws.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://ge.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yz.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ub.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pi.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://hd.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://bf.hahajie.cn

[C03] 可变参数
来源：http://vp.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://vd.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xy.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://al.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ox.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lv.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ci.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fl.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nn.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://ri.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nz.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rc.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gr.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ma.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://cl.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://qi.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://xy.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://aa.colortex.cn

[C05] 返回多个值
来源：http://fj.jctech888.com.cn

Py:   return a, b
来源：http://ge.lnxyls.cn

PHP:  return [$a, $b];
来源：http://yl.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yt.jianghongdianzi.cn

TS:   return { a, b };
来源：http://kd.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ek.szsharing.cn

Go:   return a, b
来源：http://bh.jctech888.com.cn

Ruby: return a, b
来源：http://nu.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://yl.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://bk.huanxung.cn

Py:   square = lambda x: x * x
来源：http://sw.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fg.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://oh.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://ef.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bv.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pl.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://tz.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dh.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://gl.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qd.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vd.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gi.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://qd.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://at.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jd.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://mq.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ar.jctech888.com.cn

[C08] 闭包
来源：http://jy.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mv.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rf.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fx.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zt.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hx.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cv.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jg.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fi.chemitech.net.cn

[C09] 递归
来源：http://yk.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lt.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zw.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://db.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pg.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sc.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sm.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hm.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kd.szsharing.cn

[C10] 变量作用域
来源：http://jo.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ct.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://np.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ah.haigaiapp.cn

TS:   同 JS
来源：http://cc.hnjuh.cn

Java: 方法内为块级作用域
来源：http://cl.lnxyls.cn

Go:   花括号块级作用域
来源：http://oc.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xi.huixinmuqiang.cn

C#:   块级作用域
来源：http://zk.521024.cn

[C11] 模块导入与导出
来源：http://ys.asd995.cn

Py:   from module import func
来源：http://ed.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tg.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://em.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ii.yuntaijiaju.cn

Java: import java.util.List;
来源：http://yw.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sz.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://su.shxzskj.cn

C#:   using System.Text;
来源：http://kj.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://do.521024.cn

Py:   (lambda: print("run"))()
来源：http://bc.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://qr.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://wp.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://xo.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sj.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://nn.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://sy.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://au.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://fz.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vt.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wa.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://us.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ri.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://no.asd995.cn

Go:   func add(a, b int) int
来源：http://pt.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://md.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mh.colortex.cn

[C14] 泛型函数
来源：http://hx.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wk.shtwfgs.cn

PHP:  // 无泛型
来源：http://uy.gzmigu.cn

JS:   // 无泛型
来源：http://uy.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qh.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://om.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uh.521024.cn

Ruby: # 无泛型
来源：http://su.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jn.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://pz.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ea.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://ce.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ng.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://va.nicolike.cn

Java: // 无解构
来源：http://it.bookmarksfly.cn

Go:   // 无解构
来源：http://gn.shxzukj.cn

Ruby: a, b = pair
来源：http://wv.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://gb.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://ka.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mn.szsharing.cn

PHP:  // 无重载
来源：http://eu.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tq.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://uu.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zp.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://ui.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://sx.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lv.wgjwhj.cn

================================================================================
来源：http://sd.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://ln.haigaiapp.cn

================================================================================
来源：http://lo.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://ya.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hq.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rk.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ci.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xs.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qc.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://yh.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://fc.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uh.hahajie.cn

[D02] 追加元素到末尾
来源：http://ov.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://og.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gu.huanxung.cn

JS:   arr.push(4);
来源：http://dt.lnxyls.cn

TS:   arr.push(4);
来源：http://ka.shtwfgs.cn

Java: list.add(4);
来源：http://fs.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://pz.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://lv.jctech888.com.cn

C#:   list.Add(4);
来源：http://rh.newstarts.cn

[D03] 在指定位置插入元素
来源：http://fw.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://nw.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xp.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zr.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://es.jctech888.com.cn

Java: list.add(0, 0);
来源：http://iz.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://we.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vd.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://gd.nicolike.cn

[D04] 删除元素
来源：http://he.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wi.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tt.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nj.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://pa.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zq.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bt.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gx.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wd.yuexingan06.cn

[D05] 访问与修改元素
来源：http://cx.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ju.521024.cn


<!-- 参考信息 -->