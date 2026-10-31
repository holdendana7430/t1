代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pb.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://xr.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jy.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://md.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gq.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ug.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cg.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hd.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zw.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mk.nszjky.cn

[B03] switch / match / case
来源：http://em.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kv.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://id.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dy.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kl.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nv.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ed.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ds.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hb.chemitech.net.cn

[B04] for 计数循环
来源：http://se.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://ng.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jg.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://in.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tv.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qm.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hh.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://ga.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bp.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://sk.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://fl.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dh.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ir.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ma.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://so.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rf.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://mx.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lq.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://op.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wn.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qg.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dh.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ze.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ag.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ng.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gu.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://re.szxytkj.cn

[B07] while 循环
来源：http://gf.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://bs.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://em.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://xu.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://tx.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://oc.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vz.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://pq.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://er.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://fo.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://cm.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xp.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://uv.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://hm.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://sb.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bf.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hx.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://rt.asd995.cn

[B09] break 与 continue
来源：http://za.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://da.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://li.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oo.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mn.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gw.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zi.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pf.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eo.huanxung.cn

[B10] 遍历同时拿索引
来源：http://mw.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wz.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ez.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tq.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oy.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tp.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sh.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bv.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ev.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ib.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://hp.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://wz.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://os.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jg.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ac.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ja.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://ab.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mn.hnjuh.cn

[B12] 跳出多层循环
来源：http://hs.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mb.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zz.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://se.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kn.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qe.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ve.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://po.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zb.huanxung.cn

[B13] 判断是否为数字
来源：http://bn.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://gx.szxytkj.cn

PHP:  is_numeric($x)
来源：http://jq.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ip.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hf.huanxung.cn

Java: x instanceof Number
来源：http://gs.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gw.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://su.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://la.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://zh.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bx.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vr.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ki.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://lx.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xf.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ha.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zt.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ys.hnjuh.cn

[B15] 布尔运算与取反
来源：http://vh.yuexingan06.cn

Py:   a and b or not c
来源：http://ry.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://rd.shxzskj.cn

JS:   a && b || !c
来源：http://nx.hahajie.cn

TS:   a && b || !c
来源：http://ji.nicolike.cn

Java: a && b || !c
来源：http://ci.muxihuayi.cn

Go:   a && b || !c
来源：http://uf.huanxung.cn

Ruby: a && b || !c
来源：http://oe.yuexingan06.cn

C#:   a && b || !c
来源：http://ky.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ot.chemitech.net.cn

Py:   if not data: return
来源：http://fh.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://vs.shtwfgs.cn

JS:   if (!data) return;
来源：http://hc.bjjhwx.cn

TS:   if (!data) return;
来源：http://sk.shtwfgs.cn

Java: if (data == null) return;
来源：http://ok.newstarts.cn

Go:   if data == nil { return }
来源：http://xx.panjiajie.cn

Ruby: return if data.nil?
来源：http://cx.jctech888.com.cn

C#:   if (data == null) return;
来源：http://mm.gzmigu.cn

================================================================================
来源：http://th.nszjky.cn

C. 函数与作用域
来源：http://vq.muxihuayi.cn

================================================================================
来源：http://ro.nicolike.cn

[C01] 定义函数
来源：http://ow.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ks.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mk.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://kp.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ka.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hb.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fa.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://rx.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xw.bookmarksfly.cn

[C02] 默认参数
来源：http://sq.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://zb.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cy.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://pp.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wu.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ht.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tf.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://dr.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://bt.szxytkj.cn

[C03] 可变参数
来源：http://ib.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://dc.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fz.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qz.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ff.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bl.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tt.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ks.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xi.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://pq.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bd.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qq.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sa.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://da.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://de.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://lx.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://td.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://ud.haigaiapp.cn

[C05] 返回多个值
来源：http://ti.521024.cn

Py:   return a, b
来源：http://oj.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://hw.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bi.521024.cn

TS:   return { a, b };
来源：http://jj.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yi.bjjhwx.cn

Go:   return a, b
来源：http://gj.panjiajie.cn

Ruby: return a, b
来源：http://ov.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://kn.521024.cn

[C06] 匿名函数 / lambda
来源：http://ue.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://aw.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gt.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://wp.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://km.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yz.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gw.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://vs.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xw.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://bz.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ps.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://me.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wb.szxytkj.cn

TS:   arr.map(String)
来源：http://gx.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kw.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gz.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://ue.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://it.bookmarksfly.cn

[C08] 闭包
来源：http://aj.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cz.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ct.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://np.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://et.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rg.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hr.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ct.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fg.nicolike.cn

[C09] 递归
来源：http://hm.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oz.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://le.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fh.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xm.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cc.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gt.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://df.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bc.panjiajie.cn

[C10] 变量作用域
来源：http://qd.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wh.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bd.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tp.9csxet.cn

TS:   同 JS
来源：http://eh.hahajie.cn

Java: 方法内为块级作用域
来源：http://vy.9csxet.cn

Go:   花括号块级作用域
来源：http://mp.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zq.bookmarksfly.cn

C#:   块级作用域
来源：http://th.shtwfgs.cn

[C11] 模块导入与导出
来源：http://aw.9csxet.cn

Py:   from module import func
来源：http://sd.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gr.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dg.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hd.newstarts.cn

Java: import java.util.List;
来源：http://zf.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bv.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://qv.newstarts.cn

C#:   using System.Text;
来源：http://qs.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://xd.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://lu.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://tk.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://qz.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://qe.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mb.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://el.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://ei.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gs.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://vz.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://at.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cz.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rt.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qx.lnxyls.cn

Go:   func add(a, b int) int
来源：http://eu.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ow.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cb.asd995.cn

[C14] 泛型函数
来源：http://br.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zz.asd995.cn

PHP:  // 无泛型
来源：http://zv.yuexingan06.cn

JS:   // 无泛型
来源：http://pf.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://up.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lk.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yr.shxzukj.cn

Ruby: # 无泛型
来源：http://nc.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yw.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://kw.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zi.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://ns.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qx.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yc.huixinmuqiang.cn

Java: // 无解构
来源：http://ui.nicolike.cn

Go:   // 无解构
来源：http://uo.nszjky.cn

Ruby: a, b = pair
来源：http://kk.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://sp.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://qu.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sg.huixinmuqiang.cn

PHP:  // 无重载
来源：http://zr.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://en.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://cd.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qj.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://zd.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://eu.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bj.shtwfgs.cn

================================================================================
来源：http://kj.521024.cn

D. 数组 / 列表 / 集合
来源：http://co.huanxung.cn

================================================================================
来源：http://yi.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://wg.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dd.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wa.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uk.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mt.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ky.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://hg.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://au.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vj.newstarts.cn

[D02] 追加元素到末尾
来源：http://nm.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vr.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://it.wgjwhj.cn

JS:   arr.push(4);
来源：http://kl.shxzskj.cn

TS:   arr.push(4);
来源：http://rs.hahajie.cn


<!-- 参考信息 -->