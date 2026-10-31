代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xi.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fe.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zd.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ch.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bn.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fw.haigaiapp.cn

[B07] while 循环
来源：http://qu.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://wa.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ob.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://lp.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://nn.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://fe.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ga.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://so.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://bz.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://rq.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://cs.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hr.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://tj.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://rg.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://hy.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ah.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ln.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://vl.szsharing.cn

[B09] break 与 continue
来源：http://eb.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ve.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oz.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ne.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ki.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://op.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kh.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gr.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gs.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://ku.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lj.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ay.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hc.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://co.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ee.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ay.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hb.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wg.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://ti.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://ma.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://xt.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sc.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lt.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gp.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bt.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://af.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sn.huixiangedu.cn

[B12] 跳出多层循环
来源：http://gq.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zg.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ad.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hm.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sm.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qi.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rv.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bt.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://po.muxihuayi.cn

[B13] 判断是否为数字
来源：http://ng.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://xv.gzmigu.cn

PHP:  is_numeric($x)
来源：http://iw.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nx.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xr.shxzukj.cn

Java: x instanceof Number
来源：http://fg.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ix.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://ax.shxzskj.cn

C#:   x is int or double or decimal
来源：http://pk.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://de.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cv.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cl.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ni.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://hj.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oi.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://au.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dv.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rj.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://nz.jctech888.com.cn

Py:   a and b or not c
来源：http://oc.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://et.nicolike.cn

JS:   a && b || !c
来源：http://ot.nicolike.cn

TS:   a && b || !c
来源：http://js.newstarts.cn

Java: a && b || !c
来源：http://gn.jctech888.com.cn

Go:   a && b || !c
来源：http://il.bookmarksfly.cn

Ruby: a && b || !c
来源：http://gc.shxzskj.cn

C#:   a && b || !c
来源：http://kv.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sd.chemitech.net.cn

Py:   if not data: return
来源：http://bh.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://vg.shxzskj.cn

JS:   if (!data) return;
来源：http://vo.huanxung.cn

TS:   if (!data) return;
来源：http://hv.huixiangedu.cn

Java: if (data == null) return;
来源：http://is.shxzskj.cn

Go:   if data == nil { return }
来源：http://ad.wgjwhj.cn

Ruby: return if data.nil?
来源：http://kl.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://be.bjjhwx.cn

================================================================================
来源：http://td.shxzskj.cn

C. 函数与作用域
来源：http://lu.wgjwhj.cn

================================================================================
来源：http://dr.panjiajie.cn

[C01] 定义函数
来源：http://xe.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://kq.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ot.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://zx.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gc.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://df.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ca.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://dq.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wh.gzmigu.cn

[C02] 默认参数
来源：http://fi.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://fr.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://it.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://kp.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vp.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wa.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://st.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://et.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://ep.colortex.cn

[C03] 可变参数
来源：http://ri.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://fs.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fs.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pt.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tg.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uu.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uo.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eh.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lx.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://sr.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gs.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dc.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pc.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://or.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://re.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://hu.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://qg.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://mf.jianghongdianzi.cn

[C05] 返回多个值
来源：http://om.colortex.cn

Py:   return a, b
来源：http://ol.asd995.cn

PHP:  return [$a, $b];
来源：http://qd.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cb.haigaiapp.cn

TS:   return { a, b };
来源：http://ca.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sv.haigaiapp.cn

Go:   return a, b
来源：http://hj.colortex.cn

Ruby: return a, b
来源：http://vw.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://xz.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://gd.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://uj.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xz.newstarts.cn

JS:   const square = x => x * x;
来源：http://if.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://bv.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://si.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ql.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://og.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ct.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://gy.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xy.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://az.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://js.521024.cn

TS:   arr.map(String)
来源：http://bc.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ve.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nx.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://oc.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ga.shxzukj.cn

[C08] 闭包
来源：http://pe.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nl.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tt.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://px.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qt.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qt.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wv.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lz.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yt.jianghongdianzi.cn

[C09] 递归
来源：http://tq.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://il.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lp.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ju.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://js.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pp.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vx.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cu.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ii.521024.cn

[C10] 变量作用域
来源：http://rg.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jh.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://or.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tk.panjiajie.cn

TS:   同 JS
来源：http://bo.newstarts.cn

Java: 方法内为块级作用域
来源：http://dn.chemitech.net.cn

Go:   花括号块级作用域
来源：http://ho.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dh.521024.cn

C#:   块级作用域
来源：http://ho.hahajie.cn

[C11] 模块导入与导出
来源：http://fd.jianghongdianzi.cn

Py:   from module import func
来源：http://bc.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fc.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gr.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zb.nicolike.cn

Java: import java.util.List;
来源：http://ll.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jd.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://fr.9csxet.cn

C#:   using System.Text;
来源：http://sa.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://rx.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://lj.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://gd.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://gx.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://sc.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wi.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://yj.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://sj.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kl.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://xx.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ba.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tu.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gn.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://me.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ny.asd995.cn

Go:   func add(a, b int) int
来源：http://ng.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ac.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cc.shtwfgs.cn

[C14] 泛型函数
来源：http://px.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lb.asd995.cn

PHP:  // 无泛型
来源：http://hn.chemitech.net.cn

JS:   // 无泛型
来源：http://ab.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xh.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yb.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zf.asd995.cn

Ruby: # 无泛型
来源：http://qb.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ge.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://pn.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lo.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://ni.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oc.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dz.gzmigu.cn

Java: // 无解构
来源：http://gc.jctech888.com.cn

Go:   // 无解构
来源：http://mr.asd995.cn

Ruby: a, b = pair
来源：http://jh.colortex.cn

C#:   var (a, b) = pair;
来源：http://jj.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://zb.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rh.szxytkj.cn

PHP:  // 无重载
来源：http://cj.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ne.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://yc.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yo.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://du.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://zj.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ft.hahajie.cn

================================================================================
来源：http://jy.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://ph.newstarts.cn

================================================================================
来源：http://fe.521024.cn

[D01] 创建数组 / 列表
来源：http://br.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lx.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xx.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://la.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vj.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qe.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://gg.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://tp.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bp.newstarts.cn

[D02] 追加元素到末尾
来源：http://bx.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gh.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lo.szxytkj.cn

JS:   arr.push(4);
来源：http://qw.gzmigu.cn

TS:   arr.push(4);
来源：http://oz.asd995.cn

Java: list.add(4);
来源：http://vh.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://su.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://ef.wgjwhj.cn

C#:   list.Add(4);
来源：http://ej.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://bu.521024.cn

Py:   arr.insert(0, 0)
来源：http://rv.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://si.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://el.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://fa.newstarts.cn

Java: list.add(0, 0);
来源：http://rm.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wq.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ua.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://cz.chemitech.net.cn

[D04] 删除元素
来源：http://au.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tr.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wx.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xe.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://la.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jh.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aq.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lk.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qo.hahajie.cn

[D05] 访问与修改元素
来源：http://fm.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oe.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nr.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pw.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://bj.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://kp.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://mh.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nm.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lv.szsharing.cn

[D06] 数组长度
来源：http://bu.panjiajie.cn

Py:   len(arr)
来源：http://qs.jctech888.com.cn

PHP:  count($arr);
来源：http://yq.huixinmuqiang.cn

JS:   arr.length
来源：http://sz.nicolike.cn

TS:   arr.length
来源：http://pd.huixiangedu.cn

Java: list.size();
来源：http://ap.lnxyls.cn

Go:   len(arr)
来源：http://ga.newstarts.cn

Ruby: arr.length; arr.size
来源：http://uj.huixiangedu.cn

C#:   list.Count;
来源：http://mz.hahajie.cn


<!-- 参考信息 -->