代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hm.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ml.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bl.bookmarksfly.cn

[B04] for 计数循环
来源：http://fo.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://pg.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dj.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bo.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ro.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hn.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tg.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://ud.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pd.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://vc.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://uw.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tg.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ke.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fn.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://we.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lh.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://dt.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ti.asd995.cn

[B06] 遍历字典 / 对象
来源：http://lh.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zd.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iy.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ve.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ee.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oz.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://om.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yy.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ix.wgjwhj.cn

[B07] while 循环
来源：http://qc.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://js.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lh.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://ln.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://vc.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://ka.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fy.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://dl.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://gs.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://pi.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://rc.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xl.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://qx.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://rq.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://ea.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ij.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://es.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://rh.bjjhwx.cn

[B09] break 与 continue
来源：http://kv.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ll.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bf.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pm.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fr.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lc.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jt.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zn.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gn.nicolike.cn

[B10] 遍历同时拿索引
来源：http://jm.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wk.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ro.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ul.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://om.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rr.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zt.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rs.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zt.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://om.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://vb.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://xq.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iw.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pt.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ap.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://it.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://lu.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dh.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://fn.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wb.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fu.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ur.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ir.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tj.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ds.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kv.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://im.panjiajie.cn

[B13] 判断是否为数字
来源：http://wy.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://hs.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://ng.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xv.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tl.colortex.cn

Java: x instanceof Number
来源：http://yj.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lx.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://eb.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://cj.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://qf.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ff.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yl.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://lv.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://kk.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ww.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jg.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ag.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yu.shxzukj.cn

[B15] 布尔运算与取反
来源：http://kz.szxytkj.cn

Py:   a and b or not c
来源：http://dd.szsharing.cn

PHP:  $a && $b || !$c
来源：http://cc.yuexingan06.cn

JS:   a && b || !c
来源：http://rm.shtwfgs.cn

TS:   a && b || !c
来源：http://pg.bookmarksfly.cn

Java: a && b || !c
来源：http://yt.jctech888.com.cn

Go:   a && b || !c
来源：http://sy.wgjwhj.cn

Ruby: a && b || !c
来源：http://fx.colortex.cn

C#:   a && b || !c
来源：http://mv.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kp.shxzskj.cn

Py:   if not data: return
来源：http://yy.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://zv.szxytkj.cn

JS:   if (!data) return;
来源：http://st.nszjky.cn

TS:   if (!data) return;
来源：http://hq.521024.cn

Java: if (data == null) return;
来源：http://jo.shxzskj.cn

Go:   if data == nil { return }
来源：http://ck.shtwfgs.cn

Ruby: return if data.nil?
来源：http://qm.chemitech.net.cn

C#:   if (data == null) return;
来源：http://pk.lnxyls.cn

================================================================================
来源：http://oe.nicolike.cn

C. 函数与作用域
来源：http://ys.hnjuh.cn

================================================================================
来源：http://ii.huixinmuqiang.cn

[C01] 定义函数
来源：http://vk.asd995.cn

Py:   def add(a, b): return a + b
来源：http://sr.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://db.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://hf.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lj.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ti.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nn.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://gm.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ji.9csxet.cn

[C02] 默认参数
来源：http://oz.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://hs.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dc.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://aw.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qq.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ge.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pv.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://ix.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://tw.bookmarksfly.cn

[C03] 可变参数
来源：http://en.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://gk.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hd.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ov.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fu.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ox.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ic.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tl.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xn.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://pw.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pm.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ym.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pk.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dp.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://jn.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://sg.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://wi.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://tb.szxytkj.cn

[C05] 返回多个值
来源：http://lw.nicolike.cn

Py:   return a, b
来源：http://ug.hnjuh.cn

PHP:  return [$a, $b];
来源：http://qh.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nn.colortex.cn

TS:   return { a, b };
来源：http://te.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jb.bookmarksfly.cn

Go:   return a, b
来源：http://me.shtwfgs.cn

Ruby: return a, b
来源：http://nl.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://tq.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://dw.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://bu.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ut.lnxyls.cn

JS:   const square = x => x * x;
来源：http://fl.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ad.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oa.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ym.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://ss.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vh.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://hj.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pu.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nh.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hn.yuexingan06.cn

TS:   arr.map(String)
来源：http://an.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://se.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://or.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://ib.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jx.wgjwhj.cn

[C08] 闭包
来源：http://xz.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ck.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xb.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zi.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sa.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yi.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fc.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://il.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://el.huixinmuqiang.cn

[C09] 递归
来源：http://no.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://by.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hh.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ca.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://it.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hk.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ag.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rw.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mb.shxzukj.cn

[C10] 变量作用域
来源：http://yx.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bv.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ca.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pw.gzmigu.cn

TS:   同 JS
来源：http://iv.lnxyls.cn

Java: 方法内为块级作用域
来源：http://ax.huanxung.cn

Go:   花括号块级作用域
来源：http://ub.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vc.huixiangedu.cn

C#:   块级作用域
来源：http://hu.muxihuayi.cn

[C11] 模块导入与导出
来源：http://ud.szsharing.cn

Py:   from module import func
来源：http://dt.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qk.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://st.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rf.9csxet.cn

Java: import java.util.List;
来源：http://ug.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lk.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://dc.huixinmuqiang.cn

C#:   using System.Text;
来源：http://fb.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://ha.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://dx.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://nr.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://ir.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://tb.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://we.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://lz.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://jt.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://al.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://id.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cr.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lm.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kr.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lk.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oy.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://og.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hg.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bf.muxihuayi.cn

[C14] 泛型函数
来源：http://ne.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ug.huixiangedu.cn

PHP:  // 无泛型
来源：http://uh.muxihuayi.cn

JS:   // 无泛型
来源：http://mb.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ys.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cb.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oa.jctech888.com.cn

Ruby: # 无泛型
来源：http://xh.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wx.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://zz.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gk.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://lp.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oh.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lw.shtwfgs.cn

Java: // 无解构
来源：http://gu.szsharing.cn

Go:   // 无解构
来源：http://cg.bjjhwx.cn

Ruby: a, b = pair
来源：http://kk.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://jy.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://xj.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cg.yuntaijiaju.cn

PHP:  // 无重载
来源：http://fd.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jz.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ty.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xm.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://py.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://ns.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mu.521024.cn

================================================================================
来源：http://mg.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://tn.colortex.cn

================================================================================
来源：http://wo.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://be.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://th.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rf.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bn.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pc.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vd.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://tn.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://zs.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cl.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://pr.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rp.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rs.jctech888.com.cn

JS:   arr.push(4);
来源：http://md.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://hp.jianghongdianzi.cn

Java: list.add(4);
来源：http://gk.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://su.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://oa.haigaiapp.cn

C#:   list.Add(4);
来源：http://bm.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://eq.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://cb.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vp.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jv.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://yt.hnjuh.cn

Java: list.add(0, 0);
来源：http://bu.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dx.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kw.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://ab.521024.cn

[D04] 删除元素
来源：http://pm.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jq.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bf.muxihuayi.cn


<!-- 参考信息 -->