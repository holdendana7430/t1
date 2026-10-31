代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hj.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://yw.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://uk.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://nr.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://jl.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ih.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://ld.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://ab.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://nd.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mg.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bg.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://dw.bjjhwx.cn

[B09] break 与 continue
来源：http://my.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rm.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hn.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qk.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ge.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gc.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ik.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sv.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qk.nicolike.cn

[B10] 遍历同时拿索引
来源：http://un.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xe.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wo.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://og.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://og.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sq.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://te.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ng.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pk.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://eo.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://hk.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://rl.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kt.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pa.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xo.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fb.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://mm.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://us.shxzukj.cn

[B12] 跳出多层循环
来源：http://az.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mk.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cn.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://av.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qe.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vv.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://no.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bk.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iw.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://bs.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://bj.asd995.cn

PHP:  is_numeric($x)
来源：http://gd.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xd.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nk.huixinmuqiang.cn

Java: x instanceof Number
来源：http://be.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hk.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://lr.colortex.cn

C#:   x is int or double or decimal
来源：http://dk.nicolike.cn

[B14] 判断值是否在集合内
来源：http://tm.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ag.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://go.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://wn.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://ao.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ow.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cr.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sj.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hr.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://ci.huixinmuqiang.cn

Py:   a and b or not c
来源：http://pt.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://hn.szsharing.cn

JS:   a && b || !c
来源：http://mn.nicolike.cn

TS:   a && b || !c
来源：http://pt.hnjuh.cn

Java: a && b || !c
来源：http://iz.huanxung.cn

Go:   a && b || !c
来源：http://lq.colortex.cn

Ruby: a && b || !c
来源：http://ca.muxihuayi.cn

C#:   a && b || !c
来源：http://dp.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lf.yuexingan06.cn

Py:   if not data: return
来源：http://zq.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://md.szsharing.cn

JS:   if (!data) return;
来源：http://nw.colortex.cn

TS:   if (!data) return;
来源：http://yq.nszjky.cn

Java: if (data == null) return;
来源：http://yj.hnjuh.cn

Go:   if data == nil { return }
来源：http://bt.newstarts.cn

Ruby: return if data.nil?
来源：http://am.panjiajie.cn

C#:   if (data == null) return;
来源：http://hf.yuntaijiaju.cn

================================================================================
来源：http://mz.shxzukj.cn

C. 函数与作用域
来源：http://jq.shtwfgs.cn

================================================================================
来源：http://il.haigaiapp.cn

[C01] 定义函数
来源：http://pv.colortex.cn

Py:   def add(a, b): return a + b
来源：http://nh.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ai.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://te.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nt.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yz.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zl.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://ma.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rw.shxzskj.cn

[C02] 默认参数
来源：http://nd.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://jz.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zk.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://ni.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hc.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dh.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dj.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://yk.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://lg.nszjky.cn

[C03] 可变参数
来源：http://xd.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://vz.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xd.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tb.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sv.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lk.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zf.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://er.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tl.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://fv.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://es.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jz.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hw.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://md.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://md.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://ej.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://ik.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://fr.521024.cn

[C05] 返回多个值
来源：http://qk.9csxet.cn

Py:   return a, b
来源：http://jx.shxzskj.cn

PHP:  return [$a, $b];
来源：http://im.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jz.panjiajie.cn

TS:   return { a, b };
来源：http://km.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dw.wgjwhj.cn

Go:   return a, b
来源：http://bw.hnjuh.cn

Ruby: return a, b
来源：http://qd.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://ib.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://oc.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://yz.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ix.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://xk.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://bc.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lo.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fz.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://wx.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lf.hahajie.cn

[C07] 把函数作为参数传入
来源：http://fb.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ce.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oy.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bg.szsharing.cn

TS:   arr.map(String)
来源：http://gy.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xv.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sr.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://nj.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pf.521024.cn

[C08] 闭包
来源：http://fv.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bd.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fl.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kr.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ab.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tk.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jc.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sj.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jm.asd995.cn

[C09] 递归
来源：http://ym.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ao.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dd.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uf.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ne.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ms.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ae.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ai.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://si.szsharing.cn

[C10] 变量作用域
来源：http://ce.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mv.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lz.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nv.bjjhwx.cn

TS:   同 JS
来源：http://jj.shxzukj.cn

Java: 方法内为块级作用域
来源：http://uw.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://up.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ld.huixinmuqiang.cn

C#:   块级作用域
来源：http://ca.bjjhwx.cn

[C11] 模块导入与导出
来源：http://gs.nicolike.cn

Py:   from module import func
来源：http://us.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://po.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sh.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vr.huanxung.cn

Java: import java.util.List;
来源：http://yg.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jf.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://mq.nicolike.cn

C#:   using System.Text;
来源：http://mg.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://xw.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://td.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://zg.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://ki.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://jw.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nz.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://vk.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://ta.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yd.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://bq.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yp.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yg.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lv.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hr.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eb.huanxung.cn

Go:   func add(a, b int) int
来源：http://pn.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bs.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ah.jianghongdianzi.cn

[C14] 泛型函数
来源：http://xn.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uh.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://yz.nicolike.cn

JS:   // 无泛型
来源：http://xx.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zv.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ou.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kf.newstarts.cn

Ruby: # 无泛型
来源：http://bx.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ll.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://xo.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yz.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://lm.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ih.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iy.9csxet.cn

Java: // 无解构
来源：http://rc.muxihuayi.cn

Go:   // 无解构
来源：http://sh.nicolike.cn

Ruby: a, b = pair
来源：http://an.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://zo.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://jd.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ae.chemitech.net.cn

PHP:  // 无重载
来源：http://et.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ki.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://rj.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://re.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://da.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://gc.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sv.nszjky.cn

================================================================================
来源：http://qp.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://le.gzmigu.cn

================================================================================
来源：http://pw.newstarts.cn

[D01] 创建数组 / 列表
来源：http://if.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qx.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yz.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pw.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tz.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://na.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://wc.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://ax.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hs.hnjuh.cn

[D02] 追加元素到末尾
来源：http://fu.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ot.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xy.hahajie.cn

JS:   arr.push(4);
来源：http://jc.lnxyls.cn

TS:   arr.push(4);
来源：http://rd.hahajie.cn

Java: list.add(4);
来源：http://ol.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://fe.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://ys.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://ej.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://nc.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://kx.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pf.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dv.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://kg.9csxet.cn

Java: list.add(0, 0);
来源：http://qu.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ni.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ov.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://ei.hahajie.cn

[D04] 删除元素
来源：http://td.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fr.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hr.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ec.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://ne.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pr.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://id.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xs.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pp.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://dz.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zx.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vy.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gn.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://xv.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://yb.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ud.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tp.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://li.muxihuayi.cn

[D06] 数组长度
来源：http://wy.yuexingan06.cn

Py:   len(arr)
来源：http://vl.jianghongdianzi.cn

PHP:  count($arr);
来源：http://ww.jctech888.com.cn

JS:   arr.length
来源：http://ah.hnjuh.cn

TS:   arr.length
来源：http://ux.huanxung.cn

Java: list.size();
来源：http://mf.521024.cn

Go:   len(arr)
来源：http://uc.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://re.colortex.cn

C#:   list.Count;
来源：http://nw.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://rg.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ed.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wx.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://ix.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://jd.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://ne.haigaiapp.cn

Go:   arr[1:4]
来源：http://jk.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://sr.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://zx.muxihuayi.cn

[D08] 合并两个数组
来源：http://qy.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://dj.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://yh.muxihuayi.cn


<!-- 参考信息 -->