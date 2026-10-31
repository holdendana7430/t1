代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://aq.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sv.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://tm.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://sz.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://go.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wk.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ui.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://mm.colortex.cn

[B09] break 与 continue
来源：http://im.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qv.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ho.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sx.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dr.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pn.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ej.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eu.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hd.szsharing.cn

[B10] 遍历同时拿索引
来源：http://ry.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fg.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pl.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lh.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://je.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://no.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xw.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mj.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lq.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://xt.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://lw.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://zr.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ck.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eb.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gr.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sa.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://cr.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fv.muxihuayi.cn

[B12] 跳出多层循环
来源：http://hn.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bg.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://im.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tg.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yt.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zi.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dd.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://en.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wq.hahajie.cn

[B13] 判断是否为数字
来源：http://xb.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://zd.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://ep.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qg.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wl.muxihuayi.cn

Java: x instanceof Number
来源：http://eb.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mt.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://ps.hnjuh.cn

C#:   x is int or double or decimal
来源：http://hn.nszjky.cn

[B14] 判断值是否在集合内
来源：http://sl.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tf.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cw.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://sh.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://or.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gu.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vd.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gc.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uv.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://un.shtwfgs.cn

Py:   a and b or not c
来源：http://af.hahajie.cn

PHP:  $a && $b || !$c
来源：http://tb.huixinmuqiang.cn

JS:   a && b || !c
来源：http://dr.panjiajie.cn

TS:   a && b || !c
来源：http://vd.gzmigu.cn

Java: a && b || !c
来源：http://wk.jctech888.com.cn

Go:   a && b || !c
来源：http://qp.wgjwhj.cn

Ruby: a && b || !c
来源：http://kn.panjiajie.cn

C#:   a && b || !c
来源：http://zo.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ah.newstarts.cn

Py:   if not data: return
来源：http://yz.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://vs.lnxyls.cn

JS:   if (!data) return;
来源：http://xy.hnjuh.cn

TS:   if (!data) return;
来源：http://ap.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://ch.chemitech.net.cn

Go:   if data == nil { return }
来源：http://tg.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://xa.huixiangedu.cn

C#:   if (data == null) return;
来源：http://zt.yuexingan06.cn

================================================================================
来源：http://ct.wgjwhj.cn

C. 函数与作用域
来源：http://on.hnjuh.cn

================================================================================
来源：http://zc.yuexingan06.cn

[C01] 定义函数
来源：http://tl.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://xj.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nm.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://jz.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lm.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lv.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gy.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://bj.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sl.yuexingan06.cn

[C02] 默认参数
来源：http://um.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://il.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zf.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qv.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://co.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ue.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kh.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://sq.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://cz.nszjky.cn

[C03] 可变参数
来源：http://vi.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://qp.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sv.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eg.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uk.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zz.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ms.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zg.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hk.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://ji.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hq.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qn.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qm.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jy.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://qi.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://gp.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://fu.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://qg.shxzskj.cn

[C05] 返回多个值
来源：http://mx.521024.cn

Py:   return a, b
来源：http://rf.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://cg.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ou.bjjhwx.cn

TS:   return { a, b };
来源：http://qf.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bj.nszjky.cn

Go:   return a, b
来源：http://kv.521024.cn

Ruby: return a, b
来源：http://xx.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://fd.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://nw.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://uf.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bq.nicolike.cn

JS:   const square = x => x * x;
来源：http://hd.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://dr.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vp.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qq.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://uc.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fc.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://kz.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vb.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xu.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ub.lnxyls.cn

TS:   arr.map(String)
来源：http://jt.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zz.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ap.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://we.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hg.huixinmuqiang.cn

[C08] 闭包
来源：http://uq.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hj.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rk.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ff.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mv.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rx.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dj.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iw.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nb.colortex.cn

[C09] 递归
来源：http://ng.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wc.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ek.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pi.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dw.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iv.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ya.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cy.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ir.huixiangedu.cn

[C10] 变量作用域
来源：http://jx.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xw.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pf.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sn.hnjuh.cn

TS:   同 JS
来源：http://ft.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://te.lnxyls.cn

Go:   花括号块级作用域
来源：http://ht.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qz.bjjhwx.cn

C#:   块级作用域
来源：http://fg.jctech888.com.cn

[C11] 模块导入与导出
来源：http://yj.szsharing.cn

Py:   from module import func
来源：http://oi.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://al.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ol.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kw.lnxyls.cn

Java: import java.util.List;
来源：http://iv.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wh.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://zw.521024.cn

C#:   using System.Text;
来源：http://mq.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://uq.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://dx.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://oo.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://nn.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://yu.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yh.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://fq.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://zb.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gl.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://ne.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cn.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gx.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://td.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fq.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://at.521024.cn

Go:   func add(a, b int) int
来源：http://ws.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://js.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tl.chemitech.net.cn

[C14] 泛型函数
来源：http://fo.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zm.newstarts.cn

PHP:  // 无泛型
来源：http://cs.hnjuh.cn

JS:   // 无泛型
来源：http://xu.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://td.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gd.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nc.9csxet.cn

Ruby: # 无泛型
来源：http://fz.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fg.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://zb.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pn.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://uu.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mk.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ei.gzmigu.cn

Java: // 无解构
来源：http://xm.shxzukj.cn

Go:   // 无解构
来源：http://nd.panjiajie.cn

Ruby: a, b = pair
来源：http://cc.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://hm.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://gi.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wu.nicolike.cn

PHP:  // 无重载
来源：http://ha.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mi.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://mg.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pz.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://gs.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://nu.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://re.shtwfgs.cn

================================================================================
来源：http://wm.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://xr.panjiajie.cn

================================================================================
来源：http://sk.nszjky.cn

[D01] 创建数组 / 列表
来源：http://mx.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vz.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://de.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vl.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ui.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ks.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://uv.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://vz.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qs.nszjky.cn

[D02] 追加元素到末尾
来源：http://dp.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ss.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zf.shxzskj.cn

JS:   arr.push(4);
来源：http://pi.hahajie.cn

TS:   arr.push(4);
来源：http://tv.shxzukj.cn

Java: list.add(4);
来源：http://gj.521024.cn

Go:   arr = append(arr, 4)
来源：http://pi.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://dj.asd995.cn

C#:   list.Add(4);
来源：http://lh.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://ie.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://dk.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kx.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tz.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ey.521024.cn

Java: list.add(0, 0);
来源：http://ep.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pb.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://us.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://vv.bjjhwx.cn

[D04] 删除元素
来源：http://lj.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bz.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://es.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hx.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://ow.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qc.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ly.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vj.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rq.521024.cn

[D05] 访问与修改元素
来源：http://pa.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uj.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ie.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tv.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://fr.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://ta.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://uz.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dy.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sq.haigaiapp.cn

[D06] 数组长度
来源：http://ix.chemitech.net.cn

Py:   len(arr)
来源：http://hv.bookmarksfly.cn

PHP:  count($arr);
来源：http://ar.521024.cn

JS:   arr.length
来源：http://li.yuexingan06.cn

TS:   arr.length
来源：http://kc.wgjwhj.cn

Java: list.size();
来源：http://dt.shxzukj.cn

Go:   len(arr)
来源：http://dj.asd995.cn

Ruby: arr.length; arr.size
来源：http://fp.bookmarksfly.cn

C#:   list.Count;
来源：http://mm.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://zw.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ji.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jy.colortex.cn

JS:   arr.slice(1, 4);
来源：http://xo.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://gz.szsharing.cn

Java: list.subList(1, 4);
来源：http://bw.lnxyls.cn

Go:   arr[1:4]
来源：http://in.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://cx.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://tr.asd995.cn

[D08] 合并两个数组
来源：http://de.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://nd.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://qs.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://te.nszjky.cn

TS:   [...a, ...b];
来源：http://to.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://am.szxytkj.cn

Go:   append(a, b...)
来源：http://is.shtwfgs.cn


<!-- 参考信息 -->