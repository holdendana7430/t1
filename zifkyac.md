代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://jv.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://it.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://on.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://zd.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ef.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ch.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://am.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ct.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oc.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://du.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ge.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ay.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cp.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://az.huixiangedu.cn

[B07] while 循环
来源：http://tg.szsharing.cn

Py:   while i < 10: i += 1
来源：http://jc.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zq.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://yt.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://yv.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://bc.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ve.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://mb.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://lv.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://kc.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://tn.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ku.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://sg.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://zi.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://in.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ve.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iy.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://lf.hnjuh.cn

[B09] break 与 continue
来源：http://bj.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ih.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pe.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://on.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pv.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gt.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nx.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uu.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://ir.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lk.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oi.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xu.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vw.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nr.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vo.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jm.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dp.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://rm.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://bx.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://ic.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ro.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://so.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ni.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rg.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://vd.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tj.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://wi.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eg.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sa.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wj.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://su.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hl.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bq.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tw.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cg.jctech888.com.cn

[B13] 判断是否为数字
来源：http://yg.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://uq.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://ne.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nv.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pj.asd995.cn

Java: x instanceof Number
来源：http://so.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tn.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://qq.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://cm.521024.cn

[B14] 判断值是否在集合内
来源：http://iy.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://os.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xw.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://ft.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://wa.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ry.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://us.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wf.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bh.newstarts.cn

[B15] 布尔运算与取反
来源：http://qp.shxzskj.cn

Py:   a and b or not c
来源：http://ap.nszjky.cn

PHP:  $a && $b || !$c
来源：http://jz.hahajie.cn

JS:   a && b || !c
来源：http://ko.hahajie.cn

TS:   a && b || !c
来源：http://hr.bjjhwx.cn

Java: a && b || !c
来源：http://mb.asd995.cn

Go:   a && b || !c
来源：http://vo.bookmarksfly.cn

Ruby: a && b || !c
来源：http://wr.521024.cn

C#:   a && b || !c
来源：http://th.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tp.huanxung.cn

Py:   if not data: return
来源：http://hr.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://ny.shtwfgs.cn

JS:   if (!data) return;
来源：http://or.newstarts.cn

TS:   if (!data) return;
来源：http://ij.haigaiapp.cn

Java: if (data == null) return;
来源：http://lv.panjiajie.cn

Go:   if data == nil { return }
来源：http://ff.haigaiapp.cn

Ruby: return if data.nil?
来源：http://ar.lnxyls.cn

C#:   if (data == null) return;
来源：http://pu.hnjuh.cn

================================================================================
来源：http://xe.szxytkj.cn

C. 函数与作用域
来源：http://yo.nszjky.cn

================================================================================
来源：http://ek.newstarts.cn

[C01] 定义函数
来源：http://gu.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://ty.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gw.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://mu.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://np.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yn.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vr.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://rt.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bg.9csxet.cn

[C02] 默认参数
来源：http://cx.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://fv.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ic.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://od.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jq.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yp.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iq.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://va.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://gh.wgjwhj.cn

[C03] 可变参数
来源：http://vh.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://be.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fg.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tf.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jv.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vg.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qb.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://km.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fm.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://al.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vn.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uv.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ke.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fi.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://xp.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://md.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://wi.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://go.huixinmuqiang.cn

[C05] 返回多个值
来源：http://db.huixinmuqiang.cn

Py:   return a, b
来源：http://if.szsharing.cn

PHP:  return [$a, $b];
来源：http://yb.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oi.jctech888.com.cn

TS:   return { a, b };
来源：http://sw.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iv.hahajie.cn

Go:   return a, b
来源：http://uj.bjjhwx.cn

Ruby: return a, b
来源：http://ld.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://vb.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://ho.newstarts.cn

Py:   square = lambda x: x * x
来源：http://uc.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://be.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://xy.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://qb.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lt.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zl.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://kt.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xn.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://lk.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bc.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pn.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zf.shxzukj.cn

TS:   arr.map(String)
来源：http://xp.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jt.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://so.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://pf.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ea.szsharing.cn

[C08] 闭包
来源：http://rb.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ym.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ld.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rw.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gg.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rr.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bm.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sg.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jz.lnxyls.cn

[C09] 递归
来源：http://mw.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jm.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ki.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rv.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zh.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yz.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qk.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://od.nszjky.cn

[C10] 变量作用域
来源：http://dh.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rf.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lw.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zj.huixinmuqiang.cn

TS:   同 JS
来源：http://bb.asd995.cn

Java: 方法内为块级作用域
来源：http://fa.lnxyls.cn

Go:   花括号块级作用域
来源：http://um.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qz.lnxyls.cn

C#:   块级作用域
来源：http://kd.hnjuh.cn

[C11] 模块导入与导出
来源：http://ek.huanxung.cn

Py:   from module import func
来源：http://cj.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vr.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uj.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ip.asd995.cn

Java: import java.util.List;
来源：http://qh.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://no.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://xk.colortex.cn

C#:   using System.Text;
来源：http://cn.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://op.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://hp.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://ff.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://hr.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://xy.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qq.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://pd.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://nd.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ng.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://jl.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xk.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://za.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ki.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jo.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lb.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://yo.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hr.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://aq.yuntaijiaju.cn

[C14] 泛型函数
来源：http://tb.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vr.muxihuayi.cn

PHP:  // 无泛型
来源：http://pd.muxihuayi.cn

JS:   // 无泛型
来源：http://ie.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ai.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ub.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tb.nszjky.cn

Ruby: # 无泛型
来源：http://pq.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jo.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://ay.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://it.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://hk.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uv.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pn.shtwfgs.cn

Java: // 无解构
来源：http://ck.lnxyls.cn

Go:   // 无解构
来源：http://co.shxzskj.cn

Ruby: a, b = pair
来源：http://hj.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://lh.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://vx.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gt.bjjhwx.cn

PHP:  // 无重载
来源：http://ot.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fe.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ce.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://og.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://fp.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://jy.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mi.521024.cn

================================================================================
来源：http://ex.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://lz.muxihuayi.cn

================================================================================
来源：http://an.9csxet.cn

[D01] 创建数组 / 列表
来源：http://ya.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ok.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tx.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yg.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ey.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pt.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://vs.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://ot.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bc.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://dh.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lp.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hm.chemitech.net.cn

JS:   arr.push(4);
来源：http://nk.chemitech.net.cn

TS:   arr.push(4);
来源：http://xx.shxzukj.cn

Java: list.add(4);
来源：http://to.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://dk.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://el.huanxung.cn

C#:   list.Add(4);
来源：http://wu.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://yx.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://ce.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://la.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tg.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://rm.521024.cn

Java: list.add(0, 0);
来源：http://ex.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tv.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hy.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://up.asd995.cn

[D04] 删除元素
来源：http://gz.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qq.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rx.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yo.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://om.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jg.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iv.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qf.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sy.nicolike.cn

[D05] 访问与修改元素
来源：http://ey.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mt.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eu.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xa.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://hp.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://ly.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://dc.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uo.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yx.521024.cn

[D06] 数组长度
来源：http://bm.521024.cn


<!-- 参考信息 -->