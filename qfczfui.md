代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jb.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://oi.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://hw.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://rx.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://br.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wt.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://eu.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://zs.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://tb.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zk.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gr.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://tl.muxihuayi.cn

[B09] break 与 continue
来源：http://fc.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ui.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mg.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://te.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gk.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mv.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://af.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oj.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bx.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://wd.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cq.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rh.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fz.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nz.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iw.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bf.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gb.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rz.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://vn.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://jr.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://xl.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pt.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mx.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ea.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fm.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://bv.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ig.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://nu.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zq.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://er.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pb.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tq.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jg.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aa.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xe.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eb.muxihuayi.cn

[B13] 判断是否为数字
来源：http://bj.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://ji.nicolike.cn

PHP:  is_numeric($x)
来源：http://qc.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yf.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://em.9csxet.cn

Java: x instanceof Number
来源：http://xm.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://za.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://tz.hnjuh.cn

C#:   x is int or double or decimal
来源：http://hf.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://eg.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ft.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://of.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://vv.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://qq.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yz.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vp.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://az.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ey.huanxung.cn

[B15] 布尔运算与取反
来源：http://vj.shxzukj.cn

Py:   a and b or not c
来源：http://nr.asd995.cn

PHP:  $a && $b || !$c
来源：http://fy.szxytkj.cn

JS:   a && b || !c
来源：http://ah.huanxung.cn

TS:   a && b || !c
来源：http://zu.jianghongdianzi.cn

Java: a && b || !c
来源：http://wv.asd995.cn

Go:   a && b || !c
来源：http://jd.hnjuh.cn

Ruby: a && b || !c
来源：http://ar.wgjwhj.cn

C#:   a && b || !c
来源：http://fh.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vd.9csxet.cn

Py:   if not data: return
来源：http://hh.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://gm.shtwfgs.cn

JS:   if (!data) return;
来源：http://kg.521024.cn

TS:   if (!data) return;
来源：http://bs.yuexingan06.cn

Java: if (data == null) return;
来源：http://op.muxihuayi.cn

Go:   if data == nil { return }
来源：http://xo.shxzukj.cn

Ruby: return if data.nil?
来源：http://sx.521024.cn

C#:   if (data == null) return;
来源：http://rk.wgjwhj.cn

================================================================================
来源：http://oj.hahajie.cn

C. 函数与作用域
来源：http://bm.nicolike.cn

================================================================================
来源：http://ap.huixiangedu.cn

[C01] 定义函数
来源：http://dn.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://rh.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jj.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://st.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bp.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mz.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hy.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://lh.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rs.wgjwhj.cn

[C02] 默认参数
来源：http://mn.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://hw.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fz.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://zl.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://js.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ib.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gf.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://sk.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://xj.chemitech.net.cn

[C03] 可变参数
来源：http://fn.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://th.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://an.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uo.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zv.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bk.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ge.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ln.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ns.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://cv.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tw.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kc.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zi.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vh.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://pi.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://on.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://tg.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://it.huanxung.cn

[C05] 返回多个值
来源：http://mq.shxzskj.cn

Py:   return a, b
来源：http://ed.asd995.cn

PHP:  return [$a, $b];
来源：http://nb.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vh.asd995.cn

TS:   return { a, b };
来源：http://cz.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ay.bjjhwx.cn

Go:   return a, b
来源：http://uc.szsharing.cn

Ruby: return a, b
来源：http://jc.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://pi.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://gy.szsharing.cn

Py:   square = lambda x: x * x
来源：http://zu.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uf.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://gu.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://kn.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ck.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tu.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://so.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ev.newstarts.cn

[C07] 把函数作为参数传入
来源：http://so.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pd.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ac.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zi.szxytkj.cn

TS:   arr.map(String)
来源：http://ag.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ko.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://su.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://il.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pz.chemitech.net.cn

[C08] 闭包
来源：http://qz.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nj.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ao.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ze.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qk.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dn.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://go.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iv.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bj.panjiajie.cn

[C09] 递归
来源：http://pg.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nd.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wy.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wt.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xr.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://he.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ed.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ic.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ga.521024.cn

[C10] 变量作用域
来源：http://ez.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tz.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pa.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://op.colortex.cn

TS:   同 JS
来源：http://ly.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://px.szsharing.cn

Go:   花括号块级作用域
来源：http://jo.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fo.hnjuh.cn

C#:   块级作用域
来源：http://ww.shxzukj.cn

[C11] 模块导入与导出
来源：http://ul.nicolike.cn

Py:   from module import func
来源：http://qu.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cd.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://al.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bl.newstarts.cn

Java: import java.util.List;
来源：http://lq.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ln.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://wk.chemitech.net.cn

C#:   using System.Text;
来源：http://zs.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://bu.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://it.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://bj.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://xe.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://br.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fg.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://qp.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://dy.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://if.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://rw.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://za.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vv.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sm.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hk.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zk.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://do.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zg.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wr.hnjuh.cn

[C14] 泛型函数
来源：http://sj.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ap.szsharing.cn

PHP:  // 无泛型
来源：http://vg.gzmigu.cn

JS:   // 无泛型
来源：http://kf.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dw.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mm.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hs.bookmarksfly.cn

Ruby: # 无泛型
来源：http://eg.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://si.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://on.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ce.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://ha.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lt.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sw.yuexingan06.cn

Java: // 无解构
来源：http://rf.yuexingan06.cn

Go:   // 无解构
来源：http://wy.shxzskj.cn

Ruby: a, b = pair
来源：http://vm.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://ah.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://js.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ag.huixinmuqiang.cn

PHP:  // 无重载
来源：http://sk.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gz.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://cl.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jk.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://gm.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://vc.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tf.lnxyls.cn

================================================================================
来源：http://pp.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://rv.newstarts.cn

================================================================================
来源：http://sa.nszjky.cn

[D01] 创建数组 / 列表
来源：http://tm.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://le.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cv.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oy.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wy.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ap.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://hz.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://wk.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pm.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://xs.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ec.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mm.hnjuh.cn

JS:   arr.push(4);
来源：http://oq.colortex.cn

TS:   arr.push(4);
来源：http://xs.shxzskj.cn

Java: list.add(4);
来源：http://wp.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://wu.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ye.chemitech.net.cn

C#:   list.Add(4);
来源：http://uv.521024.cn

[D03] 在指定位置插入元素
来源：http://bp.asd995.cn

Py:   arr.insert(0, 0)
来源：http://do.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dh.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gk.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://sy.shxzskj.cn

Java: list.add(0, 0);
来源：http://dx.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://te.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gz.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://xy.newstarts.cn

[D04] 删除元素
来源：http://iu.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nh.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rw.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ny.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://vn.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jo.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uu.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nj.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://te.muxihuayi.cn

[D05] 访问与修改元素
来源：http://av.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wy.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rp.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fs.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://nj.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://vc.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://vw.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ms.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://me.newstarts.cn

[D06] 数组长度
来源：http://ot.lnxyls.cn

Py:   len(arr)
来源：http://ad.panjiajie.cn

PHP:  count($arr);
来源：http://ib.jctech888.com.cn

JS:   arr.length
来源：http://nr.yuntaijiaju.cn

TS:   arr.length
来源：http://rk.wgjwhj.cn

Java: list.size();
来源：http://te.haigaiapp.cn

Go:   len(arr)
来源：http://iu.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://os.chemitech.net.cn

C#:   list.Count;
来源：http://ep.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://uu.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xd.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ln.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://as.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://ow.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://oj.gzmigu.cn

Go:   arr[1:4]
来源：http://as.colortex.cn

Ruby: arr[1, 3]
来源：http://mz.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://mm.nszjky.cn

[D08] 合并两个数组
来源：http://fo.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://tc.521024.cn

PHP:  array_merge($a, $b);
来源：http://eu.shtwfgs.cn


<!-- 参考信息 -->