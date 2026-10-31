代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mh.nszjky.cn

[B02] 多分支 else if / elif
来源：http://zm.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yi.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://at.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jf.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zo.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mb.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fa.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iy.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rr.muxihuayi.cn

[B03] switch / match / case
来源：http://as.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xh.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vi.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tp.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wp.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://be.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vl.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xx.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rq.szxytkj.cn

[B04] for 计数循环
来源：http://dw.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://ns.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yt.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ca.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dr.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sy.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kg.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://tk.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fu.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://kc.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://eg.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kg.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vm.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ql.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wn.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ap.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://yr.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sk.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://ad.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://os.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://th.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nw.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kj.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ma.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ac.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nf.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jv.shxzskj.cn

[B07] while 循环
来源：http://fm.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://lk.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ml.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://tr.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://sl.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://po.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vp.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://nn.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://nd.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://zc.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://xd.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fw.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://ca.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://la.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://bl.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zt.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://or.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://in.9csxet.cn

[B09] break 与 continue
来源：http://qf.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wb.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wd.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kq.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yl.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qc.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ui.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kw.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tp.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://yd.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://li.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vg.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://me.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nj.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://be.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xs.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://re.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yq.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://af.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://hq.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://ce.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qv.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qd.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uh.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ug.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://at.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vv.yuexingan06.cn

[B12] 跳出多层循环
来源：http://yt.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://js.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gx.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://go.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nb.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zs.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hu.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ls.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yq.asd995.cn

[B13] 判断是否为数字
来源：http://pp.521024.cn

Py:   isinstance(x, (int, float))
来源：http://fl.szxytkj.cn

PHP:  is_numeric($x)
来源：http://ei.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gy.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://su.gzmigu.cn

Java: x instanceof Number
来源：http://sj.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pi.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://ej.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://dx.huanxung.cn

[B14] 判断值是否在集合内
来源：http://sf.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ym.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gy.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://nd.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ei.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ul.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sr.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oq.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yr.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://sx.gzmigu.cn

Py:   a and b or not c
来源：http://ga.hahajie.cn

PHP:  $a && $b || !$c
来源：http://xr.shtwfgs.cn

JS:   a && b || !c
来源：http://im.lnxyls.cn

TS:   a && b || !c
来源：http://ic.panjiajie.cn

Java: a && b || !c
来源：http://uo.9csxet.cn

Go:   a && b || !c
来源：http://qh.nicolike.cn

Ruby: a && b || !c
来源：http://ij.yuntaijiaju.cn

C#:   a && b || !c
来源：http://ce.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ln.521024.cn

Py:   if not data: return
来源：http://zl.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://wp.gzmigu.cn

JS:   if (!data) return;
来源：http://yz.muxihuayi.cn

TS:   if (!data) return;
来源：http://px.yuexingan06.cn

Java: if (data == null) return;
来源：http://aq.bjjhwx.cn

Go:   if data == nil { return }
来源：http://xl.newstarts.cn

Ruby: return if data.nil?
来源：http://cm.huixiangedu.cn

C#:   if (data == null) return;
来源：http://wn.colortex.cn

================================================================================
来源：http://eh.haigaiapp.cn

C. 函数与作用域
来源：http://rh.asd995.cn

================================================================================
来源：http://xa.521024.cn

[C01] 定义函数
来源：http://ma.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://il.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ps.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://ue.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bg.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tq.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zn.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://al.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://so.bookmarksfly.cn

[C02] 默认参数
来源：http://zr.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://ee.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ap.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://xv.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dm.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bt.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hb.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://rn.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ca.nicolike.cn

[C03] 可变参数
来源：http://gr.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://fl.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ya.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ts.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qg.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xl.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://id.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jo.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wv.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://ff.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qh.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bd.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ec.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jp.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://ah.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://bb.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://so.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://hi.yuntaijiaju.cn

[C05] 返回多个值
来源：http://tw.yuntaijiaju.cn

Py:   return a, b
来源：http://hf.newstarts.cn

PHP:  return [$a, $b];
来源：http://pv.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ow.nszjky.cn

TS:   return { a, b };
来源：http://zw.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kf.shxzukj.cn

Go:   return a, b
来源：http://nc.hahajie.cn

Ruby: return a, b
来源：http://qy.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://ih.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://jc.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ad.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xy.szsharing.cn

JS:   const square = x => x * x;
来源：http://qw.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://im.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rf.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yn.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://po.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yi.huanxung.cn

[C07] 把函数作为参数传入
来源：http://rl.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qm.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hp.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ri.colortex.cn

TS:   arr.map(String)
来源：http://fh.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://et.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tp.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://od.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://we.panjiajie.cn

[C08] 闭包
来源：http://mq.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gn.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rg.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lk.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xr.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zm.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tx.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zb.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qx.nicolike.cn

[C09] 递归
来源：http://aq.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aj.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kj.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bg.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mn.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aj.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xg.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cj.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ov.huanxung.cn

[C10] 变量作用域
来源：http://ck.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yz.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pq.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qo.lnxyls.cn

TS:   同 JS
来源：http://pc.newstarts.cn

Java: 方法内为块级作用域
来源：http://jx.gzmigu.cn

Go:   花括号块级作用域
来源：http://he.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://md.hahajie.cn

C#:   块级作用域
来源：http://ll.huanxung.cn

[C11] 模块导入与导出
来源：http://zo.asd995.cn

Py:   from module import func
来源：http://mc.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tn.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://em.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sq.521024.cn

Java: import java.util.List;
来源：http://gg.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mj.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://cj.chemitech.net.cn

C#:   using System.Text;
来源：http://gm.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://kc.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://em.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://cb.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://yg.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://qd.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lc.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://sh.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://qw.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rz.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://ep.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mt.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nh.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bz.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yf.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://as.hnjuh.cn

Go:   func add(a, b int) int
来源：http://gi.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hh.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gd.nicolike.cn

[C14] 泛型函数
来源：http://ve.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sw.hnjuh.cn

PHP:  // 无泛型
来源：http://zf.521024.cn

JS:   // 无泛型
来源：http://eg.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yq.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ak.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vy.asd995.cn

Ruby: # 无泛型
来源：http://oz.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ei.hahajie.cn

[C15] 解构 / 展开参数
来源：http://hl.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pm.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://ux.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ix.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sv.521024.cn

Java: // 无解构
来源：http://hq.asd995.cn

Go:   // 无解构
来源：http://zh.szsharing.cn

Ruby: a, b = pair
来源：http://nl.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://fu.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://pi.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://og.yuntaijiaju.cn

PHP:  // 无重载
来源：http://zl.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ry.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://kf.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ea.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://nj.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://av.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nt.muxihuayi.cn

================================================================================
来源：http://ra.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://tu.521024.cn

================================================================================
来源：http://rl.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://uh.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gm.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vu.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ju.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yx.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cs.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://nu.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://es.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kz.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://wy.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://or.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bv.panjiajie.cn

JS:   arr.push(4);
来源：http://xr.szxytkj.cn

TS:   arr.push(4);
来源：http://gt.wgjwhj.cn


<!-- 参考信息 -->