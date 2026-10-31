代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jn.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yz.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://al.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://vj.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://hl.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dm.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aj.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mt.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zs.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://dq.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hg.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ji.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bq.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qa.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://un.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dx.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xb.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://in.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wa.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hh.jctech888.com.cn

[B13] 判断是否为数字
来源：http://co.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://ed.9csxet.cn

PHP:  is_numeric($x)
来源：http://zn.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ug.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xs.newstarts.cn

Java: x instanceof Number
来源：http://hq.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yk.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://hv.szxytkj.cn

C#:   x is int or double or decimal
来源：http://uc.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://pf.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bp.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qh.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://wp.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://po.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://io.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://su.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xx.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qm.nszjky.cn

[B15] 布尔运算与取反
来源：http://kv.9csxet.cn

Py:   a and b or not c
来源：http://nv.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://iv.nicolike.cn

JS:   a && b || !c
来源：http://gp.newstarts.cn

TS:   a && b || !c
来源：http://ob.newstarts.cn

Java: a && b || !c
来源：http://wt.nicolike.cn

Go:   a && b || !c
来源：http://mm.colortex.cn

Ruby: a && b || !c
来源：http://qq.521024.cn

C#:   a && b || !c
来源：http://sj.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lu.nicolike.cn

Py:   if not data: return
来源：http://xs.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://um.colortex.cn

JS:   if (!data) return;
来源：http://mf.9csxet.cn

TS:   if (!data) return;
来源：http://ce.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://ny.jctech888.com.cn

Go:   if data == nil { return }
来源：http://lz.szsharing.cn

Ruby: return if data.nil?
来源：http://fw.wgjwhj.cn

C#:   if (data == null) return;
来源：http://um.panjiajie.cn

================================================================================
来源：http://om.panjiajie.cn

C. 函数与作用域
来源：http://fy.wgjwhj.cn

================================================================================
来源：http://jb.bookmarksfly.cn

[C01] 定义函数
来源：http://cv.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://uq.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lj.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://qx.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ag.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://py.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rl.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://wy.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://te.jianghongdianzi.cn

[C02] 默认参数
来源：http://un.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://ni.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zq.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://sa.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qo.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vu.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qq.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://hb.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://vm.lnxyls.cn

[C03] 可变参数
来源：http://pl.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://se.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lw.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gw.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://da.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ds.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gx.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wc.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lb.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://ni.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ln.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fq.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rv.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rx.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://kw.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://ak.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://bg.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://yy.nicolike.cn

[C05] 返回多个值
来源：http://mq.nicolike.cn

Py:   return a, b
来源：http://nk.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://nb.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xa.panjiajie.cn

TS:   return { a, b };
来源：http://un.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hc.shxzskj.cn

Go:   return a, b
来源：http://vh.shtwfgs.cn

Ruby: return a, b
来源：http://to.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://oc.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://de.colortex.cn

Py:   square = lambda x: x * x
来源：http://tf.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mx.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://it.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://aj.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://om.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://my.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://wx.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rj.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://nj.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vj.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fj.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yb.colortex.cn

TS:   arr.map(String)
来源：http://ja.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qd.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ed.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://ta.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://st.yuexingan06.cn

[C08] 闭包
来源：http://yh.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cn.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xi.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yr.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lr.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ad.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bg.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nj.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ab.haigaiapp.cn

[C09] 递归
来源：http://kb.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ej.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oc.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fy.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fj.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vp.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fx.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ca.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xl.muxihuayi.cn

[C10] 变量作用域
来源：http://so.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cb.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kj.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://em.lnxyls.cn

TS:   同 JS
来源：http://ac.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://sk.bjjhwx.cn

Go:   花括号块级作用域
来源：http://ng.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rt.szxytkj.cn

C#:   块级作用域
来源：http://kk.huixiangedu.cn

[C11] 模块导入与导出
来源：http://ny.jianghongdianzi.cn

Py:   from module import func
来源：http://km.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dj.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mg.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gs.shxzukj.cn

Java: import java.util.List;
来源：http://rh.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vu.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://ku.shtwfgs.cn

C#:   using System.Text;
来源：http://zr.521024.cn

[C12] 立即执行函数 IIFE
来源：http://fw.521024.cn

Py:   (lambda: print("run"))()
来源：http://bl.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://un.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://dz.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://lc.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fa.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://df.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://fy.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qb.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://gn.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tw.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ho.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sz.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kf.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://en.lnxyls.cn

Go:   func add(a, b int) int
来源：http://qa.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dw.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vr.hahajie.cn

[C14] 泛型函数
来源：http://pj.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://da.asd995.cn

PHP:  // 无泛型
来源：http://yq.huanxung.cn

JS:   // 无泛型
来源：http://ap.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mq.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lh.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rw.haigaiapp.cn

Ruby: # 无泛型
来源：http://ov.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xw.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://io.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://az.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://jz.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bn.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pr.9csxet.cn

Java: // 无解构
来源：http://df.jianghongdianzi.cn

Go:   // 无解构
来源：http://rp.wgjwhj.cn

Ruby: a, b = pair
来源：http://nn.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://jx.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://lc.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vn.shxzskj.cn

PHP:  // 无重载
来源：http://fz.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xt.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://ei.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tf.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://zw.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://si.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wp.gzmigu.cn

================================================================================
来源：http://yd.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://pr.haigaiapp.cn

================================================================================
来源：http://fq.9csxet.cn

[D01] 创建数组 / 列表
来源：http://nf.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qj.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ev.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xe.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iq.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://de.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://zv.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://fu.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bq.szxytkj.cn

[D02] 追加元素到末尾
来源：http://hm.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kw.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ao.szxytkj.cn

JS:   arr.push(4);
来源：http://xz.yuexingan06.cn

TS:   arr.push(4);
来源：http://wb.haigaiapp.cn

Java: list.add(4);
来源：http://sl.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://ik.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://du.nszjky.cn

C#:   list.Add(4);
来源：http://py.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://jp.asd995.cn

Py:   arr.insert(0, 0)
来源：http://jj.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ut.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ys.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://jk.nszjky.cn

Java: list.add(0, 0);
来源：http://sv.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hh.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sf.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://za.shxzukj.cn

[D04] 删除元素
来源：http://bd.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vt.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hd.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qp.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://vd.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gm.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kh.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hw.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zm.shxzskj.cn

[D05] 访问与修改元素
来源：http://ed.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kv.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zi.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hh.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://vn.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://wa.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://kv.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://db.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sh.nicolike.cn

[D06] 数组长度
来源：http://gr.asd995.cn

Py:   len(arr)
来源：http://ge.lnxyls.cn

PHP:  count($arr);
来源：http://lg.521024.cn

JS:   arr.length
来源：http://br.wgjwhj.cn

TS:   arr.length
来源：http://pu.jianghongdianzi.cn

Java: list.size();
来源：http://jr.yuexingan06.cn

Go:   len(arr)
来源：http://bb.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://sa.521024.cn

C#:   list.Count;
来源：http://tw.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://zd.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xu.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xm.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://vw.colortex.cn

TS:   arr.slice(1, 4);
来源：http://ip.shxzukj.cn

Java: list.subList(1, 4);
来源：http://fl.yuexingan06.cn

Go:   arr[1:4]
来源：http://uy.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://ay.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://dk.nicolike.cn

[D08] 合并两个数组
来源：http://aa.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://sh.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://nu.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sp.asd995.cn

TS:   [...a, ...b];
来源：http://zb.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bk.colortex.cn

Go:   append(a, b...)
来源：http://hh.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://um.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://gs.colortex.cn

[D09] 排序（升序）
来源：http://jj.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://vb.shtwfgs.cn

PHP:  sort($arr);
来源：http://ja.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ed.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://un.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oo.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gp.bookmarksfly.cn

Ruby: arr.sort
来源：http://yn.szsharing.cn

C#:   list.Sort();
来源：http://ah.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yq.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sv.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ia.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pg.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qy.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ge.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gd.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gs.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://td.szsharing.cn

[D11] 反转数组
来源：http://wg.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zg.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://us.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://go.bjjhwx.cn


<!-- 参考信息 -->