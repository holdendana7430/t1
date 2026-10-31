代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yf.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dd.gzmigu.cn

[B03] switch / match / case
来源：http://sd.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eu.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rt.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eq.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fb.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lp.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lw.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gv.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qk.gzmigu.cn

[B04] for 计数循环
来源：http://xx.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://kf.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rk.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ei.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uq.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bq.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gn.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://si.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ge.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://gm.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://ys.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lw.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qm.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bf.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vg.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nh.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://vo.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mo.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://va.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bk.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ws.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rm.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://da.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gr.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://go.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gf.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ss.yuexingan06.cn

[B07] while 循环
来源：http://kd.asd995.cn

Py:   while i < 10: i += 1
来源：http://mu.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ne.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://vl.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://er.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://gw.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fi.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://md.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://zl.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://wl.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://ua.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jg.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://fy.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://uw.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://ub.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sj.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lq.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://ro.muxihuayi.cn

[B09] break 与 continue
来源：http://hs.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pw.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gj.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vz.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dr.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ui.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sd.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pr.newstarts.cn

[B10] 遍历同时拿索引
来源：http://wf.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pf.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://je.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://um.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tb.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://po.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vx.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yx.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uc.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://ku.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://zl.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://ll.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xg.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ax.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ii.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://os.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://hg.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lk.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://iq.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zk.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ba.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lg.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://no.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yw.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vs.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pu.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mh.lnxyls.cn

[B13] 判断是否为数字
来源：http://sz.521024.cn

Py:   isinstance(x, (int, float))
来源：http://hy.newstarts.cn

PHP:  is_numeric($x)
来源：http://lq.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wq.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hx.szxytkj.cn

Java: x instanceof Number
来源：http://sr.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hy.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://ka.521024.cn

C#:   x is int or double or decimal
来源：http://vs.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://ww.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vb.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dx.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://bi.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://zt.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jr.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rg.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vx.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eu.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://er.szxytkj.cn

Py:   a and b or not c
来源：http://rf.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://gv.wgjwhj.cn

JS:   a && b || !c
来源：http://wq.shtwfgs.cn

TS:   a && b || !c
来源：http://ly.szsharing.cn

Java: a && b || !c
来源：http://lm.bjjhwx.cn

Go:   a && b || !c
来源：http://sk.jctech888.com.cn

Ruby: a && b || !c
来源：http://xr.bookmarksfly.cn

C#:   a && b || !c
来源：http://yl.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dt.yuntaijiaju.cn

Py:   if not data: return
来源：http://mf.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://zg.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://kb.asd995.cn

TS:   if (!data) return;
来源：http://py.521024.cn

Java: if (data == null) return;
来源：http://qg.yuexingan06.cn

Go:   if data == nil { return }
来源：http://jv.jctech888.com.cn

Ruby: return if data.nil?
来源：http://ni.szxytkj.cn

C#:   if (data == null) return;
来源：http://ht.muxihuayi.cn

================================================================================
来源：http://ge.newstarts.cn

C. 函数与作用域
来源：http://ux.newstarts.cn

================================================================================
来源：http://sr.huixinmuqiang.cn

[C01] 定义函数
来源：http://my.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://js.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wy.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://om.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://en.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mj.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ue.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://lr.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ww.szxytkj.cn

[C02] 默认参数
来源：http://mw.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://wc.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vh.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://zl.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ly.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://os.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ta.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://ih.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://xq.hahajie.cn

[C03] 可变参数
来源：http://ze.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://vv.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bc.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xq.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cf.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ey.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ci.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uq.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jh.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://dr.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xk.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fq.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://py.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sv.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://mt.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://sz.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://vv.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://jm.yuexingan06.cn

[C05] 返回多个值
来源：http://jy.szxytkj.cn

Py:   return a, b
来源：http://vg.gzmigu.cn

PHP:  return [$a, $b];
来源：http://kw.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sf.shxzukj.cn

TS:   return { a, b };
来源：http://dv.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pb.521024.cn

Go:   return a, b
来源：http://gv.nicolike.cn

Ruby: return a, b
来源：http://jc.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://op.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://eb.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://ag.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sw.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://ph.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://kf.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://od.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yu.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://ci.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hn.asd995.cn

[C07] 把函数作为参数传入
来源：http://xi.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pe.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nj.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sj.newstarts.cn

TS:   arr.map(String)
来源：http://ke.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wh.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ok.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://es.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fn.wgjwhj.cn

[C08] 闭包
来源：http://qa.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qu.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ow.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yq.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://di.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uo.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sn.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://og.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eh.chemitech.net.cn

[C09] 递归
来源：http://xn.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lv.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ec.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kx.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ha.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jb.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vr.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xg.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://or.hahajie.cn

[C10] 变量作用域
来源：http://qe.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yy.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bh.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tv.9csxet.cn

TS:   同 JS
来源：http://xb.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://xb.chemitech.net.cn

Go:   花括号块级作用域
来源：http://fq.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fs.yuntaijiaju.cn

C#:   块级作用域
来源：http://yn.hahajie.cn

[C11] 模块导入与导出
来源：http://ws.szxytkj.cn

Py:   from module import func
来源：http://ma.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qr.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hy.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://an.nicolike.cn

Java: import java.util.List;
来源：http://by.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lx.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://hx.shxzukj.cn

C#:   using System.Text;
来源：http://cc.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://uj.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://tt.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://qr.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://kz.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://wp.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ae.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://ic.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://ax.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hu.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://tp.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lj.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wd.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gz.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pe.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yc.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://vr.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jm.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://so.hnjuh.cn

[C14] 泛型函数
来源：http://yh.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uz.9csxet.cn

PHP:  // 无泛型
来源：http://ff.szxytkj.cn

JS:   // 无泛型
来源：http://ii.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yh.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lh.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xz.panjiajie.cn

Ruby: # 无泛型
来源：http://dt.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gm.colortex.cn

[C15] 解构 / 展开参数
来源：http://sk.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tf.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://uf.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vq.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sp.chemitech.net.cn

Java: // 无解构
来源：http://xr.huixinmuqiang.cn

Go:   // 无解构
来源：http://dp.huanxung.cn

Ruby: a, b = pair
来源：http://cy.huanxung.cn

C#:   var (a, b) = pair;
来源：http://ql.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://ef.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qm.huixinmuqiang.cn

PHP:  // 无重载
来源：http://vk.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kw.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://kd.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kb.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://jl.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://kt.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dm.muxihuayi.cn

================================================================================
来源：http://lq.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://wm.hahajie.cn

================================================================================
来源：http://ad.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://ht.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wn.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fx.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pm.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://si.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gx.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://wu.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://aw.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yc.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://ek.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sm.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ma.nicolike.cn

JS:   arr.push(4);
来源：http://mp.colortex.cn

TS:   arr.push(4);
来源：http://ke.shxzukj.cn

Java: list.add(4);
来源：http://ov.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://az.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://he.bookmarksfly.cn

C#:   list.Add(4);
来源：http://bj.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://ke.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://cp.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kn.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ew.muxihuayi.cn


<!-- 参考信息 -->