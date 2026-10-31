代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qo.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://wv.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yp.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gu.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ma.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oi.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wv.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://za.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rg.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://it.muxihuayi.cn

[B07] while 循环
来源：http://dx.huanxung.cn

Py:   while i < 10: i += 1
来源：http://zo.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ub.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://yi.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://de.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://ua.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pw.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://th.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://fk.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://oh.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://zj.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eq.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://xh.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://lr.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://gw.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hn.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rx.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://jh.nicolike.cn

[B09] break 与 continue
来源：http://hc.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://me.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fk.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bc.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oh.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mm.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ba.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://za.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kf.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://yf.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ig.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ok.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dd.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xx.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xc.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zr.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lr.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kz.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://hx.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://jc.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://sc.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uz.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cv.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qp.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oe.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://ud.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nx.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ny.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qq.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://di.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kz.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xh.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uc.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fm.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yq.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ub.muxihuayi.cn

[B13] 判断是否为数字
来源：http://pj.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://jq.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://oj.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sb.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ej.szxytkj.cn

Java: x instanceof Number
来源：http://xk.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ip.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://ad.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://hg.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://ao.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vp.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://af.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://sd.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://bh.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ax.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sv.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kz.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pr.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://xu.muxihuayi.cn

Py:   a and b or not c
来源：http://qa.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://xx.asd995.cn

JS:   a && b || !c
来源：http://oa.hahajie.cn

TS:   a && b || !c
来源：http://bw.hahajie.cn

Java: a && b || !c
来源：http://ji.panjiajie.cn

Go:   a && b || !c
来源：http://pb.jctech888.com.cn

Ruby: a && b || !c
来源：http://lt.nicolike.cn

C#:   a && b || !c
来源：http://rv.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ll.szsharing.cn

Py:   if not data: return
来源：http://tp.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://wz.huanxung.cn

JS:   if (!data) return;
来源：http://ed.521024.cn

TS:   if (!data) return;
来源：http://mx.panjiajie.cn

Java: if (data == null) return;
来源：http://mt.huixiangedu.cn

Go:   if data == nil { return }
来源：http://xv.chemitech.net.cn

Ruby: return if data.nil?
来源：http://rz.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://ba.shtwfgs.cn

================================================================================
来源：http://ul.haigaiapp.cn

C. 函数与作用域
来源：http://jk.huanxung.cn

================================================================================
来源：http://tk.haigaiapp.cn

[C01] 定义函数
来源：http://nx.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://ty.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://my.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://bz.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sp.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nq.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rq.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://gu.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ny.wgjwhj.cn

[C02] 默认参数
来源：http://xo.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://rp.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ih.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://zk.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hg.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zm.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fo.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://uv.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://jo.huixiangedu.cn

[C03] 可变参数
来源：http://gp.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://vw.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iy.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qb.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hl.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vf.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pc.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zx.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://at.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://ei.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ye.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yd.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qe.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yq.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://bu.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://va.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://hq.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://mv.hahajie.cn

[C05] 返回多个值
来源：http://iv.yuexingan06.cn

Py:   return a, b
来源：http://ao.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://ao.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xq.hahajie.cn

TS:   return { a, b };
来源：http://kv.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lx.muxihuayi.cn

Go:   return a, b
来源：http://xe.yuntaijiaju.cn

Ruby: return a, b
来源：http://ag.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ho.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://nz.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://dq.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sw.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://vs.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://mk.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ov.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jj.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://sp.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pi.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://ps.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cl.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ym.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sd.lnxyls.cn

TS:   arr.map(String)
来源：http://gc.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rd.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ap.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://jc.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zw.huixinmuqiang.cn

[C08] 闭包
来源：http://ad.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sy.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mq.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ly.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hk.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vr.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xc.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xp.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zt.521024.cn

[C09] 递归
来源：http://fw.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://an.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://et.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jz.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fi.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wt.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nh.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ih.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nv.nszjky.cn

[C10] 变量作用域
来源：http://us.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yp.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uf.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pr.gzmigu.cn

TS:   同 JS
来源：http://rd.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://zd.shtwfgs.cn

Go:   花括号块级作用域
来源：http://sr.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uv.wgjwhj.cn

C#:   块级作用域
来源：http://pa.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://nk.wgjwhj.cn

Py:   from module import func
来源：http://ad.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ct.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fs.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tl.szxytkj.cn

Java: import java.util.List;
来源：http://fg.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hj.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://qj.muxihuayi.cn

C#:   using System.Text;
来源：http://sj.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://hw.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://yj.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://zy.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://fe.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://ze.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hw.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://sa.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://wd.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dh.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://ru.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://me.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ba.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yk.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ug.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mk.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://mi.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ld.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hu.huanxung.cn

[C14] 泛型函数
来源：http://es.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ws.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://ze.shxzukj.cn

JS:   // 无泛型
来源：http://je.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ec.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rx.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qy.asd995.cn

Ruby: # 无泛型
来源：http://ue.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yx.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://la.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ot.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://oy.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ik.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://za.wgjwhj.cn

Java: // 无解构
来源：http://xz.szsharing.cn

Go:   // 无解构
来源：http://hv.newstarts.cn

Ruby: a, b = pair
来源：http://fh.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://sg.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://ow.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://so.521024.cn

PHP:  // 无重载
来源：http://ds.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bf.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://eb.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ii.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://sw.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://vz.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rc.yuntaijiaju.cn

================================================================================
来源：http://xj.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://as.huixiangedu.cn

================================================================================
来源：http://cc.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://iq.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pk.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ds.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xy.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bo.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rw.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://ob.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://rw.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nu.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://yv.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qv.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wh.nicolike.cn

JS:   arr.push(4);
来源：http://jg.newstarts.cn

TS:   arr.push(4);
来源：http://ge.jctech888.com.cn

Java: list.add(4);
来源：http://bi.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://vi.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://rl.lnxyls.cn

C#:   list.Add(4);
来源：http://of.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://pr.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://ih.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cp.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rm.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://gp.huixiangedu.cn

Java: list.add(0, 0);
来源：http://vk.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mb.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ws.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://df.huixinmuqiang.cn

[D04] 删除元素
来源：http://xr.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nn.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mg.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uj.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://ue.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xm.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zj.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://af.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zj.bjjhwx.cn

[D05] 访问与修改元素
来源：http://tm.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gf.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ts.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ww.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://yf.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://yf.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://wz.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://up.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qt.wgjwhj.cn

[D06] 数组长度
来源：http://hu.asd995.cn

Py:   len(arr)
来源：http://jh.szsharing.cn

PHP:  count($arr);
来源：http://bg.huixinmuqiang.cn

JS:   arr.length
来源：http://tu.panjiajie.cn

TS:   arr.length
来源：http://ex.jianghongdianzi.cn


<!-- 参考信息 -->