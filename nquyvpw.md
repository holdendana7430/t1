代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eq.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sx.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://em.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ha.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ym.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://av.newstarts.cn

[B03] switch / match / case
来源：http://kh.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ug.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wm.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kz.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ki.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zm.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jv.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zl.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ld.asd995.cn

[B04] for 计数循环
来源：http://pv.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://cg.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sr.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mw.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sw.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yo.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://la.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://dt.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bh.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://yo.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://qw.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lh.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ri.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fe.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zh.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ll.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://ws.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zj.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://hm.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qx.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jv.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://it.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zb.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ph.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kp.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ab.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yv.chemitech.net.cn

[B07] while 循环
来源：http://zn.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://gp.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qo.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://vo.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://ya.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://nn.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://do.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://nu.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://un.asd995.cn

[B08] do-while（至少执行一次）
来源：http://aj.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://cz.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ge.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://qs.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://fa.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://ks.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mq.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ku.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://wz.shtwfgs.cn

[B09] break 与 continue
来源：http://dq.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ad.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fu.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://br.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rk.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mm.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xf.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hs.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cx.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://wn.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rx.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pn.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uw.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dm.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vw.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kw.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aj.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sq.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://tq.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://gk.asd995.cn

PHP:  range(0, 10, 2);
来源：http://wd.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ff.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xw.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xd.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vv.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://cr.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rc.colortex.cn

[B12] 跳出多层循环
来源：http://pc.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yj.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jt.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://df.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xc.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wh.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://up.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ft.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://il.chemitech.net.cn

[B13] 判断是否为数字
来源：http://gc.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://kl.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://hc.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ly.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qh.chemitech.net.cn

Java: x instanceof Number
来源：http://bd.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rr.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://kh.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://wl.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://od.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://td.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nn.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://fw.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://lw.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lc.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rp.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ce.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pv.asd995.cn

[B15] 布尔运算与取反
来源：http://ej.yuexingan06.cn

Py:   a and b or not c
来源：http://pm.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://po.newstarts.cn

JS:   a && b || !c
来源：http://jb.huixinmuqiang.cn

TS:   a && b || !c
来源：http://so.nszjky.cn

Java: a && b || !c
来源：http://dg.nicolike.cn

Go:   a && b || !c
来源：http://st.newstarts.cn

Ruby: a && b || !c
来源：http://de.hnjuh.cn

C#:   a && b || !c
来源：http://tl.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ad.szsharing.cn

Py:   if not data: return
来源：http://cg.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://kp.hahajie.cn

JS:   if (!data) return;
来源：http://qq.shxzskj.cn

TS:   if (!data) return;
来源：http://df.shtwfgs.cn

Java: if (data == null) return;
来源：http://xb.shxzukj.cn

Go:   if data == nil { return }
来源：http://wv.shxzukj.cn

Ruby: return if data.nil?
来源：http://co.yuexingan06.cn

C#:   if (data == null) return;
来源：http://ht.chemitech.net.cn

================================================================================
来源：http://ud.szxytkj.cn

C. 函数与作用域
来源：http://xy.gzmigu.cn

================================================================================
来源：http://lu.nicolike.cn

[C01] 定义函数
来源：http://nb.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://jp.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mx.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://dg.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ty.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fi.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xr.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://kk.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xx.newstarts.cn

[C02] 默认参数
来源：http://dv.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://sp.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hq.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://em.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://co.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kt.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oh.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://vm.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://jw.wgjwhj.cn

[C03] 可变参数
来源：http://yh.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://uc.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vt.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gj.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yk.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bd.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ki.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://us.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dk.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://mq.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mg.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lk.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wl.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jz.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://gd.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://go.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://qo.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://gf.yuexingan06.cn

[C05] 返回多个值
来源：http://mw.yuexingan06.cn

Py:   return a, b
来源：http://wu.asd995.cn

PHP:  return [$a, $b];
来源：http://fg.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gs.huanxung.cn

TS:   return { a, b };
来源：http://qn.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dt.shxzskj.cn

Go:   return a, b
来源：http://xr.jctech888.com.cn

Ruby: return a, b
来源：http://hz.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://dr.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://tw.521024.cn

Py:   square = lambda x: x * x
来源：http://me.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vr.newstarts.cn

JS:   const square = x => x * x;
来源：http://zu.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://jr.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zk.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dx.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://tk.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ao.9csxet.cn

[C07] 把函数作为参数传入
来源：http://gw.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sj.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ga.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rs.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://yd.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://is.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dv.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://ef.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sc.yuexingan06.cn

[C08] 闭包
来源：http://fm.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fk.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gc.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mj.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://md.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://va.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bx.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uf.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jq.panjiajie.cn

[C09] 递归
来源：http://yy.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sv.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vw.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ul.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rv.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ns.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ho.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ie.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yo.shtwfgs.cn

[C10] 变量作用域
来源：http://bp.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cg.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yp.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lc.huixinmuqiang.cn

TS:   同 JS
来源：http://ke.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://dh.jctech888.com.cn

Go:   花括号块级作用域
来源：http://yl.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oh.shxzskj.cn

C#:   块级作用域
来源：http://xv.jctech888.com.cn

[C11] 模块导入与导出
来源：http://vc.nicolike.cn

Py:   from module import func
来源：http://av.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lp.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jl.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fq.huixinmuqiang.cn

Java: import java.util.List;
来源：http://ka.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://it.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://dl.newstarts.cn

C#:   using System.Text;
来源：http://eg.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://sr.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://qk.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://ms.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://to.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://fs.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qh.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://ya.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://ct.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://er.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://uj.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://am.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bm.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://no.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qt.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://by.nszjky.cn

Go:   func add(a, b int) int
来源：http://vu.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ut.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bc.shxzukj.cn

[C14] 泛型函数
来源：http://km.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xy.colortex.cn

PHP:  // 无泛型
来源：http://ht.muxihuayi.cn

JS:   // 无泛型
来源：http://wp.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mt.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://za.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ok.shxzskj.cn

Ruby: # 无泛型
来源：http://jj.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ju.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://xh.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zy.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://od.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hc.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ih.szxytkj.cn

Java: // 无解构
来源：http://iz.asd995.cn

Go:   // 无解构
来源：http://ks.hnjuh.cn

Ruby: a, b = pair
来源：http://au.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://vp.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://hk.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jg.newstarts.cn

PHP:  // 无重载
来源：http://lr.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rg.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://ia.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pe.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://td.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://ve.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ug.shtwfgs.cn

================================================================================
来源：http://hq.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://zj.shxzukj.cn

================================================================================
来源：http://zz.521024.cn

[D01] 创建数组 / 列表
来源：http://qi.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pa.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tw.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yr.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uy.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zl.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://ci.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://vd.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qu.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://ep.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xx.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rr.chemitech.net.cn

JS:   arr.push(4);
来源：http://cf.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://je.hnjuh.cn

Java: list.add(4);
来源：http://fz.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://wn.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://dy.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://hi.yuexingan06.cn


<!-- 参考信息 -->