代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xk.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://rr.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vk.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tc.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://re.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fg.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fb.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ez.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xi.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gx.panjiajie.cn

[B03] switch / match / case
来源：http://mh.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fj.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vg.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ja.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zm.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nn.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eu.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ib.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bk.haigaiapp.cn

[B04] for 计数循环
来源：http://dv.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://qs.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://so.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hq.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bz.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oc.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://th.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://nj.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rt.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://fp.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://ev.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fn.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zn.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vo.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dr.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cw.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://kr.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uz.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://on.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xl.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ho.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ea.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cr.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fb.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ch.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ti.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ap.panjiajie.cn

[B07] while 循环
来源：http://vx.nszjky.cn

Py:   while i < 10: i += 1
来源：http://tx.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tu.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://tx.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://am.asd995.cn

Java: while (i < 10) { i++; }
来源：http://gp.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://og.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://gr.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://hz.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://qz.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://he.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jq.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://zd.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://pj.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://ha.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ff.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cx.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://em.huixinmuqiang.cn

[B09] break 与 continue
来源：http://ws.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ej.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pv.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yv.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bt.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dx.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hl.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://le.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://bm.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bk.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xp.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wm.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yh.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ov.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hc.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://za.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rw.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://tu.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://nm.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://vr.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://it.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ly.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xc.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wf.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://mw.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zo.nszjky.cn

[B12] 跳出多层循环
来源：http://eh.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://da.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rh.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jr.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tx.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ux.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oo.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oq.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zg.asd995.cn

[B13] 判断是否为数字
来源：http://oo.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://lp.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://yd.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gy.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vm.bookmarksfly.cn

Java: x instanceof Number
来源：http://ih.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qr.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://cx.shxzskj.cn

C#:   x is int or double or decimal
来源：http://oh.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://lx.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://di.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rt.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://px.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://yv.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lv.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eg.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jj.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nh.521024.cn

[B15] 布尔运算与取反
来源：http://gx.chemitech.net.cn

Py:   a and b or not c
来源：http://rx.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://fu.hahajie.cn

JS:   a && b || !c
来源：http://er.szsharing.cn

TS:   a && b || !c
来源：http://gw.bookmarksfly.cn

Java: a && b || !c
来源：http://vh.jianghongdianzi.cn

Go:   a && b || !c
来源：http://mt.szxytkj.cn

Ruby: a && b || !c
来源：http://ax.hnjuh.cn

C#:   a && b || !c
来源：http://ec.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zo.hahajie.cn

Py:   if not data: return
来源：http://rb.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://qr.chemitech.net.cn

JS:   if (!data) return;
来源：http://gz.asd995.cn

TS:   if (!data) return;
来源：http://xw.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://wt.jctech888.com.cn

Go:   if data == nil { return }
来源：http://ax.jctech888.com.cn

Ruby: return if data.nil?
来源：http://xr.gzmigu.cn

C#:   if (data == null) return;
来源：http://pw.szsharing.cn

================================================================================
来源：http://yj.yuexingan06.cn

C. 函数与作用域
来源：http://fr.asd995.cn

================================================================================
来源：http://ui.9csxet.cn

[C01] 定义函数
来源：http://hv.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://hp.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bo.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://vh.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dx.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dx.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ut.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://fw.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hc.wgjwhj.cn

[C02] 默认参数
来源：http://fl.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://ge.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mb.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ie.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ya.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ji.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xf.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://no.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://qb.haigaiapp.cn

[C03] 可变参数
来源：http://tz.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://zr.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xx.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tq.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ts.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xx.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yf.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yp.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iw.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://ab.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xk.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kk.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ah.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://up.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://fa.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://ya.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://fn.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://oi.nszjky.cn

[C05] 返回多个值
来源：http://ef.bookmarksfly.cn

Py:   return a, b
来源：http://mw.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://bd.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://up.9csxet.cn

TS:   return { a, b };
来源：http://ik.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wn.bookmarksfly.cn

Go:   return a, b
来源：http://ri.huixinmuqiang.cn

Ruby: return a, b
来源：http://wt.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://wq.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://zx.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://gb.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ed.nszjky.cn

JS:   const square = x => x * x;
来源：http://mu.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://nj.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xe.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hr.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://ob.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zy.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://rl.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rd.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ye.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iv.hahajie.cn

TS:   arr.map(String)
来源：http://uj.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://be.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ls.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://qs.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lu.chemitech.net.cn

[C08] 闭包
来源：http://dv.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gb.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nx.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uj.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kh.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sd.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xk.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wf.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xt.haigaiapp.cn

[C09] 递归
来源：http://dr.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yt.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://si.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ah.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tt.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://br.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yi.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wz.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://be.jianghongdianzi.cn

[C10] 变量作用域
来源：http://gp.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rt.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ld.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fn.nicolike.cn

TS:   同 JS
来源：http://af.shxzukj.cn

Java: 方法内为块级作用域
来源：http://wr.521024.cn

Go:   花括号块级作用域
来源：http://el.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mr.bjjhwx.cn

C#:   块级作用域
来源：http://vo.asd995.cn

[C11] 模块导入与导出
来源：http://uc.shtwfgs.cn

Py:   from module import func
来源：http://cn.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rd.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cx.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://km.gzmigu.cn

Java: import java.util.List;
来源：http://og.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ih.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://hq.szsharing.cn

C#:   using System.Text;
来源：http://mr.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://my.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://rc.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://cc.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://kt.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://wp.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fl.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://bm.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://hk.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gr.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://jr.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mt.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ri.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nw.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://un.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ud.shxzukj.cn

Go:   func add(a, b int) int
来源：http://wd.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kb.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ff.jctech888.com.cn

[C14] 泛型函数
来源：http://tu.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bm.wgjwhj.cn

PHP:  // 无泛型
来源：http://hd.huanxung.cn

JS:   // 无泛型
来源：http://zl.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pw.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://um.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aw.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://qm.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://da.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://zy.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ra.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://zs.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pl.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iw.wgjwhj.cn

Java: // 无解构
来源：http://or.yuexingan06.cn

Go:   // 无解构
来源：http://in.9csxet.cn

Ruby: a, b = pair
来源：http://xw.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://ci.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://qv.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rm.huanxung.cn

PHP:  // 无重载
来源：http://at.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://to.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://on.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ni.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://ns.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://aw.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://et.wgjwhj.cn

================================================================================
来源：http://ve.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://mj.huanxung.cn

================================================================================
来源：http://gk.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://ll.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://op.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ku.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lr.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jm.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dz.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://pn.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://to.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ln.asd995.cn

[D02] 追加元素到末尾
来源：http://xk.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://da.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ri.521024.cn

JS:   arr.push(4);
来源：http://di.hnjuh.cn

TS:   arr.push(4);
来源：http://fw.szxytkj.cn


<!-- 参考信息 -->