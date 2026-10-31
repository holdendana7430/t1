代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cy.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ok.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://su.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cb.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://iz.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://wx.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tg.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fc.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wu.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://te.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vy.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://sh.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jy.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://rl.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://un.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kl.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qh.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ki.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bt.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://au.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bi.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dq.bjjhwx.cn

[B07] while 循环
来源：http://tf.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://uq.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sg.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://hy.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://yz.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://ff.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pk.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://zr.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://xo.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://qh.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://ph.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wv.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://lq.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://ct.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://mf.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ao.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ed.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://oj.nszjky.cn

[B09] break 与 continue
来源：http://oc.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ig.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fk.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lr.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ib.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ry.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ad.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iz.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gr.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://xb.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ml.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tj.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://he.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ob.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bp.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ac.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ce.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eh.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://kr.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://qh.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://sa.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://me.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kj.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uy.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xv.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://vk.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xb.shtwfgs.cn

[B12] 跳出多层循环
来源：http://pl.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://aw.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sh.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qs.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ea.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://no.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dq.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://in.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lt.newstarts.cn

[B13] 判断是否为数字
来源：http://rf.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://rt.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://vr.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ul.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xp.wgjwhj.cn

Java: x instanceof Number
来源：http://eq.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aq.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://km.9csxet.cn

C#:   x is int or double or decimal
来源：http://nj.nicolike.cn

[B14] 判断值是否在集合内
来源：http://ew.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zf.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mo.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://wp.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://vl.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sw.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pi.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nm.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ud.shxzskj.cn

[B15] 布尔运算与取反
来源：http://ou.hahajie.cn

Py:   a and b or not c
来源：http://tj.9csxet.cn

PHP:  $a && $b || !$c
来源：http://oh.wgjwhj.cn

JS:   a && b || !c
来源：http://kb.szxytkj.cn

TS:   a && b || !c
来源：http://uy.szsharing.cn

Java: a && b || !c
来源：http://ay.huanxung.cn

Go:   a && b || !c
来源：http://gh.nicolike.cn

Ruby: a && b || !c
来源：http://iz.9csxet.cn

C#:   a && b || !c
来源：http://ns.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xh.newstarts.cn

Py:   if not data: return
来源：http://wu.colortex.cn

PHP:  if (!$data) { return; }
来源：http://ld.yuexingan06.cn

JS:   if (!data) return;
来源：http://yg.gzmigu.cn

TS:   if (!data) return;
来源：http://jy.asd995.cn

Java: if (data == null) return;
来源：http://le.nicolike.cn

Go:   if data == nil { return }
来源：http://zr.9csxet.cn

Ruby: return if data.nil?
来源：http://mr.chemitech.net.cn

C#:   if (data == null) return;
来源：http://nn.wgjwhj.cn

================================================================================
来源：http://md.nicolike.cn

C. 函数与作用域
来源：http://vj.jianghongdianzi.cn

================================================================================
来源：http://oo.szsharing.cn

[C01] 定义函数
来源：http://to.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://kj.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zv.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://gt.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ps.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dl.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lg.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://jf.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rj.chemitech.net.cn

[C02] 默认参数
来源：http://ro.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://su.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yo.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://yt.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zs.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sm.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zl.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://jx.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://hj.muxihuayi.cn

[C03] 可变参数
来源：http://tf.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://vj.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nh.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fc.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zd.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yx.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mk.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tk.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lg.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://ou.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wh.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aw.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://os.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kf.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://nm.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://xm.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://lz.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://nj.gzmigu.cn

[C05] 返回多个值
来源：http://iv.hnjuh.cn

Py:   return a, b
来源：http://ae.gzmigu.cn

PHP:  return [$a, $b];
来源：http://nm.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bw.lnxyls.cn

TS:   return { a, b };
来源：http://wz.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ra.nszjky.cn

Go:   return a, b
来源：http://yr.9csxet.cn

Ruby: return a, b
来源：http://oe.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://kc.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://sq.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://lj.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mn.nicolike.cn

JS:   const square = x => x * x;
来源：http://el.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://ep.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fa.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ld.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://yf.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lb.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://do.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://me.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ep.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ql.colortex.cn

TS:   arr.map(String)
来源：http://wc.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xk.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fx.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ib.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lp.wgjwhj.cn

[C08] 闭包
来源：http://fb.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://da.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://es.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://px.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kv.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zp.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://um.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hi.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ev.gzmigu.cn

[C09] 递归
来源：http://ix.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cu.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yr.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yc.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kx.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ai.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zh.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sb.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://du.nszjky.cn

[C10] 变量作用域
来源：http://yw.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gb.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vx.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://me.colortex.cn

TS:   同 JS
来源：http://rs.hahajie.cn

Java: 方法内为块级作用域
来源：http://sa.gzmigu.cn

Go:   花括号块级作用域
来源：http://wr.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://za.nszjky.cn

C#:   块级作用域
来源：http://pz.yuexingan06.cn

[C11] 模块导入与导出
来源：http://do.yuexingan06.cn

Py:   from module import func
来源：http://cw.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ob.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://en.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vy.huixinmuqiang.cn

Java: import java.util.List;
来源：http://az.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rh.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://he.hnjuh.cn

C#:   using System.Text;
来源：http://gw.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://bm.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://pk.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://xv.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://xw.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://bq.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qb.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://np.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://gz.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ta.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://hd.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vv.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://td.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fz.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mb.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://no.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://cc.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pe.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sa.yuntaijiaju.cn

[C14] 泛型函数
来源：http://tk.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ia.panjiajie.cn

PHP:  // 无泛型
来源：http://ov.hahajie.cn

JS:   // 无泛型
来源：http://bm.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://an.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://su.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://it.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://mv.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://da.szsharing.cn

[C15] 解构 / 展开参数
来源：http://tw.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ic.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://nm.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eb.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yg.lnxyls.cn

Java: // 无解构
来源：http://xq.shxzukj.cn

Go:   // 无解构
来源：http://vt.asd995.cn

Ruby: a, b = pair
来源：http://rj.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://gg.newstarts.cn

[C16] 函数 / 方法重载
来源：http://ks.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://io.521024.cn

PHP:  // 无重载
来源：http://xo.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wd.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://rd.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xd.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://hc.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://fv.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sk.szxytkj.cn

================================================================================
来源：http://fx.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://kj.huanxung.cn

================================================================================
来源：http://ca.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://ny.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ie.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wn.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zj.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ct.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://je.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://fr.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://zd.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mi.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://hw.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://co.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://so.asd995.cn

JS:   arr.push(4);
来源：http://tc.521024.cn

TS:   arr.push(4);
来源：http://ow.wgjwhj.cn

Java: list.add(4);
来源：http://ib.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://pp.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://xi.nicolike.cn

C#:   list.Add(4);
来源：http://zo.colortex.cn

[D03] 在指定位置插入元素
来源：http://te.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://zv.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sc.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vf.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://np.nszjky.cn

Java: list.add(0, 0);
来源：http://ui.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yb.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gt.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://cy.lnxyls.cn

[D04] 删除元素
来源：http://tt.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tz.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eh.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hu.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://pk.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cs.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pk.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yt.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kg.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://by.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mr.gzmigu.cn


<!-- 参考信息 -->