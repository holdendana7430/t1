代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iy.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://wb.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ut.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qj.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ws.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qn.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hv.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dx.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zw.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kx.bookmarksfly.cn

[B07] while 循环
来源：http://xs.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://dt.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cl.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://sx.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://bd.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://sp.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tm.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://xj.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://we.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://jq.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://hq.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ie.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://rc.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://jg.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://he.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sd.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ld.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://fu.lnxyls.cn

[B09] break 与 continue
来源：http://vu.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yb.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://de.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gz.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iu.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://as.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ed.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xp.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kn.521024.cn

[B10] 遍历同时拿索引
来源：http://lg.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gw.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wt.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xj.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ha.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kg.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jo.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://er.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hy.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://zh.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://tv.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://tb.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wg.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fr.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rh.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ze.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://bi.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oa.haigaiapp.cn

[B12] 跳出多层循环
来源：http://oh.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hy.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wh.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qm.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gk.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eh.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oo.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cn.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cq.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://gy.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://uy.9csxet.cn

PHP:  is_numeric($x)
来源：http://ib.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ft.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yc.gzmigu.cn

Java: x instanceof Number
来源：http://qa.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qr.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://gh.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://pm.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://po.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://db.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dh.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://gv.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://am.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ht.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://br.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hn.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wv.asd995.cn

[B15] 布尔运算与取反
来源：http://bx.huixiangedu.cn

Py:   a and b or not c
来源：http://pd.9csxet.cn

PHP:  $a && $b || !$c
来源：http://sg.shtwfgs.cn

JS:   a && b || !c
来源：http://ls.shtwfgs.cn

TS:   a && b || !c
来源：http://xp.hahajie.cn

Java: a && b || !c
来源：http://xh.nicolike.cn

Go:   a && b || !c
来源：http://an.jctech888.com.cn

Ruby: a && b || !c
来源：http://gi.newstarts.cn

C#:   a && b || !c
来源：http://ie.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://br.hahajie.cn

Py:   if not data: return
来源：http://bq.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://gn.muxihuayi.cn

JS:   if (!data) return;
来源：http://ph.nszjky.cn

TS:   if (!data) return;
来源：http://qz.huanxung.cn

Java: if (data == null) return;
来源：http://fq.hahajie.cn

Go:   if data == nil { return }
来源：http://vi.haigaiapp.cn

Ruby: return if data.nil?
来源：http://zc.shxzskj.cn

C#:   if (data == null) return;
来源：http://ie.nszjky.cn

================================================================================
来源：http://re.newstarts.cn

C. 函数与作用域
来源：http://cd.haigaiapp.cn

================================================================================
来源：http://vh.yuexingan06.cn

[C01] 定义函数
来源：http://gj.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://gi.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gg.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://gx.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qb.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nj.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jd.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://gz.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xm.yuexingan06.cn

[C02] 默认参数
来源：http://cl.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://gz.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vb.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://my.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ca.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eq.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dl.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://zf.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://sx.shxzukj.cn

[C03] 可变参数
来源：http://fm.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://pp.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xg.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iw.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://te.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ru.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aw.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bf.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hv.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ju.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yd.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kc.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wx.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ik.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://sp.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://yy.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://lf.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://ng.jianghongdianzi.cn

[C05] 返回多个值
来源：http://zi.panjiajie.cn

Py:   return a, b
来源：http://qr.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://df.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://me.jctech888.com.cn

TS:   return { a, b };
来源：http://ax.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oc.colortex.cn

Go:   return a, b
来源：http://fi.shxzskj.cn

Ruby: return a, b
来源：http://bq.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://xw.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://ye.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://kl.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lh.hnjuh.cn

JS:   const square = x => x * x;
来源：http://qx.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://vx.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sw.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ug.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://ue.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lx.nszjky.cn

[C07] 把函数作为参数传入
来源：http://jw.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://av.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fe.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nw.gzmigu.cn

TS:   arr.map(String)
来源：http://ma.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vk.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jf.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://mo.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ws.yuexingan06.cn

[C08] 闭包
来源：http://be.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bg.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tb.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yy.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ov.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hx.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gb.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ie.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ep.muxihuayi.cn

[C09] 递归
来源：http://za.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pf.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cr.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ee.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sd.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zc.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dm.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pv.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ry.521024.cn

[C10] 变量作用域
来源：http://wg.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tw.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nn.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uh.shxzskj.cn

TS:   同 JS
来源：http://ts.nicolike.cn

Java: 方法内为块级作用域
来源：http://ry.nszjky.cn

Go:   花括号块级作用域
来源：http://km.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://po.hnjuh.cn

C#:   块级作用域
来源：http://hu.shxzskj.cn

[C11] 模块导入与导出
来源：http://fy.hnjuh.cn

Py:   from module import func
来源：http://qy.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yh.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ao.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://th.hnjuh.cn

Java: import java.util.List;
来源：http://sp.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bn.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://xx.muxihuayi.cn

C#:   using System.Text;
来源：http://iv.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://qr.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://ec.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://wu.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://tj.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://nr.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ny.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://zy.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://yx.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uz.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://sy.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kw.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ca.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://us.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ca.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rt.newstarts.cn

Go:   func add(a, b int) int
来源：http://xy.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vp.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://il.colortex.cn

[C14] 泛型函数
来源：http://th.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zs.panjiajie.cn

PHP:  // 无泛型
来源：http://vz.newstarts.cn

JS:   // 无泛型
来源：http://ck.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zs.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xy.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jr.yuexingan06.cn

Ruby: # 无泛型
来源：http://pq.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xy.szsharing.cn

[C15] 解构 / 展开参数
来源：http://fr.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://du.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://ri.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ih.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ie.huixinmuqiang.cn

Java: // 无解构
来源：http://jp.szxytkj.cn

Go:   // 无解构
来源：http://zw.hahajie.cn

Ruby: a, b = pair
来源：http://bx.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://dw.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://am.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gi.gzmigu.cn

PHP:  // 无重载
来源：http://ti.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yk.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://ne.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iw.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://vt.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://xe.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://to.gzmigu.cn

================================================================================
来源：http://cd.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://zb.jctech888.com.cn

================================================================================
来源：http://kc.nicolike.cn

[D01] 创建数组 / 列表
来源：http://ut.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wu.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mh.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ro.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://el.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ym.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://xa.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://re.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://po.shxzskj.cn

[D02] 追加元素到末尾
来源：http://ih.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rk.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oi.shxzskj.cn

JS:   arr.push(4);
来源：http://ir.jctech888.com.cn

TS:   arr.push(4);
来源：http://ia.szxytkj.cn

Java: list.add(4);
来源：http://ht.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://nx.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://uw.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://hn.newstarts.cn

[D03] 在指定位置插入元素
来源：http://fj.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://nz.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://of.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dw.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://is.nicolike.cn

Java: list.add(0, 0);
来源：http://ds.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mn.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zz.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://wa.yuntaijiaju.cn

[D04] 删除元素
来源：http://wf.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sf.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cf.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xo.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://jg.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jn.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uq.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://au.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ef.colortex.cn

[D05] 访问与修改元素
来源：http://ij.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pz.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aj.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ms.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://er.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://sy.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://sm.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ax.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tx.huixinmuqiang.cn

[D06] 数组长度
来源：http://bb.szxytkj.cn

Py:   len(arr)
来源：http://hw.gzmigu.cn

PHP:  count($arr);
来源：http://dp.521024.cn

JS:   arr.length
来源：http://qv.szsharing.cn

TS:   arr.length
来源：http://od.haigaiapp.cn


<!-- 参考信息 -->