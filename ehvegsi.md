代发 wailian999

Py:   for i in range(10): print(i)
来源：http://wy.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sk.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gr.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mk.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ji.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xp.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://po.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mx.colortex.cn

[B05] 遍历数组 / 列表
来源：http://ic.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://yv.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dn.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ff.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cu.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://be.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fd.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://rc.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ra.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://ct.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://md.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uo.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bh.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ry.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gb.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wj.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://az.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://io.yuexingan06.cn

[B07] while 循环
来源：http://eo.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://fs.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wr.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://my.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://jv.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://ob.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qb.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://id.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://xj.asd995.cn

[B08] do-while（至少执行一次）
来源：http://cq.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://uw.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hn.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://ff.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://yu.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://te.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yt.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pj.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://bl.szxytkj.cn

[B09] break 与 continue
来源：http://dw.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ew.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ur.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pt.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gl.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vq.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://me.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yj.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pf.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://tm.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wc.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://as.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mn.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pr.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kg.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vh.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://in.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fc.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://vj.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://zi.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://wb.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://du.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ui.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hr.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hb.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://di.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kw.jctech888.com.cn

[B12] 跳出多层循环
来源：http://ud.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ss.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oe.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cx.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fl.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jn.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uf.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ot.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gx.haigaiapp.cn

[B13] 判断是否为数字
来源：http://pj.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://mi.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://br.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://on.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ie.huixinmuqiang.cn

Java: x instanceof Number
来源：http://yd.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wn.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://jw.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://ba.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://kl.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://an.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jf.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ph.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://gh.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qr.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oq.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://af.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://af.colortex.cn

[B15] 布尔运算与取反
来源：http://zn.yuntaijiaju.cn

Py:   a and b or not c
来源：http://ic.521024.cn

PHP:  $a && $b || !$c
来源：http://wt.panjiajie.cn

JS:   a && b || !c
来源：http://et.9csxet.cn

TS:   a && b || !c
来源：http://rb.gzmigu.cn

Java: a && b || !c
来源：http://uc.huixinmuqiang.cn

Go:   a && b || !c
来源：http://ex.muxihuayi.cn

Ruby: a && b || !c
来源：http://qm.panjiajie.cn

C#:   a && b || !c
来源：http://gs.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fx.huixiangedu.cn

Py:   if not data: return
来源：http://qb.521024.cn

PHP:  if (!$data) { return; }
来源：http://oo.hnjuh.cn

JS:   if (!data) return;
来源：http://jn.bjjhwx.cn

TS:   if (!data) return;
来源：http://pw.muxihuayi.cn

Java: if (data == null) return;
来源：http://ne.szsharing.cn

Go:   if data == nil { return }
来源：http://ox.szsharing.cn

Ruby: return if data.nil?
来源：http://ut.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://ha.hnjuh.cn

================================================================================
来源：http://ad.muxihuayi.cn

C. 函数与作用域
来源：http://um.shtwfgs.cn

================================================================================
来源：http://qg.jianghongdianzi.cn

[C01] 定义函数
来源：http://qt.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://zo.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uh.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://we.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://af.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fa.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ad.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://oa.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://de.hahajie.cn

[C02] 默认参数
来源：http://ft.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://ul.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eq.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://ng.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rn.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aq.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dn.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://ku.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://jz.lnxyls.cn

[C03] 可变参数
来源：http://kr.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://xy.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vw.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rz.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://af.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ei.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sj.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nh.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ic.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://mx.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gb.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mk.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qb.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://os.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://hv.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://ut.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://hc.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://hq.muxihuayi.cn

[C05] 返回多个值
来源：http://jj.szxytkj.cn

Py:   return a, b
来源：http://cf.lnxyls.cn

PHP:  return [$a, $b];
来源：http://go.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zx.bjjhwx.cn

TS:   return { a, b };
来源：http://eq.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sc.yuntaijiaju.cn

Go:   return a, b
来源：http://po.yuntaijiaju.cn

Ruby: return a, b
来源：http://oc.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://az.521024.cn

[C06] 匿名函数 / lambda
来源：http://jq.colortex.cn

Py:   square = lambda x: x * x
来源：http://gg.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qf.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://nk.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://hy.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://de.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rn.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://vy.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://le.colortex.cn

[C07] 把函数作为参数传入
来源：http://wn.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lx.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://th.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rf.gzmigu.cn

TS:   arr.map(String)
来源：http://kv.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fu.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wu.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://fk.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qd.panjiajie.cn

[C08] 闭包
来源：http://kv.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://im.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uo.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hl.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lv.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pe.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vh.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nn.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hl.bookmarksfly.cn

[C09] 递归
来源：http://en.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dz.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gb.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pj.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://my.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cc.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sm.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vu.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oc.haigaiapp.cn

[C10] 变量作用域
来源：http://uv.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zt.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://go.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mr.bookmarksfly.cn

TS:   同 JS
来源：http://zu.gzmigu.cn

Java: 方法内为块级作用域
来源：http://le.9csxet.cn

Go:   花括号块级作用域
来源：http://dc.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wm.nicolike.cn

C#:   块级作用域
来源：http://es.shxzskj.cn

[C11] 模块导入与导出
来源：http://nl.nicolike.cn

Py:   from module import func
来源：http://rl.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hy.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://as.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oh.bjjhwx.cn

Java: import java.util.List;
来源：http://kq.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lf.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://jk.bjjhwx.cn

C#:   using System.Text;
来源：http://gr.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://lx.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://me.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://ah.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://dl.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://db.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yw.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://zm.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://il.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://or.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://io.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cj.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xx.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vm.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ym.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yd.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://hg.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lu.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cs.muxihuayi.cn

[C14] 泛型函数
来源：http://yi.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uk.haigaiapp.cn

PHP:  // 无泛型
来源：http://yg.asd995.cn

JS:   // 无泛型
来源：http://rt.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ed.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qe.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ar.shxzskj.cn

Ruby: # 无泛型
来源：http://wb.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yl.nszjky.cn

[C15] 解构 / 展开参数
来源：http://yg.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sh.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://zf.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://si.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rr.yuntaijiaju.cn

Java: // 无解构
来源：http://ms.lnxyls.cn

Go:   // 无解构
来源：http://wy.shxzskj.cn

Ruby: a, b = pair
来源：http://lr.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://iv.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://rp.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ju.chemitech.net.cn

PHP:  // 无重载
来源：http://yq.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fw.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://mi.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tc.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://sg.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://uw.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nv.jianghongdianzi.cn

================================================================================
来源：http://is.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://jf.newstarts.cn

================================================================================
来源：http://pb.hahajie.cn

[D01] 创建数组 / 列表
来源：http://dz.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qy.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zm.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gb.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jt.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wc.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://ka.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://hk.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dm.asd995.cn

[D02] 追加元素到末尾
来源：http://ao.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qs.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sh.wgjwhj.cn

JS:   arr.push(4);
来源：http://hv.asd995.cn

TS:   arr.push(4);
来源：http://tp.hnjuh.cn

Java: list.add(4);
来源：http://mo.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://ov.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://ph.shxzskj.cn

C#:   list.Add(4);
来源：http://vo.hahajie.cn

[D03] 在指定位置插入元素
来源：http://rz.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://bq.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ka.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ek.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://et.9csxet.cn

Java: list.add(0, 0);
来源：http://wh.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tq.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gh.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://cw.gzmigu.cn

[D04] 删除元素
来源：http://kr.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://so.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rj.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zv.colortex.cn

TS:   arr.splice(0, 1);
来源：http://sd.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pv.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vj.jctech888.com.cn


<!-- 参考信息 -->