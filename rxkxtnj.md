代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zs.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lk.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ky.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aa.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://az.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wu.colortex.cn

[B04] for 计数循环
来源：http://bg.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://qs.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oi.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ek.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://si.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fh.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ai.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://sv.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xz.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://dj.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://hi.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xg.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ur.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ju.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rm.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wj.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://um.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qo.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://xi.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nf.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mq.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tb.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fm.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gp.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ki.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mx.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xa.bookmarksfly.cn

[B07] while 循环
来源：http://uf.newstarts.cn

Py:   while i < 10: i += 1
来源：http://zd.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gs.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://kq.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://ib.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://kj.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hb.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://it.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://od.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://bw.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://st.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vu.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://zg.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://qe.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://wj.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ip.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nj.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://vb.gzmigu.cn

[B09] break 与 continue
来源：http://ed.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ml.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mc.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ei.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://if.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ls.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bj.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lt.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gx.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ko.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ou.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oo.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fs.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yr.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pr.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rf.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uq.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ow.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://js.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://tb.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://lh.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sk.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dz.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kb.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vg.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://lx.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hv.yuexingan06.cn

[B12] 跳出多层循环
来源：http://mt.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bn.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wr.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sm.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zr.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ku.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://op.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iq.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ut.lnxyls.cn

[B13] 判断是否为数字
来源：http://ih.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://zu.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://gx.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xb.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nz.9csxet.cn

Java: x instanceof Number
来源：http://pv.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hv.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://dg.nszjky.cn

C#:   x is int or double or decimal
来源：http://as.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://oi.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ms.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ej.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://tu.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://zs.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pc.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lf.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eh.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rw.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://hr.hnjuh.cn

Py:   a and b or not c
来源：http://fk.9csxet.cn

PHP:  $a && $b || !$c
来源：http://sn.nicolike.cn

JS:   a && b || !c
来源：http://jk.chemitech.net.cn

TS:   a && b || !c
来源：http://gy.asd995.cn

Java: a && b || !c
来源：http://rz.nicolike.cn

Go:   a && b || !c
来源：http://uo.szxytkj.cn

Ruby: a && b || !c
来源：http://vp.szxytkj.cn

C#:   a && b || !c
来源：http://fc.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xp.bookmarksfly.cn

Py:   if not data: return
来源：http://ru.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://us.nszjky.cn

JS:   if (!data) return;
来源：http://as.9csxet.cn

TS:   if (!data) return;
来源：http://um.wgjwhj.cn

Java: if (data == null) return;
来源：http://in.haigaiapp.cn

Go:   if data == nil { return }
来源：http://yh.shtwfgs.cn

Ruby: return if data.nil?
来源：http://hr.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://ah.shxzskj.cn

================================================================================
来源：http://pl.9csxet.cn

C. 函数与作用域
来源：http://hw.chemitech.net.cn

================================================================================
来源：http://gr.bookmarksfly.cn

[C01] 定义函数
来源：http://lo.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://kj.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oi.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ni.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://as.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hr.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pq.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://ft.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pg.szxytkj.cn

[C02] 默认参数
来源：http://nj.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://ks.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dr.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://zy.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tm.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jp.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lj.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://wc.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://wx.muxihuayi.cn

[C03] 可变参数
来源：http://sm.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://eg.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lp.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://id.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uf.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vh.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bh.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tn.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qc.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ym.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tk.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jr.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qw.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vx.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://iy.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://ow.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://up.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://sn.hnjuh.cn

[C05] 返回多个值
来源：http://wz.szxytkj.cn

Py:   return a, b
来源：http://pa.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://rt.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jb.jctech888.com.cn

TS:   return { a, b };
来源：http://ur.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sc.muxihuayi.cn

Go:   return a, b
来源：http://ut.hahajie.cn

Ruby: return a, b
来源：http://tp.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ua.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://sm.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://us.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mk.huanxung.cn

JS:   const square = x => x * x;
来源：http://bn.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ec.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lc.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dr.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://mb.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ho.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://ls.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vh.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://an.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bp.nszjky.cn

TS:   arr.map(String)
来源：http://iq.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gl.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://el.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://mw.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://se.yuexingan06.cn

[C08] 闭包
来源：http://io.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hu.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://da.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gd.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uo.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qw.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gq.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://is.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cp.colortex.cn

[C09] 递归
来源：http://js.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xi.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qi.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://si.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xq.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rw.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hk.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ll.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jp.nicolike.cn

[C10] 变量作用域
来源：http://de.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sx.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pj.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rj.nicolike.cn

TS:   同 JS
来源：http://hs.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://sr.shxzskj.cn

Go:   花括号块级作用域
来源：http://jl.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nt.huixiangedu.cn

C#:   块级作用域
来源：http://hb.shxzukj.cn

[C11] 模块导入与导出
来源：http://jd.hahajie.cn

Py:   from module import func
来源：http://hn.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mh.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://my.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mn.szxytkj.cn

Java: import java.util.List;
来源：http://fr.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aw.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ef.szsharing.cn

C#:   using System.Text;
来源：http://jd.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://ux.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://ob.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://un.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://hj.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://re.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lm.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://eb.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://eb.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uz.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://au.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sj.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gu.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lx.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wh.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://da.lnxyls.cn

Go:   func add(a, b int) int
来源：http://et.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lv.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dp.colortex.cn

[C14] 泛型函数
来源：http://wa.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rz.hahajie.cn

PHP:  // 无泛型
来源：http://ac.gzmigu.cn

JS:   // 无泛型
来源：http://hu.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cu.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ej.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ik.nszjky.cn

Ruby: # 无泛型
来源：http://aa.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ba.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://bh.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gh.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://bw.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ih.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xf.huixiangedu.cn

Java: // 无解构
来源：http://qc.muxihuayi.cn

Go:   // 无解构
来源：http://cw.colortex.cn

Ruby: a, b = pair
来源：http://pj.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://si.nicolike.cn

[C16] 函数 / 方法重载
来源：http://tg.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bo.lnxyls.cn

PHP:  // 无重载
来源：http://ge.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nc.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://yi.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qe.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://qq.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://bc.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bh.shxzskj.cn

================================================================================
来源：http://ng.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://tw.lnxyls.cn

================================================================================
来源：http://je.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://di.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ei.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zi.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fd.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nl.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ys.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://jo.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://yt.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qq.shxzskj.cn

[D02] 追加元素到末尾
来源：http://kg.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lf.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bt.wgjwhj.cn

JS:   arr.push(4);
来源：http://qe.huanxung.cn

TS:   arr.push(4);
来源：http://pi.wgjwhj.cn

Java: list.add(4);
来源：http://sn.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://xq.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://pm.jctech888.com.cn

C#:   list.Add(4);
来源：http://wq.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://ol.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://za.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ll.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cs.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://bz.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://ns.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kj.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cz.colortex.cn


<!-- 参考信息 -->