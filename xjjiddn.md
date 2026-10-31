代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://id.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://rz.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://yh.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://ef.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://fy.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bv.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://tk.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://xd.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://jh.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tl.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://is.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://aw.shxzukj.cn

[B09] break 与 continue
来源：http://vt.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://du.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fu.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mt.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gs.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xf.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cx.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fk.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://gc.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xe.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jg.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yf.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ob.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jx.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gr.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lk.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xv.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://og.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://jp.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://jz.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dd.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pi.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xq.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ka.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://yd.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gs.szsharing.cn

[B12] 跳出多层循环
来源：http://bu.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pp.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tq.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ka.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qv.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wf.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://th.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ig.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yb.muxihuayi.cn

[B13] 判断是否为数字
来源：http://ao.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://bc.hnjuh.cn

PHP:  is_numeric($x)
来源：http://ya.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kw.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vz.hahajie.cn

Java: x instanceof Number
来源：http://ee.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ac.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://lf.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ut.nszjky.cn

[B14] 判断值是否在集合内
来源：http://sb.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fn.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jl.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ga.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://aa.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ev.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bc.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wu.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uq.hnjuh.cn

[B15] 布尔运算与取反
来源：http://tc.hahajie.cn

Py:   a and b or not c
来源：http://ah.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://ew.yuntaijiaju.cn

JS:   a && b || !c
来源：http://ss.jctech888.com.cn

TS:   a && b || !c
来源：http://vw.nszjky.cn

Java: a && b || !c
来源：http://si.chemitech.net.cn

Go:   a && b || !c
来源：http://fc.nszjky.cn

Ruby: a && b || !c
来源：http://bb.hahajie.cn

C#:   a && b || !c
来源：http://pc.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qz.newstarts.cn

Py:   if not data: return
来源：http://xk.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ge.bookmarksfly.cn

JS:   if (!data) return;
来源：http://lr.gzmigu.cn

TS:   if (!data) return;
来源：http://pu.nszjky.cn

Java: if (data == null) return;
来源：http://rc.shtwfgs.cn

Go:   if data == nil { return }
来源：http://bg.jctech888.com.cn

Ruby: return if data.nil?
来源：http://rt.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://gj.bjjhwx.cn

================================================================================
来源：http://jy.newstarts.cn

C. 函数与作用域
来源：http://fe.huixinmuqiang.cn

================================================================================
来源：http://cy.huixinmuqiang.cn

[C01] 定义函数
来源：http://ru.asd995.cn

Py:   def add(a, b): return a + b
来源：http://te.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fw.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://cl.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qp.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jc.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ez.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://cu.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qr.bjjhwx.cn

[C02] 默认参数
来源：http://ld.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://na.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vg.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://hg.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kg.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mw.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rp.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://ba.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://jc.9csxet.cn

[C03] 可变参数
来源：http://ba.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://do.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iv.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lh.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://is.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ri.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ui.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yy.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qz.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://ey.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ba.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kg.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iu.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mz.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://ij.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://jw.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://vo.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://ej.asd995.cn

[C05] 返回多个值
来源：http://bf.9csxet.cn

Py:   return a, b
来源：http://lp.shxzskj.cn

PHP:  return [$a, $b];
来源：http://ez.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ke.muxihuayi.cn

TS:   return { a, b };
来源：http://oo.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bp.bookmarksfly.cn

Go:   return a, b
来源：http://hp.shxzukj.cn

Ruby: return a, b
来源：http://ss.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://bg.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://ue.nicolike.cn

Py:   square = lambda x: x * x
来源：http://fi.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://er.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://wn.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://mw.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ae.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://px.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://dq.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://na.colortex.cn

[C07] 把函数作为参数传入
来源：http://no.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rn.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rj.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ab.jctech888.com.cn

TS:   arr.map(String)
来源：http://au.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://am.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fg.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://kc.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dz.newstarts.cn

[C08] 闭包
来源：http://xb.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jf.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mt.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jp.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rf.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tv.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ts.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bd.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bf.shxzukj.cn

[C09] 递归
来源：http://bn.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rh.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vd.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fl.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://in.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fq.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lr.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bz.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fg.panjiajie.cn

[C10] 变量作用域
来源：http://oi.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://um.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yz.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vu.yuexingan06.cn

TS:   同 JS
来源：http://kw.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://ep.yuexingan06.cn

Go:   花括号块级作用域
来源：http://cu.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kz.colortex.cn

C#:   块级作用域
来源：http://is.9csxet.cn

[C11] 模块导入与导出
来源：http://ws.521024.cn

Py:   from module import func
来源：http://va.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rh.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gy.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ut.huixiangedu.cn

Java: import java.util.List;
来源：http://xw.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qw.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://bb.muxihuayi.cn

C#:   using System.Text;
来源：http://ru.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://gm.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://nc.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://yc.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://lp.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://fu.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wl.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://gh.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://fd.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ot.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://oy.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qb.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xa.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ui.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gu.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qn.hnjuh.cn

Go:   func add(a, b int) int
来源：http://ex.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://si.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yi.lnxyls.cn

[C14] 泛型函数
来源：http://oj.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ej.shxzskj.cn

PHP:  // 无泛型
来源：http://ud.haigaiapp.cn

JS:   // 无泛型
来源：http://tp.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hn.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://re.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kg.colortex.cn

Ruby: # 无泛型
来源：http://er.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qd.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://lo.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zz.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://bb.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ah.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://da.9csxet.cn

Java: // 无解构
来源：http://wr.521024.cn

Go:   // 无解构
来源：http://tu.haigaiapp.cn

Ruby: a, b = pair
来源：http://yt.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://ae.colortex.cn

[C16] 函数 / 方法重载
来源：http://dw.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vy.9csxet.cn

PHP:  // 无重载
来源：http://dd.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://os.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://cv.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cx.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://vm.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://oy.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jg.panjiajie.cn

================================================================================
来源：http://va.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://cw.bjjhwx.cn

================================================================================
来源：http://cb.szsharing.cn

[D01] 创建数组 / 列表
来源：http://lh.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ir.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fx.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uz.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://di.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pa.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://vg.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://qp.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qq.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://ys.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wi.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qg.shxzukj.cn

JS:   arr.push(4);
来源：http://pp.huanxung.cn

TS:   arr.push(4);
来源：http://xa.colortex.cn

Java: list.add(4);
来源：http://tb.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://vn.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://hx.muxihuayi.cn

C#:   list.Add(4);
来源：http://pu.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://yo.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://tm.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ni.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rk.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://tz.bjjhwx.cn

Java: list.add(0, 0);
来源：http://nu.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hz.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ao.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://cr.colortex.cn

[D04] 删除元素
来源：http://gr.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fx.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qn.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cx.521024.cn

TS:   arr.splice(0, 1);
来源：http://si.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fn.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ed.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hq.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ga.jctech888.com.cn

[D05] 访问与修改元素
来源：http://be.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ln.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://af.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jx.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://dp.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://fq.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://ao.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gv.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xx.huixiangedu.cn

[D06] 数组长度
来源：http://ce.huixinmuqiang.cn

Py:   len(arr)
来源：http://io.bjjhwx.cn

PHP:  count($arr);
来源：http://dg.huixinmuqiang.cn

JS:   arr.length
来源：http://aa.colortex.cn

TS:   arr.length
来源：http://aa.hahajie.cn

Java: list.size();
来源：http://aj.shxzskj.cn

Go:   len(arr)
来源：http://nj.nicolike.cn

Ruby: arr.length; arr.size
来源：http://sd.gzmigu.cn

C#:   list.Count;
来源：http://dj.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://cf.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jq.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pc.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://ge.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://qk.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://wd.hnjuh.cn

Go:   arr[1:4]
来源：http://ij.newstarts.cn

Ruby: arr[1, 3]
来源：http://ii.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://lr.9csxet.cn

[D08] 合并两个数组
来源：http://oa.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://zy.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://ad.haigaiapp.cn


<!-- 参考信息 -->