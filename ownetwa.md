代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sh.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sn.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://da.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aq.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eg.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pd.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mq.muxihuayi.cn

[B04] for 计数循环
来源：http://rq.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://km.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://op.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dy.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gu.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pc.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://za.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://lg.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://le.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://gm.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://oj.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ml.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bg.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pc.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ue.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bm.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://xr.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qp.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://ky.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sc.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xt.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vj.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jw.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lr.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pf.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wo.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sg.wgjwhj.cn

[B07] while 循环
来源：http://av.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://uw.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hz.521024.cn

JS:   while (i < 10) { i++; }
来源：http://tb.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://ca.colortex.cn

Java: while (i < 10) { i++; }
来源：http://sa.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gu.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://lt.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://dn.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://jx.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://as.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xx.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://va.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://zu.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://fe.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://le.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dv.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://ro.521024.cn

[B09] break 与 continue
来源：http://cb.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ss.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://as.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gd.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ey.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xu.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://th.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ay.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://wg.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pq.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hv.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vv.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ah.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cn.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://up.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mo.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://at.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://bp.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://tx.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://cj.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lp.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yw.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tk.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ll.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://uv.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://es.gzmigu.cn

[B12] 跳出多层循环
来源：http://xj.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ar.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uv.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fq.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fh.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wp.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zv.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yz.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fd.haigaiapp.cn

[B13] 判断是否为数字
来源：http://qp.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://li.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://pq.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vw.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oz.panjiajie.cn

Java: x instanceof Number
来源：http://hd.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mm.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://cr.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://ly.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://cc.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ut.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vf.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://nu.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://zy.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ju.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bv.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qv.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pv.hahajie.cn

[B15] 布尔运算与取反
来源：http://un.jctech888.com.cn

Py:   a and b or not c
来源：http://hz.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://ph.9csxet.cn

JS:   a && b || !c
来源：http://fy.hahajie.cn

TS:   a && b || !c
来源：http://gj.bookmarksfly.cn

Java: a && b || !c
来源：http://ri.hahajie.cn

Go:   a && b || !c
来源：http://xh.gzmigu.cn

Ruby: a && b || !c
来源：http://ai.asd995.cn

C#:   a && b || !c
来源：http://ld.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ns.asd995.cn

Py:   if not data: return
来源：http://ds.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://yv.yuexingan06.cn

JS:   if (!data) return;
来源：http://kk.jctech888.com.cn

TS:   if (!data) return;
来源：http://sl.nszjky.cn

Java: if (data == null) return;
来源：http://iy.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://as.gzmigu.cn

Ruby: return if data.nil?
来源：http://me.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://yh.hnjuh.cn

================================================================================
来源：http://kp.panjiajie.cn

C. 函数与作用域
来源：http://cn.shxzskj.cn

================================================================================
来源：http://ft.colortex.cn

[C01] 定义函数
来源：http://zt.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://pl.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xf.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://sz.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vq.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lk.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xj.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://gp.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lz.shxzukj.cn

[C02] 默认参数
来源：http://fa.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://bc.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mt.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://zv.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yq.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fo.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yk.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://wo.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://xw.yuntaijiaju.cn

[C03] 可变参数
来源：http://ro.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://ki.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fl.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://li.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mq.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://il.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://al.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zk.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ut.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://qg.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uv.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tu.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mn.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oc.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://lx.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://sa.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://wv.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://po.shxzskj.cn

[C05] 返回多个值
来源：http://al.muxihuayi.cn

Py:   return a, b
来源：http://iu.colortex.cn

PHP:  return [$a, $b];
来源：http://wo.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tt.wgjwhj.cn

TS:   return { a, b };
来源：http://fm.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jk.huixiangedu.cn

Go:   return a, b
来源：http://zr.huixinmuqiang.cn

Ruby: return a, b
来源：http://zc.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://ch.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://vz.9csxet.cn

Py:   square = lambda x: x * x
来源：http://zy.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vd.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://ht.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://ar.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lr.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ol.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://dx.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pe.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://fn.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dv.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wz.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vz.szxytkj.cn

TS:   arr.map(String)
来源：http://fn.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yw.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sh.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://ng.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cj.asd995.cn

[C08] 闭包
来源：http://vv.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eh.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ka.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://si.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hh.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vr.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jd.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://og.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rp.bookmarksfly.cn

[C09] 递归
来源：http://yf.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vh.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ch.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xk.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://du.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jg.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zd.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ai.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gk.gzmigu.cn

[C10] 变量作用域
来源：http://nj.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lv.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://om.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zd.huanxung.cn

TS:   同 JS
来源：http://hg.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://wx.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://bt.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zw.nszjky.cn

C#:   块级作用域
来源：http://mo.lnxyls.cn

[C11] 模块导入与导出
来源：http://vq.yuntaijiaju.cn

Py:   from module import func
来源：http://du.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bb.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://az.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ym.hahajie.cn

Java: import java.util.List;
来源：http://zy.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fb.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://ep.newstarts.cn

C#:   using System.Text;
来源：http://xh.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://bc.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://zn.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://vh.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://dp.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://it.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ti.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ws.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://wo.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qz.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://dd.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hd.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lk.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://je.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zr.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gx.shxzskj.cn

Go:   func add(a, b int) int
来源：http://ti.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://np.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dv.panjiajie.cn

[C14] 泛型函数
来源：http://gh.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mm.huanxung.cn

PHP:  // 无泛型
来源：http://sq.huixinmuqiang.cn

JS:   // 无泛型
来源：http://ax.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hs.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wj.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tl.hahajie.cn

Ruby: # 无泛型
来源：http://kd.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jr.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://fw.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mc.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://wm.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ef.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mm.szsharing.cn

Java: // 无解构
来源：http://qu.shxzskj.cn

Go:   // 无解构
来源：http://hk.huixiangedu.cn

Ruby: a, b = pair
来源：http://ty.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://qv.colortex.cn

[C16] 函数 / 方法重载
来源：http://im.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lo.shtwfgs.cn

PHP:  // 无重载
来源：http://fo.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qd.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://gw.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kj.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://bq.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://fq.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sy.jctech888.com.cn

================================================================================
来源：http://nd.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://vp.9csxet.cn

================================================================================
来源：http://pc.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://be.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://og.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vo.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zm.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sy.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ll.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://wn.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://dd.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gk.asd995.cn

[D02] 追加元素到末尾
来源：http://mx.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ov.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ty.haigaiapp.cn

JS:   arr.push(4);
来源：http://du.chemitech.net.cn

TS:   arr.push(4);
来源：http://po.hnjuh.cn

Java: list.add(4);
来源：http://yj.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://op.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://qy.huixiangedu.cn

C#:   list.Add(4);
来源：http://yt.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://wr.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://fx.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ju.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yg.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://az.nicolike.cn

Java: list.add(0, 0);
来源：http://gs.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qp.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oc.lnxyls.cn


<!-- 参考信息 -->