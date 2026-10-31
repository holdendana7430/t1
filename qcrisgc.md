代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ej.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tj.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ou.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kw.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wv.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ic.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pt.bjjhwx.cn

[B04] for 计数循环
来源：http://tk.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://qd.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rh.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dv.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cw.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hf.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ca.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://uj.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uh.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://ah.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://kp.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ix.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ng.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://se.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ev.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://va.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://zg.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qm.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://tl.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tn.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rs.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kk.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wt.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yj.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jf.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ee.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lo.lnxyls.cn

[B07] while 循环
来源：http://au.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://fh.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ap.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://mu.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://bz.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://id.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pc.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://pq.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://zk.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://mv.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://xj.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gd.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://bz.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://rb.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://lb.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gp.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jk.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://qo.jianghongdianzi.cn

[B09] break 与 continue
来源：http://zu.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qh.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zt.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ii.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nx.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nx.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wp.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ft.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ki.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://ss.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ey.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bq.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jw.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gc.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yw.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lh.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ai.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cn.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://gv.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://rw.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://td.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://es.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nm.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ap.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wt.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://ne.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bk.hahajie.cn

[B12] 跳出多层循环
来源：http://uw.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ba.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ji.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fx.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ki.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wk.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vp.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uk.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nn.szsharing.cn

[B13] 判断是否为数字
来源：http://uj.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://tu.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://qe.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tb.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rx.lnxyls.cn

Java: x instanceof Number
来源：http://dj.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ab.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://az.shxzukj.cn

C#:   x is int or double or decimal
来源：http://ih.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://mr.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lk.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xc.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://ie.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://pw.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nv.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://db.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kz.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lp.shxzskj.cn

[B15] 布尔运算与取反
来源：http://sw.szsharing.cn

Py:   a and b or not c
来源：http://lj.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://tv.gzmigu.cn

JS:   a && b || !c
来源：http://kv.shxzskj.cn

TS:   a && b || !c
来源：http://sb.9csxet.cn

Java: a && b || !c
来源：http://db.yuexingan06.cn

Go:   a && b || !c
来源：http://hq.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://rk.gzmigu.cn

C#:   a && b || !c
来源：http://ib.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lu.nicolike.cn

Py:   if not data: return
来源：http://gf.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://eg.nicolike.cn

JS:   if (!data) return;
来源：http://wu.521024.cn

TS:   if (!data) return;
来源：http://gb.shtwfgs.cn

Java: if (data == null) return;
来源：http://uf.huanxung.cn

Go:   if data == nil { return }
来源：http://pf.huanxung.cn

Ruby: return if data.nil?
来源：http://yw.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://oa.hahajie.cn

================================================================================
来源：http://qv.haigaiapp.cn

C. 函数与作用域
来源：http://da.szxytkj.cn

================================================================================
来源：http://zy.9csxet.cn

[C01] 定义函数
来源：http://si.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://cb.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tj.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://hx.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gw.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dz.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hp.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://fv.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wt.huixinmuqiang.cn

[C02] 默认参数
来源：http://it.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://yp.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qw.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://ka.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zd.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pm.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uu.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ja.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://qi.bookmarksfly.cn

[C03] 可变参数
来源：http://er.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://bm.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zl.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fs.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xr.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ik.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qp.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fx.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sh.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://or.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mc.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lv.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://my.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fy.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://yf.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://go.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://hv.521024.cn

C#:   f(a: 1, b: 2)
来源：http://qu.szsharing.cn

[C05] 返回多个值
来源：http://zv.jctech888.com.cn

Py:   return a, b
来源：http://xx.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://xl.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ac.lnxyls.cn

TS:   return { a, b };
来源：http://zi.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dk.jianghongdianzi.cn

Go:   return a, b
来源：http://rq.szxytkj.cn

Ruby: return a, b
来源：http://sz.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://yv.colortex.cn

[C06] 匿名函数 / lambda
来源：http://dj.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://xk.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bz.gzmigu.cn

JS:   const square = x => x * x;
来源：http://mu.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://wp.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yn.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iy.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://gx.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bz.szsharing.cn

[C07] 把函数作为参数传入
来源：http://tr.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://if.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://as.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://if.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://xw.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hs.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jz.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://zl.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bt.hahajie.cn

[C08] 闭包
来源：http://yh.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ns.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ca.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uf.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://es.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pk.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://if.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cm.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bx.chemitech.net.cn

[C09] 递归
来源：http://tw.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bi.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ou.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://it.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cd.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qi.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yf.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vw.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://si.521024.cn

[C10] 变量作用域
来源：http://pj.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zg.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gw.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xb.haigaiapp.cn

TS:   同 JS
来源：http://as.szxytkj.cn

Java: 方法内为块级作用域
来源：http://rn.hnjuh.cn

Go:   花括号块级作用域
来源：http://vg.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ec.lnxyls.cn

C#:   块级作用域
来源：http://cx.colortex.cn

[C11] 模块导入与导出
来源：http://jg.yuexingan06.cn

Py:   from module import func
来源：http://qn.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zy.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://og.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dt.yuexingan06.cn

Java: import java.util.List;
来源：http://kz.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ow.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://rx.chemitech.net.cn

C#:   using System.Text;
来源：http://xc.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://xu.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://cr.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://xq.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://go.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://qk.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://po.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://ww.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://ag.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bt.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://cw.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fh.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ll.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wv.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qw.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cz.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://bm.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ge.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ok.asd995.cn

[C14] 泛型函数
来源：http://ra.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cp.huanxung.cn

PHP:  // 无泛型
来源：http://vh.bjjhwx.cn

JS:   // 无泛型
来源：http://eq.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jq.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pe.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hv.nicolike.cn

Ruby: # 无泛型
来源：http://aj.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cj.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://ge.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://en.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://by.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wr.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pb.nicolike.cn

Java: // 无解构
来源：http://aw.haigaiapp.cn

Go:   // 无解构
来源：http://ff.szsharing.cn

Ruby: a, b = pair
来源：http://qv.szsharing.cn

C#:   var (a, b) = pair;
来源：http://jz.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://vj.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ns.yuntaijiaju.cn

PHP:  // 无重载
来源：http://bm.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ra.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://uz.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mq.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://ni.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://um.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qw.hahajie.cn

================================================================================
来源：http://oj.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://mz.lnxyls.cn

================================================================================
来源：http://fs.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://yz.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mf.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zo.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qx.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dn.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xs.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://sd.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://qv.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yx.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://jy.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kq.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jv.muxihuayi.cn

JS:   arr.push(4);
来源：http://eb.hahajie.cn

TS:   arr.push(4);
来源：http://rc.colortex.cn

Java: list.add(4);
来源：http://pl.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://bj.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://gn.bookmarksfly.cn

C#:   list.Add(4);
来源：http://oi.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://aq.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://so.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cw.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cj.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://hw.chemitech.net.cn

Java: list.add(0, 0);
来源：http://yn.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://va.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dt.shxzskj.cn


<!-- 参考信息 -->