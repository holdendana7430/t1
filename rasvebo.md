代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lb.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bx.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://vf.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bi.asd995.cn

[B05] 遍历数组 / 列表
来源：http://sw.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://zj.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wz.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bp.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rq.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eq.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gq.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://oc.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pu.asd995.cn

[B06] 遍历字典 / 对象
来源：http://yz.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vu.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zy.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xo.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://im.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uv.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nq.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cm.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kv.szsharing.cn

[B07] while 循环
来源：http://ex.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://cf.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://an.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://nn.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://kn.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://lc.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uo.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://yn.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://rv.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://xh.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://hg.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sp.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://kc.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://wm.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://sj.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ff.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vh.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://at.szxytkj.cn

[B09] break 与 continue
来源：http://tc.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zn.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jm.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ky.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cx.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ue.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bk.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hu.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ws.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://ls.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gi.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dc.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nd.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ru.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yn.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lf.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mn.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://re.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://ua.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://dr.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://vb.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xh.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vc.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ix.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lh.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://bm.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vr.shtwfgs.cn

[B12] 跳出多层循环
来源：http://mm.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bb.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sn.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://og.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rl.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iw.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mi.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fs.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gt.shxzukj.cn

[B13] 判断是否为数字
来源：http://bg.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://ke.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://jo.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xv.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fa.521024.cn

Java: x instanceof Number
来源：http://dm.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://py.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://vd.9csxet.cn

C#:   x is int or double or decimal
来源：http://la.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://fe.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yq.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wx.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://it.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://yh.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eg.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sk.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ap.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jx.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://ng.shxzskj.cn

Py:   a and b or not c
来源：http://te.hahajie.cn

PHP:  $a && $b || !$c
来源：http://xu.shtwfgs.cn

JS:   a && b || !c
来源：http://vy.yuntaijiaju.cn

TS:   a && b || !c
来源：http://pe.jctech888.com.cn

Java: a && b || !c
来源：http://vg.wgjwhj.cn

Go:   a && b || !c
来源：http://dh.colortex.cn

Ruby: a && b || !c
来源：http://hr.shxzskj.cn

C#:   a && b || !c
来源：http://ki.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zp.panjiajie.cn

Py:   if not data: return
来源：http://xc.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://nm.szxytkj.cn

JS:   if (!data) return;
来源：http://vx.lnxyls.cn

TS:   if (!data) return;
来源：http://zu.shtwfgs.cn

Java: if (data == null) return;
来源：http://up.shtwfgs.cn

Go:   if data == nil { return }
来源：http://xh.521024.cn

Ruby: return if data.nil?
来源：http://vr.shxzskj.cn

C#:   if (data == null) return;
来源：http://ws.nszjky.cn

================================================================================
来源：http://ob.huixiangedu.cn

C. 函数与作用域
来源：http://fl.colortex.cn

================================================================================
来源：http://px.gzmigu.cn

[C01] 定义函数
来源：http://dq.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://ih.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gw.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://dl.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lw.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xb.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pi.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://pt.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sj.shxzukj.cn

[C02] 默认参数
来源：http://ba.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://pn.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vd.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://jk.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kk.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://od.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sq.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://wr.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://ut.lnxyls.cn

[C03] 可变参数
来源：http://im.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://mr.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lp.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ce.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eg.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jr.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kc.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bw.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pb.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://kp.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kv.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jx.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ye.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://am.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://ig.521024.cn

Go:   // 无：用配置结构体参数
来源：http://nb.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ua.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://vh.wgjwhj.cn

[C05] 返回多个值
来源：http://br.jctech888.com.cn

Py:   return a, b
来源：http://if.colortex.cn

PHP:  return [$a, $b];
来源：http://mk.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dl.gzmigu.cn

TS:   return { a, b };
来源：http://cj.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://af.hahajie.cn

Go:   return a, b
来源：http://dk.hahajie.cn

Ruby: return a, b
来源：http://li.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://gt.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://ia.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://rx.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ga.newstarts.cn

JS:   const square = x => x * x;
来源：http://wc.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://er.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://da.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://io.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://qr.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yo.newstarts.cn

[C07] 把函数作为参数传入
来源：http://bm.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tm.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vq.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nh.asd995.cn

TS:   arr.map(String)
来源：http://wv.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vh.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://si.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://bx.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rp.huixiangedu.cn

[C08] 闭包
来源：http://ab.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://el.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dx.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cw.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bu.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kx.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iz.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fo.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wc.lnxyls.cn

[C09] 递归
来源：http://zo.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cn.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dh.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wh.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pg.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ux.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yx.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ey.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fr.jctech888.com.cn

[C10] 变量作用域
来源：http://kl.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zx.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jj.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rg.nszjky.cn

TS:   同 JS
来源：http://fc.szxytkj.cn

Java: 方法内为块级作用域
来源：http://oz.9csxet.cn

Go:   花括号块级作用域
来源：http://gn.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rk.muxihuayi.cn

C#:   块级作用域
来源：http://ge.hnjuh.cn

[C11] 模块导入与导出
来源：http://am.shxzskj.cn

Py:   from module import func
来源：http://cd.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oa.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oi.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ks.huanxung.cn

Java: import java.util.List;
来源：http://fh.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vy.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://sx.hnjuh.cn

C#:   using System.Text;
来源：http://vm.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://zm.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://et.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://zh.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://xm.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://os.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wn.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://qv.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://pd.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gy.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://lr.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ui.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kg.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kb.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qe.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://no.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://bx.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tb.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pv.shxzukj.cn

[C14] 泛型函数
来源：http://ji.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://op.bookmarksfly.cn

PHP:  // 无泛型
来源：http://oq.haigaiapp.cn

JS:   // 无泛型
来源：http://jc.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cz.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hc.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dd.szsharing.cn

Ruby: # 无泛型
来源：http://pw.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cu.521024.cn

[C15] 解构 / 展开参数
来源：http://de.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://km.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://hs.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rw.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qa.gzmigu.cn

Java: // 无解构
来源：http://kh.shxzukj.cn

Go:   // 无解构
来源：http://vs.muxihuayi.cn

Ruby: a, b = pair
来源：http://gl.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://xv.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://tt.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rs.asd995.cn

PHP:  // 无重载
来源：http://fs.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gj.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://cl.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tf.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ko.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://yn.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pg.szxytkj.cn

================================================================================
来源：http://og.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://at.gzmigu.cn

================================================================================
来源：http://na.asd995.cn

[D01] 创建数组 / 列表
来源：http://bc.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rb.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ii.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qj.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rs.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pw.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://vt.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://ko.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ll.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://wb.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://al.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ed.hnjuh.cn

JS:   arr.push(4);
来源：http://pv.gzmigu.cn

TS:   arr.push(4);
来源：http://gr.shtwfgs.cn

Java: list.add(4);
来源：http://ya.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://fz.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://ip.colortex.cn

C#:   list.Add(4);
来源：http://ua.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://lv.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://uf.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qy.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ar.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ka.szsharing.cn

Java: list.add(0, 0);
来源：http://wj.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qr.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jo.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://mt.szxytkj.cn

[D04] 删除元素
来源：http://ew.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pz.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bo.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pi.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://lu.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ba.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ar.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://im.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://io.shxzukj.cn

[D05] 访问与修改元素
来源：http://md.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wr.huixinmuqiang.cn


<!-- 参考信息 -->