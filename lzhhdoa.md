代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://cq.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://qe.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://cn.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://mj.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xc.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://gb.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://hf.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://al.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://tz.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aq.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://kc.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://ja.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://yo.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vz.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ik.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://mv.jctech888.com.cn

[B09] break 与 continue
来源：http://gv.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://at.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ri.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ys.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ka.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qs.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://be.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lj.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rs.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://xk.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ki.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hh.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eh.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nl.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kv.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zs.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lj.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yl.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://sa.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://ho.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://lu.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dg.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rx.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jz.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cb.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://tf.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ky.szxytkj.cn

[B12] 跳出多层循环
来源：http://tr.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://es.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ck.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sk.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ut.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ku.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dt.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ti.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yo.muxihuayi.cn

[B13] 判断是否为数字
来源：http://ld.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://ki.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://wj.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sj.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qz.lnxyls.cn

Java: x instanceof Number
来源：http://cn.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gd.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://vc.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://ev.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://ex.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ej.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ky.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://nq.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://zs.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xu.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ot.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bc.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tg.szsharing.cn

[B15] 布尔运算与取反
来源：http://sq.521024.cn

Py:   a and b or not c
来源：http://li.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://bp.szsharing.cn

JS:   a && b || !c
来源：http://ra.yuntaijiaju.cn

TS:   a && b || !c
来源：http://lw.szsharing.cn

Java: a && b || !c
来源：http://hr.haigaiapp.cn

Go:   a && b || !c
来源：http://dw.newstarts.cn

Ruby: a && b || !c
来源：http://dg.muxihuayi.cn

C#:   a && b || !c
来源：http://mh.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fi.huanxung.cn

Py:   if not data: return
来源：http://jr.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://cd.panjiajie.cn

JS:   if (!data) return;
来源：http://ll.chemitech.net.cn

TS:   if (!data) return;
来源：http://zm.shxzskj.cn

Java: if (data == null) return;
来源：http://vt.shxzskj.cn

Go:   if data == nil { return }
来源：http://fd.panjiajie.cn

Ruby: return if data.nil?
来源：http://oy.hnjuh.cn

C#:   if (data == null) return;
来源：http://yc.yuntaijiaju.cn

================================================================================
来源：http://ng.nicolike.cn

C. 函数与作用域
来源：http://qd.shxzskj.cn

================================================================================
来源：http://lk.hnjuh.cn

[C01] 定义函数
来源：http://zq.asd995.cn

Py:   def add(a, b): return a + b
来源：http://at.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ys.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://gm.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zn.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oo.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://st.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://vp.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eu.szxytkj.cn

[C02] 默认参数
来源：http://xb.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://ct.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mu.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://aw.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://le.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kq.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zu.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://qr.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://hf.shtwfgs.cn

[C03] 可变参数
来源：http://ae.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://nd.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kg.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wi.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aq.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mc.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xf.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xl.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ww.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://st.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dr.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pt.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gi.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cv.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ez.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://or.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://jj.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://jl.yuntaijiaju.cn

[C05] 返回多个值
来源：http://kz.colortex.cn

Py:   return a, b
来源：http://oh.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://rl.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sz.szsharing.cn

TS:   return { a, b };
来源：http://je.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hg.asd995.cn

Go:   return a, b
来源：http://ax.gzmigu.cn

Ruby: return a, b
来源：http://kl.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://kx.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://tt.huanxung.cn

Py:   square = lambda x: x * x
来源：http://ku.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iv.nszjky.cn

JS:   const square = x => x * x;
来源：http://vq.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://su.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wk.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lc.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://ib.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nd.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://yc.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zv.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bc.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fx.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://ir.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ek.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uf.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://rw.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gh.haigaiapp.cn

[C08] 闭包
来源：http://je.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xo.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qx.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zi.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vs.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dp.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nm.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qq.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wm.newstarts.cn

[C09] 递归
来源：http://px.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ea.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pt.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wa.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xa.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wl.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ny.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ey.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vz.huanxung.cn

[C10] 变量作用域
来源：http://oo.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ne.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ed.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cq.nicolike.cn

TS:   同 JS
来源：http://lz.panjiajie.cn

Java: 方法内为块级作用域
来源：http://cj.shtwfgs.cn

Go:   花括号块级作用域
来源：http://ht.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ex.hahajie.cn

C#:   块级作用域
来源：http://vm.jctech888.com.cn

[C11] 模块导入与导出
来源：http://pr.chemitech.net.cn

Py:   from module import func
来源：http://mu.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sf.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kl.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://te.jctech888.com.cn

Java: import java.util.List;
来源：http://fq.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oj.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://xh.szsharing.cn

C#:   using System.Text;
来源：http://tn.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://ex.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://fc.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://vy.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://dg.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://dn.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zn.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://ib.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://yx.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mb.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://cs.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://je.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ql.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yo.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ie.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ux.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://pm.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fd.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://si.hnjuh.cn

[C14] 泛型函数
来源：http://mb.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fe.newstarts.cn

PHP:  // 无泛型
来源：http://vj.nszjky.cn

JS:   // 无泛型
来源：http://ri.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wn.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zr.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bt.9csxet.cn

Ruby: # 无泛型
来源：http://vy.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://op.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://vz.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://px.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://hg.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lq.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jb.newstarts.cn

Java: // 无解构
来源：http://fe.yuexingan06.cn

Go:   // 无解构
来源：http://sc.shxzskj.cn

Ruby: a, b = pair
来源：http://ok.9csxet.cn

C#:   var (a, b) = pair;
来源：http://xq.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://tx.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zk.gzmigu.cn

PHP:  // 无重载
来源：http://fm.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bg.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://pb.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://og.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://ol.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://wl.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ov.hahajie.cn

================================================================================
来源：http://tu.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://kp.muxihuayi.cn

================================================================================
来源：http://zd.huanxung.cn

[D01] 创建数组 / 列表
来源：http://fk.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nz.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jz.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://no.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ld.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lz.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://mf.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://mh.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oi.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://vp.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ao.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sq.yuexingan06.cn

JS:   arr.push(4);
来源：http://xw.huixiangedu.cn

TS:   arr.push(4);
来源：http://gq.nszjky.cn

Java: list.add(4);
来源：http://ah.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://ng.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://tr.nicolike.cn

C#:   list.Add(4);
来源：http://jl.szsharing.cn

[D03] 在指定位置插入元素
来源：http://qb.colortex.cn

Py:   arr.insert(0, 0)
来源：http://ps.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xt.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ky.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://tl.nicolike.cn

Java: list.add(0, 0);
来源：http://td.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cf.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gv.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://yo.panjiajie.cn

[D04] 删除元素
来源：http://wm.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qd.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qf.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hi.asd995.cn

TS:   arr.splice(0, 1);
来源：http://xr.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gk.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ox.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ub.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zc.9csxet.cn

[D05] 访问与修改元素
来源：http://oh.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sw.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lj.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dg.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://st.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://qp.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://tm.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mu.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ds.nszjky.cn

[D06] 数组长度
来源：http://ad.nicolike.cn

Py:   len(arr)
来源：http://wf.colortex.cn

PHP:  count($arr);
来源：http://zg.wgjwhj.cn

JS:   arr.length
来源：http://qh.bookmarksfly.cn

TS:   arr.length
来源：http://up.jctech888.com.cn

Java: list.size();
来源：http://nm.huanxung.cn

Go:   len(arr)
来源：http://ec.521024.cn

Ruby: arr.length; arr.size
来源：http://kp.yuexingan06.cn

C#:   list.Count;
来源：http://pl.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://ew.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dl.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nj.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://eb.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://cu.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://ft.bookmarksfly.cn

Go:   arr[1:4]
来源：http://kg.szxytkj.cn

Ruby: arr[1, 3]
来源：http://cv.haigaiapp.cn


<!-- 参考信息 -->