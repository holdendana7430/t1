代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jl.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.newstarts.cn

[B03] switch / match / case
来源：http://be.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fi.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nz.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jz.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tv.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bq.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ri.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bf.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ev.huixiangedu.cn

[B04] for 计数循环
来源：http://rd.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://uz.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mw.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pm.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://av.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://is.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jq.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://sp.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ts.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://xm.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ib.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lb.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xm.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qc.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cz.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lz.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://cx.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sv.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://xg.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yd.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kr.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rw.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mf.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gl.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mb.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yl.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cn.wgjwhj.cn

[B07] while 循环
来源：http://vm.huanxung.cn

Py:   while i < 10: i += 1
来源：http://ja.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://er.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://ds.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://el.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://wz.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qn.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://yz.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://oo.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://gl.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://qu.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zn.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://mz.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://ya.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://sy.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nz.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wc.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://sf.jianghongdianzi.cn

[B09] break 与 continue
来源：http://ol.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sh.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ra.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wk.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fb.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cw.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rs.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://kb.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sb.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fd.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ma.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uv.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xv.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://el.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nv.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ys.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://oj.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://my.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://ys.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vo.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lh.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dw.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sm.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://dl.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ic.muxihuayi.cn

[B12] 跳出多层循环
来源：http://pv.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bb.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zq.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uc.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zx.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qd.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uf.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uy.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ii.asd995.cn

[B13] 判断是否为数字
来源：http://ev.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://ta.panjiajie.cn

PHP:  is_numeric($x)
来源：http://mr.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ld.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nl.bjjhwx.cn

Java: x instanceof Number
来源：http://su.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://au.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://gw.szxytkj.cn

C#:   x is int or double or decimal
来源：http://oc.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://uq.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wj.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fi.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://rw.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://oi.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ij.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dj.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iw.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://et.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://vs.szsharing.cn

Py:   a and b or not c
来源：http://jm.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://lj.szsharing.cn

JS:   a && b || !c
来源：http://ql.huixiangedu.cn

TS:   a && b || !c
来源：http://dx.szsharing.cn

Java: a && b || !c
来源：http://ll.haigaiapp.cn

Go:   a && b || !c
来源：http://ot.shxzukj.cn

Ruby: a && b || !c
来源：http://iq.hnjuh.cn

C#:   a && b || !c
来源：http://yv.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qu.chemitech.net.cn

Py:   if not data: return
来源：http://th.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://ci.huixiangedu.cn

JS:   if (!data) return;
来源：http://mw.9csxet.cn

TS:   if (!data) return;
来源：http://vp.szsharing.cn

Java: if (data == null) return;
来源：http://nb.lnxyls.cn

Go:   if data == nil { return }
来源：http://ud.huanxung.cn

Ruby: return if data.nil?
来源：http://zl.szxytkj.cn

C#:   if (data == null) return;
来源：http://li.newstarts.cn

================================================================================
来源：http://pk.shxzskj.cn

C. 函数与作用域
来源：http://cz.huixiangedu.cn

================================================================================
来源：http://if.huixinmuqiang.cn

[C01] 定义函数
来源：http://pw.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://kn.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://es.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://yr.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://re.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dg.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ur.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://yh.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uq.muxihuayi.cn

[C02] 默认参数
来源：http://qe.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://rb.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ly.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://fz.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mn.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bs.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qf.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://zf.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://sg.shxzskj.cn

[C03] 可变参数
来源：http://ww.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://uk.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bt.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kj.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yo.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oe.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hb.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ak.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nw.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://wi.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vx.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://di.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ni.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ux.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://ey.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://kj.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://qq.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://dm.hnjuh.cn

[C05] 返回多个值
来源：http://nt.lnxyls.cn

Py:   return a, b
来源：http://af.gzmigu.cn

PHP:  return [$a, $b];
来源：http://xx.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wu.nicolike.cn

TS:   return { a, b };
来源：http://fs.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zh.shtwfgs.cn

Go:   return a, b
来源：http://pm.wgjwhj.cn

Ruby: return a, b
来源：http://gb.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://eg.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://ce.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://zl.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ge.shxzskj.cn

JS:   const square = x => x * x;
来源：http://qt.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://wg.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rc.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ix.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://zd.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oy.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://js.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hl.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jm.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qe.szxytkj.cn

TS:   arr.map(String)
来源：http://bd.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://so.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://oy.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cg.asd995.cn

[C08] 闭包
来源：http://fj.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hq.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://si.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nf.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ci.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ak.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kp.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xl.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ox.521024.cn

[C09] 递归
来源：http://le.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://al.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xv.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ji.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kj.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nm.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cn.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pu.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xh.9csxet.cn

[C10] 变量作用域
来源：http://am.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xr.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ml.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vu.huixiangedu.cn

TS:   同 JS
来源：http://qp.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://mw.muxihuayi.cn

Go:   花括号块级作用域
来源：http://xl.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ut.huanxung.cn

C#:   块级作用域
来源：http://iw.nszjky.cn

[C11] 模块导入与导出
来源：http://lj.shtwfgs.cn

Py:   from module import func
来源：http://qp.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wn.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://df.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wl.jctech888.com.cn

Java: import java.util.List;
来源：http://go.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iq.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://co.shxzskj.cn

C#:   using System.Text;
来源：http://kj.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://tl.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://ed.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://ah.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://is.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ii.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sj.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://mb.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://gc.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ls.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://ry.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ka.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://el.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aw.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://la.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wy.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://ug.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wj.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kr.newstarts.cn

[C14] 泛型函数
来源：http://wf.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zn.hahajie.cn

PHP:  // 无泛型
来源：http://zi.panjiajie.cn

JS:   // 无泛型
来源：http://sg.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xw.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hc.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jk.newstarts.cn

Ruby: # 无泛型
来源：http://ta.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hf.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://eh.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://on.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://jk.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cp.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gs.huanxung.cn

Java: // 无解构
来源：http://je.hahajie.cn

Go:   // 无解构
来源：http://mi.bookmarksfly.cn

Ruby: a, b = pair
来源：http://kc.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://xf.521024.cn

[C16] 函数 / 方法重载
来源：http://ls.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yy.panjiajie.cn

PHP:  // 无重载
来源：http://gb.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lw.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://kk.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tc.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://tk.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://mg.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wb.haigaiapp.cn

================================================================================
来源：http://oi.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://tz.muxihuayi.cn

================================================================================
来源：http://oc.newstarts.cn

[D01] 创建数组 / 列表
来源：http://ha.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lm.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ly.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xr.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ba.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wk.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://cd.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://at.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dx.shxzukj.cn

[D02] 追加元素到末尾
来源：http://ef.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://am.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ad.bjjhwx.cn

JS:   arr.push(4);
来源：http://lv.chemitech.net.cn

TS:   arr.push(4);
来源：http://dk.nicolike.cn

Java: list.add(4);
来源：http://po.colortex.cn

Go:   arr = append(arr, 4)
来源：http://ln.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://uo.521024.cn

C#:   list.Add(4);
来源：http://pt.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://ww.521024.cn

Py:   arr.insert(0, 0)
来源：http://el.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fp.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sd.asd995.cn


<!-- 参考信息 -->