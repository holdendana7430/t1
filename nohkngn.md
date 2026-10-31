代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nd.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ov.shtwfgs.cn

[B07] while 循环
来源：http://mg.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://na.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bd.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://zf.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://sw.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://aa.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sq.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://ln.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://ug.521024.cn

[B08] do-while（至少执行一次）
来源：http://av.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://ir.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uq.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://pd.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://on.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://sg.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bv.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ah.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://eg.shxzukj.cn

[B09] break 与 continue
来源：http://xk.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eh.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fr.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://be.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qy.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tv.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ud.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hg.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://zs.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://km.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qj.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wa.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mq.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ef.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fy.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kb.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tq.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://mo.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://ug.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://bt.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ko.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sz.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qc.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://od.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://fy.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nv.9csxet.cn

[B12] 跳出多层循环
来源：http://gm.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iq.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zr.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zo.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cl.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wz.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yk.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xa.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iy.hahajie.cn

[B13] 判断是否为数字
来源：http://db.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://yk.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://ke.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kg.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xz.huixinmuqiang.cn

Java: x instanceof Number
来源：http://rj.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://io.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://fk.nicolike.cn

C#:   x is int or double or decimal
来源：http://wn.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://ya.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://py.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mi.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://mu.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://gu.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sd.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ae.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qr.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bc.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://ow.panjiajie.cn

Py:   a and b or not c
来源：http://hb.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://we.panjiajie.cn

JS:   a && b || !c
来源：http://vj.huixiangedu.cn

TS:   a && b || !c
来源：http://tc.hnjuh.cn

Java: a && b || !c
来源：http://kn.shxzskj.cn

Go:   a && b || !c
来源：http://zl.szxytkj.cn

Ruby: a && b || !c
来源：http://cm.haigaiapp.cn

C#:   a && b || !c
来源：http://qi.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qv.9csxet.cn

Py:   if not data: return
来源：http://uq.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://nj.huixiangedu.cn

JS:   if (!data) return;
来源：http://cl.szsharing.cn

TS:   if (!data) return;
来源：http://le.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://qj.521024.cn

Go:   if data == nil { return }
来源：http://fw.szxytkj.cn

Ruby: return if data.nil?
来源：http://kg.yuexingan06.cn

C#:   if (data == null) return;
来源：http://ca.panjiajie.cn

================================================================================
来源：http://eu.jianghongdianzi.cn

C. 函数与作用域
来源：http://wt.lnxyls.cn

================================================================================
来源：http://qz.szxytkj.cn

[C01] 定义函数
来源：http://ca.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://rq.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hb.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ej.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wv.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://px.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ek.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://uq.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wq.jianghongdianzi.cn

[C02] 默认参数
来源：http://ka.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://ls.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qr.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://be.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ay.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xy.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nu.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://ue.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://lj.bjjhwx.cn

[C03] 可变参数
来源：http://px.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://kr.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dd.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vy.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tb.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cj.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ve.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wi.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tw.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ep.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hg.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fr.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pc.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://us.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://ey.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://ke.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://oh.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://qz.muxihuayi.cn

[C05] 返回多个值
来源：http://aq.nicolike.cn

Py:   return a, b
来源：http://tt.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://fx.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bu.colortex.cn

TS:   return { a, b };
来源：http://rx.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ec.bookmarksfly.cn

Go:   return a, b
来源：http://wd.szxytkj.cn

Ruby: return a, b
来源：http://lt.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://fo.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://iw.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://dx.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kn.nszjky.cn

JS:   const square = x => x * x;
来源：http://md.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://rx.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vq.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nx.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://wn.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bi.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://zn.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iz.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wy.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xa.bookmarksfly.cn

TS:   arr.map(String)
来源：http://cc.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fa.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ln.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://wg.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wn.newstarts.cn

[C08] 闭包
来源：http://wu.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dx.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://us.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qa.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://al.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pg.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vo.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rl.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uy.haigaiapp.cn

[C09] 递归
来源：http://wj.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://or.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ld.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ly.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sa.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nd.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vx.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ik.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uw.huanxung.cn

[C10] 变量作用域
来源：http://dl.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yp.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ss.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://st.bookmarksfly.cn

TS:   同 JS
来源：http://jn.shxzukj.cn

Java: 方法内为块级作用域
来源：http://gg.yuexingan06.cn

Go:   花括号块级作用域
来源：http://qe.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ti.shxzskj.cn

C#:   块级作用域
来源：http://xj.szxytkj.cn

[C11] 模块导入与导出
来源：http://fc.bookmarksfly.cn

Py:   from module import func
来源：http://vo.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lw.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qx.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ls.chemitech.net.cn

Java: import java.util.List;
来源：http://fu.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nn.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://pb.jianghongdianzi.cn

C#:   using System.Text;
来源：http://iv.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://le.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://cd.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://fw.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://jl.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://mb.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ke.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://cm.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://va.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vw.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://uh.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ua.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ex.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uv.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nu.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://no.nicolike.cn

Go:   func add(a, b int) int
来源：http://mn.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ij.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://un.shxzukj.cn

[C14] 泛型函数
来源：http://tx.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iz.shxzskj.cn

PHP:  // 无泛型
来源：http://el.yuexingan06.cn

JS:   // 无泛型
来源：http://hw.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wa.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hq.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eb.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://gp.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gq.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://pt.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xl.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://vo.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jq.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jp.haigaiapp.cn

Java: // 无解构
来源：http://ad.szxytkj.cn

Go:   // 无解构
来源：http://ku.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://yq.colortex.cn

C#:   var (a, b) = pair;
来源：http://zs.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://kg.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fi.muxihuayi.cn

PHP:  // 无重载
来源：http://xj.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wo.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://fm.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rr.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://um.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://zd.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bk.yuexingan06.cn

================================================================================
来源：http://jz.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://sw.shxzukj.cn

================================================================================
来源：http://bg.colortex.cn

[D01] 创建数组 / 列表
来源：http://ql.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tj.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hs.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ow.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iu.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pv.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://ol.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://lf.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ss.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://ii.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ll.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tx.bjjhwx.cn

JS:   arr.push(4);
来源：http://hq.9csxet.cn

TS:   arr.push(4);
来源：http://rq.bjjhwx.cn

Java: list.add(4);
来源：http://yb.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://vd.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://yz.lnxyls.cn

C#:   list.Add(4);
来源：http://cs.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://nc.colortex.cn

Py:   arr.insert(0, 0)
来源：http://vm.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jl.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xe.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://cx.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://in.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lx.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mh.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://ny.gzmigu.cn

[D04] 删除元素
来源：http://sr.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://df.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://el.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://de.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://zj.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dh.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pg.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ss.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nu.jctech888.com.cn

[D05] 访问与修改元素
来源：http://zt.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ss.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zg.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zp.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ru.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://yr.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://gf.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zt.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ar.hnjuh.cn

[D06] 数组长度
来源：http://fz.wgjwhj.cn

Py:   len(arr)
来源：http://lv.yuntaijiaju.cn

PHP:  count($arr);
来源：http://jv.nicolike.cn

JS:   arr.length
来源：http://tl.haigaiapp.cn

TS:   arr.length
来源：http://ab.jctech888.com.cn

Java: list.size();
来源：http://jl.shtwfgs.cn

Go:   len(arr)
来源：http://hx.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://mf.huanxung.cn

C#:   list.Count;
来源：http://dt.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://ig.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vs.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yx.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://ow.yuexingan06.cn


<!-- 参考信息 -->