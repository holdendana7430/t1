代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ss.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ip.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cs.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xn.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ge.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uh.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://km.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tu.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gy.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ps.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://to.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://ka.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://lc.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://in.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tl.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dv.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://un.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://yo.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://na.huanxung.cn

[B12] 跳出多层循环
来源：http://nn.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wp.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zh.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lw.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wc.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fs.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mw.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zi.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zc.jctech888.com.cn

[B13] 判断是否为数字
来源：http://xs.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://lb.szxytkj.cn

PHP:  is_numeric($x)
来源：http://xx.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pw.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hu.521024.cn

Java: x instanceof Number
来源：http://on.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pb.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://fw.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://bk.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://sa.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ay.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vh.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://fj.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://az.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ge.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ds.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zd.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://is.colortex.cn

[B15] 布尔运算与取反
来源：http://pt.gzmigu.cn

Py:   a and b or not c
来源：http://rp.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://us.huixiangedu.cn

JS:   a && b || !c
来源：http://hd.gzmigu.cn

TS:   a && b || !c
来源：http://um.huanxung.cn

Java: a && b || !c
来源：http://eu.shxzskj.cn

Go:   a && b || !c
来源：http://rq.chemitech.net.cn

Ruby: a && b || !c
来源：http://wn.bookmarksfly.cn

C#:   a && b || !c
来源：http://ex.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lj.hahajie.cn

Py:   if not data: return
来源：http://ld.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://ch.huanxung.cn

JS:   if (!data) return;
来源：http://ys.panjiajie.cn

TS:   if (!data) return;
来源：http://ip.panjiajie.cn

Java: if (data == null) return;
来源：http://wu.wgjwhj.cn

Go:   if data == nil { return }
来源：http://cr.colortex.cn

Ruby: return if data.nil?
来源：http://pn.yuexingan06.cn

C#:   if (data == null) return;
来源：http://rc.jctech888.com.cn

================================================================================
来源：http://sz.newstarts.cn

C. 函数与作用域
来源：http://dr.shxzukj.cn

================================================================================
来源：http://qx.huanxung.cn

[C01] 定义函数
来源：http://zb.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://lq.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dn.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://qu.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://td.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ly.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lk.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://zv.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ni.lnxyls.cn

[C02] 默认参数
来源：http://ux.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://px.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nm.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://cu.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bd.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bf.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vq.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ej.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://ok.huixinmuqiang.cn

[C03] 可变参数
来源：http://en.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://rg.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://en.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ow.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yc.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fn.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nb.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ob.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mn.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://hu.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rp.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ei.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sz.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oz.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://eu.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://bf.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://yy.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://qp.huixiangedu.cn

[C05] 返回多个值
来源：http://us.colortex.cn

Py:   return a, b
来源：http://jr.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://ke.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sv.nszjky.cn

TS:   return { a, b };
来源：http://zp.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iu.shxzukj.cn

Go:   return a, b
来源：http://lk.muxihuayi.cn

Ruby: return a, b
来源：http://zj.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://ti.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://nx.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://ri.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ek.nicolike.cn

JS:   const square = x => x * x;
来源：http://sy.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://gk.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bx.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yg.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://ej.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vs.nicolike.cn

[C07] 把函数作为参数传入
来源：http://mr.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zv.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dc.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dp.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://mn.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sj.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yh.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://za.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fp.huixiangedu.cn

[C08] 闭包
来源：http://ce.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tm.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bt.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ml.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ny.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ml.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rv.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qx.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://or.huixiangedu.cn

[C09] 递归
来源：http://cx.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://na.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zp.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fx.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fc.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oc.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ns.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://an.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fw.newstarts.cn

[C10] 变量作用域
来源：http://fj.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ww.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uf.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pr.9csxet.cn

TS:   同 JS
来源：http://ii.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://ri.nszjky.cn

Go:   花括号块级作用域
来源：http://dk.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uf.521024.cn

C#:   块级作用域
来源：http://ro.9csxet.cn

[C11] 模块导入与导出
来源：http://mb.9csxet.cn

Py:   from module import func
来源：http://zk.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ll.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gk.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mz.521024.cn

Java: import java.util.List;
来源：http://ky.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zo.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://jk.chemitech.net.cn

C#:   using System.Text;
来源：http://fo.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://gm.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://yt.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://vr.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://kf.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://fn.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hn.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://fh.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://uw.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mh.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://ps.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kf.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hq.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lm.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kr.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ec.huanxung.cn

Go:   func add(a, b int) int
来源：http://so.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hf.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cu.colortex.cn

[C14] 泛型函数
来源：http://sz.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ae.bookmarksfly.cn

PHP:  // 无泛型
来源：http://ez.muxihuayi.cn

JS:   // 无泛型
来源：http://io.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mk.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://av.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wq.shxzskj.cn

Ruby: # 无泛型
来源：http://pp.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://li.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://yh.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zm.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://gm.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gp.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://of.nicolike.cn

Java: // 无解构
来源：http://do.nszjky.cn

Go:   // 无解构
来源：http://zh.szxytkj.cn

Ruby: a, b = pair
来源：http://vk.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://gy.colortex.cn

[C16] 函数 / 方法重载
来源：http://cy.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rl.gzmigu.cn

PHP:  // 无重载
来源：http://df.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zs.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://gg.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nx.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://vc.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://bd.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ya.yuntaijiaju.cn

================================================================================
来源：http://by.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://tu.hahajie.cn

================================================================================
来源：http://ut.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://vl.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mu.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lk.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://em.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ub.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bh.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://lx.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://ch.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://is.huanxung.cn

[D02] 追加元素到末尾
来源：http://xz.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gq.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gu.shtwfgs.cn

JS:   arr.push(4);
来源：http://io.gzmigu.cn

TS:   arr.push(4);
来源：http://in.haigaiapp.cn

Java: list.add(4);
来源：http://nc.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://px.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://fg.521024.cn

C#:   list.Add(4);
来源：http://ca.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://ap.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://yu.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xc.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ot.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://un.panjiajie.cn

Java: list.add(0, 0);
来源：http://nz.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://he.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vi.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://aw.521024.cn

[D04] 删除元素
来源：http://yn.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jv.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fb.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cn.asd995.cn

TS:   arr.splice(0, 1);
来源：http://kn.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vn.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ms.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iy.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://py.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://xz.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qm.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bg.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sw.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://cr.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://bw.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://fq.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ed.9csxet.cn

[D06] 数组长度
来源：http://ou.9csxet.cn

Py:   len(arr)
来源：http://ik.shxzskj.cn

PHP:  count($arr);
来源：http://ev.9csxet.cn

JS:   arr.length
来源：http://zf.hahajie.cn

TS:   arr.length
来源：http://cs.gzmigu.cn

Java: list.size();
来源：http://gd.huixiangedu.cn

Go:   len(arr)
来源：http://pm.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://no.bookmarksfly.cn

C#:   list.Count;
来源：http://kf.nicolike.cn

[D07] 切片 / 取子数组
来源：http://ma.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://of.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://st.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://tl.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://am.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://si.huanxung.cn

Go:   arr[1:4]
来源：http://wl.hahajie.cn

Ruby: arr[1, 3]
来源：http://te.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://lh.nszjky.cn

[D08] 合并两个数组
来源：http://pa.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://lx.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://gp.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rm.colortex.cn

TS:   [...a, ...b];
来源：http://zd.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hk.szxytkj.cn

Go:   append(a, b...)
来源：http://fr.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://vl.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://wp.gzmigu.cn

[D09] 排序（升序）
来源：http://vn.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ov.nicolike.cn

PHP:  sort($arr);
来源：http://yn.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rj.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://am.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fr.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://at.nicolike.cn

Ruby: arr.sort
来源：http://wm.szsharing.cn

C#:   list.Sort();
来源：http://lz.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ry.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oa.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sh.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cy.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dd.huixiangedu.cn


<!-- 参考信息 -->