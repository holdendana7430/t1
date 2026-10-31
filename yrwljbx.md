代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jg.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oa.colortex.cn

[B03] switch / match / case
来源：http://bk.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kc.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ih.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hf.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zu.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://og.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dm.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uv.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ro.lnxyls.cn

[B04] for 计数循环
来源：http://rf.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://ts.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tc.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gy.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://po.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ur.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xl.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://ne.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qw.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://gp.nszjky.cn

Py:   for item in arr: print(item)
来源：http://cq.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sz.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lg.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kr.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cy.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hu.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://jb.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wh.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://br.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nx.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xj.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gc.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ae.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jh.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wf.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gr.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sj.nicolike.cn

[B07] while 循环
来源：http://mu.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://cf.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rv.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://gi.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://ka.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://pq.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://du.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://jb.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://zb.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://uh.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://fb.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vb.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://gh.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://kf.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://ac.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nj.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dx.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://rl.shxzskj.cn

[B09] break 与 continue
来源：http://xx.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zu.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ei.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rd.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gj.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xl.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wf.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://km.szsharing.cn

[B10] 遍历同时拿索引
来源：http://wq.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xg.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fa.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pw.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ns.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xr.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qe.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lk.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://du.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://xb.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://uj.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://pk.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ec.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fx.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vi.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hf.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://nq.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wp.haigaiapp.cn

[B12] 跳出多层循环
来源：http://bj.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ai.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://po.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pm.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ov.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ui.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ft.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gf.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aa.szsharing.cn

[B13] 判断是否为数字
来源：http://tb.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://xo.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://vj.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pf.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ax.nicolike.cn

Java: x instanceof Number
来源：http://gt.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ma.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://nn.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://aj.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://lt.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rk.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hk.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://az.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://yp.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dd.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wu.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rg.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rr.nicolike.cn

[B15] 布尔运算与取反
来源：http://ym.panjiajie.cn

Py:   a and b or not c
来源：http://hv.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://bs.yuntaijiaju.cn

JS:   a && b || !c
来源：http://rq.huanxung.cn

TS:   a && b || !c
来源：http://tm.lnxyls.cn

Java: a && b || !c
来源：http://sm.nszjky.cn

Go:   a && b || !c
来源：http://dv.gzmigu.cn

Ruby: a && b || !c
来源：http://am.wgjwhj.cn

C#:   a && b || !c
来源：http://lt.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jp.yuntaijiaju.cn

Py:   if not data: return
来源：http://bj.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://vj.szsharing.cn

JS:   if (!data) return;
来源：http://ac.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://yp.huixiangedu.cn

Java: if (data == null) return;
来源：http://bz.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://xl.shxzskj.cn

Ruby: return if data.nil?
来源：http://tu.hnjuh.cn

C#:   if (data == null) return;
来源：http://ms.9csxet.cn

================================================================================
来源：http://kb.newstarts.cn

C. 函数与作用域
来源：http://zf.szxytkj.cn

================================================================================
来源：http://of.huixinmuqiang.cn

[C01] 定义函数
来源：http://uv.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://mq.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://di.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://jp.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nj.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ed.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mz.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ao.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bs.szsharing.cn

[C02] 默认参数
来源：http://gw.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://zs.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vg.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://wg.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qn.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ln.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xh.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://ir.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://ri.shxzskj.cn

[C03] 可变参数
来源：http://zp.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://pu.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cn.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mz.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hw.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wh.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eb.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tl.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pe.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://xj.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://co.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xx.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bu.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jj.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://wy.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://dv.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://gb.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://td.newstarts.cn

[C05] 返回多个值
来源：http://xi.jctech888.com.cn

Py:   return a, b
来源：http://yx.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://ed.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jc.jctech888.com.cn

TS:   return { a, b };
来源：http://cr.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gm.hnjuh.cn

Go:   return a, b
来源：http://ih.huanxung.cn

Ruby: return a, b
来源：http://sj.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://qa.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://cu.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://js.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rj.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://mp.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://da.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xw.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://aw.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://ug.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hc.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://mo.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dn.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vt.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uf.nicolike.cn

TS:   arr.map(String)
来源：http://fa.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iw.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ju.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://ov.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hd.muxihuayi.cn

[C08] 闭包
来源：http://xv.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ew.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zs.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hi.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://we.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gg.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ou.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yt.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ss.huanxung.cn

[C09] 递归
来源：http://et.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uj.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zy.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yi.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wx.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qg.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zm.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hm.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kp.wgjwhj.cn

[C10] 变量作用域
来源：http://jj.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bc.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qk.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bz.szsharing.cn

TS:   同 JS
来源：http://al.521024.cn

Java: 方法内为块级作用域
来源：http://yo.szxytkj.cn

Go:   花括号块级作用域
来源：http://zf.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wz.huixiangedu.cn

C#:   块级作用域
来源：http://kj.panjiajie.cn

[C11] 模块导入与导出
来源：http://ni.521024.cn

Py:   from module import func
来源：http://oo.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yg.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wu.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ga.newstarts.cn

Java: import java.util.List;
来源：http://ct.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ra.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://ew.colortex.cn

C#:   using System.Text;
来源：http://mu.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://mi.colortex.cn

Py:   (lambda: print("run"))()
来源：http://ne.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://qp.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://en.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://am.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://td.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://wl.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://di.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wd.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://xb.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hm.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jc.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yj.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ck.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zm.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://nx.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://od.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ph.nicolike.cn

[C14] 泛型函数
来源：http://xz.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qi.521024.cn

PHP:  // 无泛型
来源：http://pi.521024.cn

JS:   // 无泛型
来源：http://yf.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mw.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pp.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://to.521024.cn

Ruby: # 无泛型
来源：http://yu.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://we.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://oi.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://au.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://ny.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yz.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ba.szsharing.cn

Java: // 无解构
来源：http://ui.panjiajie.cn

Go:   // 无解构
来源：http://rw.9csxet.cn

Ruby: a, b = pair
来源：http://ko.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://ig.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://ix.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ah.huixiangedu.cn

PHP:  // 无重载
来源：http://hb.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kk.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://lk.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kz.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://az.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://sl.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mc.yuntaijiaju.cn

================================================================================
来源：http://xz.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://yi.bjjhwx.cn

================================================================================
来源：http://jj.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://zn.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yg.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://op.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xo.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rw.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sb.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://ne.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://jj.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nk.lnxyls.cn

[D02] 追加元素到末尾
来源：http://vv.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vk.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mv.szsharing.cn

JS:   arr.push(4);
来源：http://tw.gzmigu.cn

TS:   arr.push(4);
来源：http://ao.szxytkj.cn

Java: list.add(4);
来源：http://cg.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://go.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://zn.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://zi.9csxet.cn

[D03] 在指定位置插入元素
来源：http://he.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://nr.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fh.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tg.muxihuayi.cn


<!-- 参考信息 -->