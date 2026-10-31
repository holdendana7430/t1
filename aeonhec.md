代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lj.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://ga.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://yj.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://sp.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://fp.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xh.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://tk.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://mu.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://ji.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ta.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rr.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://gz.yuexingan06.cn

[B09] break 与 continue
来源：http://mm.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hj.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hk.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ux.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ff.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ap.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zh.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://al.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eh.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://mo.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tk.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hq.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://an.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bs.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yg.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oi.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gf.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nc.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://op.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://ni.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://qk.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kr.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aa.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aq.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cp.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://rc.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xe.521024.cn

[B12] 跳出多层循环
来源：http://ty.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://co.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cs.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bx.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://se.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sq.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uj.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wa.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://me.521024.cn

[B13] 判断是否为数字
来源：http://tn.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://rf.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://we.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aa.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wr.huixinmuqiang.cn

Java: x instanceof Number
来源：http://qs.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ge.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://vs.lnxyls.cn

C#:   x is int or double or decimal
来源：http://gk.nszjky.cn

[B14] 判断值是否在集合内
来源：http://zq.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fm.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jr.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://jc.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://lo.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zt.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bh.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://th.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yo.nicolike.cn

[B15] 布尔运算与取反
来源：http://xa.521024.cn

Py:   a and b or not c
来源：http://ma.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://xp.nicolike.cn

JS:   a && b || !c
来源：http://ld.panjiajie.cn

TS:   a && b || !c
来源：http://yn.wgjwhj.cn

Java: a && b || !c
来源：http://lu.shxzukj.cn

Go:   a && b || !c
来源：http://vc.gzmigu.cn

Ruby: a && b || !c
来源：http://wv.bjjhwx.cn

C#:   a && b || !c
来源：http://tz.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rl.shxzskj.cn

Py:   if not data: return
来源：http://re.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://am.chemitech.net.cn

JS:   if (!data) return;
来源：http://ns.jctech888.com.cn

TS:   if (!data) return;
来源：http://qb.shtwfgs.cn

Java: if (data == null) return;
来源：http://eh.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://de.shxzukj.cn

Ruby: return if data.nil?
来源：http://uv.chemitech.net.cn

C#:   if (data == null) return;
来源：http://ko.9csxet.cn

================================================================================
来源：http://bw.9csxet.cn

C. 函数与作用域
来源：http://af.huixiangedu.cn

================================================================================
来源：http://yk.bjjhwx.cn

[C01] 定义函数
来源：http://tn.asd995.cn

Py:   def add(a, b): return a + b
来源：http://ar.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sz.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://uj.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://us.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uw.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ho.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://dk.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ey.nszjky.cn

[C02] 默认参数
来源：http://zs.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://gu.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://au.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://mz.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yt.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rr.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://go.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://rs.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ha.nicolike.cn

[C03] 可变参数
来源：http://es.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://ol.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ov.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xw.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pq.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hr.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://po.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ye.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iu.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://vn.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xo.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nn.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bs.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xd.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://ct.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://dk.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://wf.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://sz.wgjwhj.cn

[C05] 返回多个值
来源：http://qc.szsharing.cn

Py:   return a, b
来源：http://yg.panjiajie.cn

PHP:  return [$a, $b];
来源：http://gv.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nv.9csxet.cn

TS:   return { a, b };
来源：http://hp.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qn.nicolike.cn

Go:   return a, b
来源：http://wl.nicolike.cn

Ruby: return a, b
来源：http://va.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://to.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://cw.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://am.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vg.colortex.cn

JS:   const square = x => x * x;
来源：http://bb.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://tm.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yq.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rj.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://ry.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mv.asd995.cn

[C07] 把函数作为参数传入
来源：http://uk.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://an.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mx.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jt.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://xb.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wj.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oq.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://yc.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dp.colortex.cn

[C08] 闭包
来源：http://nf.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lq.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ji.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ny.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sh.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://de.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vj.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eg.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lf.wgjwhj.cn

[C09] 递归
来源：http://ow.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jp.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ij.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lv.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://to.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oo.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ri.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mv.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ub.gzmigu.cn

[C10] 变量作用域
来源：http://fs.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rf.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ec.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pj.hahajie.cn

TS:   同 JS
来源：http://ts.szsharing.cn

Java: 方法内为块级作用域
来源：http://uw.newstarts.cn

Go:   花括号块级作用域
来源：http://kr.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ew.wgjwhj.cn

C#:   块级作用域
来源：http://gg.colortex.cn

[C11] 模块导入与导出
来源：http://qu.yuntaijiaju.cn

Py:   from module import func
来源：http://nv.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ee.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ox.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://su.haigaiapp.cn

Java: import java.util.List;
来源：http://jv.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rj.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://mp.bjjhwx.cn

C#:   using System.Text;
来源：http://ze.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://uv.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://ff.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://jb.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://wr.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://cw.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://my.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://xn.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://ds.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wv.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://cj.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qg.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://od.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aa.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ou.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ne.huanxung.cn

Go:   func add(a, b int) int
来源：http://kn.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oc.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fg.newstarts.cn

[C14] 泛型函数
来源：http://ux.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ff.bjjhwx.cn

PHP:  // 无泛型
来源：http://uj.9csxet.cn

JS:   // 无泛型
来源：http://fl.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mf.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jf.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tx.shxzskj.cn

Ruby: # 无泛型
来源：http://yp.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jw.asd995.cn

[C15] 解构 / 展开参数
来源：http://na.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aq.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://nv.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cv.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://em.shxzukj.cn

Java: // 无解构
来源：http://jm.chemitech.net.cn

Go:   // 无解构
来源：http://jn.wgjwhj.cn

Ruby: a, b = pair
来源：http://tl.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://pn.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://sh.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fc.bookmarksfly.cn

PHP:  // 无重载
来源：http://wb.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cd.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://yk.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pc.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://aq.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://lz.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ua.nszjky.cn

================================================================================
来源：http://fm.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://rh.yuntaijiaju.cn

================================================================================
来源：http://af.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://vv.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ss.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vh.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xg.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hc.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lg.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://ve.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://ic.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vg.huanxung.cn

[D02] 追加元素到末尾
来源：http://vu.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xo.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rp.huixiangedu.cn

JS:   arr.push(4);
来源：http://xf.hnjuh.cn

TS:   arr.push(4);
来源：http://ci.521024.cn

Java: list.add(4);
来源：http://vj.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://jl.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://kc.lnxyls.cn

C#:   list.Add(4);
来源：http://dx.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://jc.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://kx.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vg.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fg.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://ew.muxihuayi.cn

Java: list.add(0, 0);
来源：http://fr.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yv.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ng.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://xg.yuntaijiaju.cn

[D04] 删除元素
来源：http://si.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zz.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ui.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dp.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://rw.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rn.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wk.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://du.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nk.colortex.cn

[D05] 访问与修改元素
来源：http://cp.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://au.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ei.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nm.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://mf.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://hf.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://ho.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://so.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eh.asd995.cn

[D06] 数组长度
来源：http://ty.9csxet.cn

Py:   len(arr)
来源：http://vp.huixiangedu.cn

PHP:  count($arr);
来源：http://fi.nicolike.cn

JS:   arr.length
来源：http://pq.shxzskj.cn

TS:   arr.length
来源：http://cr.9csxet.cn

Java: list.size();
来源：http://ds.huixiangedu.cn

Go:   len(arr)
来源：http://fy.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://bk.shxzskj.cn

C#:   list.Count;
来源：http://vx.asd995.cn

[D07] 切片 / 取子数组
来源：http://ht.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cp.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ph.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://xm.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://zp.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://ni.asd995.cn

Go:   arr[1:4]
来源：http://lx.9csxet.cn

Ruby: arr[1, 3]
来源：http://lo.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://tx.szsharing.cn

[D08] 合并两个数组
来源：http://ab.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://cn.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://yh.huanxung.cn


<!-- 参考信息 -->