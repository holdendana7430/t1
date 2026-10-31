代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pz.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mu.huanxung.cn

[B03] switch / match / case
来源：http://hl.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cc.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://io.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mv.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ly.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kj.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dj.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ta.asd995.cn

[B04] for 计数循环
来源：http://rj.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://xb.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lt.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yq.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gf.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gk.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ji.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://fg.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tb.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://zf.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://gy.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ls.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xj.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ng.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://an.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ja.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://bw.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ss.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://fy.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ve.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nj.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hq.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tj.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yy.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://me.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nv.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nn.szxytkj.cn

[B07] while 循环
来源：http://qv.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://sa.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ao.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://mk.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://hw.colortex.cn

Java: while (i < 10) { i++; }
来源：http://by.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fh.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://sy.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://dp.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://dy.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://em.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bj.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://qr.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://jb.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://tu.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tr.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://si.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://iu.muxihuayi.cn

[B09] break 与 continue
来源：http://wp.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pq.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zm.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wl.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yz.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ni.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fu.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://en.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zp.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://dw.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xq.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ma.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wh.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gp.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cj.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rr.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cd.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tw.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://lj.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://jj.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://rr.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hl.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sc.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jp.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pn.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://ja.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ul.asd995.cn

[B12] 跳出多层循环
来源：http://kr.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ks.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wy.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ub.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bi.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ym.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qg.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ce.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wj.hahajie.cn

[B13] 判断是否为数字
来源：http://zb.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://ay.szsharing.cn

PHP:  is_numeric($x)
来源：http://my.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qs.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fy.shxzukj.cn

Java: x instanceof Number
来源：http://ev.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bi.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://ue.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://xd.newstarts.cn

[B14] 判断值是否在集合内
来源：http://vn.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wf.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aw.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://tt.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://vf.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nf.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ch.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ec.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pn.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://sd.bookmarksfly.cn

Py:   a and b or not c
来源：http://jp.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://lv.nicolike.cn

JS:   a && b || !c
来源：http://tz.yuexingan06.cn

TS:   a && b || !c
来源：http://pn.szsharing.cn

Java: a && b || !c
来源：http://nh.colortex.cn

Go:   a && b || !c
来源：http://ga.bjjhwx.cn

Ruby: a && b || !c
来源：http://ek.shxzukj.cn

C#:   a && b || !c
来源：http://ar.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kh.asd995.cn

Py:   if not data: return
来源：http://bq.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ay.hahajie.cn

JS:   if (!data) return;
来源：http://oc.haigaiapp.cn

TS:   if (!data) return;
来源：http://yl.haigaiapp.cn

Java: if (data == null) return;
来源：http://ft.asd995.cn

Go:   if data == nil { return }
来源：http://xx.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://wy.wgjwhj.cn

C#:   if (data == null) return;
来源：http://kj.shtwfgs.cn

================================================================================
来源：http://mg.shtwfgs.cn

C. 函数与作用域
来源：http://qj.yuntaijiaju.cn

================================================================================
来源：http://pq.chemitech.net.cn

[C01] 定义函数
来源：http://lt.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://it.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sl.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://zm.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jd.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ox.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ga.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://ki.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ht.haigaiapp.cn

[C02] 默认参数
来源：http://oh.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://rf.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hx.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://mu.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rq.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://at.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ng.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://eo.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://xg.colortex.cn

[C03] 可变参数
来源：http://ah.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://tk.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lp.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bh.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gc.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://or.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ng.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ow.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nf.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://jp.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ny.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ma.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gc.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xa.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://yv.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://wc.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://sz.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://oj.hahajie.cn

[C05] 返回多个值
来源：http://wg.colortex.cn

Py:   return a, b
来源：http://jb.hnjuh.cn

PHP:  return [$a, $b];
来源：http://si.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tx.yuntaijiaju.cn

TS:   return { a, b };
来源：http://nx.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cz.yuntaijiaju.cn

Go:   return a, b
来源：http://aa.hnjuh.cn

Ruby: return a, b
来源：http://hd.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://cz.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://hz.nszjky.cn

Py:   square = lambda x: x * x
来源：http://oz.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://je.9csxet.cn

JS:   const square = x => x * x;
来源：http://qe.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://ws.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cb.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gb.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://vv.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tj.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://fi.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ip.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ed.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qq.panjiajie.cn

TS:   arr.map(String)
来源：http://fv.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ml.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ol.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://tp.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xw.shxzskj.cn

[C08] 闭包
来源：http://gw.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oe.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zl.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dm.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vr.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gf.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bg.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://md.wgjwhj.cn

[C09] 递归
来源：http://dh.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://st.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vi.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ry.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sx.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nj.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://my.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vg.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ow.huixiangedu.cn

[C10] 变量作用域
来源：http://os.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xi.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cf.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pi.gzmigu.cn

TS:   同 JS
来源：http://mx.shxzukj.cn

Java: 方法内为块级作用域
来源：http://md.huanxung.cn

Go:   花括号块级作用域
来源：http://xt.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gb.lnxyls.cn

C#:   块级作用域
来源：http://mr.haigaiapp.cn

[C11] 模块导入与导出
来源：http://mx.chemitech.net.cn

Py:   from module import func
来源：http://wa.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mu.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://op.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://do.hnjuh.cn

Java: import java.util.List;
来源：http://uc.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://et.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://tk.szsharing.cn

C#:   using System.Text;
来源：http://if.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://ns.asd995.cn

Py:   (lambda: print("run"))()
来源：http://nk.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://bz.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://ww.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://ce.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://du.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://ae.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://fi.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ly.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://cz.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pm.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sl.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ht.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ab.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://an.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://lj.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kg.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qi.hnjuh.cn

[C14] 泛型函数
来源：http://ic.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jx.colortex.cn

PHP:  // 无泛型
来源：http://ti.9csxet.cn

JS:   // 无泛型
来源：http://lk.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ic.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pl.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://du.newstarts.cn

Ruby: # 无泛型
来源：http://lv.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jc.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://gr.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yw.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://oz.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bu.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dt.shxzukj.cn

Java: // 无解构
来源：http://bt.haigaiapp.cn

Go:   // 无解构
来源：http://xg.colortex.cn

Ruby: a, b = pair
来源：http://cm.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://sg.huanxung.cn

[C16] 函数 / 方法重载
来源：http://yx.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vz.chemitech.net.cn

PHP:  // 无重载
来源：http://kj.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zs.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://hh.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ks.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://ce.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://lt.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pj.bjjhwx.cn

================================================================================
来源：http://zg.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://ps.newstarts.cn

================================================================================
来源：http://tg.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://xm.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qs.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gf.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ak.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xv.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yp.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://qq.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://wk.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://va.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://jh.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://il.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lw.bjjhwx.cn

JS:   arr.push(4);
来源：http://cs.szxytkj.cn

TS:   arr.push(4);
来源：http://mr.huanxung.cn

Java: list.add(4);
来源：http://ot.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://dh.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://fc.newstarts.cn

C#:   list.Add(4);
来源：http://li.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://sw.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://wd.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vx.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iv.gzmigu.cn


<!-- 参考信息 -->