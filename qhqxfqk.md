代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kt.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nc.bookmarksfly.cn

[B03] switch / match / case
来源：http://or.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cs.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gn.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xi.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rx.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sz.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uy.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vc.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eh.jianghongdianzi.cn

[B04] for 计数循环
来源：http://kq.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://oz.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ue.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cx.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pj.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wv.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qr.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://fz.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rz.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://yi.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://pb.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mn.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tx.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wk.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://op.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gr.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://at.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ar.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://my.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fm.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ym.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jc.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gx.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xo.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eo.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mh.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pd.huanxung.cn

[B07] while 循环
来源：http://bm.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://bd.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ii.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://cr.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://mz.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://xm.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gt.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://rk.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://fj.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://kb.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://mv.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mr.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://xm.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://ae.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://vv.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://el.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vn.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://yj.yuntaijiaju.cn

[B09] break 与 continue
来源：http://se.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xj.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mf.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ye.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dv.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rg.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dg.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ji.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hv.asd995.cn

[B10] 遍历同时拿索引
来源：http://im.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cx.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zp.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tc.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nr.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qz.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ou.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ol.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zy.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://ug.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://ti.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://ml.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xm.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lv.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tu.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pi.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://fi.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wn.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://np.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oc.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://um.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yc.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vj.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vw.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tw.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ft.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tl.muxihuayi.cn

[B13] 判断是否为数字
来源：http://bi.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://qq.colortex.cn

PHP:  is_numeric($x)
来源：http://uv.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jt.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ud.newstarts.cn

Java: x instanceof Number
来源：http://hm.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://on.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://rh.szsharing.cn

C#:   x is int or double or decimal
来源：http://wc.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://jh.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nk.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vu.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://qd.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://gv.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ew.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ol.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fl.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://to.newstarts.cn

[B15] 布尔运算与取反
来源：http://dp.hahajie.cn

Py:   a and b or not c
来源：http://ae.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://is.wgjwhj.cn

JS:   a && b || !c
来源：http://un.wgjwhj.cn

TS:   a && b || !c
来源：http://ay.shxzskj.cn

Java: a && b || !c
来源：http://kl.hnjuh.cn

Go:   a && b || !c
来源：http://cn.haigaiapp.cn

Ruby: a && b || !c
来源：http://vd.bookmarksfly.cn

C#:   a && b || !c
来源：http://jm.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gs.bjjhwx.cn

Py:   if not data: return
来源：http://tk.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://na.colortex.cn

JS:   if (!data) return;
来源：http://qo.colortex.cn

TS:   if (!data) return;
来源：http://hy.hahajie.cn

Java: if (data == null) return;
来源：http://mp.huixiangedu.cn

Go:   if data == nil { return }
来源：http://vm.lnxyls.cn

Ruby: return if data.nil?
来源：http://sf.hahajie.cn

C#:   if (data == null) return;
来源：http://yd.nszjky.cn

================================================================================
来源：http://kj.nszjky.cn

C. 函数与作用域
来源：http://kq.wgjwhj.cn

================================================================================
来源：http://pg.szsharing.cn

[C01] 定义函数
来源：http://qp.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://kx.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ka.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://pa.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vg.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mr.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uy.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://nz.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nr.hnjuh.cn

[C02] 默认参数
来源：http://li.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://fj.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mw.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://vq.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dd.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zr.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bo.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ua.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://nt.521024.cn

[C03] 可变参数
来源：http://ej.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://ub.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wr.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vg.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qy.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kq.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fz.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hn.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zi.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://fv.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sy.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fz.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://il.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tw.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://um.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://pq.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://sc.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://si.colortex.cn

[C05] 返回多个值
来源：http://sj.panjiajie.cn

Py:   return a, b
来源：http://cb.asd995.cn

PHP:  return [$a, $b];
来源：http://jx.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://je.nszjky.cn

TS:   return { a, b };
来源：http://ag.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kq.521024.cn

Go:   return a, b
来源：http://tu.huixiangedu.cn

Ruby: return a, b
来源：http://ds.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ls.521024.cn

[C06] 匿名函数 / lambda
来源：http://om.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://xs.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ah.asd995.cn

JS:   const square = x => x * x;
来源：http://ob.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://ks.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hu.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xl.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://pv.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gm.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://bc.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zn.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cj.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mb.muxihuayi.cn

TS:   arr.map(String)
来源：http://xp.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ra.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nf.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://wj.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xu.nicolike.cn

[C08] 闭包
来源：http://ld.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rr.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iz.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iy.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cf.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sr.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mu.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://za.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yq.nicolike.cn

[C09] 递归
来源：http://zy.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gm.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mj.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mg.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hm.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hw.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ks.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vh.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fy.yuexingan06.cn

[C10] 变量作用域
来源：http://om.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yv.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dj.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ct.jianghongdianzi.cn

TS:   同 JS
来源：http://oi.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://tz.nicolike.cn

Go:   花括号块级作用域
来源：http://gy.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://op.shxzukj.cn

C#:   块级作用域
来源：http://wz.hnjuh.cn

[C11] 模块导入与导出
来源：http://tt.huanxung.cn

Py:   from module import func
来源：http://dz.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pm.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bi.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cw.yuexingan06.cn

Java: import java.util.List;
来源：http://ys.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://du.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://ln.jianghongdianzi.cn

C#:   using System.Text;
来源：http://wi.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://uq.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://bx.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://cv.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ck.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://gm.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ta.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://lc.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://og.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cd.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://xm.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://la.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://at.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lh.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ty.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wf.szxytkj.cn

Go:   func add(a, b int) int
来源：http://ih.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hr.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ap.bjjhwx.cn

[C14] 泛型函数
来源：http://pq.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dq.szxytkj.cn

PHP:  // 无泛型
来源：http://al.jctech888.com.cn

JS:   // 无泛型
来源：http://nc.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mt.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cy.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pn.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://lt.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://go.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://cd.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mx.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://to.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ps.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xh.yuexingan06.cn

Java: // 无解构
来源：http://mn.colortex.cn

Go:   // 无解构
来源：http://er.bjjhwx.cn

Ruby: a, b = pair
来源：http://ov.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://te.asd995.cn

[C16] 函数 / 方法重载
来源：http://ph.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://le.szsharing.cn

PHP:  // 无重载
来源：http://bp.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://is.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://jj.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yu.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://xg.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://qj.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tw.huixinmuqiang.cn

================================================================================
来源：http://zp.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://cj.wgjwhj.cn

================================================================================
来源：http://wn.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://yx.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dq.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kt.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wb.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mv.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yp.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://fz.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://mv.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ew.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://bx.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://be.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ac.shtwfgs.cn

JS:   arr.push(4);
来源：http://jc.gzmigu.cn

TS:   arr.push(4);
来源：http://yy.nszjky.cn

Java: list.add(4);
来源：http://po.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://co.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://dp.bjjhwx.cn

C#:   list.Add(4);
来源：http://ep.nicolike.cn

[D03] 在指定位置插入元素
来源：http://kr.colortex.cn

Py:   arr.insert(0, 0)
来源：http://xg.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xk.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://to.bookmarksfly.cn


<!-- 参考信息 -->