代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gm.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://sh.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lg.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ec.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fr.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sb.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vj.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rq.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://da.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kb.huixiangedu.cn

[B07] while 循环
来源：http://mw.nicolike.cn

Py:   while i < 10: i += 1
来源：http://rm.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ze.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://ct.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://le.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://nm.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qr.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://zw.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://nx.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://mq.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://jn.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qw.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://gr.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://gv.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://pm.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zm.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hr.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://rj.muxihuayi.cn

[B09] break 与 continue
来源：http://zn.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://we.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bz.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://os.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yc.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bl.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kx.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hv.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aj.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://hm.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://on.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dm.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dm.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ka.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gq.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zj.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xv.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wu.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://wi.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://ri.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://is.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zo.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cb.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cx.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://no.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://rf.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sr.wgjwhj.cn

[B12] 跳出多层循环
来源：http://hw.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lc.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mk.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vx.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gi.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wx.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zj.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ak.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cr.gzmigu.cn

[B13] 判断是否为数字
来源：http://ja.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://nw.9csxet.cn

PHP:  is_numeric($x)
来源：http://cs.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rp.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rw.muxihuayi.cn

Java: x instanceof Number
来源：http://ls.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zf.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://kr.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://il.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://rw.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dt.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ee.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://qg.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://tr.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jw.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rw.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pl.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iw.lnxyls.cn

[B15] 布尔运算与取反
来源：http://ya.szxytkj.cn

Py:   a and b or not c
来源：http://lz.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://xz.521024.cn

JS:   a && b || !c
来源：http://eh.newstarts.cn

TS:   a && b || !c
来源：http://ze.lnxyls.cn

Java: a && b || !c
来源：http://ba.wgjwhj.cn

Go:   a && b || !c
来源：http://wi.shxzukj.cn

Ruby: a && b || !c
来源：http://aq.panjiajie.cn

C#:   a && b || !c
来源：http://dz.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mg.yuntaijiaju.cn

Py:   if not data: return
来源：http://uk.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://wr.chemitech.net.cn

JS:   if (!data) return;
来源：http://yq.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://bv.shtwfgs.cn

Java: if (data == null) return;
来源：http://re.wgjwhj.cn

Go:   if data == nil { return }
来源：http://yz.colortex.cn

Ruby: return if data.nil?
来源：http://rh.hnjuh.cn

C#:   if (data == null) return;
来源：http://xd.nicolike.cn

================================================================================
来源：http://im.yuexingan06.cn

C. 函数与作用域
来源：http://oi.bookmarksfly.cn

================================================================================
来源：http://qb.szxytkj.cn

[C01] 定义函数
来源：http://rs.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://tu.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zx.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://pt.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sq.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gd.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vz.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://lm.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mt.hahajie.cn

[C02] 默认参数
来源：http://fp.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://qr.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tv.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://qo.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fx.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qr.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gx.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://zs.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://vi.nszjky.cn

[C03] 可变参数
来源：http://ks.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://mo.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://po.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yu.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ek.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://az.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qw.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rh.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://us.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://ny.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yx.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kj.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gc.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zf.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ip.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://ik.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://sl.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://zb.szxytkj.cn

[C05] 返回多个值
来源：http://mt.bjjhwx.cn

Py:   return a, b
来源：http://qg.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://me.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cr.nicolike.cn

TS:   return { a, b };
来源：http://pp.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gz.lnxyls.cn

Go:   return a, b
来源：http://mn.yuexingan06.cn

Ruby: return a, b
来源：http://qm.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://hx.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://qj.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://tb.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yi.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://dg.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ru.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yx.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rv.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://fg.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dn.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://xf.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kh.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zc.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pl.bjjhwx.cn

TS:   arr.map(String)
来源：http://fd.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vj.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jj.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://yb.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wz.shxzskj.cn

[C08] 闭包
来源：http://eq.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zz.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oi.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qr.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sf.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ci.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zi.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ac.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rt.yuntaijiaju.cn

[C09] 递归
来源：http://oi.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://er.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ly.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xc.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://px.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ax.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xx.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xy.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gd.shxzukj.cn

[C10] 变量作用域
来源：http://wa.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ig.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ln.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nr.haigaiapp.cn

TS:   同 JS
来源：http://wn.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://jn.szsharing.cn

Go:   花括号块级作用域
来源：http://ua.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://id.wgjwhj.cn

C#:   块级作用域
来源：http://fw.yuexingan06.cn

[C11] 模块导入与导出
来源：http://hx.newstarts.cn

Py:   from module import func
来源：http://st.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ji.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vn.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xp.jctech888.com.cn

Java: import java.util.List;
来源：http://nl.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xk.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://yk.jctech888.com.cn

C#:   using System.Text;
来源：http://sc.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://jk.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://rd.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://lp.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://ss.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://cx.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uh.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://sh.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://if.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kc.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://um.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ps.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ea.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xb.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fl.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://si.lnxyls.cn

Go:   func add(a, b int) int
来源：http://ax.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eo.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://se.szsharing.cn

[C14] 泛型函数
来源：http://te.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://my.521024.cn

PHP:  // 无泛型
来源：http://ml.jianghongdianzi.cn

JS:   // 无泛型
来源：http://dh.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://po.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sr.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://be.yuexingan06.cn

Ruby: # 无泛型
来源：http://lh.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qv.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://lt.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qq.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://dj.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sk.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bf.9csxet.cn

Java: // 无解构
来源：http://kd.colortex.cn

Go:   // 无解构
来源：http://sc.hahajie.cn

Ruby: a, b = pair
来源：http://ed.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://lw.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://vi.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wc.huanxung.cn

PHP:  // 无重载
来源：http://bn.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dt.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://gm.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ne.521024.cn

Go:   // 无重载：用不同函数名
来源：http://he.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://md.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hb.yuexingan06.cn

================================================================================
来源：http://jt.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://cz.wgjwhj.cn

================================================================================
来源：http://ot.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://xa.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://be.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dy.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zb.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jv.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bz.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://np.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://tn.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ph.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://om.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qy.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pb.muxihuayi.cn

JS:   arr.push(4);
来源：http://ya.9csxet.cn

TS:   arr.push(4);
来源：http://kn.shxzskj.cn

Java: list.add(4);
来源：http://mz.asd995.cn

Go:   arr = append(arr, 4)
来源：http://aj.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://pk.jctech888.com.cn

C#:   list.Add(4);
来源：http://qj.szsharing.cn

[D03] 在指定位置插入元素
来源：http://rc.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://zr.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://it.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wo.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://qp.newstarts.cn

Java: list.add(0, 0);
来源：http://ro.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://du.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ws.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://tc.chemitech.net.cn

[D04] 删除元素
来源：http://pw.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xd.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gf.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wh.asd995.cn

TS:   arr.splice(0, 1);
来源：http://eo.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bi.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qm.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jj.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rb.shxzukj.cn

[D05] 访问与修改元素
来源：http://ke.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wp.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vp.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mn.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://pq.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://uv.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ti.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sk.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ct.jctech888.com.cn

[D06] 数组长度
来源：http://tq.newstarts.cn

Py:   len(arr)
来源：http://nf.jctech888.com.cn

PHP:  count($arr);
来源：http://cz.jianghongdianzi.cn

JS:   arr.length
来源：http://zw.nicolike.cn

TS:   arr.length
来源：http://zq.gzmigu.cn


<!-- 参考信息 -->