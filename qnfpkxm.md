代发 wailian999

[B05] 遍历数组 / 列表
来源：http://sb.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://xl.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fl.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ti.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mf.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eq.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zv.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://du.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zu.521024.cn

[B06] 遍历字典 / 对象
来源：http://yu.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fe.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vd.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bu.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xd.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xb.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fk.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tw.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xv.huixinmuqiang.cn

[B07] while 循环
来源：http://fe.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://ov.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zj.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://nt.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://ri.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://hj.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dm.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://vv.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://kc.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://pa.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://bw.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jb.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://gp.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://jv.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://ai.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wx.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rx.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://js.yuexingan06.cn

[B09] break 与 continue
来源：http://dn.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ag.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hi.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ut.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tk.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hv.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tf.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nm.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jg.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://wz.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fv.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fw.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pw.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fz.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ff.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dn.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dq.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yg.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://kc.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://wy.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://he.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ji.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dw.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ie.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://te.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://ru.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vf.jctech888.com.cn

[B12] 跳出多层循环
来源：http://fv.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ey.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ke.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tn.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://am.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qw.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cn.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hj.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uz.asd995.cn

[B13] 判断是否为数字
来源：http://br.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://wh.shxzukj.cn

PHP:  is_numeric($x)
来源：http://sn.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nt.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zf.yuntaijiaju.cn

Java: x instanceof Number
来源：http://bc.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pc.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://vc.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://dw.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://cn.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zt.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ja.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://zs.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://su.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wa.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qk.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jn.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jm.colortex.cn

[B15] 布尔运算与取反
来源：http://rr.bookmarksfly.cn

Py:   a and b or not c
来源：http://by.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://ox.panjiajie.cn

JS:   a && b || !c
来源：http://fo.shtwfgs.cn

TS:   a && b || !c
来源：http://ji.jianghongdianzi.cn

Java: a && b || !c
来源：http://ao.colortex.cn

Go:   a && b || !c
来源：http://lr.panjiajie.cn

Ruby: a && b || !c
来源：http://cj.huanxung.cn

C#:   a && b || !c
来源：http://hk.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uv.jctech888.com.cn

Py:   if not data: return
来源：http://vm.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://vj.colortex.cn

JS:   if (!data) return;
来源：http://fs.newstarts.cn

TS:   if (!data) return;
来源：http://wz.szsharing.cn

Java: if (data == null) return;
来源：http://vg.hahajie.cn

Go:   if data == nil { return }
来源：http://iw.huanxung.cn

Ruby: return if data.nil?
来源：http://oi.szsharing.cn

C#:   if (data == null) return;
来源：http://kt.wgjwhj.cn

================================================================================
来源：http://aq.panjiajie.cn

C. 函数与作用域
来源：http://yf.yuexingan06.cn

================================================================================
来源：http://ea.panjiajie.cn

[C01] 定义函数
来源：http://oe.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://gm.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rw.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://tn.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ga.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bz.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cs.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://nj.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vh.newstarts.cn

[C02] 默认参数
来源：http://iv.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://sm.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qq.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://jb.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hf.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sv.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cr.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://ik.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ar.asd995.cn

[C03] 可变参数
来源：http://co.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://qi.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mw.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qy.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fc.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ce.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ad.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://is.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vf.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://jd.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ep.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zu.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nq.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ns.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://ue.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://ko.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://ob.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://kc.yuexingan06.cn

[C05] 返回多个值
来源：http://kq.nszjky.cn

Py:   return a, b
来源：http://bl.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://ly.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zt.panjiajie.cn

TS:   return { a, b };
来源：http://ow.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mi.hnjuh.cn

Go:   return a, b
来源：http://ug.521024.cn

Ruby: return a, b
来源：http://fs.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://hu.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://oe.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://gj.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fi.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://pr.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://kq.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vq.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jz.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://ms.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qi.nicolike.cn

[C07] 把函数作为参数传入
来源：http://rn.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kq.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yi.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qs.hahajie.cn

TS:   arr.map(String)
来源：http://yp.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lc.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gs.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://fx.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fc.gzmigu.cn

[C08] 闭包
来源：http://jb.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rh.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://im.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lu.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ou.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rw.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://da.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yq.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zi.shtwfgs.cn

[C09] 递归
来源：http://sr.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://em.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://to.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pj.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bn.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gd.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kx.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qs.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fv.newstarts.cn

[C10] 变量作用域
来源：http://pa.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ja.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bu.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aq.huixinmuqiang.cn

TS:   同 JS
来源：http://fd.szxytkj.cn

Java: 方法内为块级作用域
来源：http://de.hahajie.cn

Go:   花括号块级作用域
来源：http://vd.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lk.521024.cn

C#:   块级作用域
来源：http://ry.521024.cn

[C11] 模块导入与导出
来源：http://sk.asd995.cn

Py:   from module import func
来源：http://hl.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://os.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ku.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nu.panjiajie.cn

Java: import java.util.List;
来源：http://zy.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qg.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://iy.panjiajie.cn

C#:   using System.Text;
来源：http://mz.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://tx.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://nx.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://ie.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://ud.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://sl.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gq.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://ya.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://kp.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hc.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://gy.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uo.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xz.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://im.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tj.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jf.nicolike.cn

Go:   func add(a, b int) int
来源：http://yl.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vd.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xa.shxzskj.cn

[C14] 泛型函数
来源：http://jp.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://af.newstarts.cn

PHP:  // 无泛型
来源：http://cd.wgjwhj.cn

JS:   // 无泛型
来源：http://lj.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://su.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ie.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rm.wgjwhj.cn

Ruby: # 无泛型
来源：http://sf.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xq.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://rk.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ss.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://pd.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sz.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gs.yuntaijiaju.cn

Java: // 无解构
来源：http://eb.shxzukj.cn

Go:   // 无解构
来源：http://ic.colortex.cn

Ruby: a, b = pair
来源：http://pe.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://fc.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://tm.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xy.huanxung.cn

PHP:  // 无重载
来源：http://ix.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zq.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://pr.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yx.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://fq.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://bb.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yc.colortex.cn

================================================================================
来源：http://uh.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ri.szsharing.cn

================================================================================
来源：http://hn.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://ir.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://km.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aq.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bs.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kn.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jl.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://zq.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://lx.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aj.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://og.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ke.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kt.panjiajie.cn

JS:   arr.push(4);
来源：http://tu.asd995.cn

TS:   arr.push(4);
来源：http://gu.shtwfgs.cn

Java: list.add(4);
来源：http://uq.asd995.cn

Go:   arr = append(arr, 4)
来源：http://fc.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://tu.huixiangedu.cn

C#:   list.Add(4);
来源：http://ed.nicolike.cn

[D03] 在指定位置插入元素
来源：http://rz.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://yj.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ja.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xh.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://ji.hahajie.cn

Java: list.add(0, 0);
来源：http://xd.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pn.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rr.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://iq.muxihuayi.cn

[D04] 删除元素
来源：http://vm.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cn.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bg.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sn.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://do.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lx.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ve.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://si.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ye.shxzukj.cn

[D05] 访问与修改元素
来源：http://gh.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cn.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rj.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tr.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://ep.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://nx.panjiajie.cn


<!-- 参考信息 -->