代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lq.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://od.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fv.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jk.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dj.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tk.wgjwhj.cn

[B07] while 循环
来源：http://de.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://rh.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zd.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://ii.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://tt.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://ap.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xq.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://ib.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://zs.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://hb.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://kj.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://co.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://vk.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://ku.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://zp.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bm.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fh.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://cz.nicolike.cn

[B09] break 与 continue
来源：http://gx.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zq.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jl.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pf.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cb.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gx.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://af.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yp.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dh.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://et.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cf.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zy.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bj.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oo.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zn.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bd.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qy.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cd.521024.cn

[B11] 生成数字序列 / 区间
来源：http://fm.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://ns.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://hp.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vx.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oo.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ox.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wp.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://zg.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vl.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://lg.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ex.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nv.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ax.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zm.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://da.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lg.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vg.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ba.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://xd.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://sl.hnjuh.cn

PHP:  is_numeric($x)
来源：http://dk.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ip.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jq.bjjhwx.cn

Java: x instanceof Number
来源：http://yj.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uo.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://br.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://sz.szsharing.cn

[B14] 判断值是否在集合内
来源：http://kc.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hr.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ue.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://ho.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://qh.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kw.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://si.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mu.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kg.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://am.yuexingan06.cn

Py:   a and b or not c
来源：http://md.nicolike.cn

PHP:  $a && $b || !$c
来源：http://jq.521024.cn

JS:   a && b || !c
来源：http://dx.shtwfgs.cn

TS:   a && b || !c
来源：http://dq.haigaiapp.cn

Java: a && b || !c
来源：http://nf.shxzskj.cn

Go:   a && b || !c
来源：http://nv.521024.cn

Ruby: a && b || !c
来源：http://iw.haigaiapp.cn

C#:   a && b || !c
来源：http://tq.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hk.9csxet.cn

Py:   if not data: return
来源：http://yt.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://iz.muxihuayi.cn

JS:   if (!data) return;
来源：http://yj.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://ai.newstarts.cn

Java: if (data == null) return;
来源：http://co.bjjhwx.cn

Go:   if data == nil { return }
来源：http://gr.jctech888.com.cn

Ruby: return if data.nil?
来源：http://hx.panjiajie.cn

C#:   if (data == null) return;
来源：http://jy.yuexingan06.cn

================================================================================
来源：http://nu.huixiangedu.cn

C. 函数与作用域
来源：http://ox.asd995.cn

================================================================================
来源：http://sz.chemitech.net.cn

[C01] 定义函数
来源：http://jt.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://nu.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gi.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://jb.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aq.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uz.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ha.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://jo.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bx.huanxung.cn

[C02] 默认参数
来源：http://tg.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://hd.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dn.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://lo.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pe.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jx.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vq.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://pp.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://lr.gzmigu.cn

[C03] 可变参数
来源：http://gt.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://xl.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zp.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ys.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yy.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ux.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tw.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xl.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rr.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://rr.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tz.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uh.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://je.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cb.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://fj.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://bz.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://zs.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://tj.muxihuayi.cn

[C05] 返回多个值
来源：http://fu.nszjky.cn

Py:   return a, b
来源：http://oi.colortex.cn

PHP:  return [$a, $b];
来源：http://hh.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vz.hahajie.cn

TS:   return { a, b };
来源：http://fu.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mz.szsharing.cn

Go:   return a, b
来源：http://oh.asd995.cn

Ruby: return a, b
来源：http://pi.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://lt.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://kv.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://xi.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hl.shxzskj.cn

JS:   const square = x => x * x;
来源：http://ln.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://sj.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ee.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sf.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://hm.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gj.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://se.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tq.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kf.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nl.lnxyls.cn

TS:   arr.map(String)
来源：http://dh.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://am.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rj.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://aq.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ku.shxzskj.cn

[C08] 闭包
来源：http://fp.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lp.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ts.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mc.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vx.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kx.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lx.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://us.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yz.hnjuh.cn

[C09] 递归
来源：http://mn.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://an.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qr.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nf.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://py.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://na.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tr.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gp.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hx.9csxet.cn

[C10] 变量作用域
来源：http://sw.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tx.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dj.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sg.szxytkj.cn

TS:   同 JS
来源：http://ah.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://kq.bjjhwx.cn

Go:   花括号块级作用域
来源：http://us.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vt.521024.cn

C#:   块级作用域
来源：http://wr.wgjwhj.cn

[C11] 模块导入与导出
来源：http://tv.nszjky.cn

Py:   from module import func
来源：http://uu.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mx.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bc.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yi.colortex.cn

Java: import java.util.List;
来源：http://hh.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yf.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://uq.panjiajie.cn

C#:   using System.Text;
来源：http://ih.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://gz.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://za.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://jb.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://ma.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://fi.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tq.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://re.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://bo.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sq.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://bu.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rs.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eo.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cm.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sl.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gh.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://oj.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vr.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hy.huanxung.cn

[C14] 泛型函数
来源：http://fm.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pu.asd995.cn

PHP:  // 无泛型
来源：http://gu.9csxet.cn

JS:   // 无泛型
来源：http://pi.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dy.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://km.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lt.bookmarksfly.cn

Ruby: # 无泛型
来源：http://jz.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bl.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://pb.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ds.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://kk.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bg.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hf.9csxet.cn

Java: // 无解构
来源：http://cu.hnjuh.cn

Go:   // 无解构
来源：http://sj.lnxyls.cn

Ruby: a, b = pair
来源：http://jj.huanxung.cn

C#:   var (a, b) = pair;
来源：http://sm.nicolike.cn

[C16] 函数 / 方法重载
来源：http://it.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cg.jctech888.com.cn

PHP:  // 无重载
来源：http://au.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ty.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://xz.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ge.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://ga.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://di.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fg.szxytkj.cn

================================================================================
来源：http://yh.521024.cn

D. 数组 / 列表 / 集合
来源：http://qv.wgjwhj.cn

================================================================================
来源：http://ve.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://qv.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pn.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ja.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gb.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ki.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ac.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://em.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://ul.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wy.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://xo.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ed.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xh.bjjhwx.cn

JS:   arr.push(4);
来源：http://fz.hahajie.cn

TS:   arr.push(4);
来源：http://rp.wgjwhj.cn

Java: list.add(4);
来源：http://po.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://oz.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://fa.yuexingan06.cn

C#:   list.Add(4);
来源：http://ws.nicolike.cn

[D03] 在指定位置插入元素
来源：http://sv.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://xz.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eb.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qw.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://nq.huixiangedu.cn

Java: list.add(0, 0);
来源：http://wu.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ln.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zk.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://gi.nicolike.cn

[D04] 删除元素
来源：http://vo.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rv.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rm.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cs.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://ka.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oz.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lm.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fk.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hg.colortex.cn

[D05] 访问与修改元素
来源：http://ct.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://te.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nu.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bm.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://lb.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://cr.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://pi.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nt.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iw.shxzukj.cn

[D06] 数组长度
来源：http://iu.shxzukj.cn

Py:   len(arr)
来源：http://ag.9csxet.cn

PHP:  count($arr);
来源：http://su.shxzskj.cn

JS:   arr.length
来源：http://px.asd995.cn

TS:   arr.length
来源：http://vj.colortex.cn

Java: list.size();
来源：http://ur.yuntaijiaju.cn

Go:   len(arr)
来源：http://yn.9csxet.cn

Ruby: arr.length; arr.size
来源：http://cl.szsharing.cn

C#:   list.Count;
来源：http://ui.newstarts.cn


<!-- 参考信息 -->