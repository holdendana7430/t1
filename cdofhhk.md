代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://fu.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://of.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://za.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://oj.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fr.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://zh.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yo.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ju.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mu.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fn.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xo.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://in.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kt.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://md.asd995.cn

[B07] while 循环
来源：http://qd.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://cm.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yv.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://gr.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://wv.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://np.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ef.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://rc.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://sl.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://ge.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://wu.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ge.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://jb.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://rg.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://ns.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mm.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zv.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://rz.gzmigu.cn

[B09] break 与 continue
来源：http://ev.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sg.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ly.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fo.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qd.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bt.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zg.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bs.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ms.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://at.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nu.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lp.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zq.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pu.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dw.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://se.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cp.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vl.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://am.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://mc.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://gm.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ik.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iy.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sd.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://th.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://fo.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ox.chemitech.net.cn

[B12] 跳出多层循环
来源：http://ja.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://st.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oh.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lx.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ck.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kq.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ai.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hr.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wd.lnxyls.cn

[B13] 判断是否为数字
来源：http://eo.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://og.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://fe.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ue.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gl.nszjky.cn

Java: x instanceof Number
来源：http://ig.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dn.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://ii.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://tu.szsharing.cn

[B14] 判断值是否在集合内
来源：http://xm.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nz.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ot.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://gv.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://st.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://io.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zh.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kq.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xv.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://pg.bookmarksfly.cn

Py:   a and b or not c
来源：http://eh.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://gx.bookmarksfly.cn

JS:   a && b || !c
来源：http://fz.hahajie.cn

TS:   a && b || !c
来源：http://ee.huixiangedu.cn

Java: a && b || !c
来源：http://la.muxihuayi.cn

Go:   a && b || !c
来源：http://yf.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://ks.hahajie.cn

C#:   a && b || !c
来源：http://lc.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sn.szxytkj.cn

Py:   if not data: return
来源：http://hg.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://xp.wgjwhj.cn

JS:   if (!data) return;
来源：http://cu.muxihuayi.cn

TS:   if (!data) return;
来源：http://kf.shxzskj.cn

Java: if (data == null) return;
来源：http://jw.panjiajie.cn

Go:   if data == nil { return }
来源：http://ai.nicolike.cn

Ruby: return if data.nil?
来源：http://zz.bjjhwx.cn

C#:   if (data == null) return;
来源：http://px.shxzukj.cn

================================================================================
来源：http://co.shxzskj.cn

C. 函数与作用域
来源：http://hu.yuntaijiaju.cn

================================================================================
来源：http://yu.shtwfgs.cn

[C01] 定义函数
来源：http://mu.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://yj.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ap.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://lb.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ae.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qn.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nk.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://jh.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://al.panjiajie.cn

[C02] 默认参数
来源：http://yp.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://pf.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fr.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://te.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pr.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mr.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sm.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://du.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://wi.asd995.cn

[C03] 可变参数
来源：http://xa.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://dd.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://id.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yt.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mg.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ws.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://il.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pg.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fb.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://qn.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://su.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dm.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xu.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wa.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://nf.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://yk.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://zp.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://wn.9csxet.cn

[C05] 返回多个值
来源：http://ol.yuexingan06.cn

Py:   return a, b
来源：http://eu.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://ni.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fu.shxzskj.cn

TS:   return { a, b };
来源：http://hr.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gd.newstarts.cn

Go:   return a, b
来源：http://pa.hahajie.cn

Ruby: return a, b
来源：http://jq.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://by.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://dw.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://rc.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vj.nszjky.cn

JS:   const square = x => x * x;
来源：http://yf.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://mg.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tk.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sr.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://pf.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sd.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://yx.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vg.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://on.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ek.colortex.cn

TS:   arr.map(String)
来源：http://cf.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gn.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nj.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://vf.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bm.nicolike.cn

[C08] 闭包
来源：http://ec.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nt.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qa.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mb.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cq.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nk.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sq.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ds.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uk.jianghongdianzi.cn

[C09] 递归
来源：http://fq.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ht.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tc.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fp.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://la.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cx.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pu.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cn.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bf.szxytkj.cn

[C10] 变量作用域
来源：http://jk.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ik.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nd.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vl.jianghongdianzi.cn

TS:   同 JS
来源：http://sa.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://gg.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://ja.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wx.shxzukj.cn

C#:   块级作用域
来源：http://eb.asd995.cn

[C11] 模块导入与导出
来源：http://ba.panjiajie.cn

Py:   from module import func
来源：http://hj.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aj.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kg.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bq.szsharing.cn

Java: import java.util.List;
来源：http://wl.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fg.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ag.yuexingan06.cn

C#:   using System.Text;
来源：http://eq.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://sy.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://up.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://kq.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://pf.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://zv.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uv.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://bt.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://ji.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vr.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://lv.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wv.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ji.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ci.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dy.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mn.nicolike.cn

Go:   func add(a, b int) int
来源：http://ul.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oe.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kq.lnxyls.cn

[C14] 泛型函数
来源：http://qx.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://br.shxzskj.cn

PHP:  // 无泛型
来源：http://sa.chemitech.net.cn

JS:   // 无泛型
来源：http://hf.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mb.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://es.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://im.gzmigu.cn

Ruby: # 无泛型
来源：http://wb.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zz.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://ua.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lw.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://mp.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://of.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vh.bjjhwx.cn

Java: // 无解构
来源：http://ce.hnjuh.cn

Go:   // 无解构
来源：http://rx.lnxyls.cn

Ruby: a, b = pair
来源：http://bb.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://ib.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://na.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tj.szxytkj.cn

PHP:  // 无重载
来源：http://mt.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://du.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://hm.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lv.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://hq.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://nz.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ob.haigaiapp.cn

================================================================================
来源：http://hf.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://xf.521024.cn

================================================================================
来源：http://nl.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://zk.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rg.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pu.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://za.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ar.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ec.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://lg.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://rf.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ql.9csxet.cn

[D02] 追加元素到末尾
来源：http://fa.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wt.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cq.jctech888.com.cn

JS:   arr.push(4);
来源：http://ts.nszjky.cn

TS:   arr.push(4);
来源：http://mn.yuexingan06.cn

Java: list.add(4);
来源：http://yr.521024.cn

Go:   arr = append(arr, 4)
来源：http://ln.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://da.huixiangedu.cn

C#:   list.Add(4);
来源：http://tx.colortex.cn

[D03] 在指定位置插入元素
来源：http://al.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://uc.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uf.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fh.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ob.chemitech.net.cn

Java: list.add(0, 0);
来源：http://fz.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://et.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kx.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://xb.huixiangedu.cn

[D04] 删除元素
来源：http://my.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gc.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cb.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zi.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://qq.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dx.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pc.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jr.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tq.szsharing.cn

[D05] 访问与修改元素
来源：http://qp.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ya.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://di.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ay.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://xe.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://zg.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://ed.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ld.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zu.haigaiapp.cn

[D06] 数组长度
来源：http://eh.muxihuayi.cn


<!-- 参考信息 -->