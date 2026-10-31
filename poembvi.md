代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jx.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://iz.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jd.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qg.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nr.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hc.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tu.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hj.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dx.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://it.jctech888.com.cn

[B07] while 循环
来源：http://hn.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://ea.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gi.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://me.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://ws.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://uh.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://je.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://oj.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://dh.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://aa.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://id.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rt.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://kg.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://sm.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://md.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pd.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://na.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://rv.9csxet.cn

[B09] break 与 continue
来源：http://rm.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kk.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bx.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kd.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vi.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zw.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kj.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://zg.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jm.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jx.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cd.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ga.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://np.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wy.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hs.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://it.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://rz.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://na.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://gd.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ri.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gk.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dc.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uf.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://uv.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pr.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ra.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xq.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mk.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oe.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cg.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hs.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bh.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://na.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hc.shtwfgs.cn

[B13] 判断是否为数字
来源：http://ag.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://vl.lnxyls.cn

PHP:  is_numeric($x)
来源：http://zo.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yy.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yr.bjjhwx.cn

Java: x instanceof Number
来源：http://ww.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xf.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://xj.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://qp.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://xr.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://un.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hf.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://pz.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://lo.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bf.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yz.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xq.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wh.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://sx.chemitech.net.cn

Py:   a and b or not c
来源：http://ev.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://nf.shxzskj.cn

JS:   a && b || !c
来源：http://au.nszjky.cn

TS:   a && b || !c
来源：http://kh.newstarts.cn

Java: a && b || !c
来源：http://vz.shtwfgs.cn

Go:   a && b || !c
来源：http://kz.shxzskj.cn

Ruby: a && b || !c
来源：http://et.hnjuh.cn

C#:   a && b || !c
来源：http://lt.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fb.szxytkj.cn

Py:   if not data: return
来源：http://xw.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://aj.hahajie.cn

JS:   if (!data) return;
来源：http://rv.chemitech.net.cn

TS:   if (!data) return;
来源：http://tb.colortex.cn

Java: if (data == null) return;
来源：http://fx.nszjky.cn

Go:   if data == nil { return }
来源：http://hj.chemitech.net.cn

Ruby: return if data.nil?
来源：http://bi.szsharing.cn

C#:   if (data == null) return;
来源：http://ih.hahajie.cn

================================================================================
来源：http://xy.gzmigu.cn

C. 函数与作用域
来源：http://ct.lnxyls.cn

================================================================================
来源：http://og.huixinmuqiang.cn

[C01] 定义函数
来源：http://qm.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://tc.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ev.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://sj.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lg.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yw.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kc.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://aj.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wq.hahajie.cn

[C02] 默认参数
来源：http://hy.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://jw.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qs.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://hv.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hl.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wj.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ws.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://nu.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://ga.asd995.cn

[C03] 可变参数
来源：http://ik.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://sj.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nr.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://db.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ty.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oh.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lj.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cy.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qc.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://ke.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nx.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fb.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ul.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gn.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://sv.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://nc.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://ly.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://bt.huanxung.cn

[C05] 返回多个值
来源：http://gy.shtwfgs.cn

Py:   return a, b
来源：http://ec.huanxung.cn

PHP:  return [$a, $b];
来源：http://mh.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jb.huanxung.cn

TS:   return { a, b };
来源：http://uz.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yz.szxytkj.cn

Go:   return a, b
来源：http://ot.yuntaijiaju.cn

Ruby: return a, b
来源：http://fh.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://wb.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://ki.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://gg.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ca.asd995.cn

JS:   const square = x => x * x;
来源：http://ly.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://cv.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ny.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rx.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://ih.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cf.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://qc.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yo.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nb.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sm.bookmarksfly.cn

TS:   arr.map(String)
来源：http://qk.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rn.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ze.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://rx.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mj.yuexingan06.cn

[C08] 闭包
来源：http://wl.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lw.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pw.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tg.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ew.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kr.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ei.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ex.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://py.szsharing.cn

[C09] 递归
来源：http://ei.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uo.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yi.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hd.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cx.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uy.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xj.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kj.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jk.521024.cn

[C10] 变量作用域
来源：http://mn.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wf.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ml.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fj.hnjuh.cn

TS:   同 JS
来源：http://lg.nszjky.cn

Java: 方法内为块级作用域
来源：http://rr.muxihuayi.cn

Go:   花括号块级作用域
来源：http://et.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ja.lnxyls.cn

C#:   块级作用域
来源：http://jh.asd995.cn

[C11] 模块导入与导出
来源：http://mf.9csxet.cn

Py:   from module import func
来源：http://xe.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://li.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jp.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ia.chemitech.net.cn

Java: import java.util.List;
来源：http://lp.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uy.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://dz.huixiangedu.cn

C#:   using System.Text;
来源：http://nm.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://wa.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://tg.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://cn.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://qz.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://pi.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ro.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://so.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://aw.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bh.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://cl.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yh.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qu.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cj.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cw.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mv.nicolike.cn

Go:   func add(a, b int) int
来源：http://nu.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kt.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yn.521024.cn

[C14] 泛型函数
来源：http://lk.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nh.haigaiapp.cn

PHP:  // 无泛型
来源：http://id.szsharing.cn

JS:   // 无泛型
来源：http://wg.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xi.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://no.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vm.haigaiapp.cn

Ruby: # 无泛型
来源：http://jx.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wo.colortex.cn

[C15] 解构 / 展开参数
来源：http://us.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xp.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://vd.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zb.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sg.hnjuh.cn

Java: // 无解构
来源：http://yr.521024.cn

Go:   // 无解构
来源：http://zj.yuexingan06.cn

Ruby: a, b = pair
来源：http://we.asd995.cn

C#:   var (a, b) = pair;
来源：http://lh.521024.cn

[C16] 函数 / 方法重载
来源：http://qs.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vs.newstarts.cn

PHP:  // 无重载
来源：http://bx.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tj.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://vd.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xv.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://vk.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://zb.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vx.huixiangedu.cn

================================================================================
来源：http://fn.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://sj.huixinmuqiang.cn

================================================================================
来源：http://gp.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://bx.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gk.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ti.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nt.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xx.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oz.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://mn.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://wf.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sr.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://mc.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ad.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kc.shtwfgs.cn

JS:   arr.push(4);
来源：http://pi.haigaiapp.cn

TS:   arr.push(4);
来源：http://co.panjiajie.cn

Java: list.add(4);
来源：http://iq.521024.cn

Go:   arr = append(arr, 4)
来源：http://wx.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://mj.szsharing.cn

C#:   list.Add(4);
来源：http://kw.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://ka.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://tq.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ny.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xj.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://so.jctech888.com.cn

Java: list.add(0, 0);
来源：http://qj.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zz.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://km.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://wm.haigaiapp.cn

[D04] 删除元素
来源：http://br.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mi.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vf.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bl.asd995.cn

TS:   arr.splice(0, 1);
来源：http://qw.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tw.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qn.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qa.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ni.szsharing.cn

[D05] 访问与修改元素
来源：http://yq.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kh.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ic.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rl.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://vu.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://do.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://wj.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kj.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ky.jianghongdianzi.cn

[D06] 数组长度
来源：http://xw.bjjhwx.cn

Py:   len(arr)
来源：http://xf.colortex.cn

PHP:  count($arr);
来源：http://ep.bjjhwx.cn

JS:   arr.length
来源：http://hv.szsharing.cn

TS:   arr.length
来源：http://do.yuntaijiaju.cn


<!-- 参考信息 -->