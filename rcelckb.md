代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xh.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vs.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cf.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vk.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ed.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ih.newstarts.cn

[B03] switch / match / case
来源：http://qw.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://za.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cp.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fc.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bf.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ma.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://us.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fl.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xr.lnxyls.cn

[B04] for 计数循环
来源：http://sy.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://ti.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vp.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zp.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jl.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jo.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ih.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://od.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xl.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://mt.nicolike.cn

Py:   for item in arr: print(item)
来源：http://bp.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ml.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sp.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tc.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yg.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tt.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://mv.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://db.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://kt.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tz.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vh.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bz.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vb.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sq.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hv.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jx.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dr.wgjwhj.cn

[B07] while 循环
来源：http://lg.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://un.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://do.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://xy.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://rl.521024.cn

Java: while (i < 10) { i++; }
来源：http://yw.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fc.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://bd.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://oc.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://jc.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://ye.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ee.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://tg.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://ii.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://rx.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yl.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oi.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://dc.bookmarksfly.cn

[B09] break 与 continue
来源：http://oy.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cb.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pd.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qf.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gt.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oz.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fk.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pr.nszjky.cn

[B10] 遍历同时拿索引
来源：http://zg.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ya.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pe.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://do.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pg.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bv.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tg.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kk.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bu.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://jh.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://yj.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://tq.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xd.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rv.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fb.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mn.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://fn.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jw.hahajie.cn

[B12] 跳出多层循环
来源：http://ay.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pj.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ie.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mz.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wl.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uf.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://em.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ty.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oe.gzmigu.cn

[B13] 判断是否为数字
来源：http://ta.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://tz.521024.cn

PHP:  is_numeric($x)
来源：http://rz.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ic.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dr.hahajie.cn

Java: x instanceof Number
来源：http://sb.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ux.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://pv.asd995.cn

C#:   x is int or double or decimal
来源：http://uq.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://vo.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yk.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mr.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://wb.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://gc.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ws.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cz.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vm.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qj.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://rq.gzmigu.cn

Py:   a and b or not c
来源：http://gm.521024.cn

PHP:  $a && $b || !$c
来源：http://sh.shtwfgs.cn

JS:   a && b || !c
来源：http://cd.szxytkj.cn

TS:   a && b || !c
来源：http://fo.szsharing.cn

Java: a && b || !c
来源：http://sx.yuntaijiaju.cn

Go:   a && b || !c
来源：http://ww.gzmigu.cn

Ruby: a && b || !c
来源：http://sv.wgjwhj.cn

C#:   a && b || !c
来源：http://sv.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pp.hnjuh.cn

Py:   if not data: return
来源：http://hs.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://nx.chemitech.net.cn

JS:   if (!data) return;
来源：http://lg.wgjwhj.cn

TS:   if (!data) return;
来源：http://kt.nicolike.cn

Java: if (data == null) return;
来源：http://vh.hnjuh.cn

Go:   if data == nil { return }
来源：http://ii.shxzukj.cn

Ruby: return if data.nil?
来源：http://tt.newstarts.cn

C#:   if (data == null) return;
来源：http://et.jianghongdianzi.cn

================================================================================
来源：http://dq.9csxet.cn

C. 函数与作用域
来源：http://tq.asd995.cn

================================================================================
来源：http://kk.szxytkj.cn

[C01] 定义函数
来源：http://xa.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://rq.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nm.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://jk.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://of.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vm.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qa.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://xa.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tr.yuexingan06.cn

[C02] 默认参数
来源：http://yz.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://ci.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vn.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://mc.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wj.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yh.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pl.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://kb.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://og.nicolike.cn

[C03] 可变参数
来源：http://af.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://py.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yg.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tw.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pt.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wh.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ef.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pc.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ug.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://pm.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bs.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ck.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cl.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zm.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://hd.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://ta.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://gi.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://gk.shtwfgs.cn

[C05] 返回多个值
来源：http://an.huixinmuqiang.cn

Py:   return a, b
来源：http://qk.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://dm.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zk.szsharing.cn

TS:   return { a, b };
来源：http://dl.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nz.nszjky.cn

Go:   return a, b
来源：http://se.bookmarksfly.cn

Ruby: return a, b
来源：http://vq.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://jk.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://ga.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://sp.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sg.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://xm.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://dh.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hb.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ll.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://ft.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://om.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://nn.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bb.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ps.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ke.newstarts.cn

TS:   arr.map(String)
来源：http://sz.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://np.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kh.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://ox.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oi.yuexingan06.cn

[C08] 闭包
来源：http://gw.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pt.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hv.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fm.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ip.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wf.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lw.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nz.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uy.jianghongdianzi.cn

[C09] 递归
来源：http://oa.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cu.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cy.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zq.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ox.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ip.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iz.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://za.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qz.newstarts.cn

[C10] 变量作用域
来源：http://ja.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zr.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://th.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qw.panjiajie.cn

TS:   同 JS
来源：http://fl.shxzskj.cn

Java: 方法内为块级作用域
来源：http://xy.huanxung.cn

Go:   花括号块级作用域
来源：http://nw.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://em.shtwfgs.cn

C#:   块级作用域
来源：http://kq.wgjwhj.cn

[C11] 模块导入与导出
来源：http://ad.szsharing.cn

Py:   from module import func
来源：http://mr.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zx.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ks.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xb.szxytkj.cn

Java: import java.util.List;
来源：http://eo.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ra.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ek.szxytkj.cn

C#:   using System.Text;
来源：http://al.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://sk.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://ve.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://hp.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://uf.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://xt.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ho.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ip.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://al.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zn.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://ui.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xg.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://be.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gc.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ym.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://me.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://ff.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ic.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yp.yuexingan06.cn

[C14] 泛型函数
来源：http://zz.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dx.haigaiapp.cn

PHP:  // 无泛型
来源：http://dy.shxzskj.cn

JS:   // 无泛型
来源：http://vm.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://an.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cp.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rp.9csxet.cn

Ruby: # 无泛型
来源：http://dr.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pa.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://lp.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rh.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://xu.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pj.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://re.panjiajie.cn

Java: // 无解构
来源：http://ar.nszjky.cn

Go:   // 无解构
来源：http://we.521024.cn

Ruby: a, b = pair
来源：http://ix.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://ey.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://jw.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mq.gzmigu.cn

PHP:  // 无重载
来源：http://ha.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qk.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://kl.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oa.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://by.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://hy.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ex.newstarts.cn

================================================================================
来源：http://fw.521024.cn

D. 数组 / 列表 / 集合
来源：http://ze.szsharing.cn

================================================================================
来源：http://xh.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://hy.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lu.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zh.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sd.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gb.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nd.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://se.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://ug.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bb.nicolike.cn

[D02] 追加元素到末尾
来源：http://ka.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lq.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://do.wgjwhj.cn

JS:   arr.push(4);
来源：http://fe.nicolike.cn

TS:   arr.push(4);
来源：http://xx.hnjuh.cn

Java: list.add(4);
来源：http://yo.asd995.cn

Go:   arr = append(arr, 4)
来源：http://lv.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://ud.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://ub.nszjky.cn


<!-- 参考信息 -->