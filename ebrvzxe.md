代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://ac.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://we.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://ad.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://mz.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://wy.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jh.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zu.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://fv.hnjuh.cn

[B09] break 与 continue
来源：http://mp.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bx.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gu.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uw.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ek.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qi.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ss.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zc.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zu.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://jc.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cz.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://he.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kr.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mi.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oc.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sz.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tn.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gl.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://yb.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://pe.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://tr.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cl.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://it.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zl.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ye.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://fj.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qg.colortex.cn

[B12] 跳出多层循环
来源：http://cm.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sa.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gu.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sm.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://to.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zh.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eo.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sr.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ea.hahajie.cn

[B13] 判断是否为数字
来源：http://mj.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://ey.shxzskj.cn

PHP:  is_numeric($x)
来源：http://fq.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ku.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ma.muxihuayi.cn

Java: x instanceof Number
来源：http://pl.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ig.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://ug.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://yn.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://gq.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sh.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://re.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://gn.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://kc.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dh.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lg.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ca.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tu.gzmigu.cn

[B15] 布尔运算与取反
来源：http://tj.hnjuh.cn

Py:   a and b or not c
来源：http://qw.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://vf.hnjuh.cn

JS:   a && b || !c
来源：http://ip.colortex.cn

TS:   a && b || !c
来源：http://yb.newstarts.cn

Java: a && b || !c
来源：http://dy.gzmigu.cn

Go:   a && b || !c
来源：http://re.shtwfgs.cn

Ruby: a && b || !c
来源：http://zw.9csxet.cn

C#:   a && b || !c
来源：http://uj.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wk.huixiangedu.cn

Py:   if not data: return
来源：http://ac.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://ln.huanxung.cn

JS:   if (!data) return;
来源：http://my.huanxung.cn

TS:   if (!data) return;
来源：http://tc.shtwfgs.cn

Java: if (data == null) return;
来源：http://sw.521024.cn

Go:   if data == nil { return }
来源：http://va.521024.cn

Ruby: return if data.nil?
来源：http://dv.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://fp.huanxung.cn

================================================================================
来源：http://nn.asd995.cn

C. 函数与作用域
来源：http://ac.hnjuh.cn

================================================================================
来源：http://da.szxytkj.cn

[C01] 定义函数
来源：http://lz.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://pd.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rq.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://af.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pm.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jl.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mf.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://vq.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ju.bjjhwx.cn

[C02] 默认参数
来源：http://el.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://vi.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yy.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://qb.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ch.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mu.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jo.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://jl.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://ps.chemitech.net.cn

[C03] 可变参数
来源：http://tt.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://qv.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yy.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vm.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://on.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yk.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wp.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xi.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ir.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://ol.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cg.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sq.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kd.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pz.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://di.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://mv.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://xc.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://fl.jianghongdianzi.cn

[C05] 返回多个值
来源：http://tc.shxzukj.cn

Py:   return a, b
来源：http://cg.nicolike.cn

PHP:  return [$a, $b];
来源：http://kc.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ws.hahajie.cn

TS:   return { a, b };
来源：http://sl.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qu.521024.cn

Go:   return a, b
来源：http://ti.muxihuayi.cn

Ruby: return a, b
来源：http://mj.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://lv.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://pt.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://po.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mh.colortex.cn

JS:   const square = x => x * x;
来源：http://xn.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://jb.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hw.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rg.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://uj.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pa.521024.cn

[C07] 把函数作为参数传入
来源：http://gq.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ya.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lx.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://co.nicolike.cn

TS:   arr.map(String)
来源：http://nc.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kh.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bv.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://tx.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fu.bjjhwx.cn

[C08] 闭包
来源：http://yi.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xw.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zw.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zn.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hd.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pb.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hk.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pd.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jw.huanxung.cn

[C09] 递归
来源：http://mw.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ci.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xo.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tt.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nx.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://th.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ny.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qd.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zr.jctech888.com.cn

[C10] 变量作用域
来源：http://qw.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zd.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://en.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ox.yuntaijiaju.cn

TS:   同 JS
来源：http://xm.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://xm.muxihuayi.cn

Go:   花括号块级作用域
来源：http://pi.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rr.521024.cn

C#:   块级作用域
来源：http://wh.huixiangedu.cn

[C11] 模块导入与导出
来源：http://dk.muxihuayi.cn

Py:   from module import func
来源：http://jr.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wg.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://au.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yp.szxytkj.cn

Java: import java.util.List;
来源：http://ql.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kh.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://uv.huixinmuqiang.cn

C#:   using System.Text;
来源：http://ul.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://jd.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://af.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://lx.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://kt.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://rq.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ba.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://xm.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://jo.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qs.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://po.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oc.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pu.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mr.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cp.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bv.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://hz.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gy.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vs.bjjhwx.cn

[C14] 泛型函数
来源：http://uy.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ah.nszjky.cn

PHP:  // 无泛型
来源：http://jq.shxzskj.cn

JS:   // 无泛型
来源：http://ym.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vx.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xy.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mf.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://ll.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mz.newstarts.cn

[C15] 解构 / 展开参数
来源：http://vw.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mo.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://hc.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xi.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ic.huanxung.cn

Java: // 无解构
来源：http://vm.jctech888.com.cn

Go:   // 无解构
来源：http://ya.szxytkj.cn

Ruby: a, b = pair
来源：http://pl.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://gi.huanxung.cn

[C16] 函数 / 方法重载
来源：http://ps.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jp.huanxung.cn

PHP:  // 无重载
来源：http://ci.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oi.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://dc.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zp.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://zq.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://tf.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iy.shtwfgs.cn

================================================================================
来源：http://qc.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://mi.jianghongdianzi.cn

================================================================================
来源：http://fn.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://yd.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yg.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sk.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sp.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jn.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gz.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://rk.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://hf.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hv.newstarts.cn

[D02] 追加元素到末尾
来源：http://lt.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zq.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tm.jctech888.com.cn

JS:   arr.push(4);
来源：http://qi.lnxyls.cn

TS:   arr.push(4);
来源：http://oz.9csxet.cn

Java: list.add(4);
来源：http://bp.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://ep.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://pv.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://cd.asd995.cn

[D03] 在指定位置插入元素
来源：http://le.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://fl.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vs.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://re.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://at.szsharing.cn

Java: list.add(0, 0);
来源：http://sc.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qf.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mk.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://zn.huanxung.cn

[D04] 删除元素
来源：http://xl.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tj.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dg.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gq.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://ad.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sv.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ok.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ri.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rc.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://fb.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yy.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ax.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xs.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://pp.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://ho.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://pl.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bv.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xq.huixinmuqiang.cn

[D06] 数组长度
来源：http://hl.panjiajie.cn

Py:   len(arr)
来源：http://bj.wgjwhj.cn

PHP:  count($arr);
来源：http://gd.huanxung.cn

JS:   arr.length
来源：http://vi.szxytkj.cn

TS:   arr.length
来源：http://tp.shxzukj.cn

Java: list.size();
来源：http://mq.panjiajie.cn

Go:   len(arr)
来源：http://ay.9csxet.cn

Ruby: arr.length; arr.size
来源：http://qt.hnjuh.cn

C#:   list.Count;
来源：http://zz.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://sb.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vw.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ft.asd995.cn

JS:   arr.slice(1, 4);
来源：http://aj.521024.cn

TS:   arr.slice(1, 4);
来源：http://hw.hahajie.cn

Java: list.subList(1, 4);
来源：http://by.newstarts.cn

Go:   arr[1:4]
来源：http://jd.huanxung.cn

Ruby: arr[1, 3]
来源：http://fk.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://wj.panjiajie.cn

[D08] 合并两个数组
来源：http://fk.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://ri.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://lk.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ro.521024.cn

TS:   [...a, ...b];
来源：http://bg.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iy.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://it.muxihuayi.cn


<!-- 参考信息 -->