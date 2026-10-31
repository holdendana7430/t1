代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ij.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ff.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yp.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yx.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ib.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zs.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wi.shxzskj.cn

[B04] for 计数循环
来源：http://xy.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://jn.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fm.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oq.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ib.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ws.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ir.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://tk.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kv.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://nq.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://at.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kr.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kp.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tu.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bq.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sx.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://kg.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ov.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://yh.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://or.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mc.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iq.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pj.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qi.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vy.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fg.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://od.colortex.cn

[B07] while 循环
来源：http://az.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://yc.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ha.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://yl.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://yb.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://fk.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kv.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ri.521024.cn

C#:   while (i < 10) { i++; }
来源：http://co.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://my.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://ib.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ah.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://qx.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://of.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://hw.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gn.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://br.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://ip.hahajie.cn

[B09] break 与 continue
来源：http://ao.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zn.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bo.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sm.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ps.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fx.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kp.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kr.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nr.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://iy.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qe.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yg.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rl.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dg.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://af.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cn.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qk.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uc.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://et.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://om.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://lc.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hx.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tl.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vm.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qi.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://tv.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jj.szxytkj.cn

[B12] 跳出多层循环
来源：http://vo.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ru.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yg.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wy.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nn.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://so.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oh.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mf.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lx.huixiangedu.cn

[B13] 判断是否为数字
来源：http://qu.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://ft.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://wi.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wl.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dq.newstarts.cn

Java: x instanceof Number
来源：http://ux.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vf.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://na.521024.cn

C#:   x is int or double or decimal
来源：http://qf.hahajie.cn

[B14] 判断值是否在集合内
来源：http://iv.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mq.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qp.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://un.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://gp.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ni.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tq.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fk.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zs.szsharing.cn

[B15] 布尔运算与取反
来源：http://bw.lnxyls.cn

Py:   a and b or not c
来源：http://yn.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://tc.panjiajie.cn

JS:   a && b || !c
来源：http://dp.wgjwhj.cn

TS:   a && b || !c
来源：http://ur.asd995.cn

Java: a && b || !c
来源：http://kh.shtwfgs.cn

Go:   a && b || !c
来源：http://pr.lnxyls.cn

Ruby: a && b || !c
来源：http://pg.hnjuh.cn

C#:   a && b || !c
来源：http://ob.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://td.szxytkj.cn

Py:   if not data: return
来源：http://xq.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://vt.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://ep.bookmarksfly.cn

TS:   if (!data) return;
来源：http://mp.521024.cn

Java: if (data == null) return;
来源：http://jh.521024.cn

Go:   if data == nil { return }
来源：http://zj.colortex.cn

Ruby: return if data.nil?
来源：http://th.lnxyls.cn

C#:   if (data == null) return;
来源：http://wx.521024.cn

================================================================================
来源：http://pq.colortex.cn

C. 函数与作用域
来源：http://on.jianghongdianzi.cn

================================================================================
来源：http://ar.lnxyls.cn

[C01] 定义函数
来源：http://qk.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://mz.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oi.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://vl.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bh.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qw.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pr.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://aa.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vy.wgjwhj.cn

[C02] 默认参数
来源：http://yk.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://zj.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ne.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://mj.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uw.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ic.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://us.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://rw.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://fj.hnjuh.cn

[C03] 可变参数
来源：http://um.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://ur.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cy.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bu.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ak.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kv.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://og.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bk.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sv.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://js.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qe.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sq.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sf.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lx.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://dh.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://uc.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://ka.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://vm.lnxyls.cn

[C05] 返回多个值
来源：http://bk.asd995.cn

Py:   return a, b
来源：http://kx.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://ge.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wq.szsharing.cn

TS:   return { a, b };
来源：http://gq.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mg.huixiangedu.cn

Go:   return a, b
来源：http://mc.yuexingan06.cn

Ruby: return a, b
来源：http://ei.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ba.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://uy.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://kn.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hs.gzmigu.cn

JS:   const square = x => x * x;
来源：http://vz.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://sb.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fz.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kw.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://ma.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ir.hahajie.cn

[C07] 把函数作为参数传入
来源：http://rb.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mg.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bf.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wm.muxihuayi.cn

TS:   arr.map(String)
来源：http://dg.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://et.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xk.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://gm.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://je.bjjhwx.cn

[C08] 闭包
来源：http://ki.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://un.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fx.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vc.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mx.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://en.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ve.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dy.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ae.haigaiapp.cn

[C09] 递归
来源：http://ny.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://by.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lb.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ri.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tx.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ah.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://et.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tl.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sh.nszjky.cn

[C10] 变量作用域
来源：http://ye.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vs.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lz.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jq.huixiangedu.cn

TS:   同 JS
来源：http://ir.colortex.cn

Java: 方法内为块级作用域
来源：http://yc.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://rv.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iy.shxzskj.cn

C#:   块级作用域
来源：http://li.gzmigu.cn

[C11] 模块导入与导出
来源：http://ha.muxihuayi.cn

Py:   from module import func
来源：http://ue.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zd.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tm.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mh.bjjhwx.cn

Java: import java.util.List;
来源：http://xe.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mh.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://jj.shxzukj.cn

C#:   using System.Text;
来源：http://dc.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://sw.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://gn.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://ct.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://nv.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://vd.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cv.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://cy.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://rv.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xx.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://hl.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yx.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tn.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hr.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://it.nszjky.cn

Go:   func add(a, b int) int
来源：http://sm.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dd.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kt.panjiajie.cn

[C14] 泛型函数
来源：http://ri.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ji.nicolike.cn

PHP:  // 无泛型
来源：http://if.chemitech.net.cn

JS:   // 无泛型
来源：http://bb.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bc.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sq.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dr.chemitech.net.cn

Ruby: # 无泛型
来源：http://ws.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qi.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://wd.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jz.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://xo.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hc.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jg.newstarts.cn

Java: // 无解构
来源：http://ms.muxihuayi.cn

Go:   // 无解构
来源：http://em.szxytkj.cn

Ruby: a, b = pair
来源：http://td.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://nj.9csxet.cn

[C16] 函数 / 方法重载
来源：http://jl.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oy.colortex.cn

PHP:  // 无重载
来源：http://br.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wy.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://hy.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pp.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://ta.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://rq.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lk.shtwfgs.cn

================================================================================
来源：http://rg.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://wa.hnjuh.cn

================================================================================
来源：http://xc.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://id.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qk.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ie.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sm.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mq.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gk.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://jl.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://vd.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sg.shxzskj.cn

[D02] 追加元素到末尾
来源：http://sj.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xp.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fu.shtwfgs.cn

JS:   arr.push(4);
来源：http://ra.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://je.chemitech.net.cn

Java: list.add(4);
来源：http://jf.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://ja.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://iy.huixiangedu.cn

C#:   list.Add(4);
来源：http://xn.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://pb.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://af.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rc.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sv.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://bl.panjiajie.cn

Java: list.add(0, 0);
来源：http://ke.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mw.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wd.shtwfgs.cn


<!-- 参考信息 -->