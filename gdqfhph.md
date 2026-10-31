代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://la.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ff.jianghongdianzi.cn

[B03] switch / match / case
来源：http://iv.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mf.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nd.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dr.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xh.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ok.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jj.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xk.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qv.jctech888.com.cn

[B04] for 计数循环
来源：http://se.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://zv.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jy.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ke.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sl.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ic.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lb.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://zs.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fy.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://dy.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://zw.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yr.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hc.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rs.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://au.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cd.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://hg.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pj.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://ms.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vs.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ta.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qk.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ix.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jy.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ev.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yx.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ik.shxzskj.cn

[B07] while 循环
来源：http://cn.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://yj.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ap.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://zx.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://kk.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://aa.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gf.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://mu.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://ja.521024.cn

[B08] do-while（至少执行一次）
来源：http://gl.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://wz.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wc.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://ca.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://dh.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://hm.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gm.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bq.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://ih.newstarts.cn

[B09] break 与 continue
来源：http://jb.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://op.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ge.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jr.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qn.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vb.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sk.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zh.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://li.nicolike.cn

[B10] 遍历同时拿索引
来源：http://xs.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ip.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mw.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wz.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gr.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ii.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mq.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://es.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ma.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://gy.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://br.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://ps.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bi.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yc.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ks.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jv.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://wj.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oc.muxihuayi.cn

[B12] 跳出多层循环
来源：http://nx.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vj.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vg.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://te.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ry.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ho.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ru.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dz.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xl.colortex.cn

[B13] 判断是否为数字
来源：http://om.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://tg.shxzskj.cn

PHP:  is_numeric($x)
来源：http://cb.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ei.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eh.hahajie.cn

Java: x instanceof Number
来源：http://db.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hg.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://ie.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://qd.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://wj.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lr.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://la.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://cf.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://be.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nb.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kx.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zs.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dr.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://sv.chemitech.net.cn

Py:   a and b or not c
来源：http://vd.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://un.wgjwhj.cn

JS:   a && b || !c
来源：http://tm.bjjhwx.cn

TS:   a && b || !c
来源：http://jd.szxytkj.cn

Java: a && b || !c
来源：http://dg.newstarts.cn

Go:   a && b || !c
来源：http://ed.huanxung.cn

Ruby: a && b || !c
来源：http://qb.lnxyls.cn

C#:   a && b || !c
来源：http://bl.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lr.gzmigu.cn

Py:   if not data: return
来源：http://ql.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://zk.shxzskj.cn

JS:   if (!data) return;
来源：http://tl.bjjhwx.cn

TS:   if (!data) return;
来源：http://iq.muxihuayi.cn

Java: if (data == null) return;
来源：http://sj.521024.cn

Go:   if data == nil { return }
来源：http://si.szsharing.cn

Ruby: return if data.nil?
来源：http://yd.jctech888.com.cn

C#:   if (data == null) return;
来源：http://yw.szxytkj.cn

================================================================================
来源：http://cr.haigaiapp.cn

C. 函数与作用域
来源：http://qs.yuexingan06.cn

================================================================================
来源：http://ef.szsharing.cn

[C01] 定义函数
来源：http://py.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://xn.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ut.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://es.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bl.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://py.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dr.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://rs.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rm.huanxung.cn

[C02] 默认参数
来源：http://go.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://rc.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bc.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qh.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jr.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hl.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hx.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://ci.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://ju.gzmigu.cn

[C03] 可变参数
来源：http://vd.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://sx.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ah.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oq.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gw.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ai.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tl.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bm.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ac.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://fh.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nk.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ec.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qq.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jp.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://gt.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://lj.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://ds.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://bc.panjiajie.cn

[C05] 返回多个值
来源：http://mq.lnxyls.cn

Py:   return a, b
来源：http://ws.nszjky.cn

PHP:  return [$a, $b];
来源：http://oh.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uy.nszjky.cn

TS:   return { a, b };
来源：http://or.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uu.szxytkj.cn

Go:   return a, b
来源：http://ly.newstarts.cn

Ruby: return a, b
来源：http://qk.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://tv.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://ac.huanxung.cn

Py:   square = lambda x: x * x
来源：http://nw.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://db.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://fh.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://kx.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ca.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://as.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://ru.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fd.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://ba.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xt.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fd.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vo.szsharing.cn

TS:   arr.map(String)
来源：http://ih.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xm.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xt.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://is.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://et.shtwfgs.cn

[C08] 闭包
来源：http://od.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zl.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ks.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://va.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tm.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hw.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bd.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kc.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://je.gzmigu.cn

[C09] 递归
来源：http://tk.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ub.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ud.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eg.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pq.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sk.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ks.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sx.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vj.hnjuh.cn

[C10] 变量作用域
来源：http://ph.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hy.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wh.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pz.shtwfgs.cn

TS:   同 JS
来源：http://rs.shxzskj.cn

Java: 方法内为块级作用域
来源：http://kz.gzmigu.cn

Go:   花括号块级作用域
来源：http://yq.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ee.jctech888.com.cn

C#:   块级作用域
来源：http://iq.bjjhwx.cn

[C11] 模块导入与导出
来源：http://uz.hahajie.cn

Py:   from module import func
来源：http://vl.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gq.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zl.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://er.hnjuh.cn

Java: import java.util.List;
来源：http://us.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cp.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://cs.gzmigu.cn

C#:   using System.Text;
来源：http://sx.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://ak.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://in.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://ha.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://gr.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://mw.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kz.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://fy.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://dj.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mx.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://nt.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fx.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zn.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pv.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zb.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qo.lnxyls.cn

Go:   func add(a, b int) int
来源：http://rs.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xb.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://go.yuntaijiaju.cn

[C14] 泛型函数
来源：http://tp.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ec.yuexingan06.cn

PHP:  // 无泛型
来源：http://qp.huixinmuqiang.cn

JS:   // 无泛型
来源：http://sm.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vx.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uh.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sx.bjjhwx.cn

Ruby: # 无泛型
来源：http://xy.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://he.asd995.cn

[C15] 解构 / 展开参数
来源：http://jr.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qh.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://by.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wr.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sz.gzmigu.cn

Java: // 无解构
来源：http://az.hahajie.cn

Go:   // 无解构
来源：http://xj.shxzukj.cn

Ruby: a, b = pair
来源：http://zh.9csxet.cn

C#:   var (a, b) = pair;
来源：http://vz.9csxet.cn

[C16] 函数 / 方法重载
来源：http://ml.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cv.haigaiapp.cn

PHP:  // 无重载
来源：http://sl.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cw.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://ea.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oy.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://ou.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://nc.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ah.shtwfgs.cn

================================================================================
来源：http://mv.521024.cn

D. 数组 / 列表 / 集合
来源：http://eh.bjjhwx.cn

================================================================================
来源：http://ec.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://mr.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mt.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hd.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://if.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iy.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tx.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://gb.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://xu.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ag.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://ge.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oi.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sc.nszjky.cn

JS:   arr.push(4);
来源：http://hb.9csxet.cn

TS:   arr.push(4);
来源：http://ob.yuntaijiaju.cn

Java: list.add(4);
来源：http://ut.asd995.cn

Go:   arr = append(arr, 4)
来源：http://gp.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://le.hnjuh.cn

C#:   list.Add(4);
来源：http://uk.521024.cn

[D03] 在指定位置插入元素
来源：http://ko.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://pm.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ps.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jl.shtwfgs.cn


<!-- 参考信息 -->