代发 wailian999

[B05] 遍历数组 / 列表
来源：http://jq.newstarts.cn

Py:   for item in arr: print(item)
来源：http://yg.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://go.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ed.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cs.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ez.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gk.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://wn.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pv.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://mz.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rg.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gr.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hv.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kg.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yx.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nj.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ll.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wp.szsharing.cn

[B07] while 循环
来源：http://sd.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://do.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wc.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://bx.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://dl.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://ta.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fk.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://vp.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://vn.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://yu.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://fb.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yv.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://dw.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://qr.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://mv.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wo.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hn.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://sl.asd995.cn

[B09] break 与 continue
来源：http://gx.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fo.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ox.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vw.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qu.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pn.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://en.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yi.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://er.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ms.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sm.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mm.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://du.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qo.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hm.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lb.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ig.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ws.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://zv.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://uk.colortex.cn

PHP:  range(0, 10, 2);
来源：http://ds.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gi.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://by.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wa.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wj.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://iz.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sg.nszjky.cn

[B12] 跳出多层循环
来源：http://wm.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ro.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nq.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wq.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xd.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yx.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hp.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gq.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aj.wgjwhj.cn

[B13] 判断是否为数字
来源：http://gp.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://mk.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://mz.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wm.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xd.newstarts.cn

Java: x instanceof Number
来源：http://vg.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zg.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://oo.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://we.huanxung.cn

[B14] 判断值是否在集合内
来源：http://sd.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ae.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fk.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://rb.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://qd.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ke.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dc.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://az.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ao.szxytkj.cn

[B15] 布尔运算与取反
来源：http://la.hnjuh.cn

Py:   a and b or not c
来源：http://ry.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://lb.huixinmuqiang.cn

JS:   a && b || !c
来源：http://mp.jctech888.com.cn

TS:   a && b || !c
来源：http://iz.shxzskj.cn

Java: a && b || !c
来源：http://ym.huanxung.cn

Go:   a && b || !c
来源：http://rl.haigaiapp.cn

Ruby: a && b || !c
来源：http://fh.hnjuh.cn

C#:   a && b || !c
来源：http://fw.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pc.szxytkj.cn

Py:   if not data: return
来源：http://yk.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://kq.521024.cn

JS:   if (!data) return;
来源：http://jk.jctech888.com.cn

TS:   if (!data) return;
来源：http://sy.panjiajie.cn

Java: if (data == null) return;
来源：http://uk.shtwfgs.cn

Go:   if data == nil { return }
来源：http://le.nicolike.cn

Ruby: return if data.nil?
来源：http://dx.shtwfgs.cn

C#:   if (data == null) return;
来源：http://cv.shxzukj.cn

================================================================================
来源：http://ke.bjjhwx.cn

C. 函数与作用域
来源：http://lt.bjjhwx.cn

================================================================================
来源：http://ap.huixinmuqiang.cn

[C01] 定义函数
来源：http://os.521024.cn

Py:   def add(a, b): return a + b
来源：http://cv.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gi.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://wv.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gh.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://je.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://si.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://ud.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lf.panjiajie.cn

[C02] 默认参数
来源：http://fv.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://hj.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xm.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://tn.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uk.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://np.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lk.521024.cn

Ruby: def greet(name = "World") = name
来源：http://tf.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://hh.muxihuayi.cn

[C03] 可变参数
来源：http://ol.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://ce.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nn.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ff.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://id.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://am.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vk.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jf.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ny.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://mv.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fj.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zm.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kg.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wr.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://uc.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://ct.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://ua.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://sj.bjjhwx.cn

[C05] 返回多个值
来源：http://il.shtwfgs.cn

Py:   return a, b
来源：http://he.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://xz.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iq.haigaiapp.cn

TS:   return { a, b };
来源：http://oj.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jj.shtwfgs.cn

Go:   return a, b
来源：http://vj.lnxyls.cn

Ruby: return a, b
来源：http://rd.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://om.colortex.cn

[C06] 匿名函数 / lambda
来源：http://xe.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://fv.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kj.nicolike.cn

JS:   const square = x => x * x;
来源：http://iz.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://cs.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bo.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://at.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://xa.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://us.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://yv.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qi.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://px.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ym.colortex.cn

TS:   arr.map(String)
来源：http://sg.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mn.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oz.521024.cn

Ruby: arr.map(&:upcase)
来源：http://nt.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qq.9csxet.cn

[C08] 闭包
来源：http://ic.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mc.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pb.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aw.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ts.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kb.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lx.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://em.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ft.chemitech.net.cn

[C09] 递归
来源：http://zw.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rj.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xd.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ud.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ms.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://go.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pa.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lx.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ji.huanxung.cn

[C10] 变量作用域
来源：http://kx.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kx.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ug.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://os.chemitech.net.cn

TS:   同 JS
来源：http://ue.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://tc.muxihuayi.cn

Go:   花括号块级作用域
来源：http://nc.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ed.jianghongdianzi.cn

C#:   块级作用域
来源：http://xb.shxzukj.cn

[C11] 模块导入与导出
来源：http://io.szxytkj.cn

Py:   from module import func
来源：http://qd.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zb.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tj.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://td.chemitech.net.cn

Java: import java.util.List;
来源：http://lz.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dt.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://bd.huixinmuqiang.cn

C#:   using System.Text;
来源：http://ts.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://mu.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://wb.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://un.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://kj.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://oy.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ua.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://xt.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://iw.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qn.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://pz.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pk.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://am.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ow.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jh.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mx.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://nm.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://do.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fg.gzmigu.cn

[C14] 泛型函数
来源：http://fb.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ft.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://ac.shtwfgs.cn

JS:   // 无泛型
来源：http://zg.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://md.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uz.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ks.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://wl.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pc.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://xl.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mo.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://fk.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ps.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://je.yuntaijiaju.cn

Java: // 无解构
来源：http://hd.yuntaijiaju.cn

Go:   // 无解构
来源：http://et.bjjhwx.cn

Ruby: a, b = pair
来源：http://pg.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://mk.521024.cn

[C16] 函数 / 方法重载
来源：http://mo.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pg.nszjky.cn

PHP:  // 无重载
来源：http://gl.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://my.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://sk.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wa.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://cp.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://qi.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ck.nicolike.cn

================================================================================
来源：http://qc.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://is.hnjuh.cn

================================================================================
来源：http://gc.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://un.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ym.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dr.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iy.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oe.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dy.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ji.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://pl.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jd.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://ol.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://je.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vw.haigaiapp.cn

JS:   arr.push(4);
来源：http://xr.lnxyls.cn

TS:   arr.push(4);
来源：http://ei.bookmarksfly.cn

Java: list.add(4);
来源：http://df.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://kb.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://zv.jctech888.com.cn

C#:   list.Add(4);
来源：http://ka.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://ai.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://ix.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rf.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ph.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://yk.huixiangedu.cn

Java: list.add(0, 0);
来源：http://km.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ks.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wg.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://tp.huixinmuqiang.cn

[D04] 删除元素
来源：http://zg.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ql.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sj.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wm.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://pd.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gr.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sg.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bd.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wc.szxytkj.cn

[D05] 访问与修改元素
来源：http://ep.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://to.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vm.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nl.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://yt.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://tw.hahajie.cn


<!-- 参考信息 -->