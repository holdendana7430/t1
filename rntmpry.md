代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cz.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://cx.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ju.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rw.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xr.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mh.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lh.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ki.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xg.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cf.asd995.cn

[B03] switch / match / case
来源：http://us.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dv.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xs.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ux.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lv.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ma.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rs.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dy.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zp.muxihuayi.cn

[B04] for 计数循环
来源：http://nv.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://vq.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://da.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ch.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tb.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://va.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://td.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://tp.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yy.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://eu.huanxung.cn

Py:   for item in arr: print(item)
来源：http://ug.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://it.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ws.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cw.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ft.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://la.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://im.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ov.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://cc.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mn.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jx.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wj.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ab.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rz.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vu.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sx.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ho.nicolike.cn

[B07] while 循环
来源：http://ir.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://bl.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bh.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://cm.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://wa.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://hi.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yi.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://iy.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://ll.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ew.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://zb.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fi.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://mq.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://gx.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://in.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ws.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gm.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://fp.jianghongdianzi.cn

[B09] break 与 continue
来源：http://on.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bo.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kr.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ns.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qi.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ji.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://te.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ld.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mj.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://ie.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://js.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hf.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ni.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ft.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ip.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ly.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mp.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pe.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://ja.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://gn.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://ts.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fz.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ug.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nn.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sm.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://gx.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mv.huixiangedu.cn

[B12] 跳出多层循环
来源：http://od.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ct.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qr.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xv.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oc.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ub.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bo.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gc.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gf.newstarts.cn

[B13] 判断是否为数字
来源：http://mg.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://mj.lnxyls.cn

PHP:  is_numeric($x)
来源：http://rq.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sb.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ke.yuexingan06.cn

Java: x instanceof Number
来源：http://wy.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kx.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://mg.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://wu.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ul.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ih.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yl.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://lh.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://ch.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oa.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bt.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yl.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xl.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://mk.shxzskj.cn

Py:   a and b or not c
来源：http://ub.hahajie.cn

PHP:  $a && $b || !$c
来源：http://or.gzmigu.cn

JS:   a && b || !c
来源：http://wp.muxihuayi.cn

TS:   a && b || !c
来源：http://mg.nszjky.cn

Java: a && b || !c
来源：http://pa.521024.cn

Go:   a && b || !c
来源：http://jx.hahajie.cn

Ruby: a && b || !c
来源：http://dl.wgjwhj.cn

C#:   a && b || !c
来源：http://vo.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gj.yuexingan06.cn

Py:   if not data: return
来源：http://fu.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://uf.panjiajie.cn

JS:   if (!data) return;
来源：http://wx.muxihuayi.cn

TS:   if (!data) return;
来源：http://gp.9csxet.cn

Java: if (data == null) return;
来源：http://pk.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://bp.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://ci.colortex.cn

C#:   if (data == null) return;
来源：http://hq.asd995.cn

================================================================================
来源：http://gw.nszjky.cn

C. 函数与作用域
来源：http://nu.haigaiapp.cn

================================================================================
来源：http://bh.hnjuh.cn

[C01] 定义函数
来源：http://jg.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://ti.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eo.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://gr.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hj.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fr.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qs.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://tp.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cf.nicolike.cn

[C02] 默认参数
来源：http://cu.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://wc.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sn.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://wq.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jg.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dh.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kx.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://ik.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://ct.hahajie.cn

[C03] 可变参数
来源：http://cg.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://gn.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iy.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gp.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zm.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oz.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ni.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zr.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qg.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://ki.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uu.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ta.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ek.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ym.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://py.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://qw.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://sv.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://hh.jianghongdianzi.cn

[C05] 返回多个值
来源：http://hb.lnxyls.cn

Py:   return a, b
来源：http://rd.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://dt.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://at.bjjhwx.cn

TS:   return { a, b };
来源：http://lz.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://de.newstarts.cn

Go:   return a, b
来源：http://we.bookmarksfly.cn

Ruby: return a, b
来源：http://on.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://kk.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://cr.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://gt.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yt.asd995.cn

JS:   const square = x => x * x;
来源：http://fx.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://uj.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nr.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fs.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://jz.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ia.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://zu.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://re.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bq.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wf.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://fb.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kq.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dx.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://xw.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hd.shxzukj.cn

[C08] 闭包
来源：http://bq.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bv.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nb.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vt.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vn.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ha.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sa.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://is.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pf.huanxung.cn

[C09] 递归
来源：http://kn.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rm.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lb.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mc.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xm.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eb.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fd.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ri.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jn.jctech888.com.cn

[C10] 变量作用域
来源：http://yb.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bf.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iw.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sr.jctech888.com.cn

TS:   同 JS
来源：http://qj.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://lo.hahajie.cn

Go:   花括号块级作用域
来源：http://wo.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cq.szsharing.cn

C#:   块级作用域
来源：http://at.shxzskj.cn

[C11] 模块导入与导出
来源：http://gs.szsharing.cn

Py:   from module import func
来源：http://fn.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xx.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sh.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mq.yuexingan06.cn

Java: import java.util.List;
来源：http://un.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lo.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://uq.yuntaijiaju.cn

C#:   using System.Text;
来源：http://of.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://as.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://af.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://hg.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ka.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://qh.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jj.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://gd.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://rq.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cb.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://wu.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ig.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qx.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yw.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yf.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oy.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://oa.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nt.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jc.wgjwhj.cn

[C14] 泛型函数
来源：http://xy.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wm.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://xl.panjiajie.cn

JS:   // 无泛型
来源：http://on.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kz.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hf.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nb.szxytkj.cn

Ruby: # 无泛型
来源：http://av.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zx.szsharing.cn

[C15] 解构 / 展开参数
来源：http://yb.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ui.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://kv.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lc.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nz.9csxet.cn

Java: // 无解构
来源：http://xw.bjjhwx.cn

Go:   // 无解构
来源：http://sq.newstarts.cn

Ruby: a, b = pair
来源：http://qs.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://nh.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://rz.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ep.szsharing.cn

PHP:  // 无重载
来源：http://mj.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://os.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://eh.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wl.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://mr.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://gz.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pk.gzmigu.cn

================================================================================
来源：http://xt.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://lb.nicolike.cn

================================================================================
来源：http://sc.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://zn.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://em.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://po.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ls.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kz.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ay.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://go.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://aj.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zz.521024.cn

[D02] 追加元素到末尾
来源：http://mm.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ij.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jo.nszjky.cn

JS:   arr.push(4);
来源：http://kx.521024.cn

TS:   arr.push(4);
来源：http://tl.jctech888.com.cn


<!-- 参考信息 -->