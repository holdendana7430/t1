代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yp.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://rm.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://lm.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://ky.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://ly.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mg.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://qv.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://od.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://dm.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fe.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ko.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://jj.shxzukj.cn

[B09] break 与 continue
来源：http://ei.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vy.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zl.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ps.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cz.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ck.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yz.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sv.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vd.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://qv.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yn.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ud.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qx.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wi.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fj.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kd.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pb.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kp.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://ic.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://xv.521024.cn

PHP:  range(0, 10, 2);
来源：http://sq.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ol.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ni.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ng.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uz.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://od.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dg.szsharing.cn

[B12] 跳出多层循环
来源：http://mb.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sv.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ju.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://px.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vw.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hv.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jz.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hs.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uq.yuexingan06.cn

[B13] 判断是否为数字
来源：http://js.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://zk.colortex.cn

PHP:  is_numeric($x)
来源：http://nb.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bz.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eb.colortex.cn

Java: x instanceof Number
来源：http://ko.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mx.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://zx.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://lt.newstarts.cn

[B14] 判断值是否在集合内
来源：http://gy.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ee.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ja.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://bo.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://zr.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qm.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ky.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bh.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fs.panjiajie.cn

[B15] 布尔运算与取反
来源：http://bt.yuntaijiaju.cn

Py:   a and b or not c
来源：http://xk.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://xn.huixinmuqiang.cn

JS:   a && b || !c
来源：http://fw.wgjwhj.cn

TS:   a && b || !c
来源：http://pq.yuexingan06.cn

Java: a && b || !c
来源：http://pl.newstarts.cn

Go:   a && b || !c
来源：http://aq.haigaiapp.cn

Ruby: a && b || !c
来源：http://kq.szxytkj.cn

C#:   a && b || !c
来源：http://kv.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pz.wgjwhj.cn

Py:   if not data: return
来源：http://sg.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://bm.chemitech.net.cn

JS:   if (!data) return;
来源：http://we.szsharing.cn

TS:   if (!data) return;
来源：http://ip.wgjwhj.cn

Java: if (data == null) return;
来源：http://yc.shxzskj.cn

Go:   if data == nil { return }
来源：http://cl.hahajie.cn

Ruby: return if data.nil?
来源：http://qc.muxihuayi.cn

C#:   if (data == null) return;
来源：http://ym.hnjuh.cn

================================================================================
来源：http://qv.jianghongdianzi.cn

C. 函数与作用域
来源：http://le.bookmarksfly.cn

================================================================================
来源：http://zb.huanxung.cn

[C01] 定义函数
来源：http://iw.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://qe.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zd.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://ci.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cm.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rz.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://de.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://xt.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nr.lnxyls.cn

[C02] 默认参数
来源：http://yj.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://rj.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tm.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://mf.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nh.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wh.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dr.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://iy.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://lt.hahajie.cn

[C03] 可变参数
来源：http://pa.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://fv.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lk.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kf.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tl.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ip.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tb.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fk.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dz.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://zk.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aw.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qd.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hu.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hl.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://ti.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://el.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://mp.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://hd.gzmigu.cn

[C05] 返回多个值
来源：http://nx.wgjwhj.cn

Py:   return a, b
来源：http://me.9csxet.cn

PHP:  return [$a, $b];
来源：http://kl.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jc.asd995.cn

TS:   return { a, b };
来源：http://us.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ez.chemitech.net.cn

Go:   return a, b
来源：http://zb.szxytkj.cn

Ruby: return a, b
来源：http://vr.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ed.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://eh.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://my.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://se.panjiajie.cn

JS:   const square = x => x * x;
来源：http://bb.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://nn.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ei.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xz.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://vi.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cn.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://jn.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wk.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ql.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zi.muxihuayi.cn

TS:   arr.map(String)
来源：http://xw.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oy.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bp.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://fz.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://km.shxzskj.cn

[C08] 闭包
来源：http://kq.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pn.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://au.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zi.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sy.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jp.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bv.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bf.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rm.colortex.cn

[C09] 递归
来源：http://ph.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qn.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mj.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ek.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ms.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://js.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xk.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ew.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ur.asd995.cn

[C10] 变量作用域
来源：http://az.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jr.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://or.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://go.huixinmuqiang.cn

TS:   同 JS
来源：http://un.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://mu.haigaiapp.cn

Go:   花括号块级作用域
来源：http://it.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ty.yuntaijiaju.cn

C#:   块级作用域
来源：http://hm.chemitech.net.cn

[C11] 模块导入与导出
来源：http://ht.haigaiapp.cn

Py:   from module import func
来源：http://sn.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iz.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sm.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gf.bjjhwx.cn

Java: import java.util.List;
来源：http://cj.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ym.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://vz.huixiangedu.cn

C#:   using System.Text;
来源：http://nk.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://ig.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://fc.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://qs.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://sa.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ka.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jz.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://kk.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://cx.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kg.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://fe.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sn.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xk.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cg.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aq.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lq.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://oh.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fl.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qr.bjjhwx.cn

[C14] 泛型函数
来源：http://yz.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gh.jctech888.com.cn

PHP:  // 无泛型
来源：http://kj.szsharing.cn

JS:   // 无泛型
来源：http://sp.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eu.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ce.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kd.nicolike.cn

Ruby: # 无泛型
来源：http://xq.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dh.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://jy.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ij.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://rz.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dt.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hb.haigaiapp.cn

Java: // 无解构
来源：http://th.huixinmuqiang.cn

Go:   // 无解构
来源：http://xl.shxzukj.cn

Ruby: a, b = pair
来源：http://nn.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://ly.nszjky.cn

[C16] 函数 / 方法重载
来源：http://vh.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pm.hnjuh.cn

PHP:  // 无重载
来源：http://dh.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sh.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://lc.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dp.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://ll.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://fe.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://id.chemitech.net.cn

================================================================================
来源：http://vm.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://aj.huanxung.cn

================================================================================
来源：http://so.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://oy.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://of.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xt.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dt.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iq.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vx.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://qy.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://sq.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tx.szsharing.cn

[D02] 追加元素到末尾
来源：http://zb.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wm.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xz.szsharing.cn

JS:   arr.push(4);
来源：http://oq.lnxyls.cn

TS:   arr.push(4);
来源：http://gv.asd995.cn

Java: list.add(4);
来源：http://cj.colortex.cn

Go:   arr = append(arr, 4)
来源：http://ae.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://jx.huanxung.cn

C#:   list.Add(4);
来源：http://tk.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://so.asd995.cn

Py:   arr.insert(0, 0)
来源：http://so.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rr.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ky.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://ce.shxzskj.cn

Java: list.add(0, 0);
来源：http://av.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dv.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nn.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://kd.huixiangedu.cn

[D04] 删除元素
来源：http://zu.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uq.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bw.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ku.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://xh.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tm.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fs.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://df.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pk.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://mh.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gd.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ui.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ig.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ii.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://hb.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://cm.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xy.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rf.hnjuh.cn

[D06] 数组长度
来源：http://br.haigaiapp.cn

Py:   len(arr)
来源：http://er.haigaiapp.cn

PHP:  count($arr);
来源：http://qt.nszjky.cn

JS:   arr.length
来源：http://mg.shxzukj.cn

TS:   arr.length
来源：http://ru.haigaiapp.cn

Java: list.size();
来源：http://lg.9csxet.cn

Go:   len(arr)
来源：http://dw.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://tk.huixinmuqiang.cn

C#:   list.Count;
来源：http://an.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://ox.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kj.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hd.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://fe.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://zm.huanxung.cn

Java: list.subList(1, 4);
来源：http://qs.newstarts.cn

Go:   arr[1:4]
来源：http://ta.nszjky.cn

Ruby: arr[1, 3]
来源：http://jd.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://tz.shxzukj.cn

[D08] 合并两个数组
来源：http://zn.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://mk.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://ju.huixinmuqiang.cn


<!-- 参考信息 -->