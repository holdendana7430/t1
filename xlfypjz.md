代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fk.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ur.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vn.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dm.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bu.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xp.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://iw.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://an.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://vi.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pz.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jy.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bw.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cl.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://op.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vr.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://vr.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vr.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vv.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wj.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ib.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mo.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://db.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oq.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://md.521024.cn

[B13] 判断是否为数字
来源：http://xw.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://ic.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://pt.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rn.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sw.panjiajie.cn

Java: x instanceof Number
来源：http://qu.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ok.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://ai.szsharing.cn

C#:   x is int or double or decimal
来源：http://ij.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://fy.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oy.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ep.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://pw.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://nq.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://od.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cr.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nb.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vr.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://qq.shxzskj.cn

Py:   a and b or not c
来源：http://ly.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://jg.colortex.cn

JS:   a && b || !c
来源：http://pf.bookmarksfly.cn

TS:   a && b || !c
来源：http://wn.newstarts.cn

Java: a && b || !c
来源：http://xr.nszjky.cn

Go:   a && b || !c
来源：http://xk.nszjky.cn

Ruby: a && b || !c
来源：http://rg.jianghongdianzi.cn

C#:   a && b || !c
来源：http://sv.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ix.panjiajie.cn

Py:   if not data: return
来源：http://sa.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://iz.haigaiapp.cn

JS:   if (!data) return;
来源：http://rx.chemitech.net.cn

TS:   if (!data) return;
来源：http://vx.huixiangedu.cn

Java: if (data == null) return;
来源：http://gs.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://wt.wgjwhj.cn

Ruby: return if data.nil?
来源：http://fw.521024.cn

C#:   if (data == null) return;
来源：http://rt.colortex.cn

================================================================================
来源：http://xb.bookmarksfly.cn

C. 函数与作用域
来源：http://pp.chemitech.net.cn

================================================================================
来源：http://gs.chemitech.net.cn

[C01] 定义函数
来源：http://lt.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://fy.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://md.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://vd.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lb.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gc.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nn.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://jc.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oh.asd995.cn

[C02] 默认参数
来源：http://yi.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://ob.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hj.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://nr.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hj.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vl.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bo.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://fj.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://qt.shxzukj.cn

[C03] 可变参数
来源：http://ow.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://rq.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jl.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qb.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fe.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fx.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pr.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vh.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gt.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://sb.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kp.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ac.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ow.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jc.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ni.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://ic.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://uj.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://zb.nicolike.cn

[C05] 返回多个值
来源：http://np.panjiajie.cn

Py:   return a, b
来源：http://ii.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://zw.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://np.hnjuh.cn

TS:   return { a, b };
来源：http://oj.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ah.colortex.cn

Go:   return a, b
来源：http://gd.szsharing.cn

Ruby: return a, b
来源：http://qq.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://jt.colortex.cn

[C06] 匿名函数 / lambda
来源：http://mx.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://eu.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://im.shxzukj.cn

JS:   const square = x => x * x;
来源：http://fj.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://he.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vi.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ix.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://ar.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jt.nicolike.cn

[C07] 把函数作为参数传入
来源：http://nq.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ky.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kg.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://av.szsharing.cn

TS:   arr.map(String)
来源：http://qv.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ai.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fb.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://cp.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wf.shxzskj.cn

[C08] 闭包
来源：http://zo.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://te.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wz.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://db.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sm.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sn.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pn.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ne.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ec.haigaiapp.cn

[C09] 递归
来源：http://lb.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zt.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pc.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jb.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://la.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wd.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dk.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aj.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lm.colortex.cn

[C10] 变量作用域
来源：http://yc.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qh.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zg.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kf.muxihuayi.cn

TS:   同 JS
来源：http://uk.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://lp.hnjuh.cn

Go:   花括号块级作用域
来源：http://la.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oy.9csxet.cn

C#:   块级作用域
来源：http://cj.9csxet.cn

[C11] 模块导入与导出
来源：http://kj.wgjwhj.cn

Py:   from module import func
来源：http://sl.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ib.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wy.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://af.wgjwhj.cn

Java: import java.util.List;
来源：http://hu.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ob.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://ra.hnjuh.cn

C#:   using System.Text;
来源：http://kr.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://wz.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://ps.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://mt.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://cl.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://cb.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nz.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://in.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://ni.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ua.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://tm.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uq.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gy.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://in.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sm.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mc.521024.cn

Go:   func add(a, b int) int
来源：http://sr.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zt.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xa.yuntaijiaju.cn

[C14] 泛型函数
来源：http://ax.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eu.szxytkj.cn

PHP:  // 无泛型
来源：http://jv.huixinmuqiang.cn

JS:   // 无泛型
来源：http://cr.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ds.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nn.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pr.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://ez.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://om.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://vd.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://za.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://rf.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aj.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://da.9csxet.cn

Java: // 无解构
来源：http://jv.521024.cn

Go:   // 无解构
来源：http://xc.newstarts.cn

Ruby: a, b = pair
来源：http://go.colortex.cn

C#:   var (a, b) = pair;
来源：http://rb.colortex.cn

[C16] 函数 / 方法重载
来源：http://fq.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://la.shxzskj.cn

PHP:  // 无重载
来源：http://zh.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wn.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ye.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rt.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://he.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://xu.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xc.newstarts.cn

================================================================================
来源：http://er.colortex.cn

D. 数组 / 列表 / 集合
来源：http://qn.nszjky.cn

================================================================================
来源：http://js.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://fg.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rl.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yh.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pl.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kz.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hi.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://it.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://zl.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bh.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://fu.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kv.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uw.hahajie.cn

JS:   arr.push(4);
来源：http://er.nszjky.cn

TS:   arr.push(4);
来源：http://dg.yuexingan06.cn

Java: list.add(4);
来源：http://qu.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://eb.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://fj.asd995.cn

C#:   list.Add(4);
来源：http://ri.huanxung.cn

[D03] 在指定位置插入元素
来源：http://qm.521024.cn

Py:   arr.insert(0, 0)
来源：http://ul.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wc.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iy.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ft.shtwfgs.cn

Java: list.add(0, 0);
来源：http://bw.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cw.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bd.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://ff.nszjky.cn

[D04] 删除元素
来源：http://xh.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://co.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fz.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hl.colortex.cn

TS:   arr.splice(0, 1);
来源：http://pv.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jq.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ig.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gs.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fu.gzmigu.cn

[D05] 访问与修改元素
来源：http://ou.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qv.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ab.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ar.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://os.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://wf.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://ec.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zh.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wm.szxytkj.cn

[D06] 数组长度
来源：http://pm.shxzukj.cn

Py:   len(arr)
来源：http://ul.szxytkj.cn

PHP:  count($arr);
来源：http://zf.huixinmuqiang.cn

JS:   arr.length
来源：http://ix.newstarts.cn

TS:   arr.length
来源：http://am.nicolike.cn

Java: list.size();
来源：http://hz.shxzskj.cn

Go:   len(arr)
来源：http://gj.asd995.cn

Ruby: arr.length; arr.size
来源：http://ay.gzmigu.cn

C#:   list.Count;
来源：http://ze.9csxet.cn

[D07] 切片 / 取子数组
来源：http://uf.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xo.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wy.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://yt.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://ar.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://ow.shxzskj.cn

Go:   arr[1:4]
来源：http://ep.521024.cn

Ruby: arr[1, 3]
来源：http://vi.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://bb.haigaiapp.cn

[D08] 合并两个数组
来源：http://kn.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://qk.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://ja.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yd.jctech888.com.cn

TS:   [...a, ...b];
来源：http://sm.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oy.lnxyls.cn

Go:   append(a, b...)
来源：http://ue.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://qx.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://wl.shtwfgs.cn

[D09] 排序（升序）
来源：http://iy.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://op.asd995.cn

PHP:  sort($arr);
来源：http://pi.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gg.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://al.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aa.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pg.shxzukj.cn

Ruby: arr.sort
来源：http://vs.panjiajie.cn

C#:   list.Sort();
来源：http://tl.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kh.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xn.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qq.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ih.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://et.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ep.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ef.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sr.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lo.huixiangedu.cn


<!-- 参考信息 -->