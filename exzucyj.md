代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://pt.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nd.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yw.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://qw.9csxet.cn

[B09] break 与 continue
来源：http://cr.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ym.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bj.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ce.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rh.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ni.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ic.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://db.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oq.huanxung.cn

[B10] 遍历同时拿索引
来源：http://ez.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nr.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://da.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gf.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zg.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mh.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ll.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://th.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yj.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://ej.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://ju.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://zv.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sy.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kr.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rp.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sb.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://vf.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vr.newstarts.cn

[B12] 跳出多层循环
来源：http://yr.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ig.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oh.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nn.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ak.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pz.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yk.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qc.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ua.wgjwhj.cn

[B13] 判断是否为数字
来源：http://le.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://ar.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://vb.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rv.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wg.yuntaijiaju.cn

Java: x instanceof Number
来源：http://au.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dd.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://rx.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://fz.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://yn.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kj.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gb.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://ms.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://nm.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://de.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xw.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ie.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://io.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://ia.gzmigu.cn

Py:   a and b or not c
来源：http://bf.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://ch.muxihuayi.cn

JS:   a && b || !c
来源：http://dm.wgjwhj.cn

TS:   a && b || !c
来源：http://hz.shxzskj.cn

Java: a && b || !c
来源：http://zo.shtwfgs.cn

Go:   a && b || !c
来源：http://yz.muxihuayi.cn

Ruby: a && b || !c
来源：http://bh.jctech888.com.cn

C#:   a && b || !c
来源：http://du.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uk.bookmarksfly.cn

Py:   if not data: return
来源：http://dz.asd995.cn

PHP:  if (!$data) { return; }
来源：http://st.asd995.cn

JS:   if (!data) return;
来源：http://tk.huanxung.cn

TS:   if (!data) return;
来源：http://av.panjiajie.cn

Java: if (data == null) return;
来源：http://xz.hahajie.cn

Go:   if data == nil { return }
来源：http://mz.szsharing.cn

Ruby: return if data.nil?
来源：http://ut.huanxung.cn

C#:   if (data == null) return;
来源：http://fv.huanxung.cn

================================================================================
来源：http://da.huanxung.cn

C. 函数与作用域
来源：http://yi.szxytkj.cn

================================================================================
来源：http://bp.hnjuh.cn

[C01] 定义函数
来源：http://uz.colortex.cn

Py:   def add(a, b): return a + b
来源：http://mf.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kw.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://wa.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bj.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wa.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zx.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://tm.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gy.yuexingan06.cn

[C02] 默认参数
来源：http://bb.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://iu.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xi.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qs.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fy.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bw.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tc.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://ge.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://dz.asd995.cn

[C03] 可变参数
来源：http://ii.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://eg.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ka.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uk.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iv.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fn.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gu.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ht.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nv.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://lx.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uz.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tk.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wb.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://se.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://dr.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://et.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://hq.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://lt.shxzukj.cn

[C05] 返回多个值
来源：http://mn.wgjwhj.cn

Py:   return a, b
来源：http://ij.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://mx.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ka.muxihuayi.cn

TS:   return { a, b };
来源：http://wl.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vf.huixiangedu.cn

Go:   return a, b
来源：http://bm.nszjky.cn

Ruby: return a, b
来源：http://pz.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://if.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://rl.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://qb.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bd.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://xn.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://qh.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rq.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pk.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://br.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ae.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://pa.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ag.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vh.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jl.szsharing.cn

TS:   arr.map(String)
来源：http://pa.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ov.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rd.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://yh.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sr.asd995.cn

[C08] 闭包
来源：http://tk.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ab.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qq.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gx.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uz.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yz.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nj.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://io.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nd.yuntaijiaju.cn

[C09] 递归
来源：http://ha.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pe.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://th.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zb.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pq.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wh.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nt.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jg.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lk.shxzskj.cn

[C10] 变量作用域
来源：http://nt.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cf.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tc.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wy.colortex.cn

TS:   同 JS
来源：http://rz.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://td.nicolike.cn

Go:   花括号块级作用域
来源：http://md.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yv.bjjhwx.cn

C#:   块级作用域
来源：http://id.9csxet.cn

[C11] 模块导入与导出
来源：http://kh.colortex.cn

Py:   from module import func
来源：http://tb.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nx.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cn.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ri.shxzskj.cn

Java: import java.util.List;
来源：http://rn.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ug.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://bs.bookmarksfly.cn

C#:   using System.Text;
来源：http://ax.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://xz.asd995.cn

Py:   (lambda: print("run"))()
来源：http://wm.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://sr.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://gi.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://zs.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bt.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://lz.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://hu.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://av.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://fk.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bk.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fw.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oc.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uw.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dx.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://nu.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://al.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pn.huanxung.cn

[C14] 泛型函数
来源：http://pf.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rs.muxihuayi.cn

PHP:  // 无泛型
来源：http://it.yuexingan06.cn

JS:   // 无泛型
来源：http://ub.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yh.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sl.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cc.yuexingan06.cn

Ruby: # 无泛型
来源：http://pg.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xm.newstarts.cn

[C15] 解构 / 展开参数
来源：http://io.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sg.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://ns.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ow.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yd.colortex.cn

Java: // 无解构
来源：http://fa.asd995.cn

Go:   // 无解构
来源：http://wf.yuexingan06.cn

Ruby: a, b = pair
来源：http://xi.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://gp.nicolike.cn

[C16] 函数 / 方法重载
来源：http://vx.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mo.bjjhwx.cn

PHP:  // 无重载
来源：http://xk.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://js.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://eh.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bq.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://ol.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://oi.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bi.jctech888.com.cn

================================================================================
来源：http://cp.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://zq.huixinmuqiang.cn

================================================================================
来源：http://wf.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://lr.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fo.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ag.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zw.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ji.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pb.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://oe.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://ck.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qa.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://ha.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kc.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yd.wgjwhj.cn

JS:   arr.push(4);
来源：http://dz.wgjwhj.cn

TS:   arr.push(4);
来源：http://gv.shxzukj.cn

Java: list.add(4);
来源：http://ep.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://td.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://kd.shxzukj.cn

C#:   list.Add(4);
来源：http://fe.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://du.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://hv.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ae.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wr.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://mh.haigaiapp.cn

Java: list.add(0, 0);
来源：http://uu.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ek.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mt.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://md.huixiangedu.cn

[D04] 删除元素
来源：http://lc.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uy.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tc.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rn.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://mb.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lv.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kf.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sn.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rr.lnxyls.cn

[D05] 访问与修改元素
来源：http://mo.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qc.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pd.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pq.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://fg.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://nx.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://xu.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ov.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://se.shtwfgs.cn

[D06] 数组长度
来源：http://ig.jianghongdianzi.cn

Py:   len(arr)
来源：http://ep.bjjhwx.cn

PHP:  count($arr);
来源：http://he.asd995.cn

JS:   arr.length
来源：http://ae.shtwfgs.cn

TS:   arr.length
来源：http://lr.521024.cn

Java: list.size();
来源：http://tw.shxzskj.cn

Go:   len(arr)
来源：http://by.9csxet.cn

Ruby: arr.length; arr.size
来源：http://rn.newstarts.cn

C#:   list.Count;
来源：http://td.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://ka.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yn.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kg.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://cu.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://vw.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://wf.hnjuh.cn

Go:   arr[1:4]
来源：http://tv.gzmigu.cn

Ruby: arr[1, 3]
来源：http://vl.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://bc.muxihuayi.cn

[D08] 合并两个数组
来源：http://yf.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://jo.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://rn.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wt.lnxyls.cn

TS:   [...a, ...b];
来源：http://wr.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jl.shxzskj.cn

Go:   append(a, b...)
来源：http://ht.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://wn.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://kg.nicolike.cn

[D09] 排序（升序）
来源：http://fl.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://fh.jianghongdianzi.cn


<!-- 参考信息 -->