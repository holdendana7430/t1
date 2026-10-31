代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mk.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hq.szsharing.cn

[B07] while 循环
来源：http://ak.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://tu.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xi.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://kd.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://kt.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://er.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dz.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://bm.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://si.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://gg.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ub.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xy.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://wc.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://ei.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://gq.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zz.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wk.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://ej.newstarts.cn

[B09] break 与 continue
来源：http://yw.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sn.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ms.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pi.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eg.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bl.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zb.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://za.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fb.asd995.cn

[B10] 遍历同时拿索引
来源：http://gx.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pi.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pi.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://db.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hw.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://su.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ck.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tv.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rq.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://ct.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://wu.521024.cn

PHP:  range(0, 10, 2);
来源：http://xf.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xb.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://px.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jl.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ke.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://pr.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://su.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://op.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mr.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rb.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zv.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://el.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uf.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lq.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ym.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fj.huixiangedu.cn

[B13] 判断是否为数字
来源：http://cm.521024.cn

Py:   isinstance(x, (int, float))
来源：http://tv.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://eh.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lt.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rx.szsharing.cn

Java: x instanceof Number
来源：http://va.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nj.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://rm.huanxung.cn

C#:   x is int or double or decimal
来源：http://rn.szsharing.cn

[B14] 判断值是否在集合内
来源：http://tn.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ri.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wl.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://kk.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://zz.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cx.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nn.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ko.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tr.newstarts.cn

[B15] 布尔运算与取反
来源：http://dp.9csxet.cn

Py:   a and b or not c
来源：http://aa.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://hr.jianghongdianzi.cn

JS:   a && b || !c
来源：http://iy.jianghongdianzi.cn

TS:   a && b || !c
来源：http://um.wgjwhj.cn

Java: a && b || !c
来源：http://qv.bjjhwx.cn

Go:   a && b || !c
来源：http://xn.muxihuayi.cn

Ruby: a && b || !c
来源：http://wr.szsharing.cn

C#:   a && b || !c
来源：http://gt.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mc.muxihuayi.cn

Py:   if not data: return
来源：http://ue.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://ui.hnjuh.cn

JS:   if (!data) return;
来源：http://tc.bjjhwx.cn

TS:   if (!data) return;
来源：http://ba.colortex.cn

Java: if (data == null) return;
来源：http://rg.shtwfgs.cn

Go:   if data == nil { return }
来源：http://at.jctech888.com.cn

Ruby: return if data.nil?
来源：http://xi.nicolike.cn

C#:   if (data == null) return;
来源：http://jp.asd995.cn

================================================================================
来源：http://ym.jianghongdianzi.cn

C. 函数与作用域
来源：http://al.nszjky.cn

================================================================================
来源：http://ht.shxzskj.cn

[C01] 定义函数
来源：http://rl.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://xt.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lz.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://iu.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://km.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jl.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wv.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://jh.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nw.yuntaijiaju.cn

[C02] 默认参数
来源：http://se.asd995.cn

Py:   def greet(name="World"): return name
来源：http://sa.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ei.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://sq.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jx.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://px.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ft.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://lf.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://ea.shtwfgs.cn

[C03] 可变参数
来源：http://ir.521024.cn

Py:   def total(*args): return sum(args)
来源：http://mx.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://il.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kf.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wr.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zz.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iy.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://io.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tp.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://jb.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ir.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rf.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://at.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mz.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://do.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://cj.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://vi.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://oh.bookmarksfly.cn

[C05] 返回多个值
来源：http://hj.wgjwhj.cn

Py:   return a, b
来源：http://qo.hahajie.cn

PHP:  return [$a, $b];
来源：http://km.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cu.521024.cn

TS:   return { a, b };
来源：http://gr.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gg.gzmigu.cn

Go:   return a, b
来源：http://zh.haigaiapp.cn

Ruby: return a, b
来源：http://vt.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://bk.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://ba.colortex.cn

Py:   square = lambda x: x * x
来源：http://gw.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ct.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://qe.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://rp.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eq.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ct.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://ft.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lw.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://gz.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ax.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yd.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kr.bookmarksfly.cn

TS:   arr.map(String)
来源：http://pi.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cw.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iq.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://le.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ir.bjjhwx.cn

[C08] 闭包
来源：http://dk.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ey.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gz.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dr.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kh.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cw.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dp.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ok.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://en.bookmarksfly.cn

[C09] 递归
来源：http://sg.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://il.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cy.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zr.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xf.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hc.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kn.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ih.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gi.9csxet.cn

[C10] 变量作用域
来源：http://wf.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://of.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bu.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zj.szsharing.cn

TS:   同 JS
来源：http://fo.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://rf.panjiajie.cn

Go:   花括号块级作用域
来源：http://xb.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vh.colortex.cn

C#:   块级作用域
来源：http://jd.huanxung.cn

[C11] 模块导入与导出
来源：http://ks.newstarts.cn

Py:   from module import func
来源：http://zu.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bd.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hn.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dm.shxzukj.cn

Java: import java.util.List;
来源：http://lz.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ei.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://en.nszjky.cn

C#:   using System.Text;
来源：http://jh.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://yu.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://pb.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://vx.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://fu.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://pi.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dp.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://ij.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://pm.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wf.521024.cn

[C13] 类型声明 / 类型注解
来源：http://uf.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qg.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pz.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cq.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rz.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uq.huanxung.cn

Go:   func add(a, b int) int
来源：http://sx.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cb.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hj.bookmarksfly.cn

[C14] 泛型函数
来源：http://ma.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kv.hnjuh.cn

PHP:  // 无泛型
来源：http://wz.gzmigu.cn

JS:   // 无泛型
来源：http://qs.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yr.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kc.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oa.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://yo.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://du.hahajie.cn

[C15] 解构 / 展开参数
来源：http://ga.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xl.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://hz.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jo.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xr.shxzskj.cn

Java: // 无解构
来源：http://kr.chemitech.net.cn

Go:   // 无解构
来源：http://oh.huixiangedu.cn

Ruby: a, b = pair
来源：http://kk.nszjky.cn

C#:   var (a, b) = pair;
来源：http://je.colortex.cn

[C16] 函数 / 方法重载
来源：http://tj.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ry.shxzukj.cn

PHP:  // 无重载
来源：http://uf.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fk.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://bn.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rt.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://dj.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://st.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gv.jianghongdianzi.cn

================================================================================
来源：http://nn.colortex.cn

D. 数组 / 列表 / 集合
来源：http://rj.hnjuh.cn

================================================================================
来源：http://bo.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://af.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mi.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hr.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mg.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gx.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nb.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://vx.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://fz.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zz.szxytkj.cn

[D02] 追加元素到末尾
来源：http://qu.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ae.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ye.wgjwhj.cn

JS:   arr.push(4);
来源：http://kn.shxzukj.cn

TS:   arr.push(4);
来源：http://ma.huixinmuqiang.cn

Java: list.add(4);
来源：http://bj.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://pj.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://kk.shxzskj.cn

C#:   list.Add(4);
来源：http://tv.colortex.cn

[D03] 在指定位置插入元素
来源：http://jy.asd995.cn

Py:   arr.insert(0, 0)
来源：http://kr.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://so.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uo.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ls.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://gs.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sg.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sn.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://ct.lnxyls.cn

[D04] 删除元素
来源：http://iv.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hs.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wg.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ca.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://sz.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://au.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hc.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cl.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wo.muxihuayi.cn

[D05] 访问与修改元素
来源：http://by.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kd.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eq.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yu.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://zk.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://dg.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://wx.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wr.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://or.lnxyls.cn

[D06] 数组长度
来源：http://jk.yuexingan06.cn

Py:   len(arr)
来源：http://yi.nszjky.cn

PHP:  count($arr);
来源：http://zw.shxzskj.cn

JS:   arr.length
来源：http://fi.colortex.cn

TS:   arr.length
来源：http://ko.yuexingan06.cn

Java: list.size();
来源：http://rz.haigaiapp.cn

Go:   len(arr)
来源：http://xa.nicolike.cn

Ruby: arr.length; arr.size
来源：http://kq.yuexingan06.cn

C#:   list.Count;
来源：http://ga.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://ig.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wi.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ha.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://dx.colortex.cn


<!-- 参考信息 -->