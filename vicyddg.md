代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://gd.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://do.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://hz.colortex.cn

Java: while (i < 10) { i++; }
来源：http://uo.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qk.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://bq.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://uf.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://kp.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://my.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uj.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://xv.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://yb.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://my.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tw.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rp.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://rp.shxzskj.cn

[B09] break 与 continue
来源：http://kg.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fo.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fd.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jp.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zi.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uu.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mr.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://er.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://mf.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ve.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nv.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://to.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://br.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fp.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://la.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gs.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dy.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://mp.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://ld.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://dx.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yh.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zi.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xk.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iq.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://fm.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hn.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ag.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bw.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://co.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oe.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ej.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rj.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kg.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wd.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ed.asd995.cn

[B13] 判断是否为数字
来源：http://xd.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://np.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://vf.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ah.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ug.nicolike.cn

Java: x instanceof Number
来源：http://sy.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vb.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://fx.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://cp.huanxung.cn

[B14] 判断值是否在集合内
来源：http://pm.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jt.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://om.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://iv.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://vr.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ck.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cw.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eg.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vi.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://wd.bjjhwx.cn

Py:   a and b or not c
来源：http://do.hahajie.cn

PHP:  $a && $b || !$c
来源：http://og.shxzskj.cn

JS:   a && b || !c
来源：http://sp.9csxet.cn

TS:   a && b || !c
来源：http://fm.hnjuh.cn

Java: a && b || !c
来源：http://zf.yuntaijiaju.cn

Go:   a && b || !c
来源：http://rv.nicolike.cn

Ruby: a && b || !c
来源：http://ae.wgjwhj.cn

C#:   a && b || !c
来源：http://ow.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ir.jctech888.com.cn

Py:   if not data: return
来源：http://zf.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://ty.wgjwhj.cn

JS:   if (!data) return;
来源：http://dm.hnjuh.cn

TS:   if (!data) return;
来源：http://vt.jctech888.com.cn

Java: if (data == null) return;
来源：http://jc.colortex.cn

Go:   if data == nil { return }
来源：http://qo.nicolike.cn

Ruby: return if data.nil?
来源：http://nx.nszjky.cn

C#:   if (data == null) return;
来源：http://mg.hahajie.cn

================================================================================
来源：http://ax.bjjhwx.cn

C. 函数与作用域
来源：http://bp.jctech888.com.cn

================================================================================
来源：http://ot.9csxet.cn

[C01] 定义函数
来源：http://px.521024.cn

Py:   def add(a, b): return a + b
来源：http://il.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jh.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://cn.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ug.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xp.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tc.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://ap.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://za.shxzskj.cn

[C02] 默认参数
来源：http://aw.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://ee.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vp.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://qo.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kv.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tq.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fo.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://ie.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://dx.jianghongdianzi.cn

[C03] 可变参数
来源：http://zv.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://zy.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wf.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mk.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fi.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oe.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hw.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ff.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sq.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://bt.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cy.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ta.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ue.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rv.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://yu.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://zy.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://wn.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://lv.yuntaijiaju.cn

[C05] 返回多个值
来源：http://wk.haigaiapp.cn

Py:   return a, b
来源：http://ui.shxzskj.cn

PHP:  return [$a, $b];
来源：http://wl.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ls.jctech888.com.cn

TS:   return { a, b };
来源：http://dz.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zl.muxihuayi.cn

Go:   return a, b
来源：http://sd.yuntaijiaju.cn

Ruby: return a, b
来源：http://fk.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://ez.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://gr.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://hs.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nf.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://ve.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://jq.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zj.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bc.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://ka.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zn.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://oh.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sl.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jj.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jv.shxzukj.cn

TS:   arr.map(String)
来源：http://zx.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bi.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sb.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://cw.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nm.nszjky.cn

[C08] 闭包
来源：http://ci.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tg.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xx.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kv.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ka.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ie.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ni.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://km.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://am.newstarts.cn

[C09] 递归
来源：http://cs.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rn.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mi.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kq.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pg.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ch.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kg.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cw.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ue.lnxyls.cn

[C10] 变量作用域
来源：http://vz.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rf.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sz.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sv.asd995.cn

TS:   同 JS
来源：http://wb.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ob.hahajie.cn

Go:   花括号块级作用域
来源：http://pn.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ns.bjjhwx.cn

C#:   块级作用域
来源：http://cd.bjjhwx.cn

[C11] 模块导入与导出
来源：http://mo.huixiangedu.cn

Py:   from module import func
来源：http://cx.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ih.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nz.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gc.colortex.cn

Java: import java.util.List;
来源：http://fn.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ya.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://mp.jctech888.com.cn

C#:   using System.Text;
来源：http://kn.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://mb.colortex.cn

Py:   (lambda: print("run"))()
来源：http://yu.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://rg.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://jr.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://sv.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fe.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://ka.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://ic.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cq.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://dv.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iv.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ah.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aw.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eu.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://il.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://vl.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kt.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zt.asd995.cn

[C14] 泛型函数
来源：http://fs.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xq.nszjky.cn

PHP:  // 无泛型
来源：http://me.newstarts.cn

JS:   // 无泛型
来源：http://rd.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sa.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yj.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://um.shxzukj.cn

Ruby: # 无泛型
来源：http://in.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fw.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://tl.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nf.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://cz.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ro.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ne.huanxung.cn

Java: // 无解构
来源：http://tx.szsharing.cn

Go:   // 无解构
来源：http://qh.szxytkj.cn

Ruby: a, b = pair
来源：http://do.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://al.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://cy.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rf.hnjuh.cn

PHP:  // 无重载
来源：http://gh.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bl.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://fk.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cc.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://xx.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://ec.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ls.newstarts.cn

================================================================================
来源：http://oh.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://mm.shxzskj.cn

================================================================================
来源：http://if.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://lm.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://at.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qe.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pn.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://em.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hr.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://nz.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://ev.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fu.asd995.cn

[D02] 追加元素到末尾
来源：http://lb.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://th.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ka.newstarts.cn

JS:   arr.push(4);
来源：http://hs.szxytkj.cn

TS:   arr.push(4);
来源：http://dq.muxihuayi.cn

Java: list.add(4);
来源：http://jh.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://xh.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://cz.jctech888.com.cn

C#:   list.Add(4);
来源：http://xm.nszjky.cn

[D03] 在指定位置插入元素
来源：http://yj.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://sy.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nw.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vf.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://am.hnjuh.cn

Java: list.add(0, 0);
来源：http://jw.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yx.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cl.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://ix.shxzukj.cn

[D04] 删除元素
来源：http://ge.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ov.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sl.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://qi.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pq.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ir.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bj.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jh.szxytkj.cn

[D05] 访问与修改元素
来源：http://ns.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zc.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yp.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fo.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://zt.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://ur.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://bs.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gd.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pj.gzmigu.cn

[D06] 数组长度
来源：http://um.521024.cn

Py:   len(arr)
来源：http://wm.huixinmuqiang.cn

PHP:  count($arr);
来源：http://rp.bjjhwx.cn

JS:   arr.length
来源：http://be.huixiangedu.cn

TS:   arr.length
来源：http://ih.jianghongdianzi.cn

Java: list.size();
来源：http://vd.huixinmuqiang.cn

Go:   len(arr)
来源：http://uu.szsharing.cn

Ruby: arr.length; arr.size
来源：http://wm.newstarts.cn

C#:   list.Count;
来源：http://jx.szsharing.cn

[D07] 切片 / 取子数组
来源：http://oe.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cc.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://va.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://ut.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://xc.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://hk.muxihuayi.cn

Go:   arr[1:4]
来源：http://zf.shxzukj.cn

Ruby: arr[1, 3]
来源：http://yl.nicolike.cn


<!-- 参考信息 -->