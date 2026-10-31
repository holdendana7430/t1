代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sr.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tc.asd995.cn

[B07] while 循环
来源：http://bs.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://hp.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bj.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://im.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://xi.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://um.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fy.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://ne.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://ye.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://yz.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://aj.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xu.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://vi.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://eb.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://uh.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nd.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vs.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://wx.hnjuh.cn

[B09] break 与 continue
来源：http://mx.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://px.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ok.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rk.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ic.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cy.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bb.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rv.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lq.asd995.cn

[B10] 遍历同时拿索引
来源：http://tr.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://op.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tb.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fq.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tg.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ug.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ze.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hc.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vf.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://ku.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://vk.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://cx.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gs.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wv.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ky.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yh.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://wm.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bz.huixiangedu.cn

[B12] 跳出多层循环
来源：http://uz.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zh.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wm.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pc.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iz.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pa.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lx.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rd.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zn.521024.cn

[B13] 判断是否为数字
来源：http://nl.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://ur.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://ez.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kg.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tg.huanxung.cn

Java: x instanceof Number
来源：http://zm.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iu.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://li.shxzskj.cn

C#:   x is int or double or decimal
来源：http://mq.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://gr.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zl.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wf.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://cm.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://my.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ge.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://um.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lk.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aj.hnjuh.cn

[B15] 布尔运算与取反
来源：http://nb.yuntaijiaju.cn

Py:   a and b or not c
来源：http://lc.nicolike.cn

PHP:  $a && $b || !$c
来源：http://oe.chemitech.net.cn

JS:   a && b || !c
来源：http://sn.shxzskj.cn

TS:   a && b || !c
来源：http://jg.hahajie.cn

Java: a && b || !c
来源：http://wb.szsharing.cn

Go:   a && b || !c
来源：http://ck.huanxung.cn

Ruby: a && b || !c
来源：http://sl.hnjuh.cn

C#:   a && b || !c
来源：http://ss.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cg.shtwfgs.cn

Py:   if not data: return
来源：http://tc.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://ts.wgjwhj.cn

JS:   if (!data) return;
来源：http://hi.panjiajie.cn

TS:   if (!data) return;
来源：http://or.lnxyls.cn

Java: if (data == null) return;
来源：http://dc.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://yf.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://yz.huixiangedu.cn

C#:   if (data == null) return;
来源：http://ai.yuexingan06.cn

================================================================================
来源：http://rj.hahajie.cn

C. 函数与作用域
来源：http://wd.wgjwhj.cn

================================================================================
来源：http://dt.yuntaijiaju.cn

[C01] 定义函数
来源：http://hp.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://wj.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wd.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://hx.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lx.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qo.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://em.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://tr.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fd.hnjuh.cn

[C02] 默认参数
来源：http://ox.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://cs.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zf.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://aj.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vd.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rh.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qf.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://lr.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://ih.bookmarksfly.cn

[C03] 可变参数
来源：http://io.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://sv.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mv.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lq.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://px.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dy.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vj.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ke.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pb.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://wv.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vq.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dz.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ds.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pd.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ye.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://nt.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://fv.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://mx.nicolike.cn

[C05] 返回多个值
来源：http://tx.asd995.cn

Py:   return a, b
来源：http://su.nicolike.cn

PHP:  return [$a, $b];
来源：http://rh.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hd.colortex.cn

TS:   return { a, b };
来源：http://bn.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://es.hnjuh.cn

Go:   return a, b
来源：http://lh.yuntaijiaju.cn

Ruby: return a, b
来源：http://pe.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://mf.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://du.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://ek.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fq.nszjky.cn

JS:   const square = x => x * x;
来源：http://kv.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://na.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sd.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qw.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://hu.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ri.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://bv.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://db.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zd.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nj.newstarts.cn

TS:   arr.map(String)
来源：http://vv.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gr.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bn.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://lt.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pn.9csxet.cn

[C08] 闭包
来源：http://jr.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fk.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ps.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://el.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cy.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tf.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rm.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ho.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gr.jctech888.com.cn

[C09] 递归
来源：http://yf.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eq.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xg.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cj.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://om.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kc.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hl.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jq.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tc.shtwfgs.cn

[C10] 变量作用域
来源：http://wx.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lm.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ze.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nx.nszjky.cn

TS:   同 JS
来源：http://dh.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://jy.shxzukj.cn

Go:   花括号块级作用域
来源：http://ev.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://if.huanxung.cn

C#:   块级作用域
来源：http://jq.huanxung.cn

[C11] 模块导入与导出
来源：http://yj.hnjuh.cn

Py:   from module import func
来源：http://cm.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zp.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pn.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yv.jianghongdianzi.cn

Java: import java.util.List;
来源：http://xu.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ii.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://tk.wgjwhj.cn

C#:   using System.Text;
来源：http://db.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://kr.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://vj.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://ag.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://em.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ra.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kh.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://xx.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://ol.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rm.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://pj.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dz.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://an.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ev.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zt.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wa.colortex.cn

Go:   func add(a, b int) int
来源：http://mt.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vm.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hn.shtwfgs.cn

[C14] 泛型函数
来源：http://za.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ql.muxihuayi.cn

PHP:  // 无泛型
来源：http://ky.szsharing.cn

JS:   // 无泛型
来源：http://kg.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ce.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vv.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rb.nicolike.cn

Ruby: # 无泛型
来源：http://sd.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gj.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://ex.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yh.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://pl.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ba.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ml.huixinmuqiang.cn

Java: // 无解构
来源：http://nl.9csxet.cn

Go:   // 无解构
来源：http://ku.9csxet.cn

Ruby: a, b = pair
来源：http://eg.521024.cn

C#:   var (a, b) = pair;
来源：http://ti.asd995.cn

[C16] 函数 / 方法重载
来源：http://tg.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lq.colortex.cn

PHP:  // 无重载
来源：http://zw.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eb.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://bi.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qf.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://qx.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://gk.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ej.gzmigu.cn

================================================================================
来源：http://cq.asd995.cn

D. 数组 / 列表 / 集合
来源：http://rx.bookmarksfly.cn

================================================================================
来源：http://ix.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://gm.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mu.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kf.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qr.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uh.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wt.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://kq.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://kc.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lk.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://kr.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gp.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xj.521024.cn

JS:   arr.push(4);
来源：http://nc.huixiangedu.cn

TS:   arr.push(4);
来源：http://mp.chemitech.net.cn

Java: list.add(4);
来源：http://xr.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://wz.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://jb.gzmigu.cn

C#:   list.Add(4);
来源：http://wh.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://lg.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://pt.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ub.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bn.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://pv.shxzukj.cn

Java: list.add(0, 0);
来源：http://px.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kl.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pk.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://fc.9csxet.cn

[D04] 删除元素
来源：http://yh.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mp.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kc.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://np.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://rb.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rp.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pf.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ld.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cr.huixiangedu.cn

[D05] 访问与修改元素
来源：http://kx.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yb.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ew.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hp.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://sd.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://je.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ur.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ke.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uc.9csxet.cn

[D06] 数组长度
来源：http://mz.jctech888.com.cn

Py:   len(arr)
来源：http://ay.huixiangedu.cn

PHP:  count($arr);
来源：http://wz.hnjuh.cn

JS:   arr.length
来源：http://li.shtwfgs.cn

TS:   arr.length
来源：http://os.hnjuh.cn

Java: list.size();
来源：http://ko.szxytkj.cn

Go:   len(arr)
来源：http://ll.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://bu.panjiajie.cn

C#:   list.Count;
来源：http://ab.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://aj.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://es.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vu.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://ns.shtwfgs.cn


<!-- 参考信息 -->