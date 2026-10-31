代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://cd.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ws.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://af.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://gc.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://ux.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pr.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yv.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://il.yuexingan06.cn

[B09] break 与 continue
来源：http://xu.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jc.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ed.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dp.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ue.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kd.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ua.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cc.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ar.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://bd.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ss.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fd.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sz.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kr.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oy.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ub.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://do.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qh.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://go.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://ol.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://us.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ee.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ac.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eh.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://or.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://ld.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qy.shxzukj.cn

[B12] 跳出多层循环
来源：http://qn.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tq.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yp.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zb.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ul.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xu.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xq.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nu.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jx.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://zo.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://dk.shxzskj.cn

PHP:  is_numeric($x)
来源：http://vr.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bg.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zl.hahajie.cn

Java: x instanceof Number
来源：http://zu.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://js.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ru.nszjky.cn

C#:   x is int or double or decimal
来源：http://io.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://yo.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mo.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vh.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://dc.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://sz.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ta.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ea.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sf.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vh.9csxet.cn

[B15] 布尔运算与取反
来源：http://gy.panjiajie.cn

Py:   a and b or not c
来源：http://dx.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://fg.szsharing.cn

JS:   a && b || !c
来源：http://pj.gzmigu.cn

TS:   a && b || !c
来源：http://xg.jctech888.com.cn

Java: a && b || !c
来源：http://fa.huixinmuqiang.cn

Go:   a && b || !c
来源：http://br.szsharing.cn

Ruby: a && b || !c
来源：http://xa.muxihuayi.cn

C#:   a && b || !c
来源：http://iq.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yh.shxzskj.cn

Py:   if not data: return
来源：http://lu.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://ye.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://qk.huixiangedu.cn

TS:   if (!data) return;
来源：http://mo.chemitech.net.cn

Java: if (data == null) return;
来源：http://xr.shxzskj.cn

Go:   if data == nil { return }
来源：http://dx.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://yz.shxzukj.cn

C#:   if (data == null) return;
来源：http://ay.szxytkj.cn

================================================================================
来源：http://xx.szsharing.cn

C. 函数与作用域
来源：http://tc.hnjuh.cn

================================================================================
来源：http://ze.shtwfgs.cn

[C01] 定义函数
来源：http://wa.colortex.cn

Py:   def add(a, b): return a + b
来源：http://tt.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jp.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://tq.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://so.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://je.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dq.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://zj.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kc.bookmarksfly.cn

[C02] 默认参数
来源：http://vh.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://bp.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fp.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://xu.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cn.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mg.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cc.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://fd.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://cm.nicolike.cn

[C03] 可变参数
来源：http://vr.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://gz.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mh.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aq.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dz.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bs.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jp.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rt.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zp.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://pk.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xo.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ld.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mp.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://un.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://rl.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://zw.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://dy.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://jc.panjiajie.cn

[C05] 返回多个值
来源：http://qb.lnxyls.cn

Py:   return a, b
来源：http://oy.nszjky.cn

PHP:  return [$a, $b];
来源：http://lk.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vh.panjiajie.cn

TS:   return { a, b };
来源：http://ww.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aj.huanxung.cn

Go:   return a, b
来源：http://ow.nszjky.cn

Ruby: return a, b
来源：http://fu.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://tz.521024.cn

[C06] 匿名函数 / lambda
来源：http://qu.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://hd.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sk.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://vg.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://vr.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gs.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wg.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://dn.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wp.nszjky.cn

[C07] 把函数作为参数传入
来源：http://gn.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yj.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hz.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rl.bjjhwx.cn

TS:   arr.map(String)
来源：http://go.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pp.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qw.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://at.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wo.lnxyls.cn

[C08] 闭包
来源：http://bp.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zf.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jz.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zx.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jk.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bp.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://us.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pc.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://te.hnjuh.cn

[C09] 递归
来源：http://rz.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ak.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://me.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fl.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fr.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zs.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ph.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yo.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zm.szsharing.cn

[C10] 变量作用域
来源：http://fs.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ax.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qi.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tr.hnjuh.cn

TS:   同 JS
来源：http://nu.nicolike.cn

Java: 方法内为块级作用域
来源：http://bw.panjiajie.cn

Go:   花括号块级作用域
来源：http://pv.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wx.lnxyls.cn

C#:   块级作用域
来源：http://ac.gzmigu.cn

[C11] 模块导入与导出
来源：http://pc.nicolike.cn

Py:   from module import func
来源：http://ra.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ti.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lx.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ey.chemitech.net.cn

Java: import java.util.List;
来源：http://ez.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lt.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://hq.szxytkj.cn

C#:   using System.Text;
来源：http://fc.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://tj.colortex.cn

Py:   (lambda: print("run"))()
来源：http://wz.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://md.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://en.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://qy.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gb.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://fn.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://vb.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ee.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://nx.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nx.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ot.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ip.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ma.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hd.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://oh.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rr.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yh.nszjky.cn

[C14] 泛型函数
来源：http://cr.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dq.szsharing.cn

PHP:  // 无泛型
来源：http://pw.panjiajie.cn

JS:   // 无泛型
来源：http://ze.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ec.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://io.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://km.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://aj.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kf.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://bj.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mw.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://yb.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zb.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sl.newstarts.cn

Java: // 无解构
来源：http://np.hahajie.cn

Go:   // 无解构
来源：http://jb.wgjwhj.cn

Ruby: a, b = pair
来源：http://xn.nszjky.cn

C#:   var (a, b) = pair;
来源：http://lp.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://mz.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uw.newstarts.cn

PHP:  // 无重载
来源：http://nw.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rc.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://ct.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mf.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://px.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://xw.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ye.szxytkj.cn

================================================================================
来源：http://mt.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://oh.muxihuayi.cn

================================================================================
来源：http://jo.asd995.cn

[D01] 创建数组 / 列表
来源：http://ma.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qm.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wh.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bq.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://aa.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mr.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://pe.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://gu.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bs.hahajie.cn

[D02] 追加元素到末尾
来源：http://bf.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wl.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ek.9csxet.cn

JS:   arr.push(4);
来源：http://pd.shxzskj.cn

TS:   arr.push(4);
来源：http://cb.wgjwhj.cn

Java: list.add(4);
来源：http://hc.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://ns.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://ax.muxihuayi.cn

C#:   list.Add(4);
来源：http://px.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://ct.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://jp.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vg.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ie.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://zv.jctech888.com.cn

Java: list.add(0, 0);
来源：http://jx.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dc.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dk.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://pc.huanxung.cn

[D04] 删除元素
来源：http://hc.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vf.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sl.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zn.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://or.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mx.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ba.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nu.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ms.chemitech.net.cn

[D05] 访问与修改元素
来源：http://nb.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kx.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jp.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://am.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://kk.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://th.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://py.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bt.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dw.lnxyls.cn

[D06] 数组长度
来源：http://vn.haigaiapp.cn

Py:   len(arr)
来源：http://pf.huixiangedu.cn

PHP:  count($arr);
来源：http://do.nicolike.cn

JS:   arr.length
来源：http://lr.gzmigu.cn

TS:   arr.length
来源：http://go.colortex.cn

Java: list.size();
来源：http://cq.huixinmuqiang.cn

Go:   len(arr)
来源：http://up.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://vd.9csxet.cn

C#:   list.Count;
来源：http://yf.newstarts.cn

[D07] 切片 / 取子数组
来源：http://cb.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dh.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fc.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://om.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://on.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://gf.huixiangedu.cn

Go:   arr[1:4]
来源：http://tt.szsharing.cn

Ruby: arr[1, 3]
来源：http://ls.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://xo.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://ee.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://av.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://fb.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vm.yuexingan06.cn

TS:   [...a, ...b];
来源：http://lw.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lh.huixiangedu.cn

Go:   append(a, b...)
来源：http://kk.muxihuayi.cn


<!-- 参考信息 -->