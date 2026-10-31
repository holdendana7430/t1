代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://yu.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xl.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://wr.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://xs.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://fh.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qd.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://de.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://zm.bookmarksfly.cn

[B09] break 与 continue
来源：http://wm.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rm.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ke.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jv.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zh.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bw.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://le.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sw.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fl.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://bh.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bz.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zk.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yt.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rb.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jf.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gk.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uf.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rg.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://sd.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://qv.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://aw.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mb.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pr.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cv.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bp.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://tb.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yh.szxytkj.cn

[B12] 跳出多层循环
来源：http://hr.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qw.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vk.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ep.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ft.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tb.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bn.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nf.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jz.shtwfgs.cn

[B13] 判断是否为数字
来源：http://mj.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://wb.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://qk.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uw.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xv.jctech888.com.cn

Java: x instanceof Number
来源：http://pn.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wf.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://ph.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://zv.hahajie.cn

[B14] 判断值是否在集合内
来源：http://kd.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qv.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kd.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://xg.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://iz.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rq.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dw.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ml.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tv.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://ms.wgjwhj.cn

Py:   a and b or not c
来源：http://hx.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://yq.jctech888.com.cn

JS:   a && b || !c
来源：http://qh.muxihuayi.cn

TS:   a && b || !c
来源：http://xe.bookmarksfly.cn

Java: a && b || !c
来源：http://mo.szsharing.cn

Go:   a && b || !c
来源：http://wz.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://kj.newstarts.cn

C#:   a && b || !c
来源：http://tu.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ef.nicolike.cn

Py:   if not data: return
来源：http://fu.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://fy.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://pl.asd995.cn

TS:   if (!data) return;
来源：http://ww.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://ha.jctech888.com.cn

Go:   if data == nil { return }
来源：http://fq.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://ex.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://bz.nszjky.cn

================================================================================
来源：http://aa.bookmarksfly.cn

C. 函数与作用域
来源：http://qy.yuexingan06.cn

================================================================================
来源：http://wb.chemitech.net.cn

[C01] 定义函数
来源：http://dc.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://hd.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dn.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://ul.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rw.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://to.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://be.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://wx.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qo.asd995.cn

[C02] 默认参数
来源：http://lv.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://ym.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dg.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://gp.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zf.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://se.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cy.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://fs.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://jb.huanxung.cn

[C03] 可变参数
来源：http://vs.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://he.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tr.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ce.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yx.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yt.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gt.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nx.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eo.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://mf.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sq.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ep.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ei.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://li.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ry.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://tb.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://rg.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://pi.shxzskj.cn

[C05] 返回多个值
来源：http://ny.chemitech.net.cn

Py:   return a, b
来源：http://uq.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://xp.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xn.chemitech.net.cn

TS:   return { a, b };
来源：http://nx.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ib.nszjky.cn

Go:   return a, b
来源：http://je.nicolike.cn

Ruby: return a, b
来源：http://cl.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://lf.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://je.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://ld.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hw.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://ho.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://gr.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ll.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://by.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://hr.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://in.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://uz.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ul.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nb.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wp.huanxung.cn

TS:   arr.map(String)
来源：http://lr.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://je.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://be.521024.cn

Ruby: arr.map(&:upcase)
来源：http://cn.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qt.haigaiapp.cn

[C08] 闭包
来源：http://zo.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wt.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ri.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bu.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fk.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hm.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qu.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hv.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vh.asd995.cn

[C09] 递归
来源：http://hd.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lb.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kc.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vh.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vl.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nh.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://la.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aa.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bm.shxzskj.cn

[C10] 变量作用域
来源：http://fo.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gn.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wi.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hc.yuntaijiaju.cn

TS:   同 JS
来源：http://cc.hahajie.cn

Java: 方法内为块级作用域
来源：http://gg.asd995.cn

Go:   花括号块级作用域
来源：http://pq.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lq.yuntaijiaju.cn

C#:   块级作用域
来源：http://ir.haigaiapp.cn

[C11] 模块导入与导出
来源：http://yb.shtwfgs.cn

Py:   from module import func
来源：http://rw.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zt.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rt.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ru.yuexingan06.cn

Java: import java.util.List;
来源：http://kp.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dh.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://hh.bjjhwx.cn

C#:   using System.Text;
来源：http://bh.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://mi.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://si.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://ov.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://kv.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://ea.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qj.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://gc.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://wx.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://na.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://lm.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qq.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qn.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kt.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eu.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kl.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://em.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ic.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ww.9csxet.cn

[C14] 泛型函数
来源：http://lt.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nc.haigaiapp.cn

PHP:  // 无泛型
来源：http://bh.521024.cn

JS:   // 无泛型
来源：http://tb.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uf.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bv.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ih.shxzukj.cn

Ruby: # 无泛型
来源：http://sh.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xi.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://xi.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jd.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://nu.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ok.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xx.huanxung.cn

Java: // 无解构
来源：http://eo.huixiangedu.cn

Go:   // 无解构
来源：http://mw.muxihuayi.cn

Ruby: a, b = pair
来源：http://xk.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://sy.hahajie.cn

[C16] 函数 / 方法重载
来源：http://zz.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pi.jctech888.com.cn

PHP:  // 无重载
来源：http://vf.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rz.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://my.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xj.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://th.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://hl.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hc.nicolike.cn

================================================================================
来源：http://op.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://hv.haigaiapp.cn

================================================================================
来源：http://hm.szsharing.cn

[D01] 创建数组 / 列表
来源：http://po.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eg.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gu.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ma.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xj.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ne.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://hh.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://dz.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://na.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://qo.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ao.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mw.jctech888.com.cn

JS:   arr.push(4);
来源：http://jr.huanxung.cn

TS:   arr.push(4);
来源：http://wa.newstarts.cn

Java: list.add(4);
来源：http://zo.colortex.cn

Go:   arr = append(arr, 4)
来源：http://pb.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://sj.haigaiapp.cn

C#:   list.Add(4);
来源：http://hn.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://io.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://di.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yp.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ll.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://wr.haigaiapp.cn

Java: list.add(0, 0);
来源：http://vp.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yc.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nx.colortex.cn

C#:   list.Insert(0, 0);
来源：http://ck.lnxyls.cn

[D04] 删除元素
来源：http://bv.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oh.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gr.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jr.521024.cn

TS:   arr.splice(0, 1);
来源：http://cd.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nb.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hv.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://se.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kk.gzmigu.cn

[D05] 访问与修改元素
来源：http://zx.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zb.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vq.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eg.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://hq.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://ow.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://mf.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://na.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yg.jctech888.com.cn

[D06] 数组长度
来源：http://gs.huixinmuqiang.cn

Py:   len(arr)
来源：http://rh.hahajie.cn

PHP:  count($arr);
来源：http://de.huanxung.cn

JS:   arr.length
来源：http://mg.hahajie.cn

TS:   arr.length
来源：http://zr.lnxyls.cn

Java: list.size();
来源：http://be.nszjky.cn

Go:   len(arr)
来源：http://od.nicolike.cn

Ruby: arr.length; arr.size
来源：http://ei.jianghongdianzi.cn

C#:   list.Count;
来源：http://lb.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://ls.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rt.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pm.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://zi.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://gd.newstarts.cn

Java: list.subList(1, 4);
来源：http://sp.yuexingan06.cn

Go:   arr[1:4]
来源：http://gu.521024.cn

Ruby: arr[1, 3]
来源：http://yg.521024.cn

C#:   list.GetRange(1, 3);
来源：http://ni.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://hm.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://sf.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://zv.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wv.shxzukj.cn

TS:   [...a, ...b];
来源：http://un.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ap.shxzskj.cn

Go:   append(a, b...)
来源：http://ug.bjjhwx.cn


<!-- 参考信息 -->