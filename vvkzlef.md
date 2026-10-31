代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://fg.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dg.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://al.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://xy.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://fj.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mv.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ss.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://rt.yuntaijiaju.cn

[B09] break 与 continue
来源：http://de.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hv.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tc.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xj.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rk.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nu.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oz.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cn.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://xc.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gi.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aa.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sp.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kf.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://es.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lb.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fq.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ha.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://xa.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://bj.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://tq.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cj.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vn.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://is.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vm.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://nj.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cz.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ak.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mz.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jt.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gj.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fx.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hc.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xh.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oq.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oa.huixiangedu.cn

[B13] 判断是否为数字
来源：http://kg.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://et.9csxet.cn

PHP:  is_numeric($x)
来源：http://jr.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gy.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nr.muxihuayi.cn

Java: x instanceof Number
来源：http://nh.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ap.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://ji.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://zb.newstarts.cn

[B14] 判断值是否在集合内
来源：http://an.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zh.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nv.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://pc.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://oo.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ou.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zr.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dk.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xa.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://eg.9csxet.cn

Py:   a and b or not c
来源：http://my.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://nl.hnjuh.cn

JS:   a && b || !c
来源：http://ny.shxzukj.cn

TS:   a && b || !c
来源：http://rw.shxzskj.cn

Java: a && b || !c
来源：http://hn.gzmigu.cn

Go:   a && b || !c
来源：http://wl.shtwfgs.cn

Ruby: a && b || !c
来源：http://ui.yuexingan06.cn

C#:   a && b || !c
来源：http://oi.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://is.huixiangedu.cn

Py:   if not data: return
来源：http://gf.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://xi.shxzukj.cn

JS:   if (!data) return;
来源：http://ht.9csxet.cn

TS:   if (!data) return;
来源：http://ji.521024.cn

Java: if (data == null) return;
来源：http://sg.huanxung.cn

Go:   if data == nil { return }
来源：http://vq.chemitech.net.cn

Ruby: return if data.nil?
来源：http://vh.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://cw.colortex.cn

================================================================================
来源：http://tp.wgjwhj.cn

C. 函数与作用域
来源：http://dv.panjiajie.cn

================================================================================
来源：http://wx.asd995.cn

[C01] 定义函数
来源：http://qu.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://bd.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yk.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://yy.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wx.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oo.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lg.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://ak.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jv.szsharing.cn

[C02] 默认参数
来源：http://jg.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://bc.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://po.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://dx.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qo.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ze.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dj.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://vv.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://qg.nszjky.cn

[C03] 可变参数
来源：http://to.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://wa.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mu.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yg.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hy.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lv.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pa.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bm.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tf.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://iu.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vn.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hu.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jg.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gb.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://ev.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://do.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://jw.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://sb.shxzskj.cn

[C05] 返回多个值
来源：http://dq.huixiangedu.cn

Py:   return a, b
来源：http://ab.521024.cn

PHP:  return [$a, $b];
来源：http://nw.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xe.szsharing.cn

TS:   return { a, b };
来源：http://xl.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://za.jianghongdianzi.cn

Go:   return a, b
来源：http://ky.lnxyls.cn

Ruby: return a, b
来源：http://bq.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://fm.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://fu.nicolike.cn

Py:   square = lambda x: x * x
来源：http://mw.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lq.gzmigu.cn

JS:   const square = x => x * x;
来源：http://bm.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://vu.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://up.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hy.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://xq.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mh.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://ne.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dz.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mm.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dn.gzmigu.cn

TS:   arr.map(String)
来源：http://th.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gs.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ff.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://fj.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ap.nszjky.cn

[C08] 闭包
来源：http://op.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gq.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gt.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://go.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://it.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zn.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jy.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://as.huixiangedu.cn

[C09] 递归
来源：http://hu.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gb.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qm.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nj.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ut.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hk.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pa.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mq.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zk.hahajie.cn

[C10] 变量作用域
来源：http://jt.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ms.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yj.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wp.szxytkj.cn

TS:   同 JS
来源：http://kq.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://go.9csxet.cn

Go:   花括号块级作用域
来源：http://xq.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yj.yuntaijiaju.cn

C#:   块级作用域
来源：http://zh.shxzskj.cn

[C11] 模块导入与导出
来源：http://tn.gzmigu.cn

Py:   from module import func
来源：http://hz.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ow.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lj.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://da.huixinmuqiang.cn

Java: import java.util.List;
来源：http://zr.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dv.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://fw.asd995.cn

C#:   using System.Text;
来源：http://kg.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://iu.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://ya.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://rg.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://cc.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://au.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://og.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ry.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://kw.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vw.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://el.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gg.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://za.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nj.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ru.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://of.9csxet.cn

Go:   func add(a, b int) int
来源：http://uh.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nv.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ff.szsharing.cn

[C14] 泛型函数
来源：http://ba.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qg.muxihuayi.cn

PHP:  // 无泛型
来源：http://go.lnxyls.cn

JS:   // 无泛型
来源：http://xc.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lf.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eo.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bb.yuexingan06.cn

Ruby: # 无泛型
来源：http://rk.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cn.colortex.cn

[C15] 解构 / 展开参数
来源：http://io.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sy.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://mq.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://st.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wk.newstarts.cn

Java: // 无解构
来源：http://nj.shtwfgs.cn

Go:   // 无解构
来源：http://un.hnjuh.cn

Ruby: a, b = pair
来源：http://ol.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://lq.newstarts.cn

[C16] 函数 / 方法重载
来源：http://md.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xq.521024.cn

PHP:  // 无重载
来源：http://kv.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zk.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ax.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pq.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://dx.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://gh.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xl.colortex.cn

================================================================================
来源：http://ah.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://sj.yuexingan06.cn

================================================================================
来源：http://kl.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://nl.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wq.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uc.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pg.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wd.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ir.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://mh.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://zs.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pn.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://sg.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dh.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yh.521024.cn

JS:   arr.push(4);
来源：http://io.huixiangedu.cn

TS:   arr.push(4);
来源：http://up.huixinmuqiang.cn

Java: list.add(4);
来源：http://qt.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://nj.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://kk.jctech888.com.cn

C#:   list.Add(4);
来源：http://hq.521024.cn

[D03] 在指定位置插入元素
来源：http://hx.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://hm.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gw.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hs.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://nl.nszjky.cn

Java: list.add(0, 0);
来源：http://qv.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oe.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wb.521024.cn

C#:   list.Insert(0, 0);
来源：http://hw.newstarts.cn

[D04] 删除元素
来源：http://sw.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pg.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ve.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xw.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://sg.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bf.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mi.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ax.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uz.szxytkj.cn

[D05] 访问与修改元素
来源：http://cl.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xr.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ux.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ww.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://lw.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://xh.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://fk.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ni.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pt.huixinmuqiang.cn

[D06] 数组长度
来源：http://oh.nicolike.cn

Py:   len(arr)
来源：http://so.bjjhwx.cn

PHP:  count($arr);
来源：http://kd.gzmigu.cn

JS:   arr.length
来源：http://hm.yuexingan06.cn

TS:   arr.length
来源：http://rx.hahajie.cn

Java: list.size();
来源：http://wa.huixiangedu.cn

Go:   len(arr)
来源：http://qz.szsharing.cn

Ruby: arr.length; arr.size
来源：http://ue.huixinmuqiang.cn

C#:   list.Count;
来源：http://jk.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://qv.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ic.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bt.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://jp.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://qf.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://ed.nicolike.cn

Go:   arr[1:4]
来源：http://pa.hnjuh.cn

Ruby: arr[1, 3]
来源：http://lb.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://fv.bookmarksfly.cn

[D08] 合并两个数组
来源：http://uk.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://gm.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://fb.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hs.yuexingan06.cn

TS:   [...a, ...b];
来源：http://jr.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ri.huanxung.cn

Go:   append(a, b...)
来源：http://gm.nszjky.cn


<!-- 参考信息 -->