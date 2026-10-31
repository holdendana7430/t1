代发 wailian999

[B09] break 与 continue
来源：http://wp.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://as.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cp.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eo.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ga.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ie.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tj.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ik.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ph.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://up.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gv.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jp.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dr.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mz.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xk.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mi.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qh.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lt.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://hv.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://ql.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://va.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vv.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ms.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cb.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xo.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://sw.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dg.colortex.cn

[B12] 跳出多层循环
来源：http://kh.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vj.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wf.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zg.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fc.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bd.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gy.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kn.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oi.bjjhwx.cn

[B13] 判断是否为数字
来源：http://qb.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://pz.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://fi.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bq.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mp.huanxung.cn

Java: x instanceof Number
来源：http://yf.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://og.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://jh.521024.cn

C#:   x is int or double or decimal
来源：http://rg.colortex.cn

[B14] 判断值是否在集合内
来源：http://pa.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pi.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gz.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://jq.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://zj.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ok.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mh.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qj.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ik.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://xd.hahajie.cn

Py:   a and b or not c
来源：http://uw.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://qk.hnjuh.cn

JS:   a && b || !c
来源：http://bu.hahajie.cn

TS:   a && b || !c
来源：http://hq.hnjuh.cn

Java: a && b || !c
来源：http://or.wgjwhj.cn

Go:   a && b || !c
来源：http://yg.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://jh.jctech888.com.cn

C#:   a && b || !c
来源：http://zq.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cn.hahajie.cn

Py:   if not data: return
来源：http://ih.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://dc.chemitech.net.cn

JS:   if (!data) return;
来源：http://an.szsharing.cn

TS:   if (!data) return;
来源：http://nb.chemitech.net.cn

Java: if (data == null) return;
来源：http://uj.jctech888.com.cn

Go:   if data == nil { return }
来源：http://uj.haigaiapp.cn

Ruby: return if data.nil?
来源：http://jl.newstarts.cn

C#:   if (data == null) return;
来源：http://yo.colortex.cn

================================================================================
来源：http://qb.wgjwhj.cn

C. 函数与作用域
来源：http://jj.haigaiapp.cn

================================================================================
来源：http://cv.nszjky.cn

[C01] 定义函数
来源：http://wc.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://eh.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vx.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://rc.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xp.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tk.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dt.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://sr.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wg.shtwfgs.cn

[C02] 默认参数
来源：http://rl.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://yh.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cm.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://od.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vi.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gf.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yk.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://sz.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://fz.panjiajie.cn

[C03] 可变参数
来源：http://cn.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://xd.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wn.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pm.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vv.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jy.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lf.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oy.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hi.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://ix.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xu.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bc.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dv.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ma.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://yr.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://my.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://jg.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://dy.shxzukj.cn

[C05] 返回多个值
来源：http://ho.yuntaijiaju.cn

Py:   return a, b
来源：http://js.nicolike.cn

PHP:  return [$a, $b];
来源：http://qa.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gt.chemitech.net.cn

TS:   return { a, b };
来源：http://ol.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://os.nicolike.cn

Go:   return a, b
来源：http://eg.shtwfgs.cn

Ruby: return a, b
来源：http://jn.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://nw.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://my.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://oa.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zd.shxzukj.cn

JS:   const square = x => x * x;
来源：http://jm.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://qs.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ke.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://op.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://us.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iu.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://jf.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sh.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ti.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ha.wgjwhj.cn

TS:   arr.map(String)
来源：http://tv.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nx.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://go.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://fg.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yf.huixiangedu.cn

[C08] 闭包
来源：http://pn.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mt.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hh.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ih.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://px.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ii.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://it.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jr.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oy.panjiajie.cn

[C09] 递归
来源：http://aa.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wy.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mx.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dw.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fm.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mi.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lx.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kz.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fw.huanxung.cn

[C10] 变量作用域
来源：http://hm.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mc.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ml.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xd.gzmigu.cn

TS:   同 JS
来源：http://hj.521024.cn

Java: 方法内为块级作用域
来源：http://eq.lnxyls.cn

Go:   花括号块级作用域
来源：http://ak.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tm.panjiajie.cn

C#:   块级作用域
来源：http://gd.asd995.cn

[C11] 模块导入与导出
来源：http://ap.shxzukj.cn

Py:   from module import func
来源：http://ig.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mi.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://va.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uy.521024.cn

Java: import java.util.List;
来源：http://vd.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wt.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://ut.colortex.cn

C#:   using System.Text;
来源：http://bk.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://xd.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://tu.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://tj.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://bm.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://fz.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yi.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://ji.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://zi.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xl.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://kn.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sf.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mk.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pe.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ot.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nf.hnjuh.cn

Go:   func add(a, b int) int
来源：http://zu.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bz.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ww.shxzskj.cn

[C14] 泛型函数
来源：http://th.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://as.shxzukj.cn

PHP:  // 无泛型
来源：http://le.jianghongdianzi.cn

JS:   // 无泛型
来源：http://ga.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dz.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ee.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ko.nszjky.cn

Ruby: # 无泛型
来源：http://en.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ss.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://lb.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jr.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://yz.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xi.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://go.huixinmuqiang.cn

Java: // 无解构
来源：http://xz.nszjky.cn

Go:   // 无解构
来源：http://ps.szsharing.cn

Ruby: a, b = pair
来源：http://cr.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://or.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://tl.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mo.newstarts.cn

PHP:  // 无重载
来源：http://ys.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fu.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://tg.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ji.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://nb.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://uj.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qh.yuntaijiaju.cn

================================================================================
来源：http://fh.521024.cn

D. 数组 / 列表 / 集合
来源：http://jx.bookmarksfly.cn

================================================================================
来源：http://dg.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://ma.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ur.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://on.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yj.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ov.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ip.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://pw.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://nv.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vn.szsharing.cn

[D02] 追加元素到末尾
来源：http://qv.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ct.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kf.colortex.cn

JS:   arr.push(4);
来源：http://iy.521024.cn

TS:   arr.push(4);
来源：http://ch.wgjwhj.cn

Java: list.add(4);
来源：http://xa.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://vp.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://ei.bookmarksfly.cn

C#:   list.Add(4);
来源：http://og.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://xq.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://dg.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ej.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vv.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://ds.szxytkj.cn

Java: list.add(0, 0);
来源：http://eo.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yp.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fq.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://pr.bookmarksfly.cn

[D04] 删除元素
来源：http://zf.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tu.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bv.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pj.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://yo.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yk.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fm.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tt.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://if.szsharing.cn

[D05] 访问与修改元素
来源：http://aa.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vd.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vl.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vq.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://wn.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://cd.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://yt.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rg.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lw.wgjwhj.cn

[D06] 数组长度
来源：http://zq.szsharing.cn

Py:   len(arr)
来源：http://lz.panjiajie.cn

PHP:  count($arr);
来源：http://if.muxihuayi.cn

JS:   arr.length
来源：http://ir.huanxung.cn

TS:   arr.length
来源：http://yq.gzmigu.cn

Java: list.size();
来源：http://sj.gzmigu.cn

Go:   len(arr)
来源：http://by.newstarts.cn

Ruby: arr.length; arr.size
来源：http://jv.colortex.cn

C#:   list.Count;
来源：http://fm.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://rq.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hs.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fc.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://pb.asd995.cn

TS:   arr.slice(1, 4);
来源：http://dc.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://bk.9csxet.cn

Go:   arr[1:4]
来源：http://gr.nicolike.cn

Ruby: arr[1, 3]
来源：http://le.521024.cn

C#:   list.GetRange(1, 3);
来源：http://yf.szxytkj.cn

[D08] 合并两个数组
来源：http://gc.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://pi.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://ms.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qu.haigaiapp.cn

TS:   [...a, ...b];
来源：http://so.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ce.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://cr.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://op.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://cv.szxytkj.cn

[D09] 排序（升序）
来源：http://qf.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://tl.shxzskj.cn

PHP:  sort($arr);
来源：http://hm.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lo.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lh.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://de.chemitech.net.cn


<!-- 参考信息 -->