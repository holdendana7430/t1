代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://rn.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cl.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xk.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://gh.yuexingan06.cn

[B09] break 与 continue
来源：http://bu.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yo.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://va.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gd.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://em.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iq.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yj.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://da.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://fv.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lk.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cg.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zo.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hv.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mf.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://at.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wo.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hh.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://mu.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://yn.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://ng.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pz.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mt.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zo.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ws.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://zn.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ky.huanxung.cn

[B12] 跳出多层循环
来源：http://xf.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ja.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kx.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://du.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://es.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dz.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xn.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gi.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ce.yuexingan06.cn

[B13] 判断是否为数字
来源：http://av.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://js.colortex.cn

PHP:  is_numeric($x)
来源：http://te.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hw.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ky.asd995.cn

Java: x instanceof Number
来源：http://kg.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yh.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://ju.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://aq.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://ww.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://le.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rk.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://an.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://zw.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zs.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kk.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ew.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jx.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://ld.panjiajie.cn

Py:   a and b or not c
来源：http://ge.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://mw.bjjhwx.cn

JS:   a && b || !c
来源：http://fv.gzmigu.cn

TS:   a && b || !c
来源：http://si.muxihuayi.cn

Java: a && b || !c
来源：http://wl.hahajie.cn

Go:   a && b || !c
来源：http://av.asd995.cn

Ruby: a && b || !c
来源：http://qd.nicolike.cn

C#:   a && b || !c
来源：http://mi.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://af.shtwfgs.cn

Py:   if not data: return
来源：http://rt.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://qc.huanxung.cn

JS:   if (!data) return;
来源：http://qb.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://di.asd995.cn

Java: if (data == null) return;
来源：http://hv.nszjky.cn

Go:   if data == nil { return }
来源：http://he.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://bw.shxzskj.cn

C#:   if (data == null) return;
来源：http://lp.huixiangedu.cn

================================================================================
来源：http://sh.asd995.cn

C. 函数与作用域
来源：http://mg.nicolike.cn

================================================================================
来源：http://fv.9csxet.cn

[C01] 定义函数
来源：http://fl.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://dt.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fi.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://tk.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yb.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aj.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ut.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://uq.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ce.yuntaijiaju.cn

[C02] 默认参数
来源：http://sc.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://lp.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rz.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://qp.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iz.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sa.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cu.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://yc.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://pd.shxzukj.cn

[C03] 可变参数
来源：http://be.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://dl.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ew.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xy.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zt.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yn.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wf.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rt.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aa.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://hd.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yz.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vp.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lz.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yn.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://ic.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://pn.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://qe.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://tf.521024.cn

[C05] 返回多个值
来源：http://ri.hahajie.cn

Py:   return a, b
来源：http://ik.521024.cn

PHP:  return [$a, $b];
来源：http://pq.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dy.chemitech.net.cn

TS:   return { a, b };
来源：http://hj.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tb.lnxyls.cn

Go:   return a, b
来源：http://qi.wgjwhj.cn

Ruby: return a, b
来源：http://jj.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://dx.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://aw.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://xr.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pq.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://gd.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://lb.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tj.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cn.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://ng.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xw.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://nw.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://it.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://td.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://at.nszjky.cn

TS:   arr.map(String)
来源：http://rn.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ax.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ka.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://nx.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://py.newstarts.cn

[C08] 闭包
来源：http://uw.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ay.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ns.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jd.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://al.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eo.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gq.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mh.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://db.gzmigu.cn

[C09] 递归
来源：http://su.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pk.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://co.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ec.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uo.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://by.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fc.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sk.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gc.jianghongdianzi.cn

[C10] 变量作用域
来源：http://de.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qb.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ys.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sw.muxihuayi.cn

TS:   同 JS
来源：http://oa.hahajie.cn

Java: 方法内为块级作用域
来源：http://yd.lnxyls.cn

Go:   花括号块级作用域
来源：http://yu.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pw.hnjuh.cn

C#:   块级作用域
来源：http://oq.muxihuayi.cn

[C11] 模块导入与导出
来源：http://dw.huixinmuqiang.cn

Py:   from module import func
来源：http://ij.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kj.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bb.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ez.yuexingan06.cn

Java: import java.util.List;
来源：http://pp.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pn.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://yx.shxzskj.cn

C#:   using System.Text;
来源：http://el.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://ju.521024.cn

Py:   (lambda: print("run"))()
来源：http://ls.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://rt.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://wf.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://tb.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hp.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ts.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://tb.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ra.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://hz.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gj.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zn.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rz.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qy.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lr.asd995.cn

Go:   func add(a, b int) int
来源：http://lj.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uw.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fu.huanxung.cn

[C14] 泛型函数
来源：http://zd.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vp.szxytkj.cn

PHP:  // 无泛型
来源：http://pa.521024.cn

JS:   // 无泛型
来源：http://zw.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qj.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bt.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yu.szsharing.cn

Ruby: # 无泛型
来源：http://so.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://np.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://io.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kr.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://ho.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eu.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kp.hnjuh.cn

Java: // 无解构
来源：http://jr.jianghongdianzi.cn

Go:   // 无解构
来源：http://tp.haigaiapp.cn

Ruby: a, b = pair
来源：http://bb.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://gj.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://er.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jq.nicolike.cn

PHP:  // 无重载
来源：http://qg.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xn.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://on.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://le.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://li.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://zh.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gy.huanxung.cn

================================================================================
来源：http://iy.521024.cn

D. 数组 / 列表 / 集合
来源：http://va.colortex.cn

================================================================================
来源：http://rg.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://yw.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ql.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lx.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vx.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bf.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://io.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://kz.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://rs.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fv.lnxyls.cn

[D02] 追加元素到末尾
来源：http://sw.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://up.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ha.hahajie.cn

JS:   arr.push(4);
来源：http://ak.newstarts.cn

TS:   arr.push(4);
来源：http://ms.panjiajie.cn

Java: list.add(4);
来源：http://ix.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://vd.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://kj.hahajie.cn

C#:   list.Add(4);
来源：http://bl.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://bh.asd995.cn

Py:   arr.insert(0, 0)
来源：http://cx.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pa.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zh.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://lo.yuexingan06.cn

Java: list.add(0, 0);
来源：http://ia.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vt.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qy.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://sh.muxihuayi.cn

[D04] 删除元素
来源：http://ak.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mx.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cj.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cc.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://aw.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fx.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ds.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://go.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ln.shxzukj.cn

[D05] 访问与修改元素
来源：http://cf.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ou.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tb.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://os.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://ci.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://yw.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://sb.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iw.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ot.asd995.cn

[D06] 数组长度
来源：http://pv.chemitech.net.cn

Py:   len(arr)
来源：http://ec.chemitech.net.cn

PHP:  count($arr);
来源：http://xm.nszjky.cn

JS:   arr.length
来源：http://ma.muxihuayi.cn

TS:   arr.length
来源：http://kh.yuexingan06.cn

Java: list.size();
来源：http://lh.haigaiapp.cn

Go:   len(arr)
来源：http://vb.9csxet.cn

Ruby: arr.length; arr.size
来源：http://ww.bookmarksfly.cn

C#:   list.Count;
来源：http://gw.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://ab.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dy.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ao.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://rm.asd995.cn

TS:   arr.slice(1, 4);
来源：http://cq.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://dn.9csxet.cn

Go:   arr[1:4]
来源：http://ud.szsharing.cn

Ruby: arr[1, 3]
来源：http://re.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://xt.yuexingan06.cn

[D08] 合并两个数组
来源：http://ho.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://yk.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://ks.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://di.hnjuh.cn

TS:   [...a, ...b];
来源：http://pv.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cp.hnjuh.cn

Go:   append(a, b...)
来源：http://zx.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://kd.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://jo.hahajie.cn

[D09] 排序（升序）
来源：http://wl.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://eo.wgjwhj.cn


<!-- 参考信息 -->