代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://fu.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://re.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ib.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://ww.jianghongdianzi.cn

[B09] break 与 continue
来源：http://za.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lu.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zx.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qt.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wi.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yu.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mv.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ye.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://er.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://zg.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gu.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wj.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qi.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uu.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ee.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qi.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://io.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://om.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://qb.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://xi.colortex.cn

PHP:  range(0, 10, 2);
来源：http://hf.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lo.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ti.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://py.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uz.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://it.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dg.bjjhwx.cn

[B12] 跳出多层循环
来源：http://qx.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sj.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vt.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cv.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://il.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fx.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ks.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hu.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hu.9csxet.cn

[B13] 判断是否为数字
来源：http://gn.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://rb.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://ja.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dd.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://of.hahajie.cn

Java: x instanceof Number
来源：http://md.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rp.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://ky.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://fj.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://tl.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fs.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oe.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://rk.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://gj.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wy.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://au.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bf.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mj.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://ts.chemitech.net.cn

Py:   a and b or not c
来源：http://xy.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://xv.shtwfgs.cn

JS:   a && b || !c
来源：http://vi.colortex.cn

TS:   a && b || !c
来源：http://gx.nszjky.cn

Java: a && b || !c
来源：http://is.9csxet.cn

Go:   a && b || !c
来源：http://qu.muxihuayi.cn

Ruby: a && b || !c
来源：http://ij.chemitech.net.cn

C#:   a && b || !c
来源：http://kf.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eg.haigaiapp.cn

Py:   if not data: return
来源：http://pm.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://rg.panjiajie.cn

JS:   if (!data) return;
来源：http://iv.9csxet.cn

TS:   if (!data) return;
来源：http://nf.panjiajie.cn

Java: if (data == null) return;
来源：http://lq.szsharing.cn

Go:   if data == nil { return }
来源：http://fc.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://xo.yuexingan06.cn

C#:   if (data == null) return;
来源：http://tg.shtwfgs.cn

================================================================================
来源：http://hi.szxytkj.cn

C. 函数与作用域
来源：http://kt.huanxung.cn

================================================================================
来源：http://vs.nszjky.cn

[C01] 定义函数
来源：http://ai.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://ci.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pd.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://yq.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pw.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://on.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wu.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://le.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sr.hnjuh.cn

[C02] 默认参数
来源：http://hd.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://vi.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gl.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://lc.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vn.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xy.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gm.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://nt.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://mv.lnxyls.cn

[C03] 可变参数
来源：http://cr.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://ls.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mc.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://on.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://il.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mj.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tz.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ow.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rv.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://gz.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mw.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lu.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zs.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://km.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://lg.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://wx.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://bi.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://yo.jianghongdianzi.cn

[C05] 返回多个值
来源：http://jl.panjiajie.cn

Py:   return a, b
来源：http://wp.gzmigu.cn

PHP:  return [$a, $b];
来源：http://mu.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ha.colortex.cn

TS:   return { a, b };
来源：http://rk.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ds.gzmigu.cn

Go:   return a, b
来源：http://xr.szsharing.cn

Ruby: return a, b
来源：http://fm.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://fr.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://xd.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://cd.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pb.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://xq.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://gp.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://li.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kv.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://ut.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cp.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://kn.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nn.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ky.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vq.huixiangedu.cn

TS:   arr.map(String)
来源：http://lo.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nv.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qp.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://es.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://io.huixiangedu.cn

[C08] 闭包
来源：http://kr.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ku.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oe.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jx.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wp.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cd.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sx.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://co.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://an.yuexingan06.cn

[C09] 递归
来源：http://oz.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fe.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sk.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iu.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sv.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jj.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ix.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://na.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://su.huixiangedu.cn

[C10] 变量作用域
来源：http://fe.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dx.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zu.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xi.nszjky.cn

TS:   同 JS
来源：http://es.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://hx.hnjuh.cn

Go:   花括号块级作用域
来源：http://qg.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pb.huixiangedu.cn

C#:   块级作用域
来源：http://jn.bjjhwx.cn

[C11] 模块导入与导出
来源：http://ev.shxzukj.cn

Py:   from module import func
来源：http://ym.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yo.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dm.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ck.huanxung.cn

Java: import java.util.List;
来源：http://vx.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yy.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://uc.jctech888.com.cn

C#:   using System.Text;
来源：http://xd.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://aa.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://qa.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://ul.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://qj.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://al.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tw.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://yq.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://kj.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fu.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://hb.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mr.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bo.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tp.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hk.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://du.newstarts.cn

Go:   func add(a, b int) int
来源：http://ca.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://at.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zh.asd995.cn

[C14] 泛型函数
来源：http://nh.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tf.huixiangedu.cn

PHP:  // 无泛型
来源：http://dk.huanxung.cn

JS:   // 无泛型
来源：http://yl.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zc.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xg.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dv.yuexingan06.cn

Ruby: # 无泛型
来源：http://zg.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lr.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://ep.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ny.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://qg.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uv.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rt.jctech888.com.cn

Java: // 无解构
来源：http://hr.nicolike.cn

Go:   // 无解构
来源：http://qa.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://gg.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://cv.colortex.cn

[C16] 函数 / 方法重载
来源：http://zx.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ov.muxihuayi.cn

PHP:  // 无重载
来源：http://hv.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lr.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://eg.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://un.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://vy.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://wf.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lz.lnxyls.cn

================================================================================
来源：http://rr.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://yg.bookmarksfly.cn

================================================================================
来源：http://lr.asd995.cn

[D01] 创建数组 / 列表
来源：http://ue.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hn.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ts.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jn.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sm.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qt.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://dn.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://tm.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oj.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://lu.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ez.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wi.gzmigu.cn

JS:   arr.push(4);
来源：http://zn.yuexingan06.cn

TS:   arr.push(4);
来源：http://nu.huixiangedu.cn

Java: list.add(4);
来源：http://cc.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://qo.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://as.bookmarksfly.cn

C#:   list.Add(4);
来源：http://ms.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://pr.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://eb.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fp.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zk.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://yo.chemitech.net.cn

Java: list.add(0, 0);
来源：http://zi.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ps.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kt.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://sf.hahajie.cn

[D04] 删除元素
来源：http://on.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qf.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jo.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oy.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://bw.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://li.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tc.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iy.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dh.hnjuh.cn

[D05] 访问与修改元素
来源：http://nm.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gp.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rc.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cm.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://ah.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://hv.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://sx.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yr.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://du.9csxet.cn

[D06] 数组长度
来源：http://yx.panjiajie.cn

Py:   len(arr)
来源：http://ul.huanxung.cn

PHP:  count($arr);
来源：http://ep.muxihuayi.cn

JS:   arr.length
来源：http://ci.wgjwhj.cn

TS:   arr.length
来源：http://la.bookmarksfly.cn

Java: list.size();
来源：http://kw.nicolike.cn

Go:   len(arr)
来源：http://yh.asd995.cn

Ruby: arr.length; arr.size
来源：http://zj.asd995.cn

C#:   list.Count;
来源：http://ia.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://yq.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yl.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hh.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://wb.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://yf.gzmigu.cn

Java: list.subList(1, 4);
来源：http://oa.yuexingan06.cn

Go:   arr[1:4]
来源：http://fe.gzmigu.cn

Ruby: arr[1, 3]
来源：http://yt.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://bo.huixiangedu.cn

[D08] 合并两个数组
来源：http://ql.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://pq.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://wy.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://na.gzmigu.cn

TS:   [...a, ...b];
来源：http://rg.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hb.9csxet.cn

Go:   append(a, b...)
来源：http://nt.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://ud.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://xu.bjjhwx.cn

[D09] 排序（升序）
来源：http://yb.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://mt.9csxet.cn


<!-- 参考信息 -->