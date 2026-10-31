代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://ac.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://da.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ap.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://ck.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://na.521024.cn

[B06] 遍历字典 / 对象
来源：http://ty.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oi.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fl.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qc.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fy.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ir.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gz.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tb.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://an.huixiangedu.cn

[B07] while 循环
来源：http://zn.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://lm.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ns.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://he.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://yr.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://qt.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oy.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://gd.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://mv.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://hv.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://pi.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uq.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://xv.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://fw.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://uf.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gb.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fe.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://rs.huixiangedu.cn

[B09] break 与 continue
来源：http://pr.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jb.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ms.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wz.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qh.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://co.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ay.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ww.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vr.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://ip.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gs.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ml.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ax.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ru.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://io.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cw.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bo.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jj.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://zr.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://my.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://lm.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ie.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oa.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://du.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gs.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://ym.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gh.shxzskj.cn

[B12] 跳出多层循环
来源：http://cu.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bh.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://am.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gz.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ii.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ox.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sy.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://np.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://se.panjiajie.cn

[B13] 判断是否为数字
来源：http://ay.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://cf.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://ir.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ax.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://es.hahajie.cn

Java: x instanceof Number
来源：http://qa.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hf.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://uh.colortex.cn

C#:   x is int or double or decimal
来源：http://pz.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://hm.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://je.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://re.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://pq.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://nt.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gn.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ha.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ju.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pp.hahajie.cn

[B15] 布尔运算与取反
来源：http://wv.shxzskj.cn

Py:   a and b or not c
来源：http://wu.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://bf.bookmarksfly.cn

JS:   a && b || !c
来源：http://ve.hahajie.cn

TS:   a && b || !c
来源：http://bt.haigaiapp.cn

Java: a && b || !c
来源：http://yz.jctech888.com.cn

Go:   a && b || !c
来源：http://at.haigaiapp.cn

Ruby: a && b || !c
来源：http://km.szxytkj.cn

C#:   a && b || !c
来源：http://hn.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ky.panjiajie.cn

Py:   if not data: return
来源：http://rl.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://sl.nszjky.cn

JS:   if (!data) return;
来源：http://lg.9csxet.cn

TS:   if (!data) return;
来源：http://yq.hahajie.cn

Java: if (data == null) return;
来源：http://xu.jctech888.com.cn

Go:   if data == nil { return }
来源：http://bq.panjiajie.cn

Ruby: return if data.nil?
来源：http://ca.lnxyls.cn

C#:   if (data == null) return;
来源：http://bd.asd995.cn

================================================================================
来源：http://dh.jianghongdianzi.cn

C. 函数与作用域
来源：http://fr.521024.cn

================================================================================
来源：http://wj.gzmigu.cn

[C01] 定义函数
来源：http://dm.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://vi.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xa.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://rz.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yr.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vi.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zq.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://wb.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vw.szxytkj.cn

[C02] 默认参数
来源：http://cx.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://qs.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ai.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://ze.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ru.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://er.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bx.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://rx.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://aw.szxytkj.cn

[C03] 可变参数
来源：http://tq.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://gf.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eo.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vf.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ny.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wq.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bo.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ow.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wh.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://ef.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bs.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rb.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nc.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ib.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ue.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://eq.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://yh.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://zr.newstarts.cn

[C05] 返回多个值
来源：http://qz.yuntaijiaju.cn

Py:   return a, b
来源：http://he.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://td.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nv.bookmarksfly.cn

TS:   return { a, b };
来源：http://ci.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ah.shtwfgs.cn

Go:   return a, b
来源：http://gz.bjjhwx.cn

Ruby: return a, b
来源：http://sa.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://vk.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://zz.huanxung.cn

Py:   square = lambda x: x * x
来源：http://be.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rg.newstarts.cn

JS:   const square = x => x * x;
来源：http://wk.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://sp.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rs.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ld.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://zm.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://du.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://vx.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hc.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jj.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wl.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://do.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oq.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ym.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://gw.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iy.huanxung.cn

[C08] 闭包
来源：http://ba.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tl.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fk.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wc.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kq.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ah.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ez.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://im.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yp.huixinmuqiang.cn

[C09] 递归
来源：http://oi.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kt.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://er.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nv.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mi.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lp.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sl.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xp.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mq.shxzukj.cn

[C10] 变量作用域
来源：http://ph.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tb.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pq.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fl.szxytkj.cn

TS:   同 JS
来源：http://gj.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://sl.bjjhwx.cn

Go:   花括号块级作用域
来源：http://wt.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nu.chemitech.net.cn

C#:   块级作用域
来源：http://dn.wgjwhj.cn

[C11] 模块导入与导出
来源：http://pe.lnxyls.cn

Py:   from module import func
来源：http://zu.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ng.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vf.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mi.jctech888.com.cn

Java: import java.util.List;
来源：http://ln.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ui.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://vd.bjjhwx.cn

C#:   using System.Text;
来源：http://gd.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://mk.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://dd.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://od.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://nb.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://rt.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wj.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ug.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://hf.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vp.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://fm.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bj.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bu.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iq.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kq.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://db.szxytkj.cn

Go:   func add(a, b int) int
来源：http://rr.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zx.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ur.szsharing.cn

[C14] 泛型函数
来源：http://yp.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yx.bjjhwx.cn

PHP:  // 无泛型
来源：http://dc.hnjuh.cn

JS:   // 无泛型
来源：http://lj.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oj.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://be.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ua.nszjky.cn

Ruby: # 无泛型
来源：http://hc.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nh.hahajie.cn

[C15] 解构 / 展开参数
来源：http://cs.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fi.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://fp.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gt.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oo.jctech888.com.cn

Java: // 无解构
来源：http://te.szxytkj.cn

Go:   // 无解构
来源：http://ge.9csxet.cn

Ruby: a, b = pair
来源：http://tf.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://lh.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://rw.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tr.lnxyls.cn

PHP:  // 无重载
来源：http://bh.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fe.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://iq.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qb.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://ot.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://go.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mw.szxytkj.cn

================================================================================
来源：http://rr.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://ry.521024.cn

================================================================================
来源：http://pt.asd995.cn

[D01] 创建数组 / 列表
来源：http://ps.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qg.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bv.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xb.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mp.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fs.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://af.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://dq.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oa.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://es.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ap.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kz.asd995.cn

JS:   arr.push(4);
来源：http://wz.huixiangedu.cn

TS:   arr.push(4);
来源：http://me.jianghongdianzi.cn

Java: list.add(4);
来源：http://lu.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://qf.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://jh.gzmigu.cn

C#:   list.Add(4);
来源：http://pc.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://cy.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://so.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gj.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bk.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://qj.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://rc.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ec.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yb.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://ba.huanxung.cn

[D04] 删除元素
来源：http://pe.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uc.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pm.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nu.521024.cn

TS:   arr.splice(0, 1);
来源：http://py.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rd.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gv.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dw.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qj.szxytkj.cn

[D05] 访问与修改元素
来源：http://zs.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dc.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ty.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rg.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://kp.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ix.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://ey.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://my.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ta.asd995.cn

[D06] 数组长度
来源：http://wy.9csxet.cn


<!-- 参考信息 -->