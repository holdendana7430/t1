代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ho.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kd.bjjhwx.cn

[B03] switch / match / case
来源：http://xm.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dp.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kk.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rr.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oa.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oq.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://em.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bc.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rx.yuexingan06.cn

[B04] for 计数循环
来源：http://sq.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://hl.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gg.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wa.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hw.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://op.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yl.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://ay.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ur.asd995.cn

[B05] 遍历数组 / 列表
来源：http://xc.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://gf.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wf.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qp.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://em.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cs.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ld.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://sf.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jg.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://fe.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bo.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://td.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ws.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xq.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kj.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zk.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mp.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://li.asd995.cn

[B07] while 循环
来源：http://hg.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://kz.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yx.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://mb.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://ho.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://tg.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mn.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://bu.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://zs.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://hw.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ui.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zl.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://yr.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://gi.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://df.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cn.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dp.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://ez.nszjky.cn

[B09] break 与 continue
来源：http://by.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gn.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ya.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://et.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jt.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eh.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yc.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vh.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lk.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://pj.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nn.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fs.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dc.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ch.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://br.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ji.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qy.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tb.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://nv.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://me.521024.cn

PHP:  range(0, 10, 2);
来源：http://ai.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gt.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lv.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vd.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hl.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://xr.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tx.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://ng.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ha.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ru.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://un.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ew.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xt.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ox.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hr.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wk.9csxet.cn

[B13] 判断是否为数字
来源：http://dx.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://ka.lnxyls.cn

PHP:  is_numeric($x)
来源：http://nz.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yz.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://px.hahajie.cn

Java: x instanceof Number
来源：http://he.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ah.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://bg.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://uj.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://dv.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oa.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gz.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://yd.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://cq.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yi.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jq.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zr.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tf.colortex.cn

[B15] 布尔运算与取反
来源：http://vs.nicolike.cn

Py:   a and b or not c
来源：http://ej.huanxung.cn

PHP:  $a && $b || !$c
来源：http://pb.hahajie.cn

JS:   a && b || !c
来源：http://mj.colortex.cn

TS:   a && b || !c
来源：http://mw.newstarts.cn

Java: a && b || !c
来源：http://jg.szxytkj.cn

Go:   a && b || !c
来源：http://hv.huixiangedu.cn

Ruby: a && b || !c
来源：http://nq.gzmigu.cn

C#:   a && b || !c
来源：http://td.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mv.gzmigu.cn

Py:   if not data: return
来源：http://qe.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://xl.newstarts.cn

JS:   if (!data) return;
来源：http://ej.jctech888.com.cn

TS:   if (!data) return;
来源：http://ue.shxzskj.cn

Java: if (data == null) return;
来源：http://gd.lnxyls.cn

Go:   if data == nil { return }
来源：http://km.hahajie.cn

Ruby: return if data.nil?
来源：http://vx.lnxyls.cn

C#:   if (data == null) return;
来源：http://gr.szsharing.cn

================================================================================
来源：http://hj.yuexingan06.cn

C. 函数与作用域
来源：http://bj.nicolike.cn

================================================================================
来源：http://om.nszjky.cn

[C01] 定义函数
来源：http://ap.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://gq.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xk.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://ir.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xo.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fg.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ah.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://my.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wa.shxzukj.cn

[C02] 默认参数
来源：http://zv.521024.cn

Py:   def greet(name="World"): return name
来源：http://tm.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ko.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://no.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cb.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rh.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ro.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ju.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://vy.colortex.cn

[C03] 可变参数
来源：http://fe.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://dc.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sb.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kh.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yn.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ku.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wz.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rl.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eg.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://hh.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rm.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ad.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cn.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zk.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://zy.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://np.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://bs.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://qa.9csxet.cn

[C05] 返回多个值
来源：http://zi.bookmarksfly.cn

Py:   return a, b
来源：http://xq.shxzukj.cn

PHP:  return [$a, $b];
来源：http://ec.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ne.lnxyls.cn

TS:   return { a, b };
来源：http://rh.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ri.huanxung.cn

Go:   return a, b
来源：http://mv.haigaiapp.cn

Ruby: return a, b
来源：http://vk.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://mk.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://gt.nszjky.cn

Py:   square = lambda x: x * x
来源：http://jh.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zq.9csxet.cn

JS:   const square = x => x * x;
来源：http://oq.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://mo.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yw.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wh.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://fs.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nt.newstarts.cn

[C07] 把函数作为参数传入
来源：http://cc.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fk.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ga.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ly.nicolike.cn

TS:   arr.map(String)
来源：http://qa.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oz.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://te.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://dg.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gv.newstarts.cn

[C08] 闭包
来源：http://db.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ys.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qz.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hi.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tm.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://os.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mm.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rh.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tk.jctech888.com.cn

[C09] 递归
来源：http://fk.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zi.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ie.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uj.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ve.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gj.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ar.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ll.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nb.yuexingan06.cn

[C10] 变量作用域
来源：http://ye.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://km.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kv.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wm.yuexingan06.cn

TS:   同 JS
来源：http://pt.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://uc.hnjuh.cn

Go:   花括号块级作用域
来源：http://ju.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xr.szxytkj.cn

C#:   块级作用域
来源：http://al.colortex.cn

[C11] 模块导入与导出
来源：http://br.shxzskj.cn

Py:   from module import func
来源：http://gp.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ma.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://us.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ih.shxzskj.cn

Java: import java.util.List;
来源：http://zp.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dk.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://lo.asd995.cn

C#:   using System.Text;
来源：http://uq.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://ib.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://me.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ix.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://yk.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://yq.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bq.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://gg.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://vb.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yh.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://xw.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xy.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xf.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vd.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gn.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ef.lnxyls.cn

Go:   func add(a, b int) int
来源：http://ip.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://re.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jq.yuexingan06.cn

[C14] 泛型函数
来源：http://ss.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vc.huanxung.cn

PHP:  // 无泛型
来源：http://sp.9csxet.cn

JS:   // 无泛型
来源：http://ah.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gi.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fw.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wp.chemitech.net.cn

Ruby: # 无泛型
来源：http://lv.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qz.9csxet.cn

[C15] 解构 / 展开参数
来源：http://zn.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jf.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://ja.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uq.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yk.panjiajie.cn

Java: // 无解构
来源：http://zj.shxzskj.cn

Go:   // 无解构
来源：http://iw.szxytkj.cn

Ruby: a, b = pair
来源：http://io.huanxung.cn

C#:   var (a, b) = pair;
来源：http://hm.huanxung.cn

[C16] 函数 / 方法重载
来源：http://hw.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ao.haigaiapp.cn

PHP:  // 无重载
来源：http://op.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ui.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://gb.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fg.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://kr.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://fc.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pb.haigaiapp.cn

================================================================================
来源：http://tq.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://ag.haigaiapp.cn

================================================================================
来源：http://dj.521024.cn

[D01] 创建数组 / 列表
来源：http://vz.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bt.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nb.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kg.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ad.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hf.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://uv.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://dz.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ev.nszjky.cn

[D02] 追加元素到末尾
来源：http://px.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ie.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://if.chemitech.net.cn

JS:   arr.push(4);
来源：http://bg.huanxung.cn

TS:   arr.push(4);
来源：http://av.huanxung.cn

Java: list.add(4);
来源：http://tc.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://je.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://iw.szxytkj.cn

C#:   list.Add(4);
来源：http://se.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://tr.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://ih.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xi.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dl.yuntaijiaju.cn


<!-- 参考信息 -->