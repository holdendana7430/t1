代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jy.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://br.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://xm.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sv.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://kk.colortex.cn

Py:   for item in arr: print(item)
来源：http://wh.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ny.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://by.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bo.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jq.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vt.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://he.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kb.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://qv.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zr.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fv.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ly.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pq.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zm.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vq.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xe.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jj.yuexingan06.cn

[B07] while 循环
来源：http://lt.colortex.cn

Py:   while i < 10: i += 1
来源：http://xt.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vf.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://mr.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://qj.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://dm.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uh.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://sg.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://lf.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://lq.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://kh.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oa.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://xy.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://bf.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://xq.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://td.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yw.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://za.nicolike.cn

[B09] break 与 continue
来源：http://qn.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rf.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ac.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sr.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pu.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mn.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lb.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gi.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dw.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://bh.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rm.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jy.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qc.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mm.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sr.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fy.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ct.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bq.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://br.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://wa.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://tb.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mh.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kn.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hs.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://px.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://xh.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ht.bjjhwx.cn

[B12] 跳出多层循环
来源：http://qi.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://um.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ex.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bs.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vu.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zg.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nn.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iy.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://id.shxzukj.cn

[B13] 判断是否为数字
来源：http://zk.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://os.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://jm.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iq.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jv.nszjky.cn

Java: x instanceof Number
来源：http://sa.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xv.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://ci.hahajie.cn

C#:   x is int or double or decimal
来源：http://ff.nszjky.cn

[B14] 判断值是否在集合内
来源：http://fh.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jv.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wl.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://dj.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://xb.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ha.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://id.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cm.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://za.shxzukj.cn

[B15] 布尔运算与取反
来源：http://go.newstarts.cn

Py:   a and b or not c
来源：http://yd.521024.cn

PHP:  $a && $b || !$c
来源：http://qq.hnjuh.cn

JS:   a && b || !c
来源：http://jg.haigaiapp.cn

TS:   a && b || !c
来源：http://lt.lnxyls.cn

Java: a && b || !c
来源：http://br.nicolike.cn

Go:   a && b || !c
来源：http://ln.szsharing.cn

Ruby: a && b || !c
来源：http://kl.hnjuh.cn

C#:   a && b || !c
来源：http://eq.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eh.lnxyls.cn

Py:   if not data: return
来源：http://ym.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://be.shtwfgs.cn

JS:   if (!data) return;
来源：http://hv.nicolike.cn

TS:   if (!data) return;
来源：http://qs.521024.cn

Java: if (data == null) return;
来源：http://gm.yuexingan06.cn

Go:   if data == nil { return }
来源：http://we.szxytkj.cn

Ruby: return if data.nil?
来源：http://mp.shtwfgs.cn

C#:   if (data == null) return;
来源：http://wo.panjiajie.cn

================================================================================
来源：http://nd.nicolike.cn

C. 函数与作用域
来源：http://lk.nszjky.cn

================================================================================
来源：http://xr.szsharing.cn

[C01] 定义函数
来源：http://gn.asd995.cn

Py:   def add(a, b): return a + b
来源：http://zt.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ge.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://uf.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://js.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ci.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lu.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://fm.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://er.colortex.cn

[C02] 默认参数
来源：http://ui.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://li.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rz.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://mn.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zz.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ro.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yn.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://jy.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://cy.9csxet.cn

[C03] 可变参数
来源：http://hv.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://jt.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gi.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qh.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://op.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://re.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fb.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qo.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xg.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://ee.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yl.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gg.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vb.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yw.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://ni.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://st.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://rh.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://mb.shxzskj.cn

[C05] 返回多个值
来源：http://fq.lnxyls.cn

Py:   return a, b
来源：http://lf.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://an.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ru.huanxung.cn

TS:   return { a, b };
来源：http://wg.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rw.shtwfgs.cn

Go:   return a, b
来源：http://qy.huanxung.cn

Ruby: return a, b
来源：http://cb.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://re.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://nu.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://cy.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ky.newstarts.cn

JS:   const square = x => x * x;
来源：http://mp.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://ek.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gd.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kd.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://nk.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ec.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://vk.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ia.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ap.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fa.lnxyls.cn

TS:   arr.map(String)
来源：http://ef.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tx.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fi.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://zw.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wt.shxzukj.cn

[C08] 闭包
来源：http://ab.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qb.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xr.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lo.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://be.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://me.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://df.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hu.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uv.haigaiapp.cn

[C09] 递归
来源：http://rv.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zm.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tz.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kw.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wl.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bo.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zw.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ov.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://op.shxzskj.cn

[C10] 变量作用域
来源：http://kj.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://df.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nf.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xb.chemitech.net.cn

TS:   同 JS
来源：http://tg.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://we.panjiajie.cn

Go:   花括号块级作用域
来源：http://wz.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ji.nszjky.cn

C#:   块级作用域
来源：http://nq.panjiajie.cn

[C11] 模块导入与导出
来源：http://ak.nszjky.cn

Py:   from module import func
来源：http://qc.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nf.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uh.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ib.521024.cn

Java: import java.util.List;
来源：http://wn.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://up.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://gp.bookmarksfly.cn

C#:   using System.Text;
来源：http://jz.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://et.521024.cn

Py:   (lambda: print("run"))()
来源：http://uj.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://kd.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://zm.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://qq.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bv.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://rq.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://sg.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cl.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://hp.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tc.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pt.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lo.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ma.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mw.lnxyls.cn

Go:   func add(a, b int) int
来源：http://xk.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lc.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rw.huixiangedu.cn

[C14] 泛型函数
来源：http://tq.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zx.bookmarksfly.cn

PHP:  // 无泛型
来源：http://zy.huixiangedu.cn

JS:   // 无泛型
来源：http://al.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wm.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cf.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://he.lnxyls.cn

Ruby: # 无泛型
来源：http://ms.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xa.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://oj.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xc.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://nu.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hs.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ef.521024.cn

Java: // 无解构
来源：http://wa.jianghongdianzi.cn

Go:   // 无解构
来源：http://zq.nszjky.cn

Ruby: a, b = pair
来源：http://lb.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://ha.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://uv.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bi.gzmigu.cn

PHP:  // 无重载
来源：http://in.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gi.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://pr.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ke.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://rh.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://tn.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bc.bjjhwx.cn

================================================================================
来源：http://gl.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://jb.huanxung.cn

================================================================================
来源：http://mm.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://jb.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ya.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bn.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://as.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dz.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zu.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://xc.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://ga.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qy.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://ej.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fw.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ha.panjiajie.cn

JS:   arr.push(4);
来源：http://ie.hahajie.cn

TS:   arr.push(4);
来源：http://xw.bjjhwx.cn

Java: list.add(4);
来源：http://ra.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://xt.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://xz.hahajie.cn

C#:   list.Add(4);
来源：http://do.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://rm.asd995.cn

Py:   arr.insert(0, 0)
来源：http://jb.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mt.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aq.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://cc.newstarts.cn

Java: list.add(0, 0);
来源：http://qi.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ck.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zq.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://et.521024.cn

[D04] 删除元素
来源：http://ok.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lw.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nm.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://om.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://cp.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sa.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oe.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qa.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fx.wgjwhj.cn

[D05] 访问与修改元素
来源：http://ks.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sp.chemitech.net.cn


<!-- 参考信息 -->