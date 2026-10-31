代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hf.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://rp.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rm.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zy.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://di.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fz.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nu.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://sd.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lu.521024.cn

[B06] 遍历字典 / 对象
来源：http://ab.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wr.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ao.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xw.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ib.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://by.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xq.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fo.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uz.yuntaijiaju.cn

[B07] while 循环
来源：http://gb.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://uo.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dk.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://fr.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://ym.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://jc.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cu.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://wy.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://ro.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://na.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://st.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yp.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://fl.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://xw.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://uc.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vc.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tz.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://pd.bjjhwx.cn

[B09] break 与 continue
来源：http://da.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wl.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sf.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cv.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dw.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xa.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fe.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tg.9csxet.cn

[B10] 遍历同时拿索引
来源：http://gd.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jc.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oh.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wc.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oq.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ak.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ja.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wc.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yw.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://cv.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://bl.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://eg.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tv.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ln.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xc.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fy.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://gv.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xn.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://jk.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xr.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xz.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yk.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gi.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ad.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pf.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ut.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rd.szxytkj.cn

[B13] 判断是否为数字
来源：http://ee.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://bv.hahajie.cn

PHP:  is_numeric($x)
来源：http://pc.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://er.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ac.gzmigu.cn

Java: x instanceof Number
来源：http://xs.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xy.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://me.nszjky.cn

C#:   x is int or double or decimal
来源：http://mp.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://nj.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lc.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ka.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://vd.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://ha.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bw.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jw.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sk.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bq.panjiajie.cn

[B15] 布尔运算与取反
来源：http://jy.hahajie.cn

Py:   a and b or not c
来源：http://zk.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://kl.haigaiapp.cn

JS:   a && b || !c
来源：http://yk.jctech888.com.cn

TS:   a && b || !c
来源：http://xk.9csxet.cn

Java: a && b || !c
来源：http://zc.nszjky.cn

Go:   a && b || !c
来源：http://ae.huanxung.cn

Ruby: a && b || !c
来源：http://ne.bjjhwx.cn

C#:   a && b || !c
来源：http://id.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wu.nicolike.cn

Py:   if not data: return
来源：http://dp.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://na.9csxet.cn

JS:   if (!data) return;
来源：http://ak.gzmigu.cn

TS:   if (!data) return;
来源：http://hk.yuexingan06.cn

Java: if (data == null) return;
来源：http://yr.huanxung.cn

Go:   if data == nil { return }
来源：http://ry.9csxet.cn

Ruby: return if data.nil?
来源：http://up.huanxung.cn

C#:   if (data == null) return;
来源：http://se.muxihuayi.cn

================================================================================
来源：http://tt.newstarts.cn

C. 函数与作用域
来源：http://qa.newstarts.cn

================================================================================
来源：http://tp.haigaiapp.cn

[C01] 定义函数
来源：http://ym.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://pn.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fk.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://sk.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://db.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pz.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hg.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://wx.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dq.yuexingan06.cn

[C02] 默认参数
来源：http://gc.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://be.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qy.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://hi.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fy.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zk.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qg.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ts.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://dn.haigaiapp.cn

[C03] 可变参数
来源：http://yg.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://bp.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lo.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yq.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dg.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zz.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ay.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lv.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://it.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://lt.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://md.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ku.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jw.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ak.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://hi.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://pb.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://fq.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://ea.muxihuayi.cn

[C05] 返回多个值
来源：http://cn.colortex.cn

Py:   return a, b
来源：http://sb.gzmigu.cn

PHP:  return [$a, $b];
来源：http://vn.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qu.hahajie.cn

TS:   return { a, b };
来源：http://kq.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cb.huixiangedu.cn

Go:   return a, b
来源：http://xf.muxihuayi.cn

Ruby: return a, b
来源：http://jw.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://zx.asd995.cn

[C06] 匿名函数 / lambda
来源：http://xp.asd995.cn

Py:   square = lambda x: x * x
来源：http://rp.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://km.panjiajie.cn

JS:   const square = x => x * x;
来源：http://eh.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://au.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xp.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ut.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://td.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mw.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://bx.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://do.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mz.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kr.shtwfgs.cn

TS:   arr.map(String)
来源：http://xy.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vq.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ao.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://tv.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xe.haigaiapp.cn

[C08] 闭包
来源：http://ri.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ak.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ca.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fi.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://an.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qq.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xt.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eu.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vl.szsharing.cn

[C09] 递归
来源：http://xd.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cp.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iz.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fg.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ry.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jg.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dt.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wr.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ig.nszjky.cn

[C10] 变量作用域
来源：http://oc.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qm.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mi.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gw.bjjhwx.cn

TS:   同 JS
来源：http://cl.asd995.cn

Java: 方法内为块级作用域
来源：http://jq.colortex.cn

Go:   花括号块级作用域
来源：http://qy.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nm.haigaiapp.cn

C#:   块级作用域
来源：http://ek.yuexingan06.cn

[C11] 模块导入与导出
来源：http://my.colortex.cn

Py:   from module import func
来源：http://vm.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://va.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://na.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.asd995.cn

Java: import java.util.List;
来源：http://na.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qf.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://ug.shtwfgs.cn

C#:   using System.Text;
来源：http://eq.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://hd.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://yx.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://gl.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://nk.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://ls.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yv.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://yt.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://of.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hu.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://cu.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dd.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ft.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sw.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ys.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://at.9csxet.cn

Go:   func add(a, b int) int
来源：http://uj.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yd.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pa.shtwfgs.cn

[C14] 泛型函数
来源：http://ep.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://du.lnxyls.cn

PHP:  // 无泛型
来源：http://zu.lnxyls.cn

JS:   // 无泛型
来源：http://dr.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wn.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tj.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hi.haigaiapp.cn

Ruby: # 无泛型
来源：http://mt.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wp.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://gy.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kf.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://pn.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mb.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nt.shxzukj.cn

Java: // 无解构
来源：http://jt.yuntaijiaju.cn

Go:   // 无解构
来源：http://ue.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://hq.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://sp.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://hb.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xu.bjjhwx.cn

PHP:  // 无重载
来源：http://kc.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wk.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ei.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lj.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://np.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://dr.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ta.szxytkj.cn

================================================================================
来源：http://xe.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://em.szsharing.cn

================================================================================
来源：http://zy.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://vc.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ek.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wk.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ah.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sx.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ke.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://zc.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://kt.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vf.hahajie.cn

[D02] 追加元素到末尾
来源：http://qz.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lx.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gr.jctech888.com.cn

JS:   arr.push(4);
来源：http://xl.haigaiapp.cn

TS:   arr.push(4);
来源：http://gu.521024.cn

Java: list.add(4);
来源：http://ba.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://wu.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://bg.bjjhwx.cn

C#:   list.Add(4);
来源：http://ei.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ot.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://bk.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uz.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vf.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://yc.szsharing.cn

Java: list.add(0, 0);
来源：http://pc.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nv.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://we.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://vi.gzmigu.cn

[D04] 删除元素
来源：http://zx.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yf.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fp.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qw.colortex.cn

TS:   arr.splice(0, 1);
来源：http://tm.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ui.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ax.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wo.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ee.bjjhwx.cn

[D05] 访问与修改元素
来源：http://tz.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vk.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bi.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mk.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://ut.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://hs.yuntaijiaju.cn


<!-- 参考信息 -->