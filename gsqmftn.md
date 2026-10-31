代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vl.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://uh.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ec.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cc.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mo.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cz.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kl.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bb.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gd.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://og.hnjuh.cn

[B07] while 循环
来源：http://eo.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://og.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ge.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://pe.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://rj.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://bb.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gk.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://qs.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://sy.asd995.cn

[B08] do-while（至少执行一次）
来源：http://kt.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://xj.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ps.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://ku.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://qs.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://jb.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tu.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sh.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://jb.gzmigu.cn

[B09] break 与 continue
来源：http://no.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ki.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ow.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zs.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://se.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mc.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tc.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hj.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ut.colortex.cn

[B10] 遍历同时拿索引
来源：http://jq.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fh.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pp.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uq.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xm.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vg.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pe.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kb.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ff.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://ld.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://ou.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://ly.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qh.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pi.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jw.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ik.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://cn.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://co.wgjwhj.cn

[B12] 跳出多层循环
来源：http://ui.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fm.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gj.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dh.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ga.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lm.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qc.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wk.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ro.jctech888.com.cn

[B13] 判断是否为数字
来源：http://yc.521024.cn

Py:   isinstance(x, (int, float))
来源：http://dh.szsharing.cn

PHP:  is_numeric($x)
来源：http://rt.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iz.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hp.newstarts.cn

Java: x instanceof Number
来源：http://od.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dk.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://yy.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://ml.szsharing.cn

[B14] 判断值是否在集合内
来源：http://es.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mf.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bh.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://gi.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://gp.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wp.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uw.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bn.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sc.hnjuh.cn

[B15] 布尔运算与取反
来源：http://mo.panjiajie.cn

Py:   a and b or not c
来源：http://sx.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ke.jctech888.com.cn

JS:   a && b || !c
来源：http://mf.wgjwhj.cn

TS:   a && b || !c
来源：http://wg.jctech888.com.cn

Java: a && b || !c
来源：http://eo.wgjwhj.cn

Go:   a && b || !c
来源：http://ny.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://ib.9csxet.cn

C#:   a && b || !c
来源：http://rb.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wv.asd995.cn

Py:   if not data: return
来源：http://ng.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://ja.bookmarksfly.cn

JS:   if (!data) return;
来源：http://ka.wgjwhj.cn

TS:   if (!data) return;
来源：http://gy.gzmigu.cn

Java: if (data == null) return;
来源：http://ih.9csxet.cn

Go:   if data == nil { return }
来源：http://te.nszjky.cn

Ruby: return if data.nil?
来源：http://tw.nszjky.cn

C#:   if (data == null) return;
来源：http://pz.haigaiapp.cn

================================================================================
来源：http://wr.wgjwhj.cn

C. 函数与作用域
来源：http://un.huixinmuqiang.cn

================================================================================
来源：http://cz.szsharing.cn

[C01] 定义函数
来源：http://ud.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://hz.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mu.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://sm.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zf.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zv.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oc.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://qx.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qz.yuntaijiaju.cn

[C02] 默认参数
来源：http://em.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://to.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cl.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://ec.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pd.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ry.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sm.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://sj.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://zc.colortex.cn

[C03] 可变参数
来源：http://nf.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://lj.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lu.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jp.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ls.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ma.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://go.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nj.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rb.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://tb.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sd.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://at.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lv.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gx.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://wg.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://bc.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://rh.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://es.huixinmuqiang.cn

[C05] 返回多个值
来源：http://xn.yuexingan06.cn

Py:   return a, b
来源：http://bv.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://vh.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bx.wgjwhj.cn

TS:   return { a, b };
来源：http://sn.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zo.jctech888.com.cn

Go:   return a, b
来源：http://du.muxihuayi.cn

Ruby: return a, b
来源：http://ad.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://qw.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://wp.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://vw.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kz.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://ms.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://nu.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://we.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jh.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://gq.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wn.521024.cn

[C07] 把函数作为参数传入
来源：http://tl.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ol.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://of.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bj.shtwfgs.cn

TS:   arr.map(String)
来源：http://hn.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://la.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tt.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://gc.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eg.huanxung.cn

[C08] 闭包
来源：http://az.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xl.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cr.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dd.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pk.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ms.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://al.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gr.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vi.chemitech.net.cn

[C09] 递归
来源：http://rd.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bq.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fa.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lj.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hd.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rm.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://us.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dh.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ml.shtwfgs.cn

[C10] 变量作用域
来源：http://qv.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://is.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jy.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ct.hahajie.cn

TS:   同 JS
来源：http://fr.gzmigu.cn

Java: 方法内为块级作用域
来源：http://db.szsharing.cn

Go:   花括号块级作用域
来源：http://hb.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yy.yuntaijiaju.cn

C#:   块级作用域
来源：http://vk.shxzukj.cn

[C11] 模块导入与导出
来源：http://ia.jianghongdianzi.cn

Py:   from module import func
来源：http://rz.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mb.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ro.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tg.huanxung.cn

Java: import java.util.List;
来源：http://tn.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ba.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://mc.jianghongdianzi.cn

C#:   using System.Text;
来源：http://kr.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://dd.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://hn.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://kl.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://ly.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://rx.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ko.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://kz.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://el.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dc.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://vu.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gd.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rz.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sr.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xu.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tq.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://ei.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pr.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wv.jianghongdianzi.cn

[C14] 泛型函数
来源：http://bl.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mm.szsharing.cn

PHP:  // 无泛型
来源：http://lz.lnxyls.cn

JS:   // 无泛型
来源：http://vh.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vb.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ol.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dv.newstarts.cn

Ruby: # 无泛型
来源：http://pn.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mt.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://sh.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ml.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://ih.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jw.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sz.bjjhwx.cn

Java: // 无解构
来源：http://wc.szsharing.cn

Go:   // 无解构
来源：http://mv.yuexingan06.cn

Ruby: a, b = pair
来源：http://bw.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://sa.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://st.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ay.nszjky.cn

PHP:  // 无重载
来源：http://fs.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eh.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://di.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rx.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://lt.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://ny.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vh.haigaiapp.cn

================================================================================
来源：http://zo.colortex.cn

D. 数组 / 列表 / 集合
来源：http://ht.hahajie.cn

================================================================================
来源：http://kp.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://pc.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mm.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kw.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sa.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://et.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oy.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://zm.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://mo.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tp.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://xy.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dj.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gr.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://ow.nicolike.cn

TS:   arr.push(4);
来源：http://zf.haigaiapp.cn

Java: list.add(4);
来源：http://te.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://xe.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ba.jctech888.com.cn

C#:   list.Add(4);
来源：http://qy.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://ee.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://wk.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mx.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yh.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://rk.521024.cn

Java: list.add(0, 0);
来源：http://xm.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zb.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ga.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://ta.yuntaijiaju.cn

[D04] 删除元素
来源：http://am.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fd.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bz.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fe.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://sw.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ga.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pu.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nd.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rb.jctech888.com.cn

[D05] 访问与修改元素
来源：http://lh.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nt.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jz.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://an.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://bp.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://av.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://fd.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sq.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qr.szsharing.cn

[D06] 数组长度
来源：http://yy.huixinmuqiang.cn

Py:   len(arr)
来源：http://is.wgjwhj.cn

PHP:  count($arr);
来源：http://sh.gzmigu.cn

JS:   arr.length
来源：http://bf.colortex.cn

TS:   arr.length
来源：http://hz.hnjuh.cn


<!-- 参考信息 -->