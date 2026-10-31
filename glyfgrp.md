代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://zl.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fx.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jg.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://kr.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tp.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://bs.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ps.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vq.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://go.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dl.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://do.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bd.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ix.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xh.wgjwhj.cn

[B07] while 循环
来源：http://nj.asd995.cn

Py:   while i < 10: i += 1
来源：http://hg.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://co.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://zi.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://js.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://ya.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nh.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://zr.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://ji.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://pu.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://vm.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yn.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://ix.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://io.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://pw.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tc.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qp.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://fp.521024.cn

[B09] break 与 continue
来源：http://vi.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ak.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ki.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ir.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sj.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://do.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cg.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uv.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jo.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://pf.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://da.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rk.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kr.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xk.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qe.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hp.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hx.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wv.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://wk.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://ol.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://yv.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ed.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://as.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wh.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kx.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://pw.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://od.huanxung.cn

[B12] 跳出多层循环
来源：http://jq.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yv.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fa.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xz.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hx.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zk.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ke.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rz.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uc.huixiangedu.cn

[B13] 判断是否为数字
来源：http://nl.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://er.gzmigu.cn

PHP:  is_numeric($x)
来源：http://ki.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qa.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vr.chemitech.net.cn

Java: x instanceof Number
来源：http://qn.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ki.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://am.szxytkj.cn

C#:   x is int or double or decimal
来源：http://yq.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://bs.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kx.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gn.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://et.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://gj.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tj.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wr.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lr.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uf.521024.cn

[B15] 布尔运算与取反
来源：http://zc.gzmigu.cn

Py:   a and b or not c
来源：http://fl.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://pk.huixiangedu.cn

JS:   a && b || !c
来源：http://bq.hahajie.cn

TS:   a && b || !c
来源：http://mt.nicolike.cn

Java: a && b || !c
来源：http://at.lnxyls.cn

Go:   a && b || !c
来源：http://we.colortex.cn

Ruby: a && b || !c
来源：http://pl.bookmarksfly.cn

C#:   a && b || !c
来源：http://tj.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ry.shxzukj.cn

Py:   if not data: return
来源：http://tk.521024.cn

PHP:  if (!$data) { return; }
来源：http://re.wgjwhj.cn

JS:   if (!data) return;
来源：http://np.wgjwhj.cn

TS:   if (!data) return;
来源：http://ha.szxytkj.cn

Java: if (data == null) return;
来源：http://bn.hahajie.cn

Go:   if data == nil { return }
来源：http://ix.szxytkj.cn

Ruby: return if data.nil?
来源：http://tr.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://ci.asd995.cn

================================================================================
来源：http://pn.asd995.cn

C. 函数与作用域
来源：http://aq.hnjuh.cn

================================================================================
来源：http://vn.wgjwhj.cn

[C01] 定义函数
来源：http://lq.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://cv.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cd.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://wb.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ho.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kq.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rj.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://ld.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://de.shxzukj.cn

[C02] 默认参数
来源：http://re.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://je.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pg.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://hv.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rp.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ic.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ij.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://sh.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://mt.9csxet.cn

[C03] 可变参数
来源：http://wj.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://qd.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ju.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mk.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uy.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nv.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hn.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yn.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ka.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://yf.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lo.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pn.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qv.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qk.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://bp.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://oi.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://dy.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://un.shxzukj.cn

[C05] 返回多个值
来源：http://af.hnjuh.cn

Py:   return a, b
来源：http://cu.nszjky.cn

PHP:  return [$a, $b];
来源：http://he.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vx.shxzskj.cn

TS:   return { a, b };
来源：http://bp.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bq.colortex.cn

Go:   return a, b
来源：http://dy.asd995.cn

Ruby: return a, b
来源：http://gn.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://pv.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://rv.521024.cn

Py:   square = lambda x: x * x
来源：http://kl.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rs.szsharing.cn

JS:   const square = x => x * x;
来源：http://go.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://pm.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hp.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sb.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://tz.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://my.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://iy.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ms.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bu.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uj.szsharing.cn

TS:   arr.map(String)
来源：http://zc.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://au.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ef.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://ym.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mt.hahajie.cn

[C08] 闭包
来源：http://wb.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fn.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jh.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://da.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lf.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://li.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uf.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ub.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ox.szxytkj.cn

[C09] 递归
来源：http://rj.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xh.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://te.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ux.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oq.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://st.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dd.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fu.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fx.lnxyls.cn

[C10] 变量作用域
来源：http://td.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ya.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fs.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ey.huixinmuqiang.cn

TS:   同 JS
来源：http://gv.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://zm.shxzskj.cn

Go:   花括号块级作用域
来源：http://ja.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tm.panjiajie.cn

C#:   块级作用域
来源：http://xo.bjjhwx.cn

[C11] 模块导入与导出
来源：http://qd.yuexingan06.cn

Py:   from module import func
来源：http://si.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nu.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rx.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bf.panjiajie.cn

Java: import java.util.List;
来源：http://pz.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kk.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://yx.lnxyls.cn

C#:   using System.Text;
来源：http://em.521024.cn

[C12] 立即执行函数 IIFE
来源：http://ly.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://ae.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://ri.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://pg.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://es.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wl.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://ta.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://ns.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://le.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://ii.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dr.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sf.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mp.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xh.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://id.gzmigu.cn

Go:   func add(a, b int) int
来源：http://ud.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wy.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ny.shtwfgs.cn

[C14] 泛型函数
来源：http://kl.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hr.gzmigu.cn

PHP:  // 无泛型
来源：http://vw.lnxyls.cn

JS:   // 无泛型
来源：http://qc.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kx.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hb.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vg.jctech888.com.cn

Ruby: # 无泛型
来源：http://iz.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rk.nicolike.cn

[C15] 解构 / 展开参数
来源：http://wo.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ai.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://gg.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ik.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ia.hnjuh.cn

Java: // 无解构
来源：http://ek.chemitech.net.cn

Go:   // 无解构
来源：http://he.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://ro.huanxung.cn

C#:   var (a, b) = pair;
来源：http://no.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://tu.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ll.panjiajie.cn

PHP:  // 无重载
来源：http://bx.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bd.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ek.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fk.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://rt.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://zf.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fw.asd995.cn

================================================================================
来源：http://bh.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://xn.shxzskj.cn

================================================================================
来源：http://uh.colortex.cn

[D01] 创建数组 / 列表
来源：http://qy.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://te.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ib.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zq.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ov.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oe.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://uz.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://fz.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://so.nicolike.cn

[D02] 追加元素到末尾
来源：http://zx.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ch.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oh.huixiangedu.cn

JS:   arr.push(4);
来源：http://su.nicolike.cn

TS:   arr.push(4);
来源：http://fy.jianghongdianzi.cn

Java: list.add(4);
来源：http://vu.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://sl.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://qg.hahajie.cn

C#:   list.Add(4);
来源：http://gt.newstarts.cn

[D03] 在指定位置插入元素
来源：http://ot.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://qs.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ri.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wk.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://hv.hahajie.cn

Java: list.add(0, 0);
来源：http://dx.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lh.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ka.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://mr.9csxet.cn

[D04] 删除元素
来源：http://my.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://if.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wv.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://at.521024.cn

TS:   arr.splice(0, 1);
来源：http://ue.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tv.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ll.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yn.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xc.jctech888.com.cn

[D05] 访问与修改元素
来源：http://pd.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://li.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ez.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eg.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://rn.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://kj.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://iy.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kn.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ts.9csxet.cn

[D06] 数组长度
来源：http://mj.yuexingan06.cn


<!-- 参考信息 -->