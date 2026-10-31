代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sy.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eh.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bx.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nf.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pu.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://re.huixiangedu.cn

[B07] while 循环
来源：http://ze.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://wu.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dt.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://yi.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://ze.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://hy.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pt.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://qw.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://pe.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ik.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://fy.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dj.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://vh.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://wa.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://or.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lr.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://th.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://kc.asd995.cn

[B09] break 与 continue
来源：http://co.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wb.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eg.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nl.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wo.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oj.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://du.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ea.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mk.colortex.cn

[B10] 遍历同时拿索引
来源：http://up.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vf.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wr.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://he.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lc.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mo.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gj.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tu.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://db.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://ri.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://th.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://gg.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ui.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cq.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://th.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tx.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://vq.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cl.asd995.cn

[B12] 跳出多层循环
来源：http://go.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tw.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sq.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nb.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tg.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gv.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ky.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ll.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vs.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://wy.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://hc.szxytkj.cn

PHP:  is_numeric($x)
来源：http://kg.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bq.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gh.gzmigu.cn

Java: x instanceof Number
来源：http://re.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ss.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://hz.521024.cn

C#:   x is int or double or decimal
来源：http://rk.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://hf.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oh.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ml.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://gs.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://fp.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ob.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://px.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://be.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jz.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://yq.huanxung.cn

Py:   a and b or not c
来源：http://oq.9csxet.cn

PHP:  $a && $b || !$c
来源：http://zb.haigaiapp.cn

JS:   a && b || !c
来源：http://bd.hnjuh.cn

TS:   a && b || !c
来源：http://zh.gzmigu.cn

Java: a && b || !c
来源：http://wl.szsharing.cn

Go:   a && b || !c
来源：http://mt.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://ae.jctech888.com.cn

C#:   a && b || !c
来源：http://ls.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://th.newstarts.cn

Py:   if not data: return
来源：http://oj.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://vi.szxytkj.cn

JS:   if (!data) return;
来源：http://nu.bjjhwx.cn

TS:   if (!data) return;
来源：http://ux.colortex.cn

Java: if (data == null) return;
来源：http://xs.colortex.cn

Go:   if data == nil { return }
来源：http://ol.hahajie.cn

Ruby: return if data.nil?
来源：http://pj.shxzskj.cn

C#:   if (data == null) return;
来源：http://vj.yuntaijiaju.cn

================================================================================
来源：http://gk.shxzskj.cn

C. 函数与作用域
来源：http://tc.colortex.cn

================================================================================
来源：http://wk.nicolike.cn

[C01] 定义函数
来源：http://iw.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://ms.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lm.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://gn.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jm.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yq.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xp.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://jh.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://po.huanxung.cn

[C02] 默认参数
来源：http://rs.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://wt.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yf.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://yx.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jy.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fc.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fs.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://gj.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ig.chemitech.net.cn

[C03] 可变参数
来源：http://xy.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://nm.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://or.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sr.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://le.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iw.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pz.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mc.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uj.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://ya.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nl.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ia.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ov.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nz.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://rp.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://bw.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://rt.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://mk.521024.cn

[C05] 返回多个值
来源：http://hv.huixinmuqiang.cn

Py:   return a, b
来源：http://yw.gzmigu.cn

PHP:  return [$a, $b];
来源：http://oy.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yu.asd995.cn

TS:   return { a, b };
来源：http://jp.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tv.shtwfgs.cn

Go:   return a, b
来源：http://bf.hnjuh.cn

Ruby: return a, b
来源：http://ap.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://uw.asd995.cn

[C06] 匿名函数 / lambda
来源：http://ac.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://gi.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wd.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://il.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://at.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hv.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yq.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ev.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tq.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://fi.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wf.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xy.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yy.bjjhwx.cn

TS:   arr.map(String)
来源：http://th.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://te.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nm.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://uu.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pw.nicolike.cn

[C08] 闭包
来源：http://vm.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hm.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gz.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oo.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ml.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://al.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kv.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bq.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bm.yuntaijiaju.cn

[C09] 递归
来源：http://hr.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zh.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://km.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://so.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lz.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rm.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zr.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yy.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://th.bookmarksfly.cn

[C10] 变量作用域
来源：http://ie.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oe.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lp.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://db.yuntaijiaju.cn

TS:   同 JS
来源：http://yp.szxytkj.cn

Java: 方法内为块级作用域
来源：http://qf.521024.cn

Go:   花括号块级作用域
来源：http://fd.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ft.bjjhwx.cn

C#:   块级作用域
来源：http://oj.shtwfgs.cn

[C11] 模块导入与导出
来源：http://xt.yuexingan06.cn

Py:   from module import func
来源：http://hq.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rb.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xn.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ew.bjjhwx.cn

Java: import java.util.List;
来源：http://iv.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ns.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://yo.newstarts.cn

C#:   using System.Text;
来源：http://jc.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://ma.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://sh.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://iy.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://ue.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://eo.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ht.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://hu.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://fl.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ze.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://ph.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qt.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vn.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xt.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vs.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cu.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://fy.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://as.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://of.huixiangedu.cn

[C14] 泛型函数
来源：http://yj.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bj.521024.cn

PHP:  // 无泛型
来源：http://ob.jianghongdianzi.cn

JS:   // 无泛型
来源：http://lr.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uo.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dd.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ix.521024.cn

Ruby: # 无泛型
来源：http://oa.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ga.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://yu.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tf.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://ag.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qr.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oo.colortex.cn

Java: // 无解构
来源：http://lf.shxzukj.cn

Go:   // 无解构
来源：http://lg.lnxyls.cn

Ruby: a, b = pair
来源：http://ht.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://gm.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://ji.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kj.nicolike.cn

PHP:  // 无重载
来源：http://by.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ds.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://im.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pg.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://zg.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://co.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fw.wgjwhj.cn

================================================================================
来源：http://el.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://ze.huanxung.cn

================================================================================
来源：http://al.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://pl.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wk.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gj.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ri.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tz.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mj.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://om.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://fz.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ja.colortex.cn

[D02] 追加元素到末尾
来源：http://lf.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://di.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ji.hahajie.cn

JS:   arr.push(4);
来源：http://st.colortex.cn

TS:   arr.push(4);
来源：http://ou.huixinmuqiang.cn

Java: list.add(4);
来源：http://yj.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://cf.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://be.shtwfgs.cn

C#:   list.Add(4);
来源：http://hz.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://wj.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://lu.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ze.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://np.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ct.huanxung.cn

Java: list.add(0, 0);
来源：http://dx.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rq.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zk.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://ac.asd995.cn

[D04] 删除元素
来源：http://bb.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xu.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kt.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ri.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://io.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hk.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lx.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hd.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rk.nicolike.cn

[D05] 访问与修改元素
来源：http://zo.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cr.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dc.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zt.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://nh.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://rv.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://qn.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eq.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zw.szxytkj.cn

[D06] 数组长度
来源：http://iv.huixiangedu.cn

Py:   len(arr)
来源：http://no.chemitech.net.cn

PHP:  count($arr);
来源：http://fz.lnxyls.cn

JS:   arr.length
来源：http://dq.szxytkj.cn

TS:   arr.length
来源：http://vx.bjjhwx.cn

Java: list.size();
来源：http://ku.nszjky.cn

Go:   len(arr)
来源：http://xq.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://wz.bjjhwx.cn

C#:   list.Count;
来源：http://ny.newstarts.cn


<!-- 参考信息 -->