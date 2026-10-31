代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://ac.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ci.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hr.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://zg.yuexingan06.cn

[B09] break 与 continue
来源：http://xd.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ir.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hr.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ui.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xe.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ye.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iu.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gt.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xo.szsharing.cn

[B10] 遍历同时拿索引
来源：http://jm.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oo.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jb.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rq.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://df.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fo.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://li.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jm.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vq.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://cr.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://bd.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://ao.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wv.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tj.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rn.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://na.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://tg.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qd.nszjky.cn

[B12] 跳出多层循环
来源：http://nl.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cv.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vi.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pu.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://us.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kn.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ep.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sl.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sw.muxihuayi.cn

[B13] 判断是否为数字
来源：http://ba.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://df.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://ty.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pa.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://le.hnjuh.cn

Java: x instanceof Number
来源：http://zn.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cs.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://lg.shxzukj.cn

C#:   x is int or double or decimal
来源：http://bg.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://sj.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dz.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aj.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://zs.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://ox.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wv.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wm.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mq.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dh.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://wl.chemitech.net.cn

Py:   a and b or not c
来源：http://bp.hahajie.cn

PHP:  $a && $b || !$c
来源：http://ax.chemitech.net.cn

JS:   a && b || !c
来源：http://bs.yuexingan06.cn

TS:   a && b || !c
来源：http://da.szsharing.cn

Java: a && b || !c
来源：http://th.shtwfgs.cn

Go:   a && b || !c
来源：http://qp.9csxet.cn

Ruby: a && b || !c
来源：http://dr.shtwfgs.cn

C#:   a && b || !c
来源：http://gg.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ui.szsharing.cn

Py:   if not data: return
来源：http://mv.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://ge.hnjuh.cn

JS:   if (!data) return;
来源：http://vw.nszjky.cn

TS:   if (!data) return;
来源：http://qn.yuexingan06.cn

Java: if (data == null) return;
来源：http://zv.colortex.cn

Go:   if data == nil { return }
来源：http://av.hnjuh.cn

Ruby: return if data.nil?
来源：http://qq.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://vq.9csxet.cn

================================================================================
来源：http://yn.colortex.cn

C. 函数与作用域
来源：http://pt.newstarts.cn

================================================================================
来源：http://aw.bjjhwx.cn

[C01] 定义函数
来源：http://dd.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://wa.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qy.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://mw.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hq.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hj.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vr.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://va.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ib.colortex.cn

[C02] 默认参数
来源：http://ir.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://tx.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bz.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://qu.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pb.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uh.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ov.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://mh.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://js.521024.cn

[C03] 可变参数
来源：http://zx.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://qp.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gm.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oz.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tj.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ug.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ik.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mh.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zd.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://qh.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vm.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nf.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gj.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hm.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://fk.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://pu.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://ps.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://er.chemitech.net.cn

[C05] 返回多个值
来源：http://mi.wgjwhj.cn

Py:   return a, b
来源：http://dc.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://ig.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uv.hahajie.cn

TS:   return { a, b };
来源：http://lc.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nh.shxzukj.cn

Go:   return a, b
来源：http://cf.yuexingan06.cn

Ruby: return a, b
来源：http://vj.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://hh.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://ee.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://bq.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tz.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://xx.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://zu.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yg.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vb.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://ad.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://az.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://jg.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yn.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hp.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lu.szxytkj.cn

TS:   arr.map(String)
来源：http://tv.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tg.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cw.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://gw.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zu.521024.cn

[C08] 闭包
来源：http://bp.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sk.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uh.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tl.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sq.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wd.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ek.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vk.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ay.yuexingan06.cn

[C09] 递归
来源：http://xw.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ld.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ez.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hc.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wh.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hq.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vw.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zx.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cx.bookmarksfly.cn

[C10] 变量作用域
来源：http://xa.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://na.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oa.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tj.bookmarksfly.cn

TS:   同 JS
来源：http://hy.shxzukj.cn

Java: 方法内为块级作用域
来源：http://lj.hahajie.cn

Go:   花括号块级作用域
来源：http://wg.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ju.wgjwhj.cn

C#:   块级作用域
来源：http://xv.jctech888.com.cn

[C11] 模块导入与导出
来源：http://va.haigaiapp.cn

Py:   from module import func
来源：http://zr.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://os.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jt.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jy.panjiajie.cn

Java: import java.util.List;
来源：http://mm.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vu.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://mz.newstarts.cn

C#:   using System.Text;
来源：http://qa.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ef.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://ob.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://er.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://hh.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://nz.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cb.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://zq.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://vk.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fq.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://fd.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ux.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://li.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yw.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ge.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ra.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://rf.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ma.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xw.jctech888.com.cn

[C14] 泛型函数
来源：http://ir.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oc.chemitech.net.cn

PHP:  // 无泛型
来源：http://gq.muxihuayi.cn

JS:   // 无泛型
来源：http://xr.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nr.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yg.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sf.yuexingan06.cn

Ruby: # 无泛型
来源：http://qr.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pr.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://hm.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wd.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://ax.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vu.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xn.bookmarksfly.cn

Java: // 无解构
来源：http://hr.hahajie.cn

Go:   // 无解构
来源：http://hh.lnxyls.cn

Ruby: a, b = pair
来源：http://qk.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://cq.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://ts.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sz.panjiajie.cn

PHP:  // 无重载
来源：http://vo.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qb.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://zp.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qa.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://xb.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://hd.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kl.jctech888.com.cn

================================================================================
来源：http://ff.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://qb.jctech888.com.cn

================================================================================
来源：http://mp.nszjky.cn

[D01] 创建数组 / 列表
来源：http://hm.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pr.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hg.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kl.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zo.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pr.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://dp.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://bn.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jb.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://di.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yh.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://of.yuexingan06.cn

JS:   arr.push(4);
来源：http://bj.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://ej.shxzukj.cn

Java: list.add(4);
来源：http://xl.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://lr.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://md.9csxet.cn

C#:   list.Add(4);
来源：http://gq.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://zq.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://zq.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ab.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lx.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://jj.panjiajie.cn

Java: list.add(0, 0);
来源：http://pv.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://so.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xj.521024.cn

C#:   list.Insert(0, 0);
来源：http://nz.shxzukj.cn

[D04] 删除元素
来源：http://zu.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cw.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fb.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ls.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://hn.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lx.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lb.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nh.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ns.9csxet.cn

[D05] 访问与修改元素
来源：http://hw.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ax.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rf.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://rz.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://yi.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://dp.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vs.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nm.muxihuayi.cn

[D06] 数组长度
来源：http://gd.huixinmuqiang.cn

Py:   len(arr)
来源：http://ty.hnjuh.cn

PHP:  count($arr);
来源：http://oj.hahajie.cn

JS:   arr.length
来源：http://ac.yuntaijiaju.cn

TS:   arr.length
来源：http://ff.huixiangedu.cn

Java: list.size();
来源：http://xf.haigaiapp.cn

Go:   len(arr)
来源：http://mk.hahajie.cn

Ruby: arr.length; arr.size
来源：http://cs.asd995.cn

C#:   list.Count;
来源：http://iu.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://kw.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pk.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yu.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://en.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://fc.9csxet.cn

Java: list.subList(1, 4);
来源：http://iq.wgjwhj.cn

Go:   arr[1:4]
来源：http://kr.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://xy.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://vo.hahajie.cn

[D08] 合并两个数组
来源：http://ex.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://ob.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://rp.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ep.hahajie.cn

TS:   [...a, ...b];
来源：http://rb.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qe.asd995.cn

Go:   append(a, b...)
来源：http://vz.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://td.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://uo.bookmarksfly.cn

[D09] 排序（升序）
来源：http://bk.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://iu.nicolike.cn


<!-- 参考信息 -->