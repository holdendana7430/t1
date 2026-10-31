代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://ps.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://di.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://nk.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://uo.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qy.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://or.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://bv.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://dx.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://bu.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kj.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://cr.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://in.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://hc.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sy.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rb.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://xn.9csxet.cn

[B09] break 与 continue
来源：http://ax.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rj.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ad.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gq.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iz.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jn.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hb.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xy.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dv.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://ed.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bb.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sq.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://br.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ml.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tj.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sh.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tk.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qk.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://zg.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://wg.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://ai.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ib.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bh.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rc.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cm.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://jd.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vh.gzmigu.cn

[B12] 跳出多层循环
来源：http://qt.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ck.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lu.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cx.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ev.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ce.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gn.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://do.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lf.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://vv.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://cn.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://nv.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rk.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://in.shxzukj.cn

Java: x instanceof Number
来源：http://ru.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nf.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://jq.hnjuh.cn

C#:   x is int or double or decimal
来源：http://ej.9csxet.cn

[B14] 判断值是否在集合内
来源：http://hq.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tv.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ir.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://lb.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://uv.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ht.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ol.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lf.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://im.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://eu.huixiangedu.cn

Py:   a and b or not c
来源：http://qu.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://bt.shtwfgs.cn

JS:   a && b || !c
来源：http://mt.muxihuayi.cn

TS:   a && b || !c
来源：http://yc.colortex.cn

Java: a && b || !c
来源：http://vp.shtwfgs.cn

Go:   a && b || !c
来源：http://ww.chemitech.net.cn

Ruby: a && b || !c
来源：http://zx.nicolike.cn

C#:   a && b || !c
来源：http://gt.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yh.shtwfgs.cn

Py:   if not data: return
来源：http://mc.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://ga.szxytkj.cn

JS:   if (!data) return;
来源：http://uc.panjiajie.cn

TS:   if (!data) return;
来源：http://fq.haigaiapp.cn

Java: if (data == null) return;
来源：http://qg.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://sd.wgjwhj.cn

Ruby: return if data.nil?
来源：http://bi.chemitech.net.cn

C#:   if (data == null) return;
来源：http://kv.521024.cn

================================================================================
来源：http://qu.gzmigu.cn

C. 函数与作用域
来源：http://mo.jctech888.com.cn

================================================================================
来源：http://id.colortex.cn

[C01] 定义函数
来源：http://za.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://sw.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fy.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://kl.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lg.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zd.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iq.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://cg.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://av.shtwfgs.cn

[C02] 默认参数
来源：http://pq.521024.cn

Py:   def greet(name="World"): return name
来源：http://ja.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wj.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://gt.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hp.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ky.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xh.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://gq.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://yr.gzmigu.cn

[C03] 可变参数
来源：http://pu.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://id.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cq.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vq.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jv.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qs.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rr.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nx.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ko.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://dh.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ut.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sa.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sj.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ye.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://me.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://wl.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://mb.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://po.huixiangedu.cn

[C05] 返回多个值
来源：http://ro.asd995.cn

Py:   return a, b
来源：http://vo.huanxung.cn

PHP:  return [$a, $b];
来源：http://fo.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zc.hahajie.cn

TS:   return { a, b };
来源：http://nw.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bn.hahajie.cn

Go:   return a, b
来源：http://oa.panjiajie.cn

Ruby: return a, b
来源：http://hh.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://xj.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://zq.huanxung.cn

Py:   square = lambda x: x * x
来源：http://oa.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://st.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://gf.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://pw.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wz.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cv.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://kl.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ry.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://qu.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://av.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xr.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pf.panjiajie.cn

TS:   arr.map(String)
来源：http://ba.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://um.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gh.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://cb.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://to.szsharing.cn

[C08] 闭包
来源：http://kr.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eu.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fz.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ce.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ba.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sd.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dk.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ww.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ld.wgjwhj.cn

[C09] 递归
来源：http://oc.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ku.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://co.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iz.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ue.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uu.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ib.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lz.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kj.jianghongdianzi.cn

[C10] 变量作用域
来源：http://rc.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xh.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vx.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ce.bookmarksfly.cn

TS:   同 JS
来源：http://nk.shxzskj.cn

Java: 方法内为块级作用域
来源：http://qy.huixiangedu.cn

Go:   花括号块级作用域
来源：http://bo.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oy.gzmigu.cn

C#:   块级作用域
来源：http://gq.shtwfgs.cn

[C11] 模块导入与导出
来源：http://ku.huixinmuqiang.cn

Py:   from module import func
来源：http://cm.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ur.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fs.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yi.bookmarksfly.cn

Java: import java.util.List;
来源：http://an.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sg.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://kx.haigaiapp.cn

C#:   using System.Text;
来源：http://bx.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://wb.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://qn.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://yj.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://ln.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://vz.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jc.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://do.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://nm.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fz.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://co.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wr.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pr.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ce.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://by.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lg.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://kh.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tw.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ir.huixiangedu.cn

[C14] 泛型函数
来源：http://yl.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oa.muxihuayi.cn

PHP:  // 无泛型
来源：http://ty.szsharing.cn

JS:   // 无泛型
来源：http://cm.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ac.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aa.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cf.jctech888.com.cn

Ruby: # 无泛型
来源：http://vu.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gg.nszjky.cn

[C15] 解构 / 展开参数
来源：http://xy.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yn.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://ld.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bg.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lv.bookmarksfly.cn

Java: // 无解构
来源：http://qc.yuexingan06.cn

Go:   // 无解构
来源：http://hd.bookmarksfly.cn

Ruby: a, b = pair
来源：http://nx.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://gn.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://qa.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yq.nszjky.cn

PHP:  // 无重载
来源：http://xx.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wp.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://hm.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ts.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://wu.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://dw.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pt.huixiangedu.cn

================================================================================
来源：http://me.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://en.szxytkj.cn

================================================================================
来源：http://pw.szsharing.cn

[D01] 创建数组 / 列表
来源：http://fj.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ka.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ez.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ux.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cn.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cr.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://pu.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://wz.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rw.panjiajie.cn

[D02] 追加元素到末尾
来源：http://or.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ak.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gl.gzmigu.cn

JS:   arr.push(4);
来源：http://kq.panjiajie.cn

TS:   arr.push(4);
来源：http://za.gzmigu.cn

Java: list.add(4);
来源：http://re.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://lg.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://gb.muxihuayi.cn

C#:   list.Add(4);
来源：http://zn.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://ov.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://kk.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lg.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yt.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://py.lnxyls.cn

Java: list.add(0, 0);
来源：http://yj.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://in.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qy.asd995.cn

C#:   list.Insert(0, 0);
来源：http://mb.521024.cn

[D04] 删除元素
来源：http://zw.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://os.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bm.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hu.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://et.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kt.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gc.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sq.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sn.chemitech.net.cn

[D05] 访问与修改元素
来源：http://mw.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lr.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vv.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ge.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://ou.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://lm.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://jv.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pt.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ux.huixinmuqiang.cn

[D06] 数组长度
来源：http://ot.nszjky.cn

Py:   len(arr)
来源：http://dx.shxzskj.cn

PHP:  count($arr);
来源：http://es.wgjwhj.cn

JS:   arr.length
来源：http://yy.shxzskj.cn

TS:   arr.length
来源：http://jh.gzmigu.cn

Java: list.size();
来源：http://jg.9csxet.cn

Go:   len(arr)
来源：http://ce.szsharing.cn

Ruby: arr.length; arr.size
来源：http://nr.huixiangedu.cn

C#:   list.Count;
来源：http://xy.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://td.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cq.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nx.colortex.cn

JS:   arr.slice(1, 4);
来源：http://ls.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://jl.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://py.panjiajie.cn

Go:   arr[1:4]
来源：http://zr.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://hl.yuexingan06.cn


<!-- 参考信息 -->