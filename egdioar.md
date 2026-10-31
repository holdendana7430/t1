代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wr.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wg.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tl.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sy.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jg.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aw.shxzukj.cn

[B07] while 循环
来源：http://ov.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://it.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mk.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://rp.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://uv.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://xm.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ku.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://gw.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://oo.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://qb.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://zc.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://up.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://wm.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://ij.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://fn.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vh.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jz.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://so.newstarts.cn

[B09] break 与 continue
来源：http://xe.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vd.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rl.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://km.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cc.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dj.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kx.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://na.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://jr.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ws.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nr.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://km.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tw.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wc.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ic.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mr.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lx.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://te.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://og.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://yo.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nz.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fy.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fs.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uv.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://ct.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ou.szsharing.cn

[B12] 跳出多层循环
来源：http://wc.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vp.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mz.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://py.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cq.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yz.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vo.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://us.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://to.yuexingan06.cn

[B13] 判断是否为数字
来源：http://ov.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://eg.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://sz.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gf.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gl.szsharing.cn

Java: x instanceof Number
来源：http://xy.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kn.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://mw.gzmigu.cn

C#:   x is int or double or decimal
来源：http://xp.nszjky.cn

[B14] 判断值是否在集合内
来源：http://wb.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://la.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jt.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://kd.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://pi.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://md.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://db.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yo.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cp.huanxung.cn

[B15] 布尔运算与取反
来源：http://sk.yuexingan06.cn

Py:   a and b or not c
来源：http://ru.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://lp.lnxyls.cn

JS:   a && b || !c
来源：http://ua.asd995.cn

TS:   a && b || !c
来源：http://kz.wgjwhj.cn

Java: a && b || !c
来源：http://ns.yuntaijiaju.cn

Go:   a && b || !c
来源：http://fq.huanxung.cn

Ruby: a && b || !c
来源：http://mq.huixinmuqiang.cn

C#:   a && b || !c
来源：http://nj.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ly.jianghongdianzi.cn

Py:   if not data: return
来源：http://jz.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://px.haigaiapp.cn

JS:   if (!data) return;
来源：http://ox.wgjwhj.cn

TS:   if (!data) return;
来源：http://xt.muxihuayi.cn

Java: if (data == null) return;
来源：http://nq.nicolike.cn

Go:   if data == nil { return }
来源：http://md.9csxet.cn

Ruby: return if data.nil?
来源：http://fc.shtwfgs.cn

C#:   if (data == null) return;
来源：http://zq.szxytkj.cn

================================================================================
来源：http://fa.wgjwhj.cn

C. 函数与作用域
来源：http://wy.huanxung.cn

================================================================================
来源：http://qk.hnjuh.cn

[C01] 定义函数
来源：http://bh.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://yn.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wr.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://vd.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qz.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xk.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xm.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://tt.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nz.panjiajie.cn

[C02] 默认参数
来源：http://ul.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://io.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xa.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://bv.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fo.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cr.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hn.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://vu.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://ag.szsharing.cn

[C03] 可变参数
来源：http://kn.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://cx.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mv.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mt.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jl.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pa.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://is.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bk.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xf.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://ju.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ws.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ui.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rg.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kw.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://sz.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://yi.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://yo.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://ux.yuexingan06.cn

[C05] 返回多个值
来源：http://kt.521024.cn

Py:   return a, b
来源：http://wa.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://te.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hi.shxzskj.cn

TS:   return { a, b };
来源：http://pd.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nicolike.cn

Go:   return a, b
来源：http://mh.asd995.cn

Ruby: return a, b
来源：http://de.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://se.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://af.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://ln.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gn.szsharing.cn

JS:   const square = x => x * x;
来源：http://us.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://zn.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lf.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nv.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://aq.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hp.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://yj.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cc.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wj.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bh.asd995.cn

TS:   arr.map(String)
来源：http://ug.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gn.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qo.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://vq.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nk.bjjhwx.cn

[C08] 闭包
来源：http://jv.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wc.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yq.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pr.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aj.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bb.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mz.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pb.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://th.nszjky.cn

[C09] 递归
来源：http://hd.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mo.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sr.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://al.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xm.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uo.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tz.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bv.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hs.colortex.cn

[C10] 变量作用域
来源：http://rw.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wa.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://do.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://la.wgjwhj.cn

TS:   同 JS
来源：http://as.gzmigu.cn

Java: 方法内为块级作用域
来源：http://rz.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://oq.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sv.9csxet.cn

C#:   块级作用域
来源：http://kn.hahajie.cn

[C11] 模块导入与导出
来源：http://dk.szxytkj.cn

Py:   from module import func
来源：http://tb.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gu.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ef.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zx.panjiajie.cn

Java: import java.util.List;
来源：http://jo.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ld.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://tw.bookmarksfly.cn

C#:   using System.Text;
来源：http://ed.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://xv.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://gd.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://dv.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://tz.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://qw.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mm.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://vv.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://eq.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xd.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://ky.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qu.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sp.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zw.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://us.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://np.asd995.cn

Go:   func add(a, b int) int
来源：http://jx.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zg.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nb.yuntaijiaju.cn

[C14] 泛型函数
来源：http://yf.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ky.gzmigu.cn

PHP:  // 无泛型
来源：http://op.9csxet.cn

JS:   // 无泛型
来源：http://jd.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xu.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gj.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ya.hnjuh.cn

Ruby: # 无泛型
来源：http://so.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yg.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://zf.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vu.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://ii.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://id.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wc.hnjuh.cn

Java: // 无解构
来源：http://jo.hahajie.cn

Go:   // 无解构
来源：http://dv.jctech888.com.cn

Ruby: a, b = pair
来源：http://ul.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://vc.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://rb.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hm.jianghongdianzi.cn

PHP:  // 无重载
来源：http://oz.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ak.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://rc.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ef.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://iv.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://hj.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gv.colortex.cn

================================================================================
来源：http://zz.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://il.haigaiapp.cn

================================================================================
来源：http://bq.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://hf.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gj.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ej.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uz.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wr.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://of.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://vu.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://nw.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fb.panjiajie.cn

[D02] 追加元素到末尾
来源：http://xv.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vc.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tq.shxzukj.cn

JS:   arr.push(4);
来源：http://af.hahajie.cn

TS:   arr.push(4);
来源：http://yo.newstarts.cn

Java: list.add(4);
来源：http://ln.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://fy.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://nm.yuexingan06.cn

C#:   list.Add(4);
来源：http://ap.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://so.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://bh.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mr.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pg.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://pj.huanxung.cn

Java: list.add(0, 0);
来源：http://pq.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mv.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rx.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://oh.9csxet.cn

[D04] 删除元素
来源：http://gx.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ga.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xi.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ha.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://oy.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qy.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bv.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://po.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ka.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://fu.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ha.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cm.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://df.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://gy.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ju.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://gf.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lz.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vt.szxytkj.cn

[D06] 数组长度
来源：http://si.colortex.cn

Py:   len(arr)
来源：http://vs.yuexingan06.cn

PHP:  count($arr);
来源：http://rn.huixiangedu.cn

JS:   arr.length
来源：http://fp.yuntaijiaju.cn

TS:   arr.length
来源：http://ut.panjiajie.cn

Java: list.size();
来源：http://ek.shxzskj.cn

Go:   len(arr)
来源：http://da.asd995.cn

Ruby: arr.length; arr.size
来源：http://wy.9csxet.cn

C#:   list.Count;
来源：http://oz.yuexingan06.cn


<!-- 参考信息 -->