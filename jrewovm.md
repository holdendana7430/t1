代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zm.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oo.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://py.jianghongdianzi.cn

[B04] for 计数循环
来源：http://bi.521024.cn

Py:   for i in range(10): print(i)
来源：http://oh.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wh.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yh.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rb.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ik.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rw.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://le.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hn.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://zv.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://dd.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ps.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://px.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jq.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bi.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://td.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://zj.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ex.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://jt.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vl.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bq.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vu.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kt.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://or.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yt.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ir.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ka.bjjhwx.cn

[B07] while 循环
来源：http://sw.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://bm.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mj.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://wy.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://oc.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://su.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oq.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://lr.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://zw.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://em.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://sg.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zb.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://am.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://re.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://tw.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yx.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://db.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://dt.nicolike.cn

[B09] break 与 continue
来源：http://cs.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yt.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xf.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hf.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://py.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tt.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zd.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vj.521024.cn

[B10] 遍历同时拿索引
来源：http://vj.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ka.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lx.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gd.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bo.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fx.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yi.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qw.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bh.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://na.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://mr.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://hz.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ki.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qw.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ik.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://id.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://er.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uj.jctech888.com.cn

[B12] 跳出多层循环
来源：http://za.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zp.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ig.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://go.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kn.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://by.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xh.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gl.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ga.jctech888.com.cn

[B13] 判断是否为数字
来源：http://fy.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://pg.nicolike.cn

PHP:  is_numeric($x)
来源：http://ha.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sb.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zc.lnxyls.cn

Java: x instanceof Number
来源：http://zw.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vk.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://ke.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://ak.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://pz.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ps.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mv.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://cw.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://my.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pt.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bq.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sd.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tl.colortex.cn

[B15] 布尔运算与取反
来源：http://kz.szxytkj.cn

Py:   a and b or not c
来源：http://cs.huanxung.cn

PHP:  $a && $b || !$c
来源：http://vt.szsharing.cn

JS:   a && b || !c
来源：http://qk.lnxyls.cn

TS:   a && b || !c
来源：http://np.bookmarksfly.cn

Java: a && b || !c
来源：http://fk.chemitech.net.cn

Go:   a && b || !c
来源：http://ix.asd995.cn

Ruby: a && b || !c
来源：http://re.jianghongdianzi.cn

C#:   a && b || !c
来源：http://ff.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ck.haigaiapp.cn

Py:   if not data: return
来源：http://rt.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://nr.szxytkj.cn

JS:   if (!data) return;
来源：http://wd.szxytkj.cn

TS:   if (!data) return;
来源：http://sm.shtwfgs.cn

Java: if (data == null) return;
来源：http://tm.yuexingan06.cn

Go:   if data == nil { return }
来源：http://rv.muxihuayi.cn

Ruby: return if data.nil?
来源：http://ip.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://ta.shxzukj.cn

================================================================================
来源：http://xn.newstarts.cn

C. 函数与作用域
来源：http://dk.yuntaijiaju.cn

================================================================================
来源：http://aw.nicolike.cn

[C01] 定义函数
来源：http://gx.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://oa.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iw.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://fv.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ss.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jq.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oq.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://ne.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mx.hahajie.cn

[C02] 默认参数
来源：http://lr.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://jm.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oa.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://rf.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://in.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://em.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wz.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://id.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://or.shxzukj.cn

[C03] 可变参数
来源：http://mc.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://js.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nu.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cg.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qu.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jn.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tg.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qw.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nf.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://bq.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zs.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yk.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://em.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wr.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ce.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://lv.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://wf.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://lq.huixinmuqiang.cn

[C05] 返回多个值
来源：http://pj.shtwfgs.cn

Py:   return a, b
来源：http://zq.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://go.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kp.huanxung.cn

TS:   return { a, b };
来源：http://oz.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ln.colortex.cn

Go:   return a, b
来源：http://tn.gzmigu.cn

Ruby: return a, b
来源：http://jg.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://ea.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://sx.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://nx.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ro.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://va.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://hf.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zm.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://up.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://hj.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zd.szsharing.cn

[C07] 把函数作为参数传入
来源：http://az.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dw.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vz.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hf.shtwfgs.cn

TS:   arr.map(String)
来源：http://vs.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://li.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yo.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://fv.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tb.yuexingan06.cn

[C08] 闭包
来源：http://od.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ni.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sp.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rr.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jx.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ir.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vc.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sb.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rk.nicolike.cn

[C09] 递归
来源：http://uy.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zk.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lv.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://io.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mh.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pf.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ia.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://or.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bs.asd995.cn

[C10] 变量作用域
来源：http://ne.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fn.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xo.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xq.chemitech.net.cn

TS:   同 JS
来源：http://ey.nicolike.cn

Java: 方法内为块级作用域
来源：http://tl.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://xb.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hk.asd995.cn

C#:   块级作用域
来源：http://jn.jctech888.com.cn

[C11] 模块导入与导出
来源：http://mg.jianghongdianzi.cn

Py:   from module import func
来源：http://hl.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cb.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nr.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ck.yuexingan06.cn

Java: import java.util.List;
来源：http://vd.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wl.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://lm.chemitech.net.cn

C#:   using System.Text;
来源：http://dl.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://af.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://du.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://nd.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://ec.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://te.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ds.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://dz.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://wl.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ta.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://im.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wq.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hc.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ne.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ge.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ng.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://gc.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vj.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bo.lnxyls.cn

[C14] 泛型函数
来源：http://cj.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yp.szxytkj.cn

PHP:  // 无泛型
来源：http://wy.huixiangedu.cn

JS:   // 无泛型
来源：http://uv.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vt.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xw.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rd.bjjhwx.cn

Ruby: # 无泛型
来源：http://yk.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ac.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://th.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ri.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://gl.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bb.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ya.panjiajie.cn

Java: // 无解构
来源：http://ky.wgjwhj.cn

Go:   // 无解构
来源：http://hm.szxytkj.cn

Ruby: a, b = pair
来源：http://hy.hahajie.cn

C#:   var (a, b) = pair;
来源：http://ki.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://nw.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tb.521024.cn

PHP:  // 无重载
来源：http://he.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sc.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://oe.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ye.521024.cn

Go:   // 无重载：用不同函数名
来源：http://zb.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://sz.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vn.hahajie.cn

================================================================================
来源：http://vy.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://yf.bjjhwx.cn

================================================================================
来源：http://ag.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://cc.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://st.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cl.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nw.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hd.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oe.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://ob.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://xg.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://as.lnxyls.cn

[D02] 追加元素到末尾
来源：http://fr.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qr.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ak.szxytkj.cn

JS:   arr.push(4);
来源：http://fs.hnjuh.cn

TS:   arr.push(4);
来源：http://dn.huixinmuqiang.cn

Java: list.add(4);
来源：http://sr.colortex.cn

Go:   arr = append(arr, 4)
来源：http://mw.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://tm.wgjwhj.cn

C#:   list.Add(4);
来源：http://uu.asd995.cn

[D03] 在指定位置插入元素
来源：http://mf.521024.cn

Py:   arr.insert(0, 0)
来源：http://xx.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qk.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://br.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://kt.9csxet.cn

Java: list.add(0, 0);
来源：http://tp.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ae.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lo.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://ry.shxzukj.cn

[D04] 删除元素
来源：http://xi.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ak.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://te.colortex.cn


<!-- 参考信息 -->