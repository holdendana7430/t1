代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://ub.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dl.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gv.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://gf.yuexingan06.cn

[B09] break 与 continue
来源：http://ps.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bq.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ho.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ko.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pj.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qw.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zt.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qt.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mm.nszjky.cn

[B10] 遍历同时拿索引
来源：http://fw.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qu.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://on.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tj.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jf.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ho.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cz.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vx.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gi.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://bt.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://hs.521024.cn

PHP:  range(0, 10, 2);
来源：http://oo.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ov.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ql.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ic.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xd.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://sl.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zx.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://ts.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ty.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tp.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eg.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tf.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cy.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gt.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ls.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ae.shxzukj.cn

[B13] 判断是否为数字
来源：http://ai.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://jv.9csxet.cn

PHP:  is_numeric($x)
来源：http://ww.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qi.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nb.chemitech.net.cn

Java: x instanceof Number
来源：http://cc.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ny.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://ov.521024.cn

C#:   x is int or double or decimal
来源：http://cm.nszjky.cn

[B14] 判断值是否在集合内
来源：http://am.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gw.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lo.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ly.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://yx.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qq.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vi.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nx.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://it.gzmigu.cn

[B15] 布尔运算与取反
来源：http://bk.9csxet.cn

Py:   a and b or not c
来源：http://nf.nszjky.cn

PHP:  $a && $b || !$c
来源：http://wg.jianghongdianzi.cn

JS:   a && b || !c
来源：http://rt.haigaiapp.cn

TS:   a && b || !c
来源：http://mq.9csxet.cn

Java: a && b || !c
来源：http://ui.yuntaijiaju.cn

Go:   a && b || !c
来源：http://nt.szxytkj.cn

Ruby: a && b || !c
来源：http://vx.huanxung.cn

C#:   a && b || !c
来源：http://bz.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lg.521024.cn

Py:   if not data: return
来源：http://ks.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://nh.jctech888.com.cn

JS:   if (!data) return;
来源：http://sf.yuexingan06.cn

TS:   if (!data) return;
来源：http://hf.szsharing.cn

Java: if (data == null) return;
来源：http://fk.jctech888.com.cn

Go:   if data == nil { return }
来源：http://lm.colortex.cn

Ruby: return if data.nil?
来源：http://cd.shxzukj.cn

C#:   if (data == null) return;
来源：http://xd.bookmarksfly.cn

================================================================================
来源：http://pa.huanxung.cn

C. 函数与作用域
来源：http://qd.shxzskj.cn

================================================================================
来源：http://xi.yuexingan06.cn

[C01] 定义函数
来源：http://ss.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://zj.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yl.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://pv.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ui.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ip.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xh.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://kf.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zr.chemitech.net.cn

[C02] 默认参数
来源：http://gf.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://xo.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bc.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://dl.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hq.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nz.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rg.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://uc.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://af.hahajie.cn

[C03] 可变参数
来源：http://pv.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://er.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ne.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kb.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zp.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dw.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vh.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gz.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://np.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://ht.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://az.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://on.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dm.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ih.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://nb.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://fx.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://uc.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://sr.nszjky.cn

[C05] 返回多个值
来源：http://sl.szxytkj.cn

Py:   return a, b
来源：http://rp.gzmigu.cn

PHP:  return [$a, $b];
来源：http://su.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hg.9csxet.cn

TS:   return { a, b };
来源：http://mu.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rx.nicolike.cn

Go:   return a, b
来源：http://dm.shxzukj.cn

Ruby: return a, b
来源：http://an.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://dj.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://xc.huanxung.cn

Py:   square = lambda x: x * x
来源：http://io.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://da.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://xm.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://kn.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pt.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eo.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://hu.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://go.huanxung.cn

[C07] 把函数作为参数传入
来源：http://mt.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pg.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wj.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fv.hahajie.cn

TS:   arr.map(String)
来源：http://zf.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rn.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ib.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://ss.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pd.huixiangedu.cn

[C08] 闭包
来源：http://yk.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pv.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fj.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gs.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vv.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ly.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hu.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://au.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gk.wgjwhj.cn

[C09] 递归
来源：http://hz.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ch.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ca.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zz.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gz.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hj.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dc.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fm.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://as.bookmarksfly.cn

[C10] 变量作用域
来源：http://zz.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nj.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qb.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sa.haigaiapp.cn

TS:   同 JS
来源：http://pq.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ll.nszjky.cn

Go:   花括号块级作用域
来源：http://gq.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mg.szxytkj.cn

C#:   块级作用域
来源：http://ui.haigaiapp.cn

[C11] 模块导入与导出
来源：http://hz.yuntaijiaju.cn

Py:   from module import func
来源：http://fe.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yw.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yt.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fr.521024.cn

Java: import java.util.List;
来源：http://bo.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eb.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://vj.szsharing.cn

C#:   using System.Text;
来源：http://ht.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://sc.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://xr.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://ig.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://po.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://sm.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pe.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://mg.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://lm.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lb.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://pb.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tl.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gb.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://op.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kx.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cr.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://vs.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://al.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vf.gzmigu.cn

[C14] 泛型函数
来源：http://jh.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://is.panjiajie.cn

PHP:  // 无泛型
来源：http://jk.newstarts.cn

JS:   // 无泛型
来源：http://jp.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://id.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eu.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lc.shxzukj.cn

Ruby: # 无泛型
来源：http://nb.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mh.szsharing.cn

[C15] 解构 / 展开参数
来源：http://xx.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yq.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://fk.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zy.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cx.huanxung.cn

Java: // 无解构
来源：http://nd.haigaiapp.cn

Go:   // 无解构
来源：http://fa.chemitech.net.cn

Ruby: a, b = pair
来源：http://wc.hahajie.cn

C#:   var (a, b) = pair;
来源：http://ts.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://up.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ca.jianghongdianzi.cn

PHP:  // 无重载
来源：http://gy.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ik.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://iv.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wd.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://kn.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://ks.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kt.chemitech.net.cn

================================================================================
来源：http://wx.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://wm.jctech888.com.cn

================================================================================
来源：http://hq.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://hz.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gf.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vd.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://of.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zq.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jf.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://lw.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://ze.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gf.nicolike.cn

[D02] 追加元素到末尾
来源：http://ep.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cx.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ms.haigaiapp.cn

JS:   arr.push(4);
来源：http://ps.jctech888.com.cn

TS:   arr.push(4);
来源：http://mm.nicolike.cn

Java: list.add(4);
来源：http://ss.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://yb.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://nu.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://gn.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://hw.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://id.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vp.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ey.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://yv.shxzskj.cn

Java: list.add(0, 0);
来源：http://pk.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vs.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://po.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://zm.nszjky.cn

[D04] 删除元素
来源：http://rj.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rv.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hm.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wi.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://wi.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lg.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lw.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gb.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gb.shxzukj.cn

[D05] 访问与修改元素
来源：http://uf.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sf.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qn.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ah.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://ze.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://sw.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://yw.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yb.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cu.muxihuayi.cn

[D06] 数组长度
来源：http://aj.muxihuayi.cn

Py:   len(arr)
来源：http://ks.jctech888.com.cn

PHP:  count($arr);
来源：http://vo.huixinmuqiang.cn

JS:   arr.length
来源：http://xc.yuntaijiaju.cn

TS:   arr.length
来源：http://de.wgjwhj.cn

Java: list.size();
来源：http://fj.colortex.cn

Go:   len(arr)
来源：http://od.szsharing.cn

Ruby: arr.length; arr.size
来源：http://os.hnjuh.cn

C#:   list.Count;
来源：http://bc.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://xt.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://in.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qc.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://sx.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://dy.521024.cn

Java: list.subList(1, 4);
来源：http://aq.wgjwhj.cn

Go:   arr[1:4]
来源：http://er.shxzskj.cn

Ruby: arr[1, 3]
来源：http://un.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://nw.huixiangedu.cn

[D08] 合并两个数组
来源：http://kf.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://pi.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://fb.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yp.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://ms.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fw.muxihuayi.cn

Go:   append(a, b...)
来源：http://gy.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://jk.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://wz.asd995.cn

[D09] 排序（升序）
来源：http://dy.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zf.panjiajie.cn


<!-- 参考信息 -->