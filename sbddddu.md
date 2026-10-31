代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vq.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rw.muxihuayi.cn

[B07] while 循环
来源：http://qg.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://zw.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ik.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://hp.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://gn.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://pn.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sn.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://ik.521024.cn

C#:   while (i < 10) { i++; }
来源：http://vw.colortex.cn

[B08] do-while（至少执行一次）
来源：http://bp.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://vz.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pl.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://tc.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://gi.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://xl.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bx.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ec.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://ic.bookmarksfly.cn

[B09] break 与 continue
来源：http://fg.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wo.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://op.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vq.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ge.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rr.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sr.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ws.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://qq.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ey.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://np.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zw.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gn.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zf.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cj.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://du.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://py.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://mn.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://ux.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://vs.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pw.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sy.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uc.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ww.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://al.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dr.asd995.cn

[B12] 跳出多层循环
来源：http://zg.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eo.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vj.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ff.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://we.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://so.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mk.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vu.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ab.asd995.cn

[B13] 判断是否为数字
来源：http://gl.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://vk.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://xq.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nk.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lc.szxytkj.cn

Java: x instanceof Number
来源：http://ls.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kn.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://bn.szsharing.cn

C#:   x is int or double or decimal
来源：http://bh.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://lq.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hr.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mg.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://aw.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://yz.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xo.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://er.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sk.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ba.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://mb.bjjhwx.cn

Py:   a and b or not c
来源：http://rs.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://tp.wgjwhj.cn

JS:   a && b || !c
来源：http://yz.jctech888.com.cn

TS:   a && b || !c
来源：http://vz.newstarts.cn

Java: a && b || !c
来源：http://dw.chemitech.net.cn

Go:   a && b || !c
来源：http://it.haigaiapp.cn

Ruby: a && b || !c
来源：http://vh.panjiajie.cn

C#:   a && b || !c
来源：http://qj.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gk.shtwfgs.cn

Py:   if not data: return
来源：http://eq.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://qx.newstarts.cn

JS:   if (!data) return;
来源：http://lc.wgjwhj.cn

TS:   if (!data) return;
来源：http://yw.haigaiapp.cn

Java: if (data == null) return;
来源：http://ho.bjjhwx.cn

Go:   if data == nil { return }
来源：http://rp.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://de.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://vx.muxihuayi.cn

================================================================================
来源：http://ru.chemitech.net.cn

C. 函数与作用域
来源：http://qe.huanxung.cn

================================================================================
来源：http://hw.szsharing.cn

[C01] 定义函数
来源：http://ed.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://ho.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xf.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://xj.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cj.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pe.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qf.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://gn.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wt.yuntaijiaju.cn

[C02] 默认参数
来源：http://lh.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://vk.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uq.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ks.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://aj.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mx.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zz.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://iu.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://ap.shtwfgs.cn

[C03] 可变参数
来源：http://pw.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://xy.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fm.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mu.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wd.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wq.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kg.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ec.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cg.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://mc.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fu.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bo.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oz.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ai.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://qd.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://md.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://al.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://tu.wgjwhj.cn

[C05] 返回多个值
来源：http://kw.shxzskj.cn

Py:   return a, b
来源：http://el.gzmigu.cn

PHP:  return [$a, $b];
来源：http://uc.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qs.9csxet.cn

TS:   return { a, b };
来源：http://qi.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rz.wgjwhj.cn

Go:   return a, b
来源：http://cj.jianghongdianzi.cn

Ruby: return a, b
来源：http://lm.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://cl.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://fe.nicolike.cn

Py:   square = lambda x: x * x
来源：http://jg.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cc.newstarts.cn

JS:   const square = x => x * x;
来源：http://tb.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://lt.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://az.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pd.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://rs.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kc.nszjky.cn

[C07] 把函数作为参数传入
来源：http://fh.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ub.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wz.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gs.newstarts.cn

TS:   arr.map(String)
来源：http://zc.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eg.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ux.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://kp.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ij.colortex.cn

[C08] 闭包
来源：http://ez.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://in.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bb.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mn.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hc.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bv.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rb.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nk.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wp.bookmarksfly.cn

[C09] 递归
来源：http://az.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ny.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hi.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://of.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://px.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nf.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lg.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sl.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vj.szsharing.cn

[C10] 变量作用域
来源：http://yz.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hx.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uh.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qm.haigaiapp.cn

TS:   同 JS
来源：http://xd.nicolike.cn

Java: 方法内为块级作用域
来源：http://dp.asd995.cn

Go:   花括号块级作用域
来源：http://fg.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ek.huixiangedu.cn

C#:   块级作用域
来源：http://rj.9csxet.cn

[C11] 模块导入与导出
来源：http://bx.lnxyls.cn

Py:   from module import func
来源：http://cn.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rb.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kd.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://be.hnjuh.cn

Java: import java.util.List;
来源：http://as.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ob.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://ec.lnxyls.cn

C#:   using System.Text;
来源：http://jy.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://zj.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://qh.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://pf.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://yz.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://bb.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://le.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://dk.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://af.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wz.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://wf.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gr.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wb.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nh.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cj.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wn.szsharing.cn

Go:   func add(a, b int) int
来源：http://ld.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ad.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://en.muxihuayi.cn

[C14] 泛型函数
来源：http://ei.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dc.9csxet.cn

PHP:  // 无泛型
来源：http://wx.muxihuayi.cn

JS:   // 无泛型
来源：http://sn.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wm.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vn.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ow.521024.cn

Ruby: # 无泛型
来源：http://rj.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zt.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://ty.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pi.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://ex.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ys.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fi.szxytkj.cn

Java: // 无解构
来源：http://eq.szsharing.cn

Go:   // 无解构
来源：http://vw.huixiangedu.cn

Ruby: a, b = pair
来源：http://od.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://op.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://uq.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tr.szsharing.cn

PHP:  // 无重载
来源：http://tc.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bi.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://oo.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kt.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://me.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://xx.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qz.shxzskj.cn

================================================================================
来源：http://ip.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://kz.huixiangedu.cn

================================================================================
来源：http://ee.nszjky.cn

[D01] 创建数组 / 列表
来源：http://ca.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wf.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xw.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ql.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gf.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ox.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://qg.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://is.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pd.szxytkj.cn

[D02] 追加元素到末尾
来源：http://ll.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sp.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yz.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://fv.hahajie.cn

TS:   arr.push(4);
来源：http://hd.jianghongdianzi.cn

Java: list.add(4);
来源：http://pk.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://kx.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://ck.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://ie.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://jp.asd995.cn

Py:   arr.insert(0, 0)
来源：http://gs.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uv.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fn.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://lj.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://zv.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fs.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zr.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://af.chemitech.net.cn

[D04] 删除元素
来源：http://ys.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nk.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lv.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jc.521024.cn

TS:   arr.splice(0, 1);
来源：http://df.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mi.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dr.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xb.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xj.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://ru.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ci.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yf.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jf.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://rq.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://cy.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://dy.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ms.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oq.hahajie.cn

[D06] 数组长度
来源：http://bx.huanxung.cn

Py:   len(arr)
来源：http://ui.nszjky.cn

PHP:  count($arr);
来源：http://sq.huanxung.cn

JS:   arr.length
来源：http://hk.shxzskj.cn

TS:   arr.length
来源：http://en.newstarts.cn

Java: list.size();
来源：http://fg.nszjky.cn

Go:   len(arr)
来源：http://tf.huanxung.cn

Ruby: arr.length; arr.size
来源：http://td.asd995.cn

C#:   list.Count;
来源：http://aw.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://bk.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qf.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ox.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://qt.nicolike.cn


<!-- 参考信息 -->