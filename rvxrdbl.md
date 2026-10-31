代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yo.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://sx.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://du.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://py.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://xj.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gn.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://ga.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://fy.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://px.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ux.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wv.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://uc.shxzukj.cn

[B09] break 与 continue
来源：http://mz.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://up.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://io.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pn.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zo.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qc.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://et.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hh.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://ku.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ig.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wb.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ui.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ay.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://co.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pb.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jv.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sx.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://ff.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://mv.colortex.cn

PHP:  range(0, 10, 2);
来源：http://zg.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fk.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ii.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gc.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ls.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://ya.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kg.chemitech.net.cn

[B12] 跳出多层循环
来源：http://xp.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sc.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hc.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://le.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bx.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eu.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://km.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ob.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zp.gzmigu.cn

[B13] 判断是否为数字
来源：http://tn.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://du.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://wq.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iz.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ci.huanxung.cn

Java: x instanceof Number
来源：http://mn.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pm.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://la.colortex.cn

C#:   x is int or double or decimal
来源：http://pw.szsharing.cn

[B14] 判断值是否在集合内
来源：http://dk.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fr.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vv.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://oh.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://hv.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cm.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dk.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lw.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ea.hnjuh.cn

[B15] 布尔运算与取反
来源：http://wo.nicolike.cn

Py:   a and b or not c
来源：http://oc.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://gn.hahajie.cn

JS:   a && b || !c
来源：http://ac.shxzskj.cn

TS:   a && b || !c
来源：http://sv.wgjwhj.cn

Java: a && b || !c
来源：http://te.huanxung.cn

Go:   a && b || !c
来源：http://uv.muxihuayi.cn

Ruby: a && b || !c
来源：http://fb.lnxyls.cn

C#:   a && b || !c
来源：http://en.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sf.yuntaijiaju.cn

Py:   if not data: return
来源：http://kf.521024.cn

PHP:  if (!$data) { return; }
来源：http://zm.hahajie.cn

JS:   if (!data) return;
来源：http://sd.521024.cn

TS:   if (!data) return;
来源：http://ec.huixiangedu.cn

Java: if (data == null) return;
来源：http://gr.shxzskj.cn

Go:   if data == nil { return }
来源：http://ox.haigaiapp.cn

Ruby: return if data.nil?
来源：http://qi.bjjhwx.cn

C#:   if (data == null) return;
来源：http://lz.colortex.cn

================================================================================
来源：http://uf.chemitech.net.cn

C. 函数与作用域
来源：http://yv.muxihuayi.cn

================================================================================
来源：http://fl.yuexingan06.cn

[C01] 定义函数
来源：http://bl.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://xl.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://re.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://vz.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rv.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pc.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rm.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://yb.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qt.chemitech.net.cn

[C02] 默认参数
来源：http://qg.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://fz.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mo.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://jb.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bj.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cs.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xy.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://uo.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://aq.hnjuh.cn

[C03] 可变参数
来源：http://nv.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://ym.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cp.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sc.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ky.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tk.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bt.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oj.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ds.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://cu.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xp.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ra.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yj.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://za.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://je.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://dj.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://hl.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://uh.newstarts.cn

[C05] 返回多个值
来源：http://ue.nszjky.cn

Py:   return a, b
来源：http://qo.lnxyls.cn

PHP:  return [$a, $b];
来源：http://ip.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nw.hahajie.cn

TS:   return { a, b };
来源：http://jo.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oe.521024.cn

Go:   return a, b
来源：http://kk.nszjky.cn

Ruby: return a, b
来源：http://al.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://im.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://oj.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://dr.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uw.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://uj.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://dd.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://je.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hb.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://kl.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fi.nicolike.cn

[C07] 把函数作为参数传入
来源：http://ew.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bb.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ed.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gb.huixiangedu.cn

TS:   arr.map(String)
来源：http://yl.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wg.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qy.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://yd.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ar.asd995.cn

[C08] 闭包
来源：http://fh.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hv.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rj.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dn.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ib.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ty.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pf.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jo.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ja.bjjhwx.cn

[C09] 递归
来源：http://vi.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xk.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://un.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ar.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ws.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xb.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://le.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xy.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dw.gzmigu.cn

[C10] 变量作用域
来源：http://as.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uo.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ix.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jc.shxzukj.cn

TS:   同 JS
来源：http://mh.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://br.shtwfgs.cn

Go:   花括号块级作用域
来源：http://nv.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ub.jianghongdianzi.cn

C#:   块级作用域
来源：http://zx.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://az.hnjuh.cn

Py:   from module import func
来源：http://uq.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hi.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lp.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mb.huanxung.cn

Java: import java.util.List;
来源：http://ea.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gt.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://ir.yuntaijiaju.cn

C#:   using System.Text;
来源：http://br.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://po.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://dq.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://zy.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://dq.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://qp.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yk.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://bv.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://on.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vv.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://rb.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gp.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vu.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pg.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dv.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://re.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://qp.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pq.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cj.huixinmuqiang.cn

[C14] 泛型函数
来源：http://iq.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vp.521024.cn

PHP:  // 无泛型
来源：http://gu.shxzukj.cn

JS:   // 无泛型
来源：http://te.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gf.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dx.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vo.szxytkj.cn

Ruby: # 无泛型
来源：http://av.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ru.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://jo.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wh.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://fb.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gs.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fn.521024.cn

Java: // 无解构
来源：http://an.521024.cn

Go:   // 无解构
来源：http://bm.newstarts.cn

Ruby: a, b = pair
来源：http://kg.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://cf.hahajie.cn

[C16] 函数 / 方法重载
来源：http://lg.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sx.bookmarksfly.cn

PHP:  // 无重载
来源：http://mt.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vt.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://cp.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ts.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://io.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://qm.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nz.shxzukj.cn

================================================================================
来源：http://ox.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://ln.szsharing.cn

================================================================================
来源：http://nv.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://gi.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yv.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rc.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xw.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nh.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gx.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://ab.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://db.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gw.hahajie.cn

[D02] 追加元素到末尾
来源：http://yb.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sx.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://la.szsharing.cn

JS:   arr.push(4);
来源：http://tt.huixiangedu.cn

TS:   arr.push(4);
来源：http://le.shxzukj.cn

Java: list.add(4);
来源：http://rc.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://wn.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://ax.asd995.cn

C#:   list.Add(4);
来源：http://tl.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://zx.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://uf.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tv.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ol.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://zl.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://lb.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jd.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ja.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://da.jianghongdianzi.cn

[D04] 删除元素
来源：http://gr.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tg.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ro.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qz.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://rl.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rr.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eg.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tj.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fk.panjiajie.cn

[D05] 访问与修改元素
来源：http://ty.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ny.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ce.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ah.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://kk.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ph.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://am.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ed.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ta.huanxung.cn

[D06] 数组长度
来源：http://oy.huixiangedu.cn

Py:   len(arr)
来源：http://bu.colortex.cn

PHP:  count($arr);
来源：http://yn.bookmarksfly.cn

JS:   arr.length
来源：http://qs.muxihuayi.cn

TS:   arr.length
来源：http://te.shtwfgs.cn

Java: list.size();
来源：http://ok.shxzukj.cn

Go:   len(arr)
来源：http://of.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://vy.wgjwhj.cn

C#:   list.Count;
来源：http://jb.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://hl.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nb.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mp.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://ee.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://fa.hnjuh.cn

Java: list.subList(1, 4);
来源：http://ky.colortex.cn

Go:   arr[1:4]
来源：http://co.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://nr.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://id.haigaiapp.cn

[D08] 合并两个数组
来源：http://ua.521024.cn

Py:   a + b;  a.extend(b)
来源：http://sl.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://fk.shxzskj.cn


<!-- 参考信息 -->