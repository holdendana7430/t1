代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nc.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fw.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ju.muxihuayi.cn

[B04] for 计数循环
来源：http://re.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://qn.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lg.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://my.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jy.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uz.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rp.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://dd.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hp.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://wa.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://sp.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ac.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ge.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mf.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xc.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wv.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://si.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ih.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://er.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oi.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qf.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://py.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zi.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ih.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bu.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oh.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gs.huixinmuqiang.cn

[B07] while 循环
来源：http://wz.nicolike.cn

Py:   while i < 10: i += 1
来源：http://jy.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gx.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://hn.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://gf.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://xc.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iq.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://my.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://mg.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://tu.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://kz.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hy.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://qm.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://yi.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://ca.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://se.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jh.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://kg.shtwfgs.cn

[B09] break 与 continue
来源：http://kx.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vh.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xy.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tx.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qw.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ra.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://he.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ov.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zk.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://er.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://re.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yr.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hv.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://th.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gy.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mu.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pa.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nr.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://mq.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://xn.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://kx.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qh.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wq.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zd.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gs.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://zj.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mx.shxzukj.cn

[B12] 跳出多层循环
来源：http://rj.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://of.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ht.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ss.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bz.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jh.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lc.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qw.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ho.jctech888.com.cn

[B13] 判断是否为数字
来源：http://ac.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://sl.shxzskj.cn

PHP:  is_numeric($x)
来源：http://nb.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://za.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eg.bookmarksfly.cn

Java: x instanceof Number
来源：http://yb.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://du.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://mv.lnxyls.cn

C#:   x is int or double or decimal
来源：http://tq.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://lh.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xb.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yu.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://sm.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://aw.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ln.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://os.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lg.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nf.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://dl.bookmarksfly.cn

Py:   a and b or not c
来源：http://vr.nszjky.cn

PHP:  $a && $b || !$c
来源：http://uk.szsharing.cn

JS:   a && b || !c
来源：http://as.nicolike.cn

TS:   a && b || !c
来源：http://wv.chemitech.net.cn

Java: a && b || !c
来源：http://zk.szsharing.cn

Go:   a && b || !c
来源：http://yz.gzmigu.cn

Ruby: a && b || !c
来源：http://jd.yuntaijiaju.cn

C#:   a && b || !c
来源：http://dk.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vo.huanxung.cn

Py:   if not data: return
来源：http://rb.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://jy.hahajie.cn

JS:   if (!data) return;
来源：http://rd.newstarts.cn

TS:   if (!data) return;
来源：http://lt.colortex.cn

Java: if (data == null) return;
来源：http://hv.bjjhwx.cn

Go:   if data == nil { return }
来源：http://lu.jctech888.com.cn

Ruby: return if data.nil?
来源：http://sd.lnxyls.cn

C#:   if (data == null) return;
来源：http://cn.bookmarksfly.cn

================================================================================
来源：http://sz.szxytkj.cn

C. 函数与作用域
来源：http://tr.newstarts.cn

================================================================================
来源：http://ux.shxzukj.cn

[C01] 定义函数
来源：http://hs.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://mv.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tv.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://lh.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jo.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dz.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uf.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://ys.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hm.asd995.cn

[C02] 默认参数
来源：http://th.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://wk.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oc.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://bc.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xj.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sn.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ff.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://bu.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://qd.huanxung.cn

[C03] 可变参数
来源：http://oz.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://sx.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vf.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ed.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lf.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tb.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ib.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rc.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bb.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://fn.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tm.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://et.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ao.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sa.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://le.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://wt.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://xz.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://ws.szxytkj.cn

[C05] 返回多个值
来源：http://uy.gzmigu.cn

Py:   return a, b
来源：http://jt.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://rx.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jz.huanxung.cn

TS:   return { a, b };
来源：http://ab.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zs.huanxung.cn

Go:   return a, b
来源：http://vt.yuexingan06.cn

Ruby: return a, b
来源：http://vb.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://zc.521024.cn

[C06] 匿名函数 / lambda
来源：http://kg.szsharing.cn

Py:   square = lambda x: x * x
来源：http://rm.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oo.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://ib.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://ga.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sx.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://op.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://bi.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jc.521024.cn

[C07] 把函数作为参数传入
来源：http://bj.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rx.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wm.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gu.haigaiapp.cn

TS:   arr.map(String)
来源：http://oj.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ku.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eb.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://ca.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cr.muxihuayi.cn

[C08] 闭包
来源：http://gs.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gp.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ab.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wc.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oq.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jk.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hn.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jo.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ij.chemitech.net.cn

[C09] 递归
来源：http://pt.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ud.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gl.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cf.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qq.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cc.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wc.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ie.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fl.nszjky.cn

[C10] 变量作用域
来源：http://pe.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fd.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gl.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kg.szsharing.cn

TS:   同 JS
来源：http://xi.shxzskj.cn

Java: 方法内为块级作用域
来源：http://gy.colortex.cn

Go:   花括号块级作用域
来源：http://dq.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gv.chemitech.net.cn

C#:   块级作用域
来源：http://iz.nicolike.cn

[C11] 模块导入与导出
来源：http://di.bookmarksfly.cn

Py:   from module import func
来源：http://yy.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fc.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jq.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vk.bookmarksfly.cn

Java: import java.util.List;
来源：http://me.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://my.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://qc.shxzukj.cn

C#:   using System.Text;
来源：http://gb.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://yf.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://sz.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://ge.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://ht.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://lf.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gm.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://gm.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://xr.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fs.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://yr.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tt.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sn.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xm.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jx.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pw.hahajie.cn

Go:   func add(a, b int) int
来源：http://gf.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nd.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ol.szsharing.cn

[C14] 泛型函数
来源：http://hn.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pc.newstarts.cn

PHP:  // 无泛型
来源：http://ks.newstarts.cn

JS:   // 无泛型
来源：http://fc.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yb.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rn.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kx.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://pe.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rg.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://mp.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ty.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://pw.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pw.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ma.yuntaijiaju.cn

Java: // 无解构
来源：http://nr.9csxet.cn

Go:   // 无解构
来源：http://ro.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://yb.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://kd.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://wd.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jj.nicolike.cn

PHP:  // 无重载
来源：http://qd.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wz.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://sk.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vh.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://uy.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://wn.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xo.hnjuh.cn

================================================================================
来源：http://ud.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://jh.bookmarksfly.cn

================================================================================
来源：http://ku.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://us.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gy.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tg.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://us.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ri.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cr.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://df.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://pg.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://da.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://bd.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qc.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gl.asd995.cn

JS:   arr.push(4);
来源：http://vq.jctech888.com.cn

TS:   arr.push(4);
来源：http://ws.nicolike.cn

Java: list.add(4);
来源：http://pg.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://fa.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ze.shxzukj.cn

C#:   list.Add(4);
来源：http://ji.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://jb.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://vk.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://so.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eq.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://kd.shtwfgs.cn

Java: list.add(0, 0);
来源：http://ki.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://om.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sq.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://hu.szsharing.cn

[D04] 删除元素
来源：http://sd.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bv.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bv.hnjuh.cn


<!-- 参考信息 -->