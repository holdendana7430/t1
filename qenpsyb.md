代发 wailian999

Py:   for i in range(10): print(i)
来源：http://wa.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xe.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kd.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ac.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vt.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://si.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://vg.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vq.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://kz.521024.cn

Py:   for item in arr: print(item)
来源：http://cw.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://os.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://od.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://le.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fy.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://co.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://pt.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lg.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://cp.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://es.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jj.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bp.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ly.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ts.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lr.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xw.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ny.nszjky.cn

[B07] while 循环
来源：http://to.nszjky.cn

Py:   while i < 10: i += 1
来源：http://rr.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nh.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://gu.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://at.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://lh.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hk.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://xz.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://pl.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://di.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://ku.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://um.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://va.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://va.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://xv.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eg.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xw.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://kl.jctech888.com.cn

[B09] break 与 continue
来源：http://vz.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yl.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zb.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cp.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vf.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dm.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hv.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gz.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yp.hahajie.cn

[B10] 遍历同时拿索引
来源：http://np.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bv.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jj.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://as.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uq.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ka.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ud.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nr.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://il.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://vq.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://vs.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://wu.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zu.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ej.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nv.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://do.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://di.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xw.hahajie.cn

[B12] 跳出多层循环
来源：http://gi.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oi.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hs.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pr.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eh.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hc.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vh.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zu.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ts.shxzukj.cn

[B13] 判断是否为数字
来源：http://xe.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://uv.asd995.cn

PHP:  is_numeric($x)
来源：http://fd.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yn.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cr.shtwfgs.cn

Java: x instanceof Number
来源：http://pd.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nk.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://fs.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://gb.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://oo.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ho.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sj.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://vt.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://sb.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://me.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yl.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://um.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zk.521024.cn

[B15] 布尔运算与取反
来源：http://qz.jctech888.com.cn

Py:   a and b or not c
来源：http://pf.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://lx.bjjhwx.cn

JS:   a && b || !c
来源：http://nt.newstarts.cn

TS:   a && b || !c
来源：http://gd.wgjwhj.cn

Java: a && b || !c
来源：http://uk.szxytkj.cn

Go:   a && b || !c
来源：http://oe.szsharing.cn

Ruby: a && b || !c
来源：http://bh.panjiajie.cn

C#:   a && b || !c
来源：http://cf.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ke.colortex.cn

Py:   if not data: return
来源：http://vm.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://lw.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://mc.521024.cn

TS:   if (!data) return;
来源：http://gv.bookmarksfly.cn

Java: if (data == null) return;
来源：http://bx.wgjwhj.cn

Go:   if data == nil { return }
来源：http://vn.szsharing.cn

Ruby: return if data.nil?
来源：http://br.szxytkj.cn

C#:   if (data == null) return;
来源：http://sj.yuexingan06.cn

================================================================================
来源：http://wu.nicolike.cn

C. 函数与作用域
来源：http://wc.muxihuayi.cn

================================================================================
来源：http://mo.shxzskj.cn

[C01] 定义函数
来源：http://te.colortex.cn

Py:   def add(a, b): return a + b
来源：http://lf.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bp.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ir.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ai.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://af.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://lr.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vq.yuntaijiaju.cn

[C02] 默认参数
来源：http://ke.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://ho.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nd.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://ib.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fs.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sk.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wh.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://lk.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://fs.muxihuayi.cn

[C03] 可变参数
来源：http://jk.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://gp.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hp.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lf.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://um.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vu.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hq.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ba.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uf.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://mu.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rw.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vg.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://js.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fl.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://tb.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://pi.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://xl.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://uq.bookmarksfly.cn

[C05] 返回多个值
来源：http://px.wgjwhj.cn

Py:   return a, b
来源：http://qb.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://wk.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zr.szxytkj.cn

TS:   return { a, b };
来源：http://ix.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ox.yuntaijiaju.cn

Go:   return a, b
来源：http://uc.shxzskj.cn

Ruby: return a, b
来源：http://st.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://kg.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://zb.szsharing.cn

Py:   square = lambda x: x * x
来源：http://lw.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kg.szxytkj.cn

JS:   const square = x => x * x;
来源：http://xf.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ng.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jf.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zn.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://ou.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qn.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://kb.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qq.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://za.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mp.szsharing.cn

TS:   arr.map(String)
来源：http://iw.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://px.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jo.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://qh.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mw.521024.cn

[C08] 闭包
来源：http://ub.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ho.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jg.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sv.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yf.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kv.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pv.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ze.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fx.huixinmuqiang.cn

[C09] 递归
来源：http://xd.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yv.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dw.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bf.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tt.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pk.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sh.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ya.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kr.wgjwhj.cn

[C10] 变量作用域
来源：http://aa.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sq.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rt.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://du.lnxyls.cn

TS:   同 JS
来源：http://ue.colortex.cn

Java: 方法内为块级作用域
来源：http://oo.muxihuayi.cn

Go:   花括号块级作用域
来源：http://gq.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gd.asd995.cn

C#:   块级作用域
来源：http://jo.newstarts.cn

[C11] 模块导入与导出
来源：http://rc.hnjuh.cn

Py:   from module import func
来源：http://pu.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pk.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pn.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bi.huanxung.cn

Java: import java.util.List;
来源：http://gm.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jq.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://ot.shxzskj.cn

C#:   using System.Text;
来源：http://bz.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://me.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://or.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://wt.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://vg.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://ex.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ra.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://il.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://xp.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ym.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://cf.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mq.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kh.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zt.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ux.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ji.521024.cn

Go:   func add(a, b int) int
来源：http://kn.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pd.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zi.haigaiapp.cn

[C14] 泛型函数
来源：http://wq.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sj.szxytkj.cn

PHP:  // 无泛型
来源：http://dy.panjiajie.cn

JS:   // 无泛型
来源：http://kc.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xv.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://il.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pi.newstarts.cn

Ruby: # 无泛型
来源：http://rm.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yf.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://tw.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zv.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://si.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://un.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ag.panjiajie.cn

Java: // 无解构
来源：http://jf.huanxung.cn

Go:   // 无解构
来源：http://ha.9csxet.cn

Ruby: a, b = pair
来源：http://ei.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://gt.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://fo.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ij.huixiangedu.cn

PHP:  // 无重载
来源：http://li.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hk.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://pu.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nt.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://qz.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://jh.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bw.bookmarksfly.cn

================================================================================
来源：http://qb.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://xh.bookmarksfly.cn

================================================================================
来源：http://av.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://cj.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xj.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fg.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ff.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ny.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xv.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://my.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://af.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bk.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://le.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ln.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vo.wgjwhj.cn

JS:   arr.push(4);
来源：http://wn.szxytkj.cn

TS:   arr.push(4);
来源：http://ee.hnjuh.cn

Java: list.add(4);
来源：http://wt.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://df.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://aa.9csxet.cn

C#:   list.Add(4);
来源：http://pp.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://hn.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://xa.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uu.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eb.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://bb.521024.cn

Java: list.add(0, 0);
来源：http://yl.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hb.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fc.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://et.muxihuayi.cn

[D04] 删除元素
来源：http://am.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tp.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mh.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lt.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://oa.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yx.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lz.521024.cn


<!-- 参考信息 -->