代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://tb.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://dg.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://yv.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://ps.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fo.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://vo.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://ed.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://fu.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://al.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zy.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://mb.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://qu.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://fy.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uj.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hk.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://fe.bjjhwx.cn

[B09] break 与 continue
来源：http://ps.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sy.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://br.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://og.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qb.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://if.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wl.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vd.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vx.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://vr.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tp.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lp.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tp.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lx.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vc.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xp.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jq.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pa.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://cy.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://nj.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://ne.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tw.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ew.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qa.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://we.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://vx.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kn.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://lk.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cd.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cc.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://db.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wt.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ta.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ns.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fi.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pn.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://rv.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://ch.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://pw.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kn.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ia.shtwfgs.cn

Java: x instanceof Number
来源：http://wy.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vs.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://cu.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://mv.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://dy.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iu.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://um.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://te.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://jc.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nc.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vd.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bb.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vh.hnjuh.cn

[B15] 布尔运算与取反
来源：http://gu.521024.cn

Py:   a and b or not c
来源：http://pe.nicolike.cn

PHP:  $a && $b || !$c
来源：http://rh.521024.cn

JS:   a && b || !c
来源：http://kb.yuexingan06.cn

TS:   a && b || !c
来源：http://ko.newstarts.cn

Java: a && b || !c
来源：http://ci.shxzukj.cn

Go:   a && b || !c
来源：http://es.shxzukj.cn

Ruby: a && b || !c
来源：http://tb.huixinmuqiang.cn

C#:   a && b || !c
来源：http://ka.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tz.bjjhwx.cn

Py:   if not data: return
来源：http://ey.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://sr.nicolike.cn

JS:   if (!data) return;
来源：http://yn.nicolike.cn

TS:   if (!data) return;
来源：http://zh.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://vx.szxytkj.cn

Go:   if data == nil { return }
来源：http://ee.shxzukj.cn

Ruby: return if data.nil?
来源：http://uw.shtwfgs.cn

C#:   if (data == null) return;
来源：http://hf.colortex.cn

================================================================================
来源：http://kp.hahajie.cn

C. 函数与作用域
来源：http://cj.nszjky.cn

================================================================================
来源：http://qn.yuexingan06.cn

[C01] 定义函数
来源：http://hi.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://fh.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jt.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://bo.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zl.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ph.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qa.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://xm.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ga.jianghongdianzi.cn

[C02] 默认参数
来源：http://qe.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://ud.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ht.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://vc.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dv.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ab.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rl.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://ad.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://zw.asd995.cn

[C03] 可变参数
来源：http://jq.521024.cn

Py:   def total(*args): return sum(args)
来源：http://ln.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ow.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://re.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pv.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vp.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sc.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qf.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://th.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://tk.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aw.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rb.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nu.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ma.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://lm.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://um.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://dl.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://yp.huixinmuqiang.cn

[C05] 返回多个值
来源：http://re.asd995.cn

Py:   return a, b
来源：http://in.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://pn.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ii.shxzskj.cn

TS:   return { a, b };
来源：http://cg.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hb.bjjhwx.cn

Go:   return a, b
来源：http://dz.asd995.cn

Ruby: return a, b
来源：http://ai.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://jt.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://ib.521024.cn

Py:   square = lambda x: x * x
来源：http://xz.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hh.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://nr.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ou.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bx.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lw.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://wl.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pd.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://jf.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ch.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ys.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bi.hahajie.cn

TS:   arr.map(String)
来源：http://ym.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wr.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wo.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://yb.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qi.colortex.cn

[C08] 闭包
来源：http://hd.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://me.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eb.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cs.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jr.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xp.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jk.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ol.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mk.hnjuh.cn

[C09] 递归
来源：http://df.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qn.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vh.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ko.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sd.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ga.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gv.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lw.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gb.gzmigu.cn

[C10] 变量作用域
来源：http://lw.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wl.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cf.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kv.huanxung.cn

TS:   同 JS
来源：http://ef.lnxyls.cn

Java: 方法内为块级作用域
来源：http://ct.jctech888.com.cn

Go:   花括号块级作用域
来源：http://tu.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hv.9csxet.cn

C#:   块级作用域
来源：http://sa.huixiangedu.cn

[C11] 模块导入与导出
来源：http://oh.panjiajie.cn

Py:   from module import func
来源：http://sk.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qj.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ct.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zr.muxihuayi.cn

Java: import java.util.List;
来源：http://qs.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jj.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://bf.panjiajie.cn

C#:   using System.Text;
来源：http://ke.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://rv.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://tc.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://rl.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://yj.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://lc.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://au.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://xs.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://ci.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wa.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://fp.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ja.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ik.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uv.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gy.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lp.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://jw.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zs.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sw.muxihuayi.cn

[C14] 泛型函数
来源：http://xo.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gg.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://tu.colortex.cn

JS:   // 无泛型
来源：http://jz.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cs.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ao.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ua.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://my.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vx.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://dh.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ly.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://oz.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qt.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gf.newstarts.cn

Java: // 无解构
来源：http://xf.hahajie.cn

Go:   // 无解构
来源：http://sr.521024.cn

Ruby: a, b = pair
来源：http://jh.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://cb.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://ha.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nk.nszjky.cn

PHP:  // 无重载
来源：http://gi.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xh.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://mm.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tu.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://ua.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://mv.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iw.szsharing.cn

================================================================================
来源：http://nu.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://ie.huixiangedu.cn

================================================================================
来源：http://ir.9csxet.cn

[D01] 创建数组 / 列表
来源：http://pb.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gt.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ir.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mf.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://re.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vx.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://mf.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://zh.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fc.521024.cn

[D02] 追加元素到末尾
来源：http://rm.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lu.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://th.wgjwhj.cn

JS:   arr.push(4);
来源：http://oo.huanxung.cn

TS:   arr.push(4);
来源：http://bh.huanxung.cn

Java: list.add(4);
来源：http://fi.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://uh.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://oj.panjiajie.cn

C#:   list.Add(4);
来源：http://jd.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://lz.colortex.cn

Py:   arr.insert(0, 0)
来源：http://ck.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://je.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://os.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://dd.hahajie.cn

Java: list.add(0, 0);
来源：http://wm.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ef.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tj.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://hs.shxzukj.cn

[D04] 删除元素
来源：http://lk.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ue.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kz.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uc.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://ud.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mz.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ft.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yp.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://br.chemitech.net.cn

[D05] 访问与修改元素
来源：http://fs.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nj.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mj.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gm.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://cn.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://ia.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://lm.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wb.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oq.szsharing.cn

[D06] 数组长度
来源：http://ox.szxytkj.cn

Py:   len(arr)
来源：http://tg.shxzskj.cn

PHP:  count($arr);
来源：http://er.muxihuayi.cn

JS:   arr.length
来源：http://bg.jianghongdianzi.cn

TS:   arr.length
来源：http://jm.huixiangedu.cn

Java: list.size();
来源：http://wr.shxzskj.cn

Go:   len(arr)
来源：http://na.521024.cn

Ruby: arr.length; arr.size
来源：http://bi.yuntaijiaju.cn

C#:   list.Count;
来源：http://rr.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://mv.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oq.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ju.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://rg.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://hx.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://px.bookmarksfly.cn

Go:   arr[1:4]
来源：http://gw.newstarts.cn

Ruby: arr[1, 3]
来源：http://so.huixiangedu.cn


<!-- 参考信息 -->