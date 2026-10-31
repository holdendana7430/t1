代发 wailian999

Py:   for i in range(10): print(i)
来源：http://lc.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jp.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sd.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bv.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fj.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://of.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://zi.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ef.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://un.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://mm.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mm.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://af.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oq.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gg.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tr.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://ee.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://so.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://zm.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yf.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wi.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yl.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eo.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sx.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uq.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ei.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rv.9csxet.cn

[B07] while 循环
来源：http://je.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://ga.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zd.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://vc.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://bq.521024.cn

Java: while (i < 10) { i++; }
来源：http://gl.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yy.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://ac.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://bc.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://db.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://ej.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eq.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://dk.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://dm.521024.cn

Java: do { i++; } while (i < 10);
来源：http://hc.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://in.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jr.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://pw.nszjky.cn

[B09] break 与 continue
来源：http://rz.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qm.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aq.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fq.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://it.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pv.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://li.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yi.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://rd.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://do.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://st.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ps.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ik.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qd.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wn.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qm.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bn.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://uz.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://tn.asd995.cn

PHP:  range(0, 10, 2);
来源：http://bm.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eb.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gr.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lm.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pf.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://ej.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fu.nszjky.cn

[B12] 跳出多层循环
来源：http://ci.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hp.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://he.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ph.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iy.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ck.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yc.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cg.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dt.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://jc.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://ot.colortex.cn

PHP:  is_numeric($x)
来源：http://ak.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zy.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nb.haigaiapp.cn

Java: x instanceof Number
来源：http://cx.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://am.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://cu.nicolike.cn

C#:   x is int or double or decimal
来源：http://ze.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://hn.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mc.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sj.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://le.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://an.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fi.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zv.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ef.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lv.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://pf.nicolike.cn

Py:   a and b or not c
来源：http://fm.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ka.jctech888.com.cn

JS:   a && b || !c
来源：http://zo.9csxet.cn

TS:   a && b || !c
来源：http://gm.9csxet.cn

Java: a && b || !c
来源：http://pn.nszjky.cn

Go:   a && b || !c
来源：http://el.yuexingan06.cn

Ruby: a && b || !c
来源：http://hi.colortex.cn

C#:   a && b || !c
来源：http://gl.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://re.yuntaijiaju.cn

Py:   if not data: return
来源：http://cg.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://zo.yuexingan06.cn

JS:   if (!data) return;
来源：http://jg.shxzukj.cn

TS:   if (!data) return;
来源：http://ts.bookmarksfly.cn

Java: if (data == null) return;
来源：http://nd.shxzskj.cn

Go:   if data == nil { return }
来源：http://tv.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://yk.9csxet.cn

C#:   if (data == null) return;
来源：http://cv.szsharing.cn

================================================================================
来源：http://yg.huixiangedu.cn

C. 函数与作用域
来源：http://rf.shxzskj.cn

================================================================================
来源：http://ss.nicolike.cn

[C01] 定义函数
来源：http://qa.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://ts.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uu.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://ic.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jj.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://iu.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ni.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://xq.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zn.huixiangedu.cn

[C02] 默认参数
来源：http://ky.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://xy.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ux.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://lc.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cf.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hu.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zh.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://xv.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://bz.huanxung.cn

[C03] 可变参数
来源：http://bn.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://sz.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lt.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aj.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aw.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mo.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sv.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pn.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oh.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://yx.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://at.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kl.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ox.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ti.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://os.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://jb.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://mf.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://nh.colortex.cn

[C05] 返回多个值
来源：http://lw.nszjky.cn

Py:   return a, b
来源：http://cm.asd995.cn

PHP:  return [$a, $b];
来源：http://gx.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bu.panjiajie.cn

TS:   return { a, b };
来源：http://jv.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://td.nszjky.cn

Go:   return a, b
来源：http://mg.shxzukj.cn

Ruby: return a, b
来源：http://yw.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://uq.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://ob.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://aa.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nt.nicolike.cn

JS:   const square = x => x * x;
来源：http://bv.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ra.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dz.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ak.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://cl.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xp.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://qy.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ki.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uv.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://an.wgjwhj.cn

TS:   arr.map(String)
来源：http://kz.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gi.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rv.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://vk.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hs.9csxet.cn

[C08] 闭包
来源：http://je.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ax.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gf.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nu.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dl.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ep.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zi.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lk.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cl.szsharing.cn

[C09] 递归
来源：http://wh.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://op.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gi.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dw.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://it.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bi.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qh.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ui.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jv.newstarts.cn

[C10] 变量作用域
来源：http://rz.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ur.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rt.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://be.haigaiapp.cn

TS:   同 JS
来源：http://rs.hnjuh.cn

Java: 方法内为块级作用域
来源：http://nl.wgjwhj.cn

Go:   花括号块级作用域
来源：http://so.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mn.haigaiapp.cn

C#:   块级作用域
来源：http://nn.9csxet.cn

[C11] 模块导入与导出
来源：http://ev.shtwfgs.cn

Py:   from module import func
来源：http://sz.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://el.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hx.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nt.jianghongdianzi.cn

Java: import java.util.List;
来源：http://ae.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dt.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://up.newstarts.cn

C#:   using System.Text;
来源：http://qz.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://hq.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://au.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://ic.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://zp.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://wc.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zl.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://va.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://ye.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kf.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://rt.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nb.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://li.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ll.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xn.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ql.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://ux.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wq.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vf.szsharing.cn

[C14] 泛型函数
来源：http://ot.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gf.szxytkj.cn

PHP:  // 无泛型
来源：http://eo.huixiangedu.cn

JS:   // 无泛型
来源：http://xb.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iz.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tm.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rm.hahajie.cn

Ruby: # 无泛型
来源：http://zy.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eu.colortex.cn

[C15] 解构 / 展开参数
来源：http://vu.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kn.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://pp.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://la.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xj.9csxet.cn

Java: // 无解构
来源：http://ik.shxzukj.cn

Go:   // 无解构
来源：http://fp.lnxyls.cn

Ruby: a, b = pair
来源：http://gp.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://eh.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://bx.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bg.nszjky.cn

PHP:  // 无重载
来源：http://iw.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sp.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://eb.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pd.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ob.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://vh.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uj.huanxung.cn

================================================================================
来源：http://tc.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://vv.muxihuayi.cn

================================================================================
来源：http://iu.9csxet.cn

[D01] 创建数组 / 列表
来源：http://ys.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://av.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yg.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://te.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kb.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hs.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://zh.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://cr.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cb.shxzskj.cn

[D02] 追加元素到末尾
来源：http://cx.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ro.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://py.wgjwhj.cn

JS:   arr.push(4);
来源：http://oj.hnjuh.cn

TS:   arr.push(4);
来源：http://ps.521024.cn

Java: list.add(4);
来源：http://jy.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://bt.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://ti.bjjhwx.cn

C#:   list.Add(4);
来源：http://lu.asd995.cn

[D03] 在指定位置插入元素
来源：http://ps.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://bo.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cb.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fb.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://aa.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://zv.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lk.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ql.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://dm.shxzskj.cn

[D04] 删除元素
来源：http://gd.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qz.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sx.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vh.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://le.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fq.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zj.hahajie.cn


<!-- 参考信息 -->