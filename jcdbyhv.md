代发 wailian999

[B05] 遍历数组 / 列表
来源：http://mq.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://av.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rz.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jb.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tk.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hf.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://la.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://zt.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ef.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://cd.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vh.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vv.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hs.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://io.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qs.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://my.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://px.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ac.jctech888.com.cn

[B07] while 循环
来源：http://mk.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://mu.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dd.521024.cn

JS:   while (i < 10) { i++; }
来源：http://ua.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://ni.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://em.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://km.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://kl.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://px.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://xn.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://hm.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ly.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://hf.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://mk.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://xm.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://un.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ct.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://vk.jianghongdianzi.cn

[B09] break 与 continue
来源：http://bf.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gk.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qf.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://am.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pb.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hq.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vk.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://av.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pz.newstarts.cn

[B10] 遍历同时拿索引
来源：http://wt.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dy.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://an.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wr.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://om.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hs.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fp.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mo.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lb.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://hj.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://it.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://pm.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pr.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mp.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ca.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://do.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://et.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zd.jctech888.com.cn

[B12] 跳出多层循环
来源：http://mo.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yr.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pl.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fc.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mf.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jp.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gt.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cs.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vb.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://rw.521024.cn

Py:   isinstance(x, (int, float))
来源：http://hh.panjiajie.cn

PHP:  is_numeric($x)
来源：http://ne.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ot.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kt.nicolike.cn

Java: x instanceof Number
来源：http://sz.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ev.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://no.szsharing.cn

C#:   x is int or double or decimal
来源：http://ub.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://fg.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xa.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nf.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://wj.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://yn.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://al.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hb.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gz.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cl.asd995.cn

[B15] 布尔运算与取反
来源：http://nj.lnxyls.cn

Py:   a and b or not c
来源：http://tg.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://bm.bjjhwx.cn

JS:   a && b || !c
来源：http://oe.asd995.cn

TS:   a && b || !c
来源：http://da.lnxyls.cn

Java: a && b || !c
来源：http://vw.chemitech.net.cn

Go:   a && b || !c
来源：http://nb.yuexingan06.cn

Ruby: a && b || !c
来源：http://am.bjjhwx.cn

C#:   a && b || !c
来源：http://ly.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vd.gzmigu.cn

Py:   if not data: return
来源：http://mt.asd995.cn

PHP:  if (!$data) { return; }
来源：http://sn.shxzskj.cn

JS:   if (!data) return;
来源：http://mp.lnxyls.cn

TS:   if (!data) return;
来源：http://wm.szsharing.cn

Java: if (data == null) return;
来源：http://el.asd995.cn

Go:   if data == nil { return }
来源：http://yt.nicolike.cn

Ruby: return if data.nil?
来源：http://ul.hahajie.cn

C#:   if (data == null) return;
来源：http://wk.asd995.cn

================================================================================
来源：http://nw.szsharing.cn

C. 函数与作用域
来源：http://zc.szxytkj.cn

================================================================================
来源：http://xu.muxihuayi.cn

[C01] 定义函数
来源：http://of.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://tm.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ad.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://yr.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sv.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zy.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ji.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://fp.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rd.haigaiapp.cn

[C02] 默认参数
来源：http://rz.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://mz.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mr.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://qo.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fx.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://da.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iq.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://ma.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://te.lnxyls.cn

[C03] 可变参数
来源：http://vu.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://sh.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wy.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ab.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kn.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ml.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mu.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sc.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bv.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://hy.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mr.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hb.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ru.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nl.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://fl.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://ib.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://pz.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://rh.jctech888.com.cn

[C05] 返回多个值
来源：http://fs.gzmigu.cn

Py:   return a, b
来源：http://cl.szxytkj.cn

PHP:  return [$a, $b];
来源：http://rx.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ps.jctech888.com.cn

TS:   return { a, b };
来源：http://gp.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ss.muxihuayi.cn

Go:   return a, b
来源：http://ia.shtwfgs.cn

Ruby: return a, b
来源：http://hs.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://eh.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://rq.huanxung.cn

Py:   square = lambda x: x * x
来源：http://ba.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sc.9csxet.cn

JS:   const square = x => x * x;
来源：http://uj.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://yy.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ud.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pg.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://xl.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gg.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://qx.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ti.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zz.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wz.szxytkj.cn

TS:   arr.map(String)
来源：http://wi.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ue.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nh.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://yt.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fb.jctech888.com.cn

[C08] 闭包
来源：http://pc.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zy.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://io.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ep.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tp.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hm.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mo.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ub.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yy.hahajie.cn

[C09] 递归
来源：http://gb.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dd.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cq.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ly.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zg.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bt.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vx.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tx.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wn.lnxyls.cn

[C10] 变量作用域
来源：http://mh.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oa.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://px.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gm.chemitech.net.cn

TS:   同 JS
来源：http://yq.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://ne.nicolike.cn

Go:   花括号块级作用域
来源：http://on.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rs.yuexingan06.cn

C#:   块级作用域
来源：http://cu.chemitech.net.cn

[C11] 模块导入与导出
来源：http://it.asd995.cn

Py:   from module import func
来源：http://uz.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://go.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kw.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zy.shxzskj.cn

Java: import java.util.List;
来源：http://cr.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ue.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://cj.yuexingan06.cn

C#:   using System.Text;
来源：http://fo.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://vu.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://db.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ib.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://tb.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://en.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vz.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://ai.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://ay.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ze.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://tf.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ji.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://em.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kf.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lr.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dg.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://cp.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://st.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jy.colortex.cn

[C14] 泛型函数
来源：http://bz.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iw.9csxet.cn

PHP:  // 无泛型
来源：http://yf.jctech888.com.cn

JS:   // 无泛型
来源：http://rt.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nh.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wo.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bc.hnjuh.cn

Ruby: # 无泛型
来源：http://tv.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ql.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://aw.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pp.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ec.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sw.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://du.newstarts.cn

Java: // 无解构
来源：http://wy.9csxet.cn

Go:   // 无解构
来源：http://fm.lnxyls.cn

Ruby: a, b = pair
来源：http://ew.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://az.521024.cn

[C16] 函数 / 方法重载
来源：http://kz.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ub.muxihuayi.cn

PHP:  // 无重载
来源：http://tz.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gh.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://jd.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://es.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://bp.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://pb.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://do.nicolike.cn

================================================================================
来源：http://kd.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://cw.haigaiapp.cn

================================================================================
来源：http://id.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://ql.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ed.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bb.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mf.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qo.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bx.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://zq.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://gh.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://al.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://cw.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zm.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ar.shtwfgs.cn

JS:   arr.push(4);
来源：http://eq.panjiajie.cn

TS:   arr.push(4);
来源：http://zb.shtwfgs.cn

Java: list.add(4);
来源：http://wy.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://nk.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://kb.panjiajie.cn

C#:   list.Add(4);
来源：http://iu.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://gr.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://cd.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cs.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vy.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://fd.shtwfgs.cn

Java: list.add(0, 0);
来源：http://qy.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zp.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rv.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://fr.szxytkj.cn

[D04] 删除元素
来源：http://bp.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sr.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mn.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ak.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://yo.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://au.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hi.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cj.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zd.muxihuayi.cn

[D05] 访问与修改元素
来源：http://ss.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://th.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mn.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ua.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://le.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://mp.gzmigu.cn


<!-- 参考信息 -->