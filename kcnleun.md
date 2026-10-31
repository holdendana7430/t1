代发 wailian999

[B05] 遍历数组 / 列表
来源：http://bd.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://ip.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://up.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mt.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zt.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ux.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tb.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://ct.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qf.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://rr.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pl.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ip.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pv.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kf.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hm.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cw.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kk.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bm.yuntaijiaju.cn

[B07] while 循环
来源：http://np.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://tf.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ur.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://rt.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://tf.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://sz.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ho.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://vo.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://lw.colortex.cn

[B08] do-while（至少执行一次）
来源：http://qe.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://td.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xx.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://rr.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://dg.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://tw.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fu.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ks.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://wp.hahajie.cn

[B09] break 与 continue
来源：http://dg.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xt.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ss.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wn.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kw.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ia.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pw.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ks.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://co.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://fr.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://or.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oc.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://no.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pb.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mp.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kd.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vf.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yo.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://eo.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://jh.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://hd.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sf.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dx.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wd.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://re.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://vc.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vu.nszjky.cn

[B12] 跳出多层循环
来源：http://gn.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oe.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pp.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lk.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://li.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uq.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uq.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://va.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rq.9csxet.cn

[B13] 判断是否为数字
来源：http://dc.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://tj.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://ki.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://au.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yg.yuexingan06.cn

Java: x instanceof Number
来源：http://dy.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://an.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://kw.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://ts.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://wa.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ra.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bu.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://xe.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://dv.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wi.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cd.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cg.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://da.gzmigu.cn

[B15] 布尔运算与取反
来源：http://uo.jctech888.com.cn

Py:   a and b or not c
来源：http://tm.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://aw.hnjuh.cn

JS:   a && b || !c
来源：http://ow.bjjhwx.cn

TS:   a && b || !c
来源：http://di.colortex.cn

Java: a && b || !c
来源：http://zz.wgjwhj.cn

Go:   a && b || !c
来源：http://ag.nicolike.cn

Ruby: a && b || !c
来源：http://eu.muxihuayi.cn

C#:   a && b || !c
来源：http://jz.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xw.hnjuh.cn

Py:   if not data: return
来源：http://ru.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://dn.yuexingan06.cn

JS:   if (!data) return;
来源：http://rt.haigaiapp.cn

TS:   if (!data) return;
来源：http://mh.hahajie.cn

Java: if (data == null) return;
来源：http://fu.nicolike.cn

Go:   if data == nil { return }
来源：http://ij.shtwfgs.cn

Ruby: return if data.nil?
来源：http://mo.szsharing.cn

C#:   if (data == null) return;
来源：http://nd.nszjky.cn

================================================================================
来源：http://tu.huixinmuqiang.cn

C. 函数与作用域
来源：http://mv.asd995.cn

================================================================================
来源：http://yd.jianghongdianzi.cn

[C01] 定义函数
来源：http://zl.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://ub.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rw.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ov.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bo.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fb.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vr.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://gb.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rb.huixiangedu.cn

[C02] 默认参数
来源：http://ez.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://dx.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nm.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://xh.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pi.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nw.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kz.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://zf.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://et.nszjky.cn

[C03] 可变参数
来源：http://ki.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://vz.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jt.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://za.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qp.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mi.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kn.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://el.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hd.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://lb.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bv.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ou.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://il.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ka.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://yy.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://pw.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://ta.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://lp.jianghongdianzi.cn

[C05] 返回多个值
来源：http://sh.bjjhwx.cn

Py:   return a, b
来源：http://vu.9csxet.cn

PHP:  return [$a, $b];
来源：http://qx.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lq.huanxung.cn

TS:   return { a, b };
来源：http://un.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rf.szsharing.cn

Go:   return a, b
来源：http://ih.gzmigu.cn

Ruby: return a, b
来源：http://zy.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://gj.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://yt.huanxung.cn

Py:   square = lambda x: x * x
来源：http://jp.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tf.shxzukj.cn

JS:   const square = x => x * x;
来源：http://xz.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://wr.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://al.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ww.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://by.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ak.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://ps.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://my.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pp.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mp.nszjky.cn

TS:   arr.map(String)
来源：http://zp.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://td.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tp.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://bo.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ob.9csxet.cn

[C08] 闭包
来源：http://qg.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sd.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bj.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hn.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rj.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ld.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sh.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ez.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qq.nicolike.cn

[C09] 递归
来源：http://zg.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ty.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tq.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://br.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xq.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ek.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vi.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wt.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shxzskj.cn

[C10] 变量作用域
来源：http://di.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vo.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ip.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://da.shxzskj.cn

TS:   同 JS
来源：http://un.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://wd.wgjwhj.cn

Go:   花括号块级作用域
来源：http://oa.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cm.hnjuh.cn

C#:   块级作用域
来源：http://cw.shxzukj.cn

[C11] 模块导入与导出
来源：http://hx.szxytkj.cn

Py:   from module import func
来源：http://sa.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tc.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gv.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fl.newstarts.cn

Java: import java.util.List;
来源：http://wr.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sh.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://tp.bjjhwx.cn

C#:   using System.Text;
来源：http://jb.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://wh.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://op.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://kk.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://jj.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://gz.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ph.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://bh.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://sb.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ca.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://eb.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fc.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://an.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sn.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ia.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wy.521024.cn

Go:   func add(a, b int) int
来源：http://lf.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mv.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hg.huanxung.cn

[C14] 泛型函数
来源：http://my.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pd.nszjky.cn

PHP:  // 无泛型
来源：http://ji.nszjky.cn

JS:   // 无泛型
来源：http://gd.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gh.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xd.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pf.panjiajie.cn

Ruby: # 无泛型
来源：http://dn.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lo.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://rm.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://al.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://gs.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bm.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xb.hnjuh.cn

Java: // 无解构
来源：http://bb.bjjhwx.cn

Go:   // 无解构
来源：http://hm.szxytkj.cn

Ruby: a, b = pair
来源：http://wn.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://xx.huanxung.cn

[C16] 函数 / 方法重载
来源：http://fy.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gn.yuntaijiaju.cn

PHP:  // 无重载
来源：http://qb.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ah.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://hw.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fy.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://wk.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://of.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://az.bookmarksfly.cn

================================================================================
来源：http://hi.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://cx.nicolike.cn

================================================================================
来源：http://nj.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://em.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qx.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://om.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rh.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pu.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ni.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://rg.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ph.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vh.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://cq.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bk.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nb.huanxung.cn

JS:   arr.push(4);
来源：http://lp.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://dg.panjiajie.cn

Java: list.add(4);
来源：http://hr.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://zg.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://kz.colortex.cn

C#:   list.Add(4);
来源：http://iv.colortex.cn

[D03] 在指定位置插入元素
来源：http://xb.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://rg.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ri.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nl.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://wc.chemitech.net.cn

Java: list.add(0, 0);
来源：http://ls.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zw.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rn.521024.cn

C#:   list.Insert(0, 0);
来源：http://jm.huanxung.cn

[D04] 删除元素
来源：http://hx.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fx.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wi.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://es.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://nx.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yb.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kt.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gg.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ds.nszjky.cn

[D05] 访问与修改元素
来源：http://kb.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gn.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://au.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tn.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://gc.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://do.asd995.cn


<!-- 参考信息 -->