代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://um.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qi.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ik.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jo.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ox.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://be.gzmigu.cn

[B03] switch / match / case
来源：http://oj.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vt.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fh.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ox.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uz.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bn.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ik.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ai.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kw.bjjhwx.cn

[B04] for 计数循环
来源：http://uc.colortex.cn

Py:   for i in range(10): print(i)
来源：http://gx.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bi.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sy.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wi.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nl.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ia.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://np.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cn.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://ti.colortex.cn

Py:   for item in arr: print(item)
来源：http://np.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ym.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qx.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nz.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xf.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iw.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://wm.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bv.asd995.cn

[B06] 遍历字典 / 对象
来源：http://ox.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rq.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wq.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ca.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ds.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fm.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fi.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://er.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ub.newstarts.cn

[B07] while 循环
来源：http://sr.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://fk.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://me.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://eo.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://gt.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://jj.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qy.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://hn.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://ur.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://qe.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://bs.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tp.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://kw.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://ca.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://bt.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://et.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hr.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://os.hnjuh.cn

[B09] break 与 continue
来源：http://sr.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ck.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ee.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hc.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ly.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ez.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hl.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ye.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://ux.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fl.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sl.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xd.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qk.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wb.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xu.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://do.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ge.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://yh.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://ee.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://wf.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iq.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kf.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dx.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tb.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://vr.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gr.haigaiapp.cn

[B12] 跳出多层循环
来源：http://bj.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uf.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yo.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://in.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nx.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sl.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wz.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nq.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ws.wgjwhj.cn

[B13] 判断是否为数字
来源：http://fl.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://vk.nicolike.cn

PHP:  is_numeric($x)
来源：http://if.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rw.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fw.nicolike.cn

Java: x instanceof Number
来源：http://me.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://za.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://de.nicolike.cn

C#:   x is int or double or decimal
来源：http://hy.nszjky.cn

[B14] 判断值是否在集合内
来源：http://iy.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mj.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yr.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://as.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://is.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pr.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tk.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dm.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vk.9csxet.cn

[B15] 布尔运算与取反
来源：http://kz.bjjhwx.cn

Py:   a and b or not c
来源：http://uv.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://ew.colortex.cn

JS:   a && b || !c
来源：http://yf.hahajie.cn

TS:   a && b || !c
来源：http://up.asd995.cn

Java: a && b || !c
来源：http://dq.szsharing.cn

Go:   a && b || !c
来源：http://je.shtwfgs.cn

Ruby: a && b || !c
来源：http://ie.huixiangedu.cn

C#:   a && b || !c
来源：http://ea.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ob.colortex.cn

Py:   if not data: return
来源：http://qs.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://jr.asd995.cn

JS:   if (!data) return;
来源：http://zn.lnxyls.cn

TS:   if (!data) return;
来源：http://yq.muxihuayi.cn

Java: if (data == null) return;
来源：http://bn.newstarts.cn

Go:   if data == nil { return }
来源：http://vp.muxihuayi.cn

Ruby: return if data.nil?
来源：http://zq.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://dk.bjjhwx.cn

================================================================================
来源：http://ey.chemitech.net.cn

C. 函数与作用域
来源：http://wm.hahajie.cn

================================================================================
来源：http://vh.yuexingan06.cn

[C01] 定义函数
来源：http://rq.521024.cn

Py:   def add(a, b): return a + b
来源：http://iu.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://up.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://xc.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ss.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ps.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xx.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://yu.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ke.colortex.cn

[C02] 默认参数
来源：http://kj.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://by.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mu.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qy.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xo.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rl.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nq.521024.cn

Ruby: def greet(name = "World") = name
来源：http://rw.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://ce.szxytkj.cn

[C03] 可变参数
来源：http://pj.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://jb.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uc.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wf.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://di.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ih.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yo.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oe.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ax.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://qq.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wg.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://at.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qo.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xa.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://eo.521024.cn

Go:   // 无：用配置结构体参数
来源：http://kj.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://ks.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://vg.szxytkj.cn

[C05] 返回多个值
来源：http://ss.nszjky.cn

Py:   return a, b
来源：http://dn.nicolike.cn

PHP:  return [$a, $b];
来源：http://ll.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yw.asd995.cn

TS:   return { a, b };
来源：http://rm.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nf.lnxyls.cn

Go:   return a, b
来源：http://sh.jctech888.com.cn

Ruby: return a, b
来源：http://st.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://pl.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://px.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://bc.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fh.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://xk.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://yc.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xv.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://us.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://as.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tt.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://eo.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fs.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jr.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jc.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://xm.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tm.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rv.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://ih.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rp.shtwfgs.cn

[C08] 闭包
来源：http://fi.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hw.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nt.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://to.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vk.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fs.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hk.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ay.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yh.panjiajie.cn

[C09] 递归
来源：http://lg.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gt.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pc.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ae.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ts.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nl.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ne.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bs.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://of.shxzskj.cn

[C10] 变量作用域
来源：http://db.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lp.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ac.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qg.shxzskj.cn

TS:   同 JS
来源：http://ce.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://sh.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://ev.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uj.haigaiapp.cn

C#:   块级作用域
来源：http://cq.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://ic.yuexingan06.cn

Py:   from module import func
来源：http://xq.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ff.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pa.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.bookmarksfly.cn

Java: import java.util.List;
来源：http://lu.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ep.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://pp.yuexingan06.cn

C#:   using System.Text;
来源：http://ec.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://vs.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://wr.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ih.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://pw.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://qr.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://za.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://mz.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://ci.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://av.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://sy.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yl.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yb.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://id.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ln.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ep.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://vz.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ml.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xk.hahajie.cn

[C14] 泛型函数
来源：http://az.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kx.lnxyls.cn

PHP:  // 无泛型
来源：http://ti.jctech888.com.cn

JS:   // 无泛型
来源：http://eu.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hu.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ae.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jj.shtwfgs.cn

Ruby: # 无泛型
来源：http://vp.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fp.nicolike.cn

[C15] 解构 / 展开参数
来源：http://os.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ef.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://fg.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dm.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ms.newstarts.cn

Java: // 无解构
来源：http://ni.nicolike.cn

Go:   // 无解构
来源：http://vx.colortex.cn

Ruby: a, b = pair
来源：http://hv.asd995.cn

C#:   var (a, b) = pair;
来源：http://dj.colortex.cn

[C16] 函数 / 方法重载
来源：http://ek.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hy.szsharing.cn

PHP:  // 无重载
来源：http://kv.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://be.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ul.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ex.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://zy.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://au.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lc.wgjwhj.cn

================================================================================
来源：http://vu.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://sv.haigaiapp.cn

================================================================================
来源：http://ue.colortex.cn

[D01] 创建数组 / 列表
来源：http://yn.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ul.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qz.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xa.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zv.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ae.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://rp.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://jj.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gu.newstarts.cn

[D02] 追加元素到末尾
来源：http://cc.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fd.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xk.gzmigu.cn

JS:   arr.push(4);
来源：http://vx.asd995.cn

TS:   arr.push(4);
来源：http://sm.hnjuh.cn

Java: list.add(4);
来源：http://re.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://vu.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://di.huanxung.cn

C#:   list.Add(4);
来源：http://lz.yuexingan06.cn


<!-- 参考信息 -->