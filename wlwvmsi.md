代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vt.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iy.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://st.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gv.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ze.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sp.huixinmuqiang.cn

[B07] while 循环
来源：http://pn.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://ov.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://si.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://ys.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://bb.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://zs.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fn.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://tt.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://dy.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://nd.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://we.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ga.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://hs.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://xh.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://ww.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hh.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pi.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://qr.jctech888.com.cn

[B09] break 与 continue
来源：http://ao.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dh.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gi.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://am.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cr.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cf.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bf.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kd.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ph.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://dx.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fy.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xh.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yr.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eh.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://am.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ab.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fy.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cr.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://zp.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://ms.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://ma.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cd.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jm.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sf.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ev.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://ia.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rv.hahajie.cn

[B12] 跳出多层循环
来源：http://hq.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dk.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sk.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://de.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ae.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ze.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xq.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ci.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dv.huanxung.cn

[B13] 判断是否为数字
来源：http://gc.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://pj.9csxet.cn

PHP:  is_numeric($x)
来源：http://tj.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mg.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eu.shxzukj.cn

Java: x instanceof Number
来源：http://mi.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ap.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://nc.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://pw.newstarts.cn

[B14] 判断值是否在集合内
来源：http://qj.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ii.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vf.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://nl.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://jz.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vd.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wt.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qa.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dk.nicolike.cn

[B15] 布尔运算与取反
来源：http://cy.huixiangedu.cn

Py:   a and b or not c
来源：http://nx.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://jr.lnxyls.cn

JS:   a && b || !c
来源：http://ip.muxihuayi.cn

TS:   a && b || !c
来源：http://bc.hnjuh.cn

Java: a && b || !c
来源：http://kr.huanxung.cn

Go:   a && b || !c
来源：http://no.szxytkj.cn

Ruby: a && b || !c
来源：http://rf.szsharing.cn

C#:   a && b || !c
来源：http://yo.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ij.nszjky.cn

Py:   if not data: return
来源：http://bs.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://uf.huanxung.cn

JS:   if (!data) return;
来源：http://ps.huixiangedu.cn

TS:   if (!data) return;
来源：http://wm.nicolike.cn

Java: if (data == null) return;
来源：http://ox.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://wr.muxihuayi.cn

Ruby: return if data.nil?
来源：http://zd.yuexingan06.cn

C#:   if (data == null) return;
来源：http://oi.panjiajie.cn

================================================================================
来源：http://fm.nszjky.cn

C. 函数与作用域
来源：http://vu.bookmarksfly.cn

================================================================================
来源：http://ej.newstarts.cn

[C01] 定义函数
来源：http://kg.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://ae.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ro.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://vb.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ay.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://du.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wh.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://wc.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ym.9csxet.cn

[C02] 默认参数
来源：http://mc.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://sl.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ti.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://vj.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yj.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tv.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nb.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://pz.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://cs.szxytkj.cn

[C03] 可变参数
来源：http://hd.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://nn.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://on.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lj.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nd.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cb.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xn.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hn.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uu.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://at.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jt.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nj.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pw.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zp.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://cp.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://ay.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://kg.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://io.huixinmuqiang.cn

[C05] 返回多个值
来源：http://vj.bookmarksfly.cn

Py:   return a, b
来源：http://te.lnxyls.cn

PHP:  return [$a, $b];
来源：http://wi.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://if.hahajie.cn

TS:   return { a, b };
来源：http://nc.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sv.nszjky.cn

Go:   return a, b
来源：http://or.jctech888.com.cn

Ruby: return a, b
来源：http://sc.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ky.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://qk.asd995.cn

Py:   square = lambda x: x * x
来源：http://mk.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rk.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://tj.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://rf.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dy.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nu.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://oj.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hj.nicolike.cn

[C07] 把函数作为参数传入
来源：http://hs.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ae.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ru.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gv.colortex.cn

TS:   arr.map(String)
来源：http://cu.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ap.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hu.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://om.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xd.521024.cn

[C08] 闭包
来源：http://wk.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lk.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vf.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gm.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yo.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cn.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://be.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gv.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://un.gzmigu.cn

[C09] 递归
来源：http://eq.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dr.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bt.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pp.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fr.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pp.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sf.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fa.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dw.wgjwhj.cn

[C10] 变量作用域
来源：http://tb.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kt.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fe.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xd.bjjhwx.cn

TS:   同 JS
来源：http://ps.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://rg.lnxyls.cn

Go:   花括号块级作用域
来源：http://we.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://is.huanxung.cn

C#:   块级作用域
来源：http://no.szsharing.cn

[C11] 模块导入与导出
来源：http://am.wgjwhj.cn

Py:   from module import func
来源：http://cz.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vq.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xj.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fs.jctech888.com.cn

Java: import java.util.List;
来源：http://ln.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xy.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://af.hahajie.cn

C#:   using System.Text;
来源：http://pk.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://vi.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://ny.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://xd.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://by.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://kk.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dd.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://vv.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://ag.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://is.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://hy.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jv.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ie.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bu.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gn.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dz.colortex.cn

Go:   func add(a, b int) int
来源：http://co.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ss.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cl.newstarts.cn

[C14] 泛型函数
来源：http://rb.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://no.wgjwhj.cn

PHP:  // 无泛型
来源：http://rm.panjiajie.cn

JS:   // 无泛型
来源：http://ec.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://py.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xb.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ph.shxzukj.cn

Ruby: # 无泛型
来源：http://pn.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://no.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://xh.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://py.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ug.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gs.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hu.bookmarksfly.cn

Java: // 无解构
来源：http://se.huixiangedu.cn

Go:   // 无解构
来源：http://dt.szxytkj.cn

Ruby: a, b = pair
来源：http://bd.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://vm.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://ct.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pt.hahajie.cn

PHP:  // 无重载
来源：http://oy.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rn.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://nv.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ml.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://sv.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://lr.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mr.shxzukj.cn

================================================================================
来源：http://jl.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://bk.huixinmuqiang.cn

================================================================================
来源：http://wb.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://tp.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cg.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gb.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sh.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ma.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mw.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://wy.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://so.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oa.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://nl.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://do.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qd.nszjky.cn

JS:   arr.push(4);
来源：http://lb.szxytkj.cn

TS:   arr.push(4);
来源：http://hb.shtwfgs.cn

Java: list.add(4);
来源：http://kh.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://ef.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://po.lnxyls.cn

C#:   list.Add(4);
来源：http://vv.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://og.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://le.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hh.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kl.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://bp.shxzskj.cn

Java: list.add(0, 0);
来源：http://va.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ks.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sz.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://su.hahajie.cn

[D04] 删除元素
来源：http://sd.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eo.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cj.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tz.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://gw.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fu.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pd.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lm.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uk.hnjuh.cn

[D05] 访问与修改元素
来源：http://wh.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xi.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://da.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mx.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://pw.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://qf.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://hs.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pj.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://em.nszjky.cn

[D06] 数组长度
来源：http://dk.yuntaijiaju.cn

Py:   len(arr)
来源：http://vp.huixiangedu.cn

PHP:  count($arr);
来源：http://ky.chemitech.net.cn

JS:   arr.length
来源：http://kh.huanxung.cn

TS:   arr.length
来源：http://nk.yuntaijiaju.cn

Java: list.size();
来源：http://zo.huanxung.cn

Go:   len(arr)
来源：http://fx.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://aw.szsharing.cn

C#:   list.Count;
来源：http://tk.shxzukj.cn


<!-- 参考信息 -->