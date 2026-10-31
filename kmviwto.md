代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://gf.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wp.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://yn.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://lt.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://pu.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ct.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wr.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://ce.nicolike.cn

[B09] break 与 continue
来源：http://an.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hw.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bu.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pn.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xi.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ci.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pu.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fv.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vs.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://gj.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kd.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yl.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sx.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mo.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wf.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cr.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rs.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vr.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://sc.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://ay.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://nj.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yu.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pi.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fp.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vs.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://om.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uk.shtwfgs.cn

[B12] 跳出多层循环
来源：http://hf.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lu.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mg.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yc.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ar.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ru.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xb.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pj.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://on.hahajie.cn

[B13] 判断是否为数字
来源：http://ep.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://ce.newstarts.cn

PHP:  is_numeric($x)
来源：http://rq.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ld.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ow.521024.cn

Java: x instanceof Number
来源：http://hz.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ra.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://lk.nszjky.cn

C#:   x is int or double or decimal
来源：http://xd.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://sx.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iz.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vq.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://km.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://gz.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vm.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ho.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lj.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ly.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://pt.huixiangedu.cn

Py:   a and b or not c
来源：http://lv.asd995.cn

PHP:  $a && $b || !$c
来源：http://wo.haigaiapp.cn

JS:   a && b || !c
来源：http://jd.hahajie.cn

TS:   a && b || !c
来源：http://ot.nszjky.cn

Java: a && b || !c
来源：http://jl.lnxyls.cn

Go:   a && b || !c
来源：http://zf.huixiangedu.cn

Ruby: a && b || !c
来源：http://ty.panjiajie.cn

C#:   a && b || !c
来源：http://dk.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dm.hahajie.cn

Py:   if not data: return
来源：http://yi.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://zn.hnjuh.cn

JS:   if (!data) return;
来源：http://rz.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://mu.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://sb.wgjwhj.cn

Go:   if data == nil { return }
来源：http://to.shxzukj.cn

Ruby: return if data.nil?
来源：http://rv.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://av.hahajie.cn

================================================================================
来源：http://fq.jianghongdianzi.cn

C. 函数与作用域
来源：http://qc.shxzukj.cn

================================================================================
来源：http://yg.szxytkj.cn

[C01] 定义函数
来源：http://rb.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://kq.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jl.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://fq.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mz.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fo.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ee.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://pe.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tf.colortex.cn

[C02] 默认参数
来源：http://jt.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://qu.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xe.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ob.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fr.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://px.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vy.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://ip.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://vt.chemitech.net.cn

[C03] 可变参数
来源：http://qy.521024.cn

Py:   def total(*args): return sum(args)
来源：http://el.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wd.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qm.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://px.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xj.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wg.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kr.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sp.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://mm.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yr.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lm.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fi.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xg.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://ah.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://qe.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://oa.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://rf.9csxet.cn

[C05] 返回多个值
来源：http://yd.9csxet.cn

Py:   return a, b
来源：http://la.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://vs.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rr.panjiajie.cn

TS:   return { a, b };
来源：http://vf.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vg.shxzskj.cn

Go:   return a, b
来源：http://jw.wgjwhj.cn

Ruby: return a, b
来源：http://ak.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://pw.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://hv.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://sn.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xn.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://zh.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://op.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iu.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://en.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://ii.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sp.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://xp.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ng.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zd.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pb.huanxung.cn

TS:   arr.map(String)
来源：http://ig.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rk.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ks.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://bv.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xm.nszjky.cn

[C08] 闭包
来源：http://id.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sn.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ry.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xp.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gv.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ik.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dl.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wj.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jm.shxzukj.cn

[C09] 递归
来源：http://lx.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wr.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yl.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iq.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bx.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://is.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jv.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ik.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qy.colortex.cn

[C10] 变量作用域
来源：http://hm.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kv.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nc.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mh.hnjuh.cn

TS:   同 JS
来源：http://ys.nicolike.cn

Java: 方法内为块级作用域
来源：http://po.huanxung.cn

Go:   花括号块级作用域
来源：http://ap.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hk.nszjky.cn

C#:   块级作用域
来源：http://ys.521024.cn

[C11] 模块导入与导出
来源：http://kr.bjjhwx.cn

Py:   from module import func
来源：http://nq.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hg.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wc.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cr.nicolike.cn

Java: import java.util.List;
来源：http://mw.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iq.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://ri.huixiangedu.cn

C#:   using System.Text;
来源：http://nj.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://xw.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://oc.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://hi.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://hu.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://tr.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lx.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ek.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://kf.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vs.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://sp.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pe.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ay.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://en.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bt.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oq.gzmigu.cn

Go:   func add(a, b int) int
来源：http://ut.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gz.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ie.shtwfgs.cn

[C14] 泛型函数
来源：http://wj.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pi.panjiajie.cn

PHP:  // 无泛型
来源：http://vx.szxytkj.cn

JS:   // 无泛型
来源：http://qn.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ny.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ji.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ph.wgjwhj.cn

Ruby: # 无泛型
来源：http://al.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://az.9csxet.cn

[C15] 解构 / 展开参数
来源：http://bo.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zh.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://gl.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vq.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ad.shxzskj.cn

Java: // 无解构
来源：http://nw.hnjuh.cn

Go:   // 无解构
来源：http://ls.521024.cn

Ruby: a, b = pair
来源：http://ep.newstarts.cn

C#:   var (a, b) = pair;
来源：http://km.szsharing.cn

[C16] 函数 / 方法重载
来源：http://yd.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zt.asd995.cn

PHP:  // 无重载
来源：http://mu.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://iv.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://fo.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kx.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://tv.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://os.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yh.szsharing.cn

================================================================================
来源：http://uo.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://rf.gzmigu.cn

================================================================================
来源：http://dr.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://ol.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ga.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iz.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://is.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yb.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qz.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://nl.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://yg.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tv.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://zw.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eg.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rz.gzmigu.cn

JS:   arr.push(4);
来源：http://xy.yuexingan06.cn

TS:   arr.push(4);
来源：http://jk.huixinmuqiang.cn

Java: list.add(4);
来源：http://xn.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://sv.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://th.huixiangedu.cn

C#:   list.Add(4);
来源：http://xz.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://pm.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://dl.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wx.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rw.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://ru.shxzskj.cn

Java: list.add(0, 0);
来源：http://hk.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ny.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zb.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://oj.bookmarksfly.cn

[D04] 删除元素
来源：http://qh.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qb.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xk.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qf.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://rx.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://io.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xr.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nq.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tw.newstarts.cn

[D05] 访问与修改元素
来源：http://ku.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uy.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zv.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xc.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://fc.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://zv.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://tk.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jo.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nu.szxytkj.cn

[D06] 数组长度
来源：http://gt.asd995.cn

Py:   len(arr)
来源：http://tj.szxytkj.cn

PHP:  count($arr);
来源：http://yn.szxytkj.cn

JS:   arr.length
来源：http://xj.haigaiapp.cn

TS:   arr.length
来源：http://ve.jianghongdianzi.cn

Java: list.size();
来源：http://gg.chemitech.net.cn

Go:   len(arr)
来源：http://qg.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://cp.asd995.cn

C#:   list.Count;
来源：http://yw.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://ec.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gk.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tr.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://vb.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://th.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://tj.jctech888.com.cn

Go:   arr[1:4]
来源：http://qz.shxzskj.cn

Ruby: arr[1, 3]
来源：http://fj.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://ft.colortex.cn

[D08] 合并两个数组
来源：http://eh.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://qi.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://ux.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nq.bjjhwx.cn

TS:   [...a, ...b];
来源：http://vo.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sn.hahajie.cn

Go:   append(a, b...)
来源：http://xy.yuntaijiaju.cn


<!-- 参考信息 -->