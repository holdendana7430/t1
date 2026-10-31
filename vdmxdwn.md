代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qo.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fe.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gl.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yf.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.colortex.cn

[B03] switch / match / case
来源：http://tn.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ch.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://po.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ux.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wo.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://br.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uk.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qs.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yu.yuntaijiaju.cn

[B04] for 计数循环
来源：http://yf.colortex.cn

Py:   for i in range(10): print(i)
来源：http://sa.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bk.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qg.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bm.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iq.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ty.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://hh.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tm.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://ot.huanxung.cn

Py:   for item in arr: print(item)
来源：http://zz.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iz.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bx.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hq.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ig.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qg.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://qe.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://he.521024.cn

[B06] 遍历字典 / 对象
来源：http://ov.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dg.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tk.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uj.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qa.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fi.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xm.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vw.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vt.hahajie.cn

[B07] while 循环
来源：http://bj.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://fn.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zx.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://yq.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://nr.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://ed.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gy.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://bt.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://bp.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://fi.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://cp.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gn.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ec.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://da.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://fh.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ap.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lu.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://uu.hahajie.cn

[B09] break 与 continue
来源：http://tn.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pj.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jy.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vl.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ag.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wg.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jc.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cg.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ry.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://mc.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yi.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ed.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hh.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gs.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jr.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ni.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ay.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ro.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://xr.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://nr.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://ry.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wq.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://up.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://up.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ka.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://gw.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bd.panjiajie.cn

[B12] 跳出多层循环
来源：http://ts.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uq.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://aw.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nd.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ub.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nx.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jy.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ch.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gn.huixiangedu.cn

[B13] 判断是否为数字
来源：http://pl.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://ip.521024.cn

PHP:  is_numeric($x)
来源：http://ov.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nq.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cd.huixinmuqiang.cn

Java: x instanceof Number
来源：http://ez.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hv.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://hp.gzmigu.cn

C#:   x is int or double or decimal
来源：http://ld.szsharing.cn

[B14] 判断值是否在集合内
来源：http://zr.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zj.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rd.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://gt.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://oh.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://az.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mj.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yh.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xk.szxytkj.cn

[B15] 布尔运算与取反
来源：http://ae.yuexingan06.cn

Py:   a and b or not c
来源：http://hx.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://lt.yuexingan06.cn

JS:   a && b || !c
来源：http://rh.panjiajie.cn

TS:   a && b || !c
来源：http://zi.hnjuh.cn

Java: a && b || !c
来源：http://cx.newstarts.cn

Go:   a && b || !c
来源：http://qo.shtwfgs.cn

Ruby: a && b || !c
来源：http://je.gzmigu.cn

C#:   a && b || !c
来源：http://mf.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rz.jctech888.com.cn

Py:   if not data: return
来源：http://yb.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://qq.chemitech.net.cn

JS:   if (!data) return;
来源：http://sd.muxihuayi.cn

TS:   if (!data) return;
来源：http://be.yuexingan06.cn

Java: if (data == null) return;
来源：http://ir.haigaiapp.cn

Go:   if data == nil { return }
来源：http://lj.szsharing.cn

Ruby: return if data.nil?
来源：http://nx.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://tc.wgjwhj.cn

================================================================================
来源：http://bt.szsharing.cn

C. 函数与作用域
来源：http://do.huixinmuqiang.cn

================================================================================
来源：http://pe.9csxet.cn

[C01] 定义函数
来源：http://ea.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://ho.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zu.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://wt.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rd.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jn.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lv.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://jw.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tj.muxihuayi.cn

[C02] 默认参数
来源：http://ly.colortex.cn

Py:   def greet(name="World"): return name
来源：http://ye.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://km.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://ug.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://at.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kt.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pw.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://vo.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://dp.jianghongdianzi.cn

[C03] 可变参数
来源：http://kn.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://af.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vk.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rh.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qs.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qr.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fv.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ar.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qv.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://ka.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aw.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tx.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kv.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://si.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ko.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://ds.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://cc.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://jq.haigaiapp.cn

[C05] 返回多个值
来源：http://we.521024.cn

Py:   return a, b
来源：http://jb.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://tr.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ng.jianghongdianzi.cn

TS:   return { a, b };
来源：http://cs.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://af.nicolike.cn

Go:   return a, b
来源：http://wl.szxytkj.cn

Ruby: return a, b
来源：http://ws.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://os.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://oj.9csxet.cn

Py:   square = lambda x: x * x
来源：http://zf.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qw.huanxung.cn

JS:   const square = x => x * x;
来源：http://yq.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://am.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xc.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jc.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://hj.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tg.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://kk.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lw.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wo.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vw.haigaiapp.cn

TS:   arr.map(String)
来源：http://nt.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ks.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://py.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://qr.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fj.hnjuh.cn

[C08] 闭包
来源：http://nl.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tm.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jr.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ry.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ga.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ph.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://do.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tt.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gw.shxzskj.cn

[C09] 递归
来源：http://lo.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yd.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uy.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ip.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dz.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pm.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ii.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wz.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hr.huixinmuqiang.cn

[C10] 变量作用域
来源：http://sg.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://os.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://st.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ta.hnjuh.cn

TS:   同 JS
来源：http://bq.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://fm.nszjky.cn

Go:   花括号块级作用域
来源：http://vk.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hu.jianghongdianzi.cn

C#:   块级作用域
来源：http://kw.yuexingan06.cn

[C11] 模块导入与导出
来源：http://bu.shxzskj.cn

Py:   from module import func
来源：http://wd.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zu.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jv.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mx.asd995.cn

Java: import java.util.List;
来源：http://bs.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ly.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ck.yuntaijiaju.cn

C#:   using System.Text;
来源：http://ks.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://kn.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://ge.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://yn.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://nw.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://ox.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dw.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://op.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://mm.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dz.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://ba.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gq.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cp.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fs.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qt.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://du.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://ih.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ag.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xa.yuntaijiaju.cn

[C14] 泛型函数
来源：http://uu.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wt.huixiangedu.cn

PHP:  // 无泛型
来源：http://hq.huanxung.cn

JS:   // 无泛型
来源：http://no.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qr.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yb.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fq.jctech888.com.cn

Ruby: # 无泛型
来源：http://se.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yw.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://hc.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ui.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://ur.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gy.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tz.jianghongdianzi.cn

Java: // 无解构
来源：http://ub.nszjky.cn

Go:   // 无解构
来源：http://tm.bjjhwx.cn

Ruby: a, b = pair
来源：http://ts.hahajie.cn

C#:   var (a, b) = pair;
来源：http://uf.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://wk.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hd.panjiajie.cn

PHP:  // 无重载
来源：http://ct.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ca.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://qs.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xr.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://ry.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://oc.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uk.jianghongdianzi.cn

================================================================================
来源：http://cq.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://to.haigaiapp.cn

================================================================================
来源：http://tu.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://nc.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rt.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zs.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ak.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qs.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eb.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://of.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://sn.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fy.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://mj.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zr.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hl.9csxet.cn

JS:   arr.push(4);
来源：http://li.szsharing.cn

TS:   arr.push(4);
来源：http://rs.gzmigu.cn

Java: list.add(4);
来源：http://pz.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://ci.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://mv.lnxyls.cn

C#:   list.Add(4);
来源：http://ni.colortex.cn


<!-- 参考信息 -->