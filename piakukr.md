代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://of.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://rk.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://sf.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://gk.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ux.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kn.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://ya.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://vn.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://fe.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rn.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ms.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://fr.hnjuh.cn

[B09] break 与 continue
来源：http://rp.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dq.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sw.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rr.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://um.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qm.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wh.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://zq.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://al.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xy.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tu.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qd.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nf.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bj.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ab.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ea.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://or.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://ko.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://vt.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://in.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rw.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pc.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://af.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://fm.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qn.shtwfgs.cn

[B12] 跳出多层循环
来源：http://tj.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rs.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jf.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yh.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tj.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nb.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vt.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wp.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ny.bjjhwx.cn

[B13] 判断是否为数字
来源：http://ad.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://ag.9csxet.cn

PHP:  is_numeric($x)
来源：http://nl.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ib.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xr.bjjhwx.cn

Java: x instanceof Number
来源：http://bo.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://er.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://cw.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://cc.hahajie.cn

[B14] 判断值是否在集合内
来源：http://fc.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fh.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gd.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ps.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://nw.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zn.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sj.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ad.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yk.colortex.cn

[B15] 布尔运算与取反
来源：http://da.hnjuh.cn

Py:   a and b or not c
来源：http://ts.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://kt.chemitech.net.cn

JS:   a && b || !c
来源：http://bs.bjjhwx.cn

TS:   a && b || !c
来源：http://ah.huixinmuqiang.cn

Java: a && b || !c
来源：http://cj.521024.cn

Go:   a && b || !c
来源：http://hm.huanxung.cn

Ruby: a && b || !c
来源：http://ag.jianghongdianzi.cn

C#:   a && b || !c
来源：http://ui.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jh.muxihuayi.cn

Py:   if not data: return
来源：http://dx.asd995.cn

PHP:  if (!$data) { return; }
来源：http://uh.lnxyls.cn

JS:   if (!data) return;
来源：http://pt.gzmigu.cn

TS:   if (!data) return;
来源：http://eo.huanxung.cn

Java: if (data == null) return;
来源：http://gc.chemitech.net.cn

Go:   if data == nil { return }
来源：http://qy.shxzukj.cn

Ruby: return if data.nil?
来源：http://bq.panjiajie.cn

C#:   if (data == null) return;
来源：http://ho.jianghongdianzi.cn

================================================================================
来源：http://af.hnjuh.cn

C. 函数与作用域
来源：http://cs.shxzukj.cn

================================================================================
来源：http://gl.szsharing.cn

[C01] 定义函数
来源：http://th.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://cm.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gg.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://nu.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gu.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qb.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fz.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://xg.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rl.newstarts.cn

[C02] 默认参数
来源：http://fg.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://cp.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wq.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://kf.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hb.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ux.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ax.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://rq.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://kx.shxzskj.cn

[C03] 可变参数
来源：http://ob.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://ft.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ke.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qm.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wl.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qy.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qf.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fy.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mf.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://hs.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gt.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cc.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lc.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rq.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://nn.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://dm.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://od.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://np.haigaiapp.cn

[C05] 返回多个值
来源：http://rn.muxihuayi.cn

Py:   return a, b
来源：http://rj.newstarts.cn

PHP:  return [$a, $b];
来源：http://cf.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://at.asd995.cn

TS:   return { a, b };
来源：http://rl.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jt.9csxet.cn

Go:   return a, b
来源：http://qy.bjjhwx.cn

Ruby: return a, b
来源：http://oe.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://yl.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://al.521024.cn

Py:   square = lambda x: x * x
来源：http://ho.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kv.panjiajie.cn

JS:   const square = x => x * x;
来源：http://cb.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://on.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xc.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vn.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://fh.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wo.nszjky.cn

[C07] 把函数作为参数传入
来源：http://qw.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jg.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hy.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uk.shxzukj.cn

TS:   arr.map(String)
来源：http://xu.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lu.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xk.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://ps.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rx.szxytkj.cn

[C08] 闭包
来源：http://yd.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fe.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sx.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rm.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cp.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://si.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ej.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vn.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kd.bjjhwx.cn

[C09] 递归
来源：http://mk.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dt.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://we.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hs.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fd.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rg.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ja.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://np.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qw.nicolike.cn

[C10] 变量作用域
来源：http://xn.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cu.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nq.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ss.wgjwhj.cn

TS:   同 JS
来源：http://gb.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://zi.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://mw.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tp.yuexingan06.cn

C#:   块级作用域
来源：http://lv.nicolike.cn

[C11] 模块导入与导出
来源：http://lu.bjjhwx.cn

Py:   from module import func
来源：http://rg.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://un.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lc.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qe.jctech888.com.cn

Java: import java.util.List;
来源：http://pd.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lf.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://oy.521024.cn

C#:   using System.Text;
来源：http://ki.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://jo.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://ty.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://oe.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://im.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ke.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pg.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://ll.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://oh.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ob.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://rv.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ko.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ys.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yx.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://op.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pn.nicolike.cn

Go:   func add(a, b int) int
来源：http://dd.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iu.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tj.hahajie.cn

[C14] 泛型函数
来源：http://vh.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yw.hnjuh.cn

PHP:  // 无泛型
来源：http://wl.shtwfgs.cn

JS:   // 无泛型
来源：http://qx.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lb.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fc.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tl.shtwfgs.cn

Ruby: # 无泛型
来源：http://ww.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ma.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://at.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ro.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://ni.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nc.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://te.szxytkj.cn

Java: // 无解构
来源：http://su.gzmigu.cn

Go:   // 无解构
来源：http://zp.bookmarksfly.cn

Ruby: a, b = pair
来源：http://ki.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://gi.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://vb.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vo.szsharing.cn

PHP:  // 无重载
来源：http://ms.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rb.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://yl.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yq.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://ws.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://fh.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qg.bjjhwx.cn

================================================================================
来源：http://rx.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ve.gzmigu.cn

================================================================================
来源：http://qq.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://fh.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mw.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wp.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pn.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rn.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iz.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://ww.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://ff.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ff.nszjky.cn

[D02] 追加元素到末尾
来源：http://ki.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gl.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ip.bookmarksfly.cn

JS:   arr.push(4);
来源：http://pc.szxytkj.cn

TS:   arr.push(4);
来源：http://wc.9csxet.cn

Java: list.add(4);
来源：http://ln.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://ym.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://fr.szsharing.cn

C#:   list.Add(4);
来源：http://ct.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://dc.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://pm.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://em.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tr.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://gk.nszjky.cn

Java: list.add(0, 0);
来源：http://pw.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dr.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yi.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://kj.shxzukj.cn

[D04] 删除元素
来源：http://df.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ff.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cc.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qw.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://ez.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sf.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ut.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qg.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zc.panjiajie.cn

[D05] 访问与修改元素
来源：http://qr.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jr.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pc.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uy.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://zi.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://pz.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://bc.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fw.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jj.chemitech.net.cn

[D06] 数组长度
来源：http://vi.asd995.cn

Py:   len(arr)
来源：http://jj.shxzukj.cn

PHP:  count($arr);
来源：http://ex.asd995.cn

JS:   arr.length
来源：http://ro.szxytkj.cn

TS:   arr.length
来源：http://os.panjiajie.cn

Java: list.size();
来源：http://wb.shtwfgs.cn

Go:   len(arr)
来源：http://dz.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://nr.nszjky.cn

C#:   list.Count;
来源：http://yk.521024.cn

[D07] 切片 / 取子数组
来源：http://qt.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cn.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rc.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://mk.521024.cn

TS:   arr.slice(1, 4);
来源：http://aa.szxytkj.cn

Java: list.subList(1, 4);
来源：http://fi.9csxet.cn

Go:   arr[1:4]
来源：http://yf.hahajie.cn

Ruby: arr[1, 3]
来源：http://qk.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://ot.bjjhwx.cn

[D08] 合并两个数组
来源：http://jx.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://vk.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://sj.yuntaijiaju.cn


<!-- 参考信息 -->