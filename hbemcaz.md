代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iu.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hi.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vd.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yi.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oa.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sc.shxzukj.cn

[B07] while 循环
来源：http://fx.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://xa.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ta.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://zv.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://bx.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://rv.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sh.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://dv.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://sv.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://ik.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://el.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ks.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://aj.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://qu.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://rb.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yq.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gr.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://hi.panjiajie.cn

[B09] break 与 continue
来源：http://ry.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jo.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qj.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kh.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lt.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uo.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uq.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eh.huanxung.cn

[B10] 遍历同时拿索引
来源：http://rr.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pj.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gj.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://je.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qm.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://za.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jp.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ay.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ln.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://uk.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://qh.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://or.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xv.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ki.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xr.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tp.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://ss.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qw.muxihuayi.cn

[B12] 跳出多层循环
来源：http://hh.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rd.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vt.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rp.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xl.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ts.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ii.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zf.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ud.bjjhwx.cn

[B13] 判断是否为数字
来源：http://xa.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://rz.huanxung.cn

PHP:  is_numeric($x)
来源：http://sp.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bn.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pr.wgjwhj.cn

Java: x instanceof Number
来源：http://my.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ql.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://rp.szsharing.cn

C#:   x is int or double or decimal
来源：http://yp.hahajie.cn

[B14] 判断值是否在集合内
来源：http://wl.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tq.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hn.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://rk.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://zr.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qj.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hp.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pj.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uz.nszjky.cn

[B15] 布尔运算与取反
来源：http://cp.bjjhwx.cn

Py:   a and b or not c
来源：http://vt.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://pw.szsharing.cn

JS:   a && b || !c
来源：http://xl.nszjky.cn

TS:   a && b || !c
来源：http://gy.521024.cn

Java: a && b || !c
来源：http://nc.huanxung.cn

Go:   a && b || !c
来源：http://nz.huanxung.cn

Ruby: a && b || !c
来源：http://hp.hahajie.cn

C#:   a && b || !c
来源：http://kx.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ea.chemitech.net.cn

Py:   if not data: return
来源：http://oc.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://as.colortex.cn

JS:   if (!data) return;
来源：http://mm.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://xw.asd995.cn

Java: if (data == null) return;
来源：http://al.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://ht.szxytkj.cn

Ruby: return if data.nil?
来源：http://nq.hahajie.cn

C#:   if (data == null) return;
来源：http://db.shtwfgs.cn

================================================================================
来源：http://eg.szsharing.cn

C. 函数与作用域
来源：http://dm.muxihuayi.cn

================================================================================
来源：http://al.hahajie.cn

[C01] 定义函数
来源：http://vc.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://wi.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kf.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://sv.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tw.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://la.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://at.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://ii.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hd.yuexingan06.cn

[C02] 默认参数
来源：http://hv.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://kw.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bs.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://kz.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sw.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ty.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xp.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://jl.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ql.bjjhwx.cn

[C03] 可变参数
来源：http://gl.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://xh.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ub.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rw.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yk.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qg.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zi.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rl.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ye.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://bw.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nk.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wd.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wc.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qf.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://wd.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://as.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://mt.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://gx.shtwfgs.cn

[C05] 返回多个值
来源：http://nh.bookmarksfly.cn

Py:   return a, b
来源：http://ki.lnxyls.cn

PHP:  return [$a, $b];
来源：http://zc.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ru.shxzukj.cn

TS:   return { a, b };
来源：http://rv.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ix.bookmarksfly.cn

Go:   return a, b
来源：http://xe.jctech888.com.cn

Ruby: return a, b
来源：http://pp.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://xq.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://sj.521024.cn

Py:   square = lambda x: x * x
来源：http://qb.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ez.hahajie.cn

JS:   const square = x => x * x;
来源：http://xm.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://et.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://en.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bv.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://og.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oa.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://kp.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xy.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ar.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bw.521024.cn

TS:   arr.map(String)
来源：http://hi.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gm.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zm.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://uo.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cz.bookmarksfly.cn

[C08] 闭包
来源：http://ho.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qi.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zm.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wh.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ih.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aa.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fn.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://un.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wd.jctech888.com.cn

[C09] 递归
来源：http://wj.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xb.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dt.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lv.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rt.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rk.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pb.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jy.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dn.huanxung.cn

[C10] 变量作用域
来源：http://kp.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dz.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yk.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://be.huanxung.cn

TS:   同 JS
来源：http://cs.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://nr.chemitech.net.cn

Go:   花括号块级作用域
来源：http://fd.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://km.jctech888.com.cn

C#:   块级作用域
来源：http://sc.szsharing.cn

[C11] 模块导入与导出
来源：http://mh.shxzukj.cn

Py:   from module import func
来源：http://qk.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jb.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sy.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hy.gzmigu.cn

Java: import java.util.List;
来源：http://tk.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ru.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ud.shxzukj.cn

C#:   using System.Text;
来源：http://io.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://ws.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://zj.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://rt.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://mq.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://zp.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jx.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://nh.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://lp.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eo.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://dj.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jr.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zx.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kw.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zl.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mn.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://ub.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rn.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gs.yuexingan06.cn

[C14] 泛型函数
来源：http://sj.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wm.wgjwhj.cn

PHP:  // 无泛型
来源：http://sh.yuntaijiaju.cn

JS:   // 无泛型
来源：http://ub.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nx.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tw.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vs.bjjhwx.cn

Ruby: # 无泛型
来源：http://dl.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ec.nicolike.cn

[C15] 解构 / 展开参数
来源：http://wg.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yk.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://hh.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nj.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cw.bjjhwx.cn

Java: // 无解构
来源：http://po.wgjwhj.cn

Go:   // 无解构
来源：http://lz.huixiangedu.cn

Ruby: a, b = pair
来源：http://xx.521024.cn

C#:   var (a, b) = pair;
来源：http://te.hahajie.cn

[C16] 函数 / 方法重载
来源：http://jj.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zz.hnjuh.cn

PHP:  // 无重载
来源：http://xu.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tq.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ns.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kn.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://mx.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://ju.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gh.szsharing.cn

================================================================================
来源：http://im.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://jc.huixiangedu.cn

================================================================================
来源：http://pz.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://tb.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pk.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sk.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jc.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lw.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aw.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://bj.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://tu.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ym.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://oz.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wn.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ik.shtwfgs.cn

JS:   arr.push(4);
来源：http://qe.shxzukj.cn

TS:   arr.push(4);
来源：http://qw.lnxyls.cn

Java: list.add(4);
来源：http://yz.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://pe.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://rc.lnxyls.cn

C#:   list.Add(4);
来源：http://qg.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://ra.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://xy.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dt.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wl.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://yi.yuexingan06.cn

Java: list.add(0, 0);
来源：http://dp.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yj.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://md.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://ej.hahajie.cn

[D04] 删除元素
来源：http://dg.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pn.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sd.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hy.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://ur.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://up.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cf.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sd.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nm.shtwfgs.cn

[D05] 访问与修改元素
来源：http://af.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nz.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nj.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kj.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://rf.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://tm.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://my.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ep.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cv.nicolike.cn

[D06] 数组长度
来源：http://qn.huixinmuqiang.cn

Py:   len(arr)
来源：http://ev.shxzskj.cn

PHP:  count($arr);
来源：http://di.hahajie.cn

JS:   arr.length
来源：http://ge.9csxet.cn

TS:   arr.length
来源：http://nf.szxytkj.cn

Java: list.size();
来源：http://xd.shxzskj.cn

Go:   len(arr)
来源：http://dy.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://pd.panjiajie.cn

C#:   list.Count;
来源：http://wj.colortex.cn


<!-- 参考信息 -->