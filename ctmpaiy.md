代发 wailian999

[B09] break 与 continue
来源：http://hm.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fl.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hh.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ah.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fl.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zz.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nt.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mi.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cp.9csxet.cn

[B10] 遍历同时拿索引
来源：http://jh.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://br.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hw.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ks.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gu.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kn.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://od.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zm.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wd.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://ay.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://ek.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://li.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ea.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zv.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wv.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zg.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://lm.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tr.jctech888.com.cn

[B12] 跳出多层循环
来源：http://tb.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yj.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wb.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zn.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pe.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hk.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sk.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xp.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ji.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://is.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://if.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://wn.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cv.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bs.colortex.cn

Java: x instanceof Number
来源：http://wp.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lv.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://oc.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://si.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://bm.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oz.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wr.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ey.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://xh.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://of.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ie.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oq.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lu.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://pc.chemitech.net.cn

Py:   a and b or not c
来源：http://kt.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://xm.haigaiapp.cn

JS:   a && b || !c
来源：http://zj.shtwfgs.cn

TS:   a && b || !c
来源：http://eu.shtwfgs.cn

Java: a && b || !c
来源：http://nv.shxzskj.cn

Go:   a && b || !c
来源：http://dq.colortex.cn

Ruby: a && b || !c
来源：http://ql.asd995.cn

C#:   a && b || !c
来源：http://gt.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wt.panjiajie.cn

Py:   if not data: return
来源：http://wv.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://uj.shtwfgs.cn

JS:   if (!data) return;
来源：http://xv.shxzskj.cn

TS:   if (!data) return;
来源：http://zy.nicolike.cn

Java: if (data == null) return;
来源：http://dn.szsharing.cn

Go:   if data == nil { return }
来源：http://mr.bjjhwx.cn

Ruby: return if data.nil?
来源：http://al.9csxet.cn

C#:   if (data == null) return;
来源：http://nh.szxytkj.cn

================================================================================
来源：http://uj.huixiangedu.cn

C. 函数与作用域
来源：http://gi.shtwfgs.cn

================================================================================
来源：http://hi.panjiajie.cn

[C01] 定义函数
来源：http://ds.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://sk.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oa.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://mb.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ez.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zn.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aq.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://tz.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fl.9csxet.cn

[C02] 默认参数
来源：http://tl.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://jq.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pv.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://oj.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bv.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ll.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nv.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://xt.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://vx.shxzskj.cn

[C03] 可变参数
来源：http://kg.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://tx.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://to.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sr.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zx.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://an.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lb.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kp.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zu.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://fc.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fl.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rt.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zo.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wj.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://pd.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://mh.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://hm.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://ao.szxytkj.cn

[C05] 返回多个值
来源：http://vp.521024.cn

Py:   return a, b
来源：http://no.newstarts.cn

PHP:  return [$a, $b];
来源：http://lp.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qa.szsharing.cn

TS:   return { a, b };
来源：http://di.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jx.gzmigu.cn

Go:   return a, b
来源：http://qb.shxzskj.cn

Ruby: return a, b
来源：http://wt.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://ce.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://pf.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://xv.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://us.lnxyls.cn

JS:   const square = x => x * x;
来源：http://tz.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://nc.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rl.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oo.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://ok.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qu.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://hc.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ul.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jh.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xg.wgjwhj.cn

TS:   arr.map(String)
来源：http://gk.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vt.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pp.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://vj.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nb.huixinmuqiang.cn

[C08] 闭包
来源：http://yi.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kc.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ff.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lx.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yq.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ru.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cv.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cd.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wz.9csxet.cn

[C09] 递归
来源：http://tb.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wk.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://he.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://io.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vy.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jl.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bb.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://md.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ia.colortex.cn

[C10] 变量作用域
来源：http://ae.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cw.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xd.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://by.bjjhwx.cn

TS:   同 JS
来源：http://xm.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://tl.huixiangedu.cn

Go:   花括号块级作用域
来源：http://jr.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dw.haigaiapp.cn

C#:   块级作用域
来源：http://pg.521024.cn

[C11] 模块导入与导出
来源：http://uu.lnxyls.cn

Py:   from module import func
来源：http://tx.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ba.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pw.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iv.huixinmuqiang.cn

Java: import java.util.List;
来源：http://ap.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://af.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://xt.shxzskj.cn

C#:   using System.Text;
来源：http://lk.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://dg.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://xa.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://at.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://hq.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://wo.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://do.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://jl.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://xd.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eq.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://dc.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oj.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xq.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xv.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://va.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mw.newstarts.cn

Go:   func add(a, b int) int
来源：http://ah.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zu.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lm.jctech888.com.cn

[C14] 泛型函数
来源：http://ye.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yi.colortex.cn

PHP:  // 无泛型
来源：http://if.9csxet.cn

JS:   // 无泛型
来源：http://qc.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bh.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uv.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tl.asd995.cn

Ruby: # 无泛型
来源：http://gy.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kx.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://hx.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ts.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://xk.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cu.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://px.panjiajie.cn

Java: // 无解构
来源：http://mu.colortex.cn

Go:   // 无解构
来源：http://sv.haigaiapp.cn

Ruby: a, b = pair
来源：http://em.newstarts.cn

C#:   var (a, b) = pair;
来源：http://rk.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://ck.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ul.huanxung.cn

PHP:  // 无重载
来源：http://bb.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rz.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://lh.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sa.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://uw.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://ew.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fc.bookmarksfly.cn

================================================================================
来源：http://mb.521024.cn

D. 数组 / 列表 / 集合
来源：http://lh.jctech888.com.cn

================================================================================
来源：http://uf.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://ke.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sf.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eq.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uv.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://do.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bx.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://pj.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://ft.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jz.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://at.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fi.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ty.yuexingan06.cn

JS:   arr.push(4);
来源：http://gm.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://po.521024.cn

Java: list.add(4);
来源：http://st.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://ge.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://vd.nicolike.cn

C#:   list.Add(4);
来源：http://mj.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://ip.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://gx.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lq.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xx.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://vt.9csxet.cn

Java: list.add(0, 0);
来源：http://eb.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wj.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bv.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://fb.asd995.cn

[D04] 删除元素
来源：http://gm.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zn.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mn.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://so.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://or.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pz.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://of.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ar.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qf.nicolike.cn

[D05] 访问与修改元素
来源：http://xi.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://at.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ed.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tu.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://ib.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://nz.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ce.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ru.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hs.gzmigu.cn

[D06] 数组长度
来源：http://qo.huixiangedu.cn

Py:   len(arr)
来源：http://co.gzmigu.cn

PHP:  count($arr);
来源：http://hz.wgjwhj.cn

JS:   arr.length
来源：http://ft.wgjwhj.cn

TS:   arr.length
来源：http://yi.panjiajie.cn

Java: list.size();
来源：http://cl.muxihuayi.cn

Go:   len(arr)
来源：http://ac.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://he.haigaiapp.cn

C#:   list.Count;
来源：http://ll.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://ce.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ee.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fc.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://av.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://oo.shxzskj.cn

Java: list.subList(1, 4);
来源：http://iw.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://oz.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://ih.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://sf.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://gz.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://ta.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://kn.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xx.nszjky.cn

TS:   [...a, ...b];
来源：http://yf.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hv.nszjky.cn

Go:   append(a, b...)
来源：http://qq.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://io.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://uc.huixiangedu.cn

[D09] 排序（升序）
来源：http://hz.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://at.shxzukj.cn

PHP:  sort($arr);
来源：http://ix.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ev.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ot.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dr.hnjuh.cn


<!-- 参考信息 -->