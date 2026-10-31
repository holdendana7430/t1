代发 wailian999

[B05] 遍历数组 / 列表
来源：http://ez.521024.cn

Py:   for item in arr: print(item)
来源：http://bd.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bf.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uk.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wk.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qe.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ls.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://dz.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zd.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://cm.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dd.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bi.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://al.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cd.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cp.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hq.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ts.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fn.panjiajie.cn

[B07] while 循环
来源：http://pi.asd995.cn

Py:   while i < 10: i += 1
来源：http://ah.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tk.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://bv.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://nb.521024.cn

Java: while (i < 10) { i++; }
来源：http://lx.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nn.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://vx.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://rv.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://sl.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://vy.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rp.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://ed.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://qg.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://wj.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ry.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pk.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://bk.9csxet.cn

[B09] break 与 continue
来源：http://wm.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wn.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xd.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hl.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xz.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ki.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qo.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yb.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://in.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://tx.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cs.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nf.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ya.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ms.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uu.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ob.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qq.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lp.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://ga.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://ai.521024.cn

PHP:  range(0, 10, 2);
来源：http://aj.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fl.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bi.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eo.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jt.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://ir.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eq.jctech888.com.cn

[B12] 跳出多层循环
来源：http://sh.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tl.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ts.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wd.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sx.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qs.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ed.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sv.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nl.yuexingan06.cn

[B13] 判断是否为数字
来源：http://yn.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://sj.521024.cn

PHP:  is_numeric($x)
来源：http://pk.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qi.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ni.bookmarksfly.cn

Java: x instanceof Number
来源：http://ul.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jk.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://bm.panjiajie.cn

C#:   x is int or double or decimal
来源：http://at.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://ca.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mx.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yf.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://it.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://fs.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ma.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://om.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zf.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gi.hahajie.cn

[B15] 布尔运算与取反
来源：http://ne.bookmarksfly.cn

Py:   a and b or not c
来源：http://mq.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://xu.yuexingan06.cn

JS:   a && b || !c
来源：http://kj.9csxet.cn

TS:   a && b || !c
来源：http://gi.huixiangedu.cn

Java: a && b || !c
来源：http://je.colortex.cn

Go:   a && b || !c
来源：http://rn.huanxung.cn

Ruby: a && b || !c
来源：http://yc.hnjuh.cn

C#:   a && b || !c
来源：http://ql.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sl.bjjhwx.cn

Py:   if not data: return
来源：http://nt.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://qs.gzmigu.cn

JS:   if (!data) return;
来源：http://jr.9csxet.cn

TS:   if (!data) return;
来源：http://cg.9csxet.cn

Java: if (data == null) return;
来源：http://qh.9csxet.cn

Go:   if data == nil { return }
来源：http://jt.shxzukj.cn

Ruby: return if data.nil?
来源：http://ro.newstarts.cn

C#:   if (data == null) return;
来源：http://se.shxzukj.cn

================================================================================
来源：http://rw.haigaiapp.cn

C. 函数与作用域
来源：http://cr.panjiajie.cn

================================================================================
来源：http://al.newstarts.cn

[C01] 定义函数
来源：http://ys.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://ur.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gn.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://tb.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://at.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xn.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uh.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://sv.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nu.bjjhwx.cn

[C02] 默认参数
来源：http://gm.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://qd.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uh.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://kx.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lr.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zh.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vo.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://tx.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://if.jianghongdianzi.cn

[C03] 可变参数
来源：http://fv.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://bj.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ay.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lv.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yo.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gq.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xh.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ya.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uf.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://dl.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ne.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kg.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mg.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://or.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://eo.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://lz.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://pz.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://dx.szxytkj.cn

[C05] 返回多个值
来源：http://te.chemitech.net.cn

Py:   return a, b
来源：http://mq.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://ie.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bs.521024.cn

TS:   return { a, b };
来源：http://ub.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gn.shxzukj.cn

Go:   return a, b
来源：http://yt.521024.cn

Ruby: return a, b
来源：http://sv.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://lt.asd995.cn

[C06] 匿名函数 / lambda
来源：http://pf.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://px.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gz.shxzukj.cn

JS:   const square = x => x * x;
来源：http://vt.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://dy.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vi.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://am.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://bg.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oi.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://rq.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ua.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://my.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tn.hahajie.cn

TS:   arr.map(String)
来源：http://jc.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yx.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sx.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://hr.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://az.szxytkj.cn

[C08] 闭包
来源：http://db.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rl.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kq.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bv.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yo.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ed.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ly.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wy.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ta.haigaiapp.cn

[C09] 递归
来源：http://mp.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rw.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ec.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yg.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lg.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qm.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xe.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zo.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gk.hnjuh.cn

[C10] 变量作用域
来源：http://qo.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wq.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fv.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://de.521024.cn

TS:   同 JS
来源：http://yx.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://ab.haigaiapp.cn

Go:   花括号块级作用域
来源：http://wt.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xl.haigaiapp.cn

C#:   块级作用域
来源：http://jj.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://jn.muxihuayi.cn

Py:   from module import func
来源：http://co.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://li.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ko.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hb.szxytkj.cn

Java: import java.util.List;
来源：http://ps.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nc.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://bu.szxytkj.cn

C#:   using System.Text;
来源：http://hc.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://nx.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://ik.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://zv.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://po.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://jm.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vq.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://vu.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://iw.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ka.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://mi.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cx.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gp.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nm.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hd.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qb.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://jw.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aj.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nx.newstarts.cn

[C14] 泛型函数
来源：http://hs.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tz.521024.cn

PHP:  // 无泛型
来源：http://ki.521024.cn

JS:   // 无泛型
来源：http://dz.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rk.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jz.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wx.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://jb.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eh.521024.cn

[C15] 解构 / 展开参数
来源：http://vu.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eq.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ve.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lg.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rm.bookmarksfly.cn

Java: // 无解构
来源：http://co.shxzskj.cn

Go:   // 无解构
来源：http://bw.haigaiapp.cn

Ruby: a, b = pair
来源：http://ug.asd995.cn

C#:   var (a, b) = pair;
来源：http://vp.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://dr.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ak.521024.cn

PHP:  // 无重载
来源：http://nr.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wv.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://qp.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hc.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://pj.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://hb.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wh.hnjuh.cn

================================================================================
来源：http://zb.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://ja.bjjhwx.cn

================================================================================
来源：http://lu.huanxung.cn

[D01] 创建数组 / 列表
来源：http://nh.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tg.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://be.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://so.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iv.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ar.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://tj.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ge.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xv.hahajie.cn

[D02] 追加元素到末尾
来源：http://dw.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://da.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pv.haigaiapp.cn

JS:   arr.push(4);
来源：http://sw.szxytkj.cn

TS:   arr.push(4);
来源：http://sa.huixinmuqiang.cn

Java: list.add(4);
来源：http://si.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://xw.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://lh.panjiajie.cn

C#:   list.Add(4);
来源：http://uv.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://bw.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://fm.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bd.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rd.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ej.muxihuayi.cn

Java: list.add(0, 0);
来源：http://qd.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://le.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://me.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://fz.lnxyls.cn

[D04] 删除元素
来源：http://ck.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fs.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://id.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ua.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://ce.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qk.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ia.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fd.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://np.hnjuh.cn

[D05] 访问与修改元素
来源：http://gy.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sa.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iq.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vs.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ry.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://tv.szsharing.cn


<!-- 参考信息 -->