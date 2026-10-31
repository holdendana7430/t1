代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bf.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ov.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ud.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zp.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://no.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yv.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pa.shxzukj.cn

[B04] for 计数循环
来源：http://br.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://ay.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jt.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zm.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wt.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ir.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ab.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://ac.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wr.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://uv.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://uf.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ak.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dc.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vk.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ea.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cy.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://at.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wq.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://hd.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mm.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wl.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gv.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ow.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://px.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sm.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wu.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vs.nicolike.cn

[B07] while 循环
来源：http://dq.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://he.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zq.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://bc.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://bf.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://rx.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xh.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://zj.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ld.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://pr.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://tr.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xt.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://pa.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://dz.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://ua.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pf.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lx.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://vb.huixinmuqiang.cn

[B09] break 与 continue
来源：http://sx.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nr.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tm.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aq.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yj.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://se.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://by.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://on.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yg.colortex.cn

[B10] 遍历同时拿索引
来源：http://ut.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iu.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pt.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cu.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oh.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yb.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kg.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rc.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tn.521024.cn

[B11] 生成数字序列 / 区间
来源：http://mc.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://km.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://gz.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ph.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dn.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qs.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://se.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://pr.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qk.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://ft.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rc.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oh.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pl.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fa.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ns.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gk.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xz.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ws.nszjky.cn

[B13] 判断是否为数字
来源：http://jd.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://ll.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://aa.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cy.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ah.colortex.cn

Java: x instanceof Number
来源：http://jk.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xw.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://rt.hahajie.cn

C#:   x is int or double or decimal
来源：http://fs.nszjky.cn

[B14] 判断值是否在集合内
来源：http://ym.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yp.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gg.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://aw.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://ms.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ko.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nh.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://av.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ar.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://zt.yuexingan06.cn

Py:   a and b or not c
来源：http://js.hahajie.cn

PHP:  $a && $b || !$c
来源：http://us.panjiajie.cn

JS:   a && b || !c
来源：http://cp.huixinmuqiang.cn

TS:   a && b || !c
来源：http://as.newstarts.cn

Java: a && b || !c
来源：http://rb.yuntaijiaju.cn

Go:   a && b || !c
来源：http://sw.wgjwhj.cn

Ruby: a && b || !c
来源：http://zh.jctech888.com.cn

C#:   a && b || !c
来源：http://fr.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mr.haigaiapp.cn

Py:   if not data: return
来源：http://uc.521024.cn

PHP:  if (!$data) { return; }
来源：http://ab.haigaiapp.cn

JS:   if (!data) return;
来源：http://cw.nicolike.cn

TS:   if (!data) return;
来源：http://hs.hnjuh.cn

Java: if (data == null) return;
来源：http://hd.hnjuh.cn

Go:   if data == nil { return }
来源：http://sx.hnjuh.cn

Ruby: return if data.nil?
来源：http://kx.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://kc.chemitech.net.cn

================================================================================
来源：http://vl.jctech888.com.cn

C. 函数与作用域
来源：http://xl.jctech888.com.cn

================================================================================
来源：http://sf.panjiajie.cn

[C01] 定义函数
来源：http://ym.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://ia.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sl.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://as.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eq.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vr.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ne.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://oh.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ku.wgjwhj.cn

[C02] 默认参数
来源：http://ps.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://xc.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ap.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://is.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pg.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dh.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bk.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://hj.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://tq.chemitech.net.cn

[C03] 可变参数
来源：http://ya.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://kr.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mb.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xo.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gk.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qd.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hk.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hr.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ie.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://jv.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xr.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tf.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oz.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pt.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://bg.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://si.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://gz.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://hg.panjiajie.cn

[C05] 返回多个值
来源：http://ka.huixinmuqiang.cn

Py:   return a, b
来源：http://ey.shxzskj.cn

PHP:  return [$a, $b];
来源：http://dx.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://du.newstarts.cn

TS:   return { a, b };
来源：http://es.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ac.shtwfgs.cn

Go:   return a, b
来源：http://qw.lnxyls.cn

Ruby: return a, b
来源：http://od.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://fj.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://rg.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://ha.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eb.szxytkj.cn

JS:   const square = x => x * x;
来源：http://yo.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://xz.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xt.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rg.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://il.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ts.newstarts.cn

[C07] 把函数作为参数传入
来源：http://ov.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://it.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lk.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ha.huanxung.cn

TS:   arr.map(String)
来源：http://lz.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rv.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ev.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://iz.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tt.colortex.cn

[C08] 闭包
来源：http://og.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tu.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oj.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ot.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nt.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bh.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nl.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ol.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://co.huanxung.cn

[C09] 递归
来源：http://ay.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tw.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://to.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rp.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ia.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dt.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dl.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ii.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pa.huixiangedu.cn

[C10] 变量作用域
来源：http://dv.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ww.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ja.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nz.9csxet.cn

TS:   同 JS
来源：http://la.9csxet.cn

Java: 方法内为块级作用域
来源：http://qg.shtwfgs.cn

Go:   花括号块级作用域
来源：http://xz.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://si.szxytkj.cn

C#:   块级作用域
来源：http://lt.huanxung.cn

[C11] 模块导入与导出
来源：http://zl.yuexingan06.cn

Py:   from module import func
来源：http://hm.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gv.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lf.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ya.huixiangedu.cn

Java: import java.util.List;
来源：http://bm.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bx.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://pg.9csxet.cn

C#:   using System.Text;
来源：http://cm.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://ke.colortex.cn

Py:   (lambda: print("run"))()
来源：http://ve.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://pa.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://os.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://we.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sg.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://jo.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://oy.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oa.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://bd.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ye.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sv.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ro.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jw.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://af.9csxet.cn

Go:   func add(a, b int) int
来源：http://au.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rx.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mr.bjjhwx.cn

[C14] 泛型函数
来源：http://yw.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bc.9csxet.cn

PHP:  // 无泛型
来源：http://th.szsharing.cn

JS:   // 无泛型
来源：http://lo.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jw.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dr.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sw.newstarts.cn

Ruby: # 无泛型
来源：http://te.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ie.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://mk.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ka.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://xq.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tc.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ha.shxzskj.cn

Java: // 无解构
来源：http://fr.szxytkj.cn

Go:   // 无解构
来源：http://nt.bjjhwx.cn

Ruby: a, b = pair
来源：http://if.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://fz.newstarts.cn

[C16] 函数 / 方法重载
来源：http://kp.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ux.gzmigu.cn

PHP:  // 无重载
来源：http://og.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ii.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://jc.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hr.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://eu.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://ik.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ke.shxzukj.cn

================================================================================
来源：http://sa.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://ht.muxihuayi.cn

================================================================================
来源：http://dk.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://dz.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://be.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lk.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fu.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mu.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bn.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://rj.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://se.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ep.asd995.cn

[D02] 追加元素到末尾
来源：http://yh.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sa.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lk.jctech888.com.cn

JS:   arr.push(4);
来源：http://qz.muxihuayi.cn

TS:   arr.push(4);
来源：http://el.521024.cn

Java: list.add(4);
来源：http://vo.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://rq.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ex.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://al.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://ix.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://nw.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://di.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nz.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://jg.colortex.cn

Java: list.add(0, 0);
来源：http://tc.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yv.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ly.bookmarksfly.cn


<!-- 参考信息 -->