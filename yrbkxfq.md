代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dc.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://hi.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://us.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://bb.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://te.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ax.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://fu.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://pu.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://sl.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zt.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vi.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://bd.9csxet.cn

[B09] break 与 continue
来源：http://tc.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nn.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xg.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ty.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://si.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ro.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tg.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xd.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fs.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://tw.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gn.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://va.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tn.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yk.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ey.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tg.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://go.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pl.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://yu.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://ml.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://or.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wk.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ey.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://et.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hh.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://of.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xf.asd995.cn

[B12] 跳出多层循环
来源：http://nb.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dh.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ib.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hn.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oe.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xv.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mz.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uq.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kl.szxytkj.cn

[B13] 判断是否为数字
来源：http://pb.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://rt.nicolike.cn

PHP:  is_numeric($x)
来源：http://ra.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nr.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qn.gzmigu.cn

Java: x instanceof Number
来源：http://oy.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ee.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://kn.gzmigu.cn

C#:   x is int or double or decimal
来源：http://kt.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://to.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://au.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xd.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://at.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://dw.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rs.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pq.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gc.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vp.lnxyls.cn

[B15] 布尔运算与取反
来源：http://sw.9csxet.cn

Py:   a and b or not c
来源：http://bl.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://yz.panjiajie.cn

JS:   a && b || !c
来源：http://ee.shxzukj.cn

TS:   a && b || !c
来源：http://kt.huixiangedu.cn

Java: a && b || !c
来源：http://ef.yuexingan06.cn

Go:   a && b || !c
来源：http://bw.szxytkj.cn

Ruby: a && b || !c
来源：http://cl.shxzskj.cn

C#:   a && b || !c
来源：http://kh.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wh.szxytkj.cn

Py:   if not data: return
来源：http://er.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://kz.muxihuayi.cn

JS:   if (!data) return;
来源：http://gy.wgjwhj.cn

TS:   if (!data) return;
来源：http://st.huixiangedu.cn

Java: if (data == null) return;
来源：http://kz.nszjky.cn

Go:   if data == nil { return }
来源：http://dm.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://ab.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://ih.lnxyls.cn

================================================================================
来源：http://pe.szsharing.cn

C. 函数与作用域
来源：http://rm.jianghongdianzi.cn

================================================================================
来源：http://tz.wgjwhj.cn

[C01] 定义函数
来源：http://ck.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://tz.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://si.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://tw.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oe.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bd.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bm.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://vn.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qe.huixiangedu.cn

[C02] 默认参数
来源：http://xf.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://he.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ur.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://lm.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rq.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rm.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sy.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://rj.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://rn.szxytkj.cn

[C03] 可变参数
来源：http://nu.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://gw.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ws.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qa.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vs.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ym.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://do.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sx.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uo.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://ey.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zo.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://og.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://do.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sx.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://bu.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://cz.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://mx.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://xi.szsharing.cn

[C05] 返回多个值
来源：http://kt.nszjky.cn

Py:   return a, b
来源：http://mg.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://cq.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://to.yuexingan06.cn

TS:   return { a, b };
来源：http://qz.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gm.9csxet.cn

Go:   return a, b
来源：http://kr.bookmarksfly.cn

Ruby: return a, b
来源：http://vo.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://gw.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://kt.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ea.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://if.colortex.cn

JS:   const square = x => x * x;
来源：http://ow.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://wm.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://la.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oa.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://ma.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fv.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://ft.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zm.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sw.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aq.nicolike.cn

TS:   arr.map(String)
来源：http://tk.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eu.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hk.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://xt.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://th.shxzukj.cn

[C08] 闭包
来源：http://qs.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ix.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kv.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tz.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jo.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gh.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xg.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://op.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pv.chemitech.net.cn

[C09] 递归
来源：http://jn.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pd.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ns.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ii.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zt.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uh.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lb.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://th.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pe.newstarts.cn

[C10] 变量作用域
来源：http://js.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jg.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rm.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oi.colortex.cn

TS:   同 JS
来源：http://pt.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://sb.jctech888.com.cn

Go:   花括号块级作用域
来源：http://uk.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xx.shtwfgs.cn

C#:   块级作用域
来源：http://pk.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://ve.9csxet.cn

Py:   from module import func
来源：http://or.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mr.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wb.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wd.muxihuayi.cn

Java: import java.util.List;
来源：http://xd.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tz.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://yb.bjjhwx.cn

C#:   using System.Text;
来源：http://ci.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://uo.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://xm.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://wr.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://as.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://oa.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hx.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://rz.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://pv.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lv.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://rk.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://px.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dz.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fh.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ts.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tp.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://gf.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wm.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sk.jctech888.com.cn

[C14] 泛型函数
来源：http://ic.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gk.9csxet.cn

PHP:  // 无泛型
来源：http://iu.jianghongdianzi.cn

JS:   // 无泛型
来源：http://dn.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nc.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zi.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://es.muxihuayi.cn

Ruby: # 无泛型
来源：http://gw.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wu.colortex.cn

[C15] 解构 / 展开参数
来源：http://ul.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dv.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://rg.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ak.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bm.shtwfgs.cn

Java: // 无解构
来源：http://sy.wgjwhj.cn

Go:   // 无解构
来源：http://ww.9csxet.cn

Ruby: a, b = pair
来源：http://ev.szsharing.cn

C#:   var (a, b) = pair;
来源：http://ai.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://tz.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ry.yuntaijiaju.cn

PHP:  // 无重载
来源：http://ng.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qv.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://zm.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rg.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://ax.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://hz.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hy.hahajie.cn

================================================================================
来源：http://ua.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://dn.wgjwhj.cn

================================================================================
来源：http://ff.9csxet.cn

[D01] 创建数组 / 列表
来源：http://mu.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eb.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tr.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oh.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rm.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nf.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://xk.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://pk.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://en.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://bi.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://os.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vh.newstarts.cn

JS:   arr.push(4);
来源：http://kl.jctech888.com.cn

TS:   arr.push(4);
来源：http://sy.colortex.cn

Java: list.add(4);
来源：http://ty.521024.cn

Go:   arr = append(arr, 4)
来源：http://wj.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://jn.shtwfgs.cn

C#:   list.Add(4);
来源：http://oh.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ix.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://sb.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rc.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ev.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://jh.wgjwhj.cn

Java: list.add(0, 0);
来源：http://zy.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ll.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nc.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://kn.wgjwhj.cn

[D04] 删除元素
来源：http://li.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fv.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ev.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lt.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://en.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cd.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gy.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nk.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://js.muxihuayi.cn

[D05] 访问与修改元素
来源：http://te.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qk.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wq.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ej.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://sc.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://ej.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://go.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zk.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bz.wgjwhj.cn

[D06] 数组长度
来源：http://do.newstarts.cn

Py:   len(arr)
来源：http://dr.haigaiapp.cn

PHP:  count($arr);
来源：http://gk.chemitech.net.cn

JS:   arr.length
来源：http://sg.jctech888.com.cn

TS:   arr.length
来源：http://ny.shxzskj.cn

Java: list.size();
来源：http://xs.newstarts.cn

Go:   len(arr)
来源：http://ho.9csxet.cn

Ruby: arr.length; arr.size
来源：http://mw.asd995.cn

C#:   list.Count;
来源：http://jg.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://gy.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kj.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fe.asd995.cn

JS:   arr.slice(1, 4);
来源：http://ay.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://kx.colortex.cn

Java: list.subList(1, 4);
来源：http://ux.nszjky.cn

Go:   arr[1:4]
来源：http://bd.nicolike.cn

Ruby: arr[1, 3]
来源：http://fr.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://xu.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://ge.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://af.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://ib.hnjuh.cn


<!-- 参考信息 -->