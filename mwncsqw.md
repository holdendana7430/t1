代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://uz.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://lu.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://ae.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://qx.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oe.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://jn.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://et.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://ff.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://sx.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jc.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://uh.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://gj.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://lt.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jq.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vm.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://jp.szsharing.cn

[B09] break 与 continue
来源：http://fo.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pq.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gy.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yw.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zr.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cz.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cb.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fg.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://vj.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://em.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tl.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rq.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://od.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dd.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iq.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mw.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ko.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://ng.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://wu.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://nq.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ck.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xq.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rh.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xa.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://xq.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xm.bjjhwx.cn

[B12] 跳出多层循环
来源：http://yq.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://np.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://db.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hi.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kb.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cn.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zc.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://no.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uo.haigaiapp.cn

[B13] 判断是否为数字
来源：http://vz.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://tt.nszjky.cn

PHP:  is_numeric($x)
来源：http://ln.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ld.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sb.gzmigu.cn

Java: x instanceof Number
来源：http://so.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uy.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://ti.gzmigu.cn

C#:   x is int or double or decimal
来源：http://lw.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://gw.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mz.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jm.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://iq.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://yo.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://na.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qp.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kg.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hh.panjiajie.cn

[B15] 布尔运算与取反
来源：http://ri.muxihuayi.cn

Py:   a and b or not c
来源：http://pb.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://fu.nszjky.cn

JS:   a && b || !c
来源：http://wh.hnjuh.cn

TS:   a && b || !c
来源：http://gi.521024.cn

Java: a && b || !c
来源：http://gr.yuexingan06.cn

Go:   a && b || !c
来源：http://qp.newstarts.cn

Ruby: a && b || !c
来源：http://gv.chemitech.net.cn

C#:   a && b || !c
来源：http://rr.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gw.hahajie.cn

Py:   if not data: return
来源：http://yz.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://tx.nicolike.cn

JS:   if (!data) return;
来源：http://om.bookmarksfly.cn

TS:   if (!data) return;
来源：http://fd.szxytkj.cn

Java: if (data == null) return;
来源：http://vs.muxihuayi.cn

Go:   if data == nil { return }
来源：http://oz.521024.cn

Ruby: return if data.nil?
来源：http://dc.jctech888.com.cn

C#:   if (data == null) return;
来源：http://pq.521024.cn

================================================================================
来源：http://fn.panjiajie.cn

C. 函数与作用域
来源：http://gw.newstarts.cn

================================================================================
来源：http://bj.nszjky.cn

[C01] 定义函数
来源：http://gp.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://yl.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ju.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://ir.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://im.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xo.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cu.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://wq.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fz.huixinmuqiang.cn

[C02] 默认参数
来源：http://al.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://jx.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pr.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://vy.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ue.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uu.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dr.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://ap.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://fa.bookmarksfly.cn

[C03] 可变参数
来源：http://bh.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://tc.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fw.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sv.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eq.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ty.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fp.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sc.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ru.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://zw.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://an.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jl.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ie.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lc.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://yh.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://go.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://en.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://sv.asd995.cn

[C05] 返回多个值
来源：http://cp.wgjwhj.cn

Py:   return a, b
来源：http://qp.nszjky.cn

PHP:  return [$a, $b];
来源：http://iu.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sx.shxzskj.cn

TS:   return { a, b };
来源：http://ly.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ty.yuntaijiaju.cn

Go:   return a, b
来源：http://zm.shxzskj.cn

Ruby: return a, b
来源：http://fs.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://og.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://so.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://cu.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zy.nszjky.cn

JS:   const square = x => x * x;
来源：http://dl.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://sy.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xr.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ss.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://kv.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gr.huanxung.cn

[C07] 把函数作为参数传入
来源：http://ww.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iv.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cy.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fd.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://gf.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kw.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wd.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://po.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hi.chemitech.net.cn

[C08] 闭包
来源：http://ts.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kn.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tq.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qi.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ud.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ef.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hi.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iy.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ae.muxihuayi.cn

[C09] 递归
来源：http://jn.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://du.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ck.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://of.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cv.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yl.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://al.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zy.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uh.yuntaijiaju.cn

[C10] 变量作用域
来源：http://jg.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://or.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ju.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ym.haigaiapp.cn

TS:   同 JS
来源：http://ex.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://yz.huixiangedu.cn

Go:   花括号块级作用域
来源：http://se.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hj.gzmigu.cn

C#:   块级作用域
来源：http://tt.gzmigu.cn

[C11] 模块导入与导出
来源：http://rv.521024.cn

Py:   from module import func
来源：http://ma.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ww.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bu.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xv.panjiajie.cn

Java: import java.util.List;
来源：http://sd.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ic.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://th.colortex.cn

C#:   using System.Text;
来源：http://oc.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://al.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://ff.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://wm.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://mj.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://zw.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dd.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://lm.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://rd.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ke.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://lm.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rg.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://au.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ry.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yc.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ou.asd995.cn

Go:   func add(a, b int) int
来源：http://sa.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zr.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rs.jctech888.com.cn

[C14] 泛型函数
来源：http://uw.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rs.chemitech.net.cn

PHP:  // 无泛型
来源：http://fd.huixiangedu.cn

JS:   // 无泛型
来源：http://gm.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nj.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ro.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nz.lnxyls.cn

Ruby: # 无泛型
来源：http://ub.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://co.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://rb.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xr.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://vp.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hl.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qw.9csxet.cn

Java: // 无解构
来源：http://ns.yuntaijiaju.cn

Go:   // 无解构
来源：http://ua.yuexingan06.cn

Ruby: a, b = pair
来源：http://pf.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://ur.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://qv.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dh.huixinmuqiang.cn

PHP:  // 无重载
来源：http://iz.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://no.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://qd.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gj.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://ih.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://cs.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aa.521024.cn

================================================================================
来源：http://kk.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://if.shxzskj.cn

================================================================================
来源：http://ta.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://fe.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ha.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zr.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lj.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tf.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vj.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://cu.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://iy.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zj.newstarts.cn

[D02] 追加元素到末尾
来源：http://zb.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rw.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wg.gzmigu.cn

JS:   arr.push(4);
来源：http://ol.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://sw.lnxyls.cn

Java: list.add(4);
来源：http://vp.asd995.cn

Go:   arr = append(arr, 4)
来源：http://rc.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://wq.hnjuh.cn

C#:   list.Add(4);
来源：http://br.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://rs.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://vl.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pp.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://km.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://mv.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://fc.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ll.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yf.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://ev.newstarts.cn

[D04] 删除元素
来源：http://uz.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sa.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fy.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oy.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://jg.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zb.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ee.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pa.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qh.szxytkj.cn

[D05] 访问与修改元素
来源：http://nl.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eh.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ls.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ho.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://lf.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://zq.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://hu.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gs.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qf.hahajie.cn

[D06] 数组长度
来源：http://uq.chemitech.net.cn

Py:   len(arr)
来源：http://fw.bjjhwx.cn

PHP:  count($arr);
来源：http://os.hnjuh.cn

JS:   arr.length
来源：http://zc.nszjky.cn

TS:   arr.length
来源：http://ki.asd995.cn

Java: list.size();
来源：http://xc.yuntaijiaju.cn

Go:   len(arr)
来源：http://ks.521024.cn

Ruby: arr.length; arr.size
来源：http://wr.hnjuh.cn

C#:   list.Count;
来源：http://xz.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://tv.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hd.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mk.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://kd.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://bg.panjiajie.cn

Java: list.subList(1, 4);
来源：http://uf.huanxung.cn

Go:   arr[1:4]
来源：http://bp.szsharing.cn

Ruby: arr[1, 3]
来源：http://fs.wgjwhj.cn


<!-- 参考信息 -->