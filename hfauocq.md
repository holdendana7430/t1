代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fd.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://td.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://to.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ne.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nv.huanxung.cn

[B10] 遍历同时拿索引
来源：http://py.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yf.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ar.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pk.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://im.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tn.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vc.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hx.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yj.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://ty.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://zn.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://ls.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hf.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wf.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jx.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lr.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://yl.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ae.shxzukj.cn

[B12] 跳出多层循环
来源：http://pb.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ce.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cm.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fl.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iw.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ty.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ma.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ii.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pv.shxzskj.cn

[B13] 判断是否为数字
来源：http://bf.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://xd.lnxyls.cn

PHP:  is_numeric($x)
来源：http://mz.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qw.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wm.lnxyls.cn

Java: x instanceof Number
来源：http://am.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ud.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://ts.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://sm.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://hl.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yc.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cl.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://bb.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ab.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jp.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gz.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vf.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oc.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://ro.hahajie.cn

Py:   a and b or not c
来源：http://rn.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://xi.jctech888.com.cn

JS:   a && b || !c
来源：http://qs.muxihuayi.cn

TS:   a && b || !c
来源：http://lx.jctech888.com.cn

Java: a && b || !c
来源：http://fv.bjjhwx.cn

Go:   a && b || !c
来源：http://bk.panjiajie.cn

Ruby: a && b || !c
来源：http://eg.szsharing.cn

C#:   a && b || !c
来源：http://uk.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lw.jianghongdianzi.cn

Py:   if not data: return
来源：http://wq.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://td.huixiangedu.cn

JS:   if (!data) return;
来源：http://ud.hahajie.cn

TS:   if (!data) return;
来源：http://al.huixiangedu.cn

Java: if (data == null) return;
来源：http://ep.hnjuh.cn

Go:   if data == nil { return }
来源：http://dg.jctech888.com.cn

Ruby: return if data.nil?
来源：http://jl.szxytkj.cn

C#:   if (data == null) return;
来源：http://is.bookmarksfly.cn

================================================================================
来源：http://nj.9csxet.cn

C. 函数与作用域
来源：http://wu.colortex.cn

================================================================================
来源：http://am.hnjuh.cn

[C01] 定义函数
来源：http://ll.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://vd.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fj.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://vr.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://is.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ir.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://up.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://su.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://js.huixinmuqiang.cn

[C02] 默认参数
来源：http://ur.521024.cn

Py:   def greet(name="World"): return name
来源：http://ba.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uy.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://iv.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jx.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hx.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fy.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://ye.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://zw.muxihuayi.cn

[C03] 可变参数
来源：http://sy.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://ba.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tg.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gs.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lm.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://en.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kd.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uk.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pb.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://hc.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ri.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sm.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ad.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vq.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://du.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://na.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://ws.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://nm.muxihuayi.cn

[C05] 返回多个值
来源：http://nn.jctech888.com.cn

Py:   return a, b
来源：http://dk.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://kn.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://az.jctech888.com.cn

TS:   return { a, b };
来源：http://fb.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hg.huanxung.cn

Go:   return a, b
来源：http://jr.szxytkj.cn

Ruby: return a, b
来源：http://ke.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://rb.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://nj.nicolike.cn

Py:   square = lambda x: x * x
来源：http://mz.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pt.nszjky.cn

JS:   const square = x => x * x;
来源：http://tk.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://oo.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gd.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gu.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://ec.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xh.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://jq.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://id.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qi.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zt.shxzukj.cn

TS:   arr.map(String)
来源：http://kb.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gj.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sf.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://bo.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gb.huixiangedu.cn

[C08] 闭包
来源：http://dy.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ed.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gp.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iu.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gs.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ta.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cd.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mt.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nj.nszjky.cn

[C09] 递归
来源：http://vf.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ld.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nl.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uy.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wb.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ps.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ab.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mh.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cq.colortex.cn

[C10] 变量作用域
来源：http://gv.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hh.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qt.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dt.shxzskj.cn

TS:   同 JS
来源：http://al.asd995.cn

Java: 方法内为块级作用域
来源：http://xz.521024.cn

Go:   花括号块级作用域
来源：http://if.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ln.haigaiapp.cn

C#:   块级作用域
来源：http://wh.9csxet.cn

[C11] 模块导入与导出
来源：http://fn.lnxyls.cn

Py:   from module import func
来源：http://yr.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rj.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://em.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bn.hnjuh.cn

Java: import java.util.List;
来源：http://kp.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ql.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://uz.newstarts.cn

C#:   using System.Text;
来源：http://sh.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://ia.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://sv.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://gs.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://rj.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://wb.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nm.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://xc.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://yh.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ky.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://gg.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rp.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cn.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hg.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mi.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wa.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://vp.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qi.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bl.shxzskj.cn

[C14] 泛型函数
来源：http://su.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ro.huanxung.cn

PHP:  // 无泛型
来源：http://ch.huanxung.cn

JS:   // 无泛型
来源：http://go.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://as.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oh.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ut.panjiajie.cn

Ruby: # 无泛型
来源：http://ke.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://si.newstarts.cn

[C15] 解构 / 展开参数
来源：http://hz.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qc.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://cu.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xz.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kg.nicolike.cn

Java: // 无解构
来源：http://eu.yuexingan06.cn

Go:   // 无解构
来源：http://bp.gzmigu.cn

Ruby: a, b = pair
来源：http://so.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://hh.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://ok.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yl.shxzskj.cn

PHP:  // 无重载
来源：http://xt.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ut.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://do.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jp.521024.cn

Go:   // 无重载：用不同函数名
来源：http://gq.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://zr.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ow.panjiajie.cn

================================================================================
来源：http://th.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://ap.gzmigu.cn

================================================================================
来源：http://ph.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://lw.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://os.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ek.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yq.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gl.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bn.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://np.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://xj.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aa.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://rp.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qz.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yb.shxzskj.cn

JS:   arr.push(4);
来源：http://xq.haigaiapp.cn

TS:   arr.push(4);
来源：http://cn.9csxet.cn

Java: list.add(4);
来源：http://jr.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://hf.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://oh.szsharing.cn

C#:   list.Add(4);
来源：http://vn.colortex.cn

[D03] 在指定位置插入元素
来源：http://ir.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://eu.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bl.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jr.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://uj.newstarts.cn

Java: list.add(0, 0);
来源：http://ha.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qs.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nj.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://vu.hnjuh.cn

[D04] 删除元素
来源：http://wx.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lp.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yc.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oz.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://an.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ih.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hv.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kz.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sk.huixiangedu.cn

[D05] 访问与修改元素
来源：http://oc.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zh.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ua.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cs.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://jt.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://yc.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://mn.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bu.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sn.nszjky.cn

[D06] 数组长度
来源：http://go.newstarts.cn

Py:   len(arr)
来源：http://tr.yuntaijiaju.cn

PHP:  count($arr);
来源：http://di.hnjuh.cn

JS:   arr.length
来源：http://io.newstarts.cn

TS:   arr.length
来源：http://ys.nicolike.cn

Java: list.size();
来源：http://hp.chemitech.net.cn

Go:   len(arr)
来源：http://za.colortex.cn

Ruby: arr.length; arr.size
来源：http://xq.colortex.cn

C#:   list.Count;
来源：http://jw.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://bl.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pb.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lu.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://tz.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://ri.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://jh.muxihuayi.cn

Go:   arr[1:4]
来源：http://nc.nszjky.cn

Ruby: arr[1, 3]
来源：http://pl.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://ly.szsharing.cn

[D08] 合并两个数组
来源：http://xd.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://vv.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://up.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nn.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://yx.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zl.panjiajie.cn

Go:   append(a, b...)
来源：http://uz.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://hn.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://xw.haigaiapp.cn

[D09] 排序（升序）
来源：http://vm.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://bd.yuexingan06.cn

PHP:  sort($arr);
来源：http://ir.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pp.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tj.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xj.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kw.wgjwhj.cn

Ruby: arr.sort
来源：http://gs.panjiajie.cn

C#:   list.Sort();
来源：http://rg.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mf.jctech888.com.cn


<!-- 参考信息 -->