代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ra.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dp.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ed.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mj.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://km.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kd.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gp.shtwfgs.cn

[B04] for 计数循环
来源：http://nn.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://dr.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fk.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kq.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tt.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qs.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sx.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://no.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jx.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://qh.nszjky.cn

Py:   for item in arr: print(item)
来源：http://sj.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lq.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hr.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rb.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hx.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cb.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://fr.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://za.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://pw.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yq.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qo.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uf.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ay.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rt.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pw.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zw.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ze.shtwfgs.cn

[B07] while 循环
来源：http://fc.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://md.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gc.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://zg.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://tb.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://ur.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ia.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://pu.521024.cn

C#:   while (i < 10) { i++; }
来源：http://ym.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://yh.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://er.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://df.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://be.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://zn.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://sp.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rl.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eu.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://va.muxihuayi.cn

[B09] break 与 continue
来源：http://qb.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ag.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jq.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://va.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rw.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wq.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ba.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://tf.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ah.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eb.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kl.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bv.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ln.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yk.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gl.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xh.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://sg.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://qd.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://gw.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fx.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vv.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ry.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zg.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://hm.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ra.nicolike.cn

[B12] 跳出多层循环
来源：http://lk.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mz.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ev.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nl.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yd.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uq.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rx.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lf.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fr.hahajie.cn

[B13] 判断是否为数字
来源：http://zt.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://px.szxytkj.cn

PHP:  is_numeric($x)
来源：http://dz.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gc.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xq.shtwfgs.cn

Java: x instanceof Number
来源：http://gb.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rs.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://mc.panjiajie.cn

C#:   x is int or double or decimal
来源：http://vt.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://wc.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://js.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sd.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://nx.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://sw.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ux.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zj.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qy.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dh.szxytkj.cn

[B15] 布尔运算与取反
来源：http://na.chemitech.net.cn

Py:   a and b or not c
来源：http://do.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://zq.panjiajie.cn

JS:   a && b || !c
来源：http://qz.asd995.cn

TS:   a && b || !c
来源：http://vw.bookmarksfly.cn

Java: a && b || !c
来源：http://kd.wgjwhj.cn

Go:   a && b || !c
来源：http://fj.hnjuh.cn

Ruby: a && b || !c
来源：http://ds.chemitech.net.cn

C#:   a && b || !c
来源：http://ir.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uh.chemitech.net.cn

Py:   if not data: return
来源：http://jt.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://ox.panjiajie.cn

JS:   if (!data) return;
来源：http://zo.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://zt.huanxung.cn

Java: if (data == null) return;
来源：http://pz.hahajie.cn

Go:   if data == nil { return }
来源：http://qy.huanxung.cn

Ruby: return if data.nil?
来源：http://gm.colortex.cn

C#:   if (data == null) return;
来源：http://dw.szxytkj.cn

================================================================================
来源：http://tw.yuexingan06.cn

C. 函数与作用域
来源：http://uf.panjiajie.cn

================================================================================
来源：http://av.shxzskj.cn

[C01] 定义函数
来源：http://tn.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ip.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qw.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://tu.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bj.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kl.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://po.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://tm.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nb.chemitech.net.cn

[C02] 默认参数
来源：http://ps.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://nu.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ch.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qv.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mj.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cp.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://du.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://ia.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://pr.szsharing.cn

[C03] 可变参数
来源：http://df.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://bs.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qv.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ax.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mm.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xv.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qr.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ae.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fl.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://pf.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ju.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xf.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vd.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mq.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://mf.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://sr.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://pw.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://qa.szxytkj.cn

[C05] 返回多个值
来源：http://mv.szxytkj.cn

Py:   return a, b
来源：http://fm.shxzukj.cn

PHP:  return [$a, $b];
来源：http://az.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tc.bookmarksfly.cn

TS:   return { a, b };
来源：http://fj.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fi.shxzukj.cn

Go:   return a, b
来源：http://fl.bjjhwx.cn

Ruby: return a, b
来源：http://qw.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://vi.521024.cn

[C06] 匿名函数 / lambda
来源：http://sw.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://hp.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qm.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://je.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://zq.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fl.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iz.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://tw.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ur.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://ik.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wc.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gn.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rg.haigaiapp.cn

TS:   arr.map(String)
来源：http://ze.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://at.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mu.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://bk.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tw.jctech888.com.cn

[C08] 闭包
来源：http://kj.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yu.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sq.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jb.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ju.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://su.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xt.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uj.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rx.muxihuayi.cn

[C09] 递归
来源：http://xg.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dn.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sg.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xy.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fq.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qi.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://va.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vh.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jh.nicolike.cn

[C10] 变量作用域
来源：http://nw.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fu.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vj.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://td.haigaiapp.cn

TS:   同 JS
来源：http://pd.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://ek.nicolike.cn

Go:   花括号块级作用域
来源：http://hh.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wu.hnjuh.cn

C#:   块级作用域
来源：http://ym.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://hg.jianghongdianzi.cn

Py:   from module import func
来源：http://wm.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bm.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fp.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cy.huanxung.cn

Java: import java.util.List;
来源：http://pc.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://is.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://co.shxzskj.cn

C#:   using System.Text;
来源：http://oh.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://dr.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://qh.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://yi.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://hs.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://nr.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bg.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://fu.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://bt.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ov.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://rm.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ko.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ie.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wt.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pd.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://of.shxzukj.cn

Go:   func add(a, b int) int
来源：http://jf.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fb.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cx.huanxung.cn

[C14] 泛型函数
来源：http://ux.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ll.haigaiapp.cn

PHP:  // 无泛型
来源：http://yk.panjiajie.cn

JS:   // 无泛型
来源：http://pf.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wd.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sp.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uh.shxzukj.cn

Ruby: # 无泛型
来源：http://gq.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://at.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://bj.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wc.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://eh.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ir.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tf.shtwfgs.cn

Java: // 无解构
来源：http://rl.haigaiapp.cn

Go:   // 无解构
来源：http://mz.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://cq.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://yc.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://bi.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ac.nicolike.cn

PHP:  // 无重载
来源：http://mc.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jn.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://kp.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wl.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://cj.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://jy.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sz.gzmigu.cn

================================================================================
来源：http://dt.521024.cn

D. 数组 / 列表 / 集合
来源：http://kg.panjiajie.cn

================================================================================
来源：http://wa.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://pc.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tj.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ds.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iw.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sx.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://kk.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://hf.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lk.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://wv.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sl.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uk.chemitech.net.cn

JS:   arr.push(4);
来源：http://jz.521024.cn

TS:   arr.push(4);
来源：http://gv.panjiajie.cn

Java: list.add(4);
来源：http://fm.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://qi.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://kn.nszjky.cn

C#:   list.Add(4);
来源：http://vy.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://iy.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://yt.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xe.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hq.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://cy.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://dh.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pf.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qd.jctech888.com.cn


<!-- 参考信息 -->