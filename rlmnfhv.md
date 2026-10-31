代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://or.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://im.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://ht.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://nq.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ou.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://zb.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://kv.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://jc.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ow.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lh.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://qh.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://cc.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://lh.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vc.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ea.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://ge.9csxet.cn

[B09] break 与 continue
来源：http://ir.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ey.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vh.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rn.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ds.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ut.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gp.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tz.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ri.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://ft.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vw.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jz.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bv.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ou.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qf.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ba.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hh.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ql.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://pa.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://dm.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://dx.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gj.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ke.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nr.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hf.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://zo.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zp.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://sr.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iy.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hb.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ag.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://av.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lc.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qp.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wc.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gw.asd995.cn

[B13] 判断是否为数字
来源：http://md.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://we.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://zq.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rz.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://it.hahajie.cn

Java: x instanceof Number
来源：http://qt.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tq.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://ga.huanxung.cn

C#:   x is int or double or decimal
来源：http://ww.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://rn.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fp.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mc.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://iq.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://xg.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jf.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ny.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uv.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uz.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://du.shxzskj.cn

Py:   a and b or not c
来源：http://ti.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://xy.jianghongdianzi.cn

JS:   a && b || !c
来源：http://td.bookmarksfly.cn

TS:   a && b || !c
来源：http://rw.muxihuayi.cn

Java: a && b || !c
来源：http://iu.huixiangedu.cn

Go:   a && b || !c
来源：http://pg.asd995.cn

Ruby: a && b || !c
来源：http://an.newstarts.cn

C#:   a && b || !c
来源：http://ff.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ng.lnxyls.cn

Py:   if not data: return
来源：http://xs.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://mn.colortex.cn

JS:   if (!data) return;
来源：http://jk.nicolike.cn

TS:   if (!data) return;
来源：http://ws.hnjuh.cn

Java: if (data == null) return;
来源：http://ms.wgjwhj.cn

Go:   if data == nil { return }
来源：http://km.shxzukj.cn

Ruby: return if data.nil?
来源：http://oy.chemitech.net.cn

C#:   if (data == null) return;
来源：http://rp.jctech888.com.cn

================================================================================
来源：http://vl.jianghongdianzi.cn

C. 函数与作用域
来源：http://tz.asd995.cn

================================================================================
来源：http://nc.newstarts.cn

[C01] 定义函数
来源：http://fe.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://vi.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lr.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ff.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://te.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://na.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cc.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://rg.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gx.chemitech.net.cn

[C02] 默认参数
来源：http://zc.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://gi.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sk.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://tl.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nq.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ku.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jt.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://ms.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://bu.yuexingan06.cn

[C03] 可变参数
来源：http://uv.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://nl.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jw.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ew.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xv.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vk.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kn.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nb.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tj.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://vk.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cc.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sn.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ns.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yd.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://hj.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://av.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://vg.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://ks.shxzukj.cn

[C05] 返回多个值
来源：http://wo.nicolike.cn

Py:   return a, b
来源：http://sh.hnjuh.cn

PHP:  return [$a, $b];
来源：http://zy.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gh.asd995.cn

TS:   return { a, b };
来源：http://wr.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fo.nicolike.cn

Go:   return a, b
来源：http://qp.chemitech.net.cn

Ruby: return a, b
来源：http://cd.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://hm.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://yr.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://ud.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dy.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://oe.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://gh.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bp.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hq.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://yi.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://km.9csxet.cn

[C07] 把函数作为参数传入
来源：http://gq.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tg.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kd.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nn.shtwfgs.cn

TS:   arr.map(String)
来源：http://xz.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wg.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ly.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://qe.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qs.9csxet.cn

[C08] 闭包
来源：http://xa.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vp.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sy.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ls.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dk.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hg.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kg.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ik.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dr.panjiajie.cn

[C09] 递归
来源：http://ka.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://za.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ez.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jj.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ip.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xw.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://po.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cm.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lg.jianghongdianzi.cn

[C10] 变量作用域
来源：http://ik.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uk.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bx.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kl.panjiajie.cn

TS:   同 JS
来源：http://ar.gzmigu.cn

Java: 方法内为块级作用域
来源：http://hl.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://uk.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xk.lnxyls.cn

C#:   块级作用域
来源：http://iy.panjiajie.cn

[C11] 模块导入与导出
来源：http://ug.colortex.cn

Py:   from module import func
来源：http://bg.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ad.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ov.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uv.huanxung.cn

Java: import java.util.List;
来源：http://pw.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://au.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://zt.shtwfgs.cn

C#:   using System.Text;
来源：http://oa.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://lz.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://rp.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://ua.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://xu.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://ti.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dd.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://zm.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://wq.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lt.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://vm.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xt.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zl.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pl.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uo.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qw.asd995.cn

Go:   func add(a, b int) int
来源：http://sb.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iv.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kr.newstarts.cn

[C14] 泛型函数
来源：http://qv.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yt.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://qj.muxihuayi.cn

JS:   // 无泛型
来源：http://kf.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zr.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xu.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://je.gzmigu.cn

Ruby: # 无泛型
来源：http://ke.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gh.nszjky.cn

[C15] 解构 / 展开参数
来源：http://fx.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zg.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://lf.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gu.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vo.nicolike.cn

Java: // 无解构
来源：http://wq.muxihuayi.cn

Go:   // 无解构
来源：http://pf.gzmigu.cn

Ruby: a, b = pair
来源：http://yc.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://bz.nszjky.cn

[C16] 函数 / 方法重载
来源：http://tw.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pf.newstarts.cn

PHP:  // 无重载
来源：http://zd.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sm.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://tj.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hn.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://gu.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://vs.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://op.9csxet.cn

================================================================================
来源：http://eg.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://cc.lnxyls.cn

================================================================================
来源：http://et.colortex.cn

[D01] 创建数组 / 列表
来源：http://hg.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gj.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ea.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ya.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lp.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fw.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://yx.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://rv.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nf.gzmigu.cn

[D02] 追加元素到末尾
来源：http://cu.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yk.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ep.9csxet.cn

JS:   arr.push(4);
来源：http://hl.yuexingan06.cn

TS:   arr.push(4);
来源：http://rc.shtwfgs.cn

Java: list.add(4);
来源：http://qu.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://tu.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://pz.gzmigu.cn

C#:   list.Add(4);
来源：http://rh.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://nr.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://gu.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qn.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qv.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://fj.wgjwhj.cn

Java: list.add(0, 0);
来源：http://dg.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sp.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jy.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://em.gzmigu.cn

[D04] 删除元素
来源：http://cl.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://il.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hs.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ah.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://mh.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rl.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rc.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cy.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kk.hnjuh.cn

[D05] 访问与修改元素
来源：http://gw.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xr.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ae.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bc.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://oh.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://gl.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://xp.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rg.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oq.nszjky.cn

[D06] 数组长度
来源：http://jb.bjjhwx.cn

Py:   len(arr)
来源：http://vp.jianghongdianzi.cn

PHP:  count($arr);
来源：http://tu.jctech888.com.cn

JS:   arr.length
来源：http://ml.nszjky.cn

TS:   arr.length
来源：http://di.huanxung.cn

Java: list.size();
来源：http://ph.hnjuh.cn

Go:   len(arr)
来源：http://me.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://ye.shtwfgs.cn

C#:   list.Count;
来源：http://cz.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://tn.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kl.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oj.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://mg.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://xd.szxytkj.cn

Java: list.subList(1, 4);
来源：http://mr.asd995.cn

Go:   arr[1:4]
来源：http://wz.nicolike.cn

Ruby: arr[1, 3]
来源：http://wc.gzmigu.cn


<!-- 参考信息 -->