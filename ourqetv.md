代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pa.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://xn.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cb.bjjhwx.cn

[B12] 跳出多层循环
来源：http://lv.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bj.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://du.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ws.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xh.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ko.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fu.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eh.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zk.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://ae.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://kq.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://vt.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fz.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nk.nicolike.cn

Java: x instanceof Number
来源：http://fu.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yu.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://su.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://af.asd995.cn

[B14] 判断值是否在集合内
来源：http://nr.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ft.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rn.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://kb.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://bx.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lc.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://od.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://av.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fi.colortex.cn

[B15] 布尔运算与取反
来源：http://zi.bookmarksfly.cn

Py:   a and b or not c
来源：http://jk.newstarts.cn

PHP:  $a && $b || !$c
来源：http://kr.huixinmuqiang.cn

JS:   a && b || !c
来源：http://vl.haigaiapp.cn

TS:   a && b || !c
来源：http://zq.nicolike.cn

Java: a && b || !c
来源：http://aw.9csxet.cn

Go:   a && b || !c
来源：http://nt.szsharing.cn

Ruby: a && b || !c
来源：http://mx.nicolike.cn

C#:   a && b || !c
来源：http://ad.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rm.shxzskj.cn

Py:   if not data: return
来源：http://ss.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://rw.panjiajie.cn

JS:   if (!data) return;
来源：http://ml.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://ge.hnjuh.cn

Java: if (data == null) return;
来源：http://ko.huanxung.cn

Go:   if data == nil { return }
来源：http://xj.haigaiapp.cn

Ruby: return if data.nil?
来源：http://ce.wgjwhj.cn

C#:   if (data == null) return;
来源：http://vw.shxzskj.cn

================================================================================
来源：http://ba.shtwfgs.cn

C. 函数与作用域
来源：http://in.shxzukj.cn

================================================================================
来源：http://hk.huixinmuqiang.cn

[C01] 定义函数
来源：http://vm.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://kt.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ud.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ix.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ru.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kf.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ot.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://zh.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bm.hahajie.cn

[C02] 默认参数
来源：http://zn.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://cq.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ka.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://mr.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yy.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mc.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ww.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://pc.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://il.bookmarksfly.cn

[C03] 可变参数
来源：http://hs.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://tu.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uj.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bq.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kn.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bm.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rm.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qv.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gc.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://av.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ti.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sk.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cb.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oe.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://cm.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://kh.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://ft.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://vp.newstarts.cn

[C05] 返回多个值
来源：http://fs.gzmigu.cn

Py:   return a, b
来源：http://yn.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://up.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fc.lnxyls.cn

TS:   return { a, b };
来源：http://ow.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oo.nszjky.cn

Go:   return a, b
来源：http://oq.nszjky.cn

Ruby: return a, b
来源：http://zc.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://cv.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://sb.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://ph.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nr.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://oo.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://nm.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mv.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xw.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://cs.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sk.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://az.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cu.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ri.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hj.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://el.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ji.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://az.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://bs.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oa.huanxung.cn

[C08] 闭包
来源：http://pb.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zi.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qt.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yu.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bq.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lo.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zt.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jl.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wz.szxytkj.cn

[C09] 递归
来源：http://pn.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lr.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jn.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yd.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dc.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vg.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mb.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ey.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bs.gzmigu.cn

[C10] 变量作用域
来源：http://qe.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mu.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fx.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xa.hahajie.cn

TS:   同 JS
来源：http://ud.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://aj.nszjky.cn

Go:   花括号块级作用域
来源：http://yh.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bc.gzmigu.cn

C#:   块级作用域
来源：http://mw.nicolike.cn

[C11] 模块导入与导出
来源：http://km.nicolike.cn

Py:   from module import func
来源：http://ze.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gg.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hm.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ex.colortex.cn

Java: import java.util.List;
来源：http://ad.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://my.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ve.shxzskj.cn

C#:   using System.Text;
来源：http://ia.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://ql.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://vx.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://rt.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://pk.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://ac.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ed.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://jx.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://oj.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bt.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://la.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tu.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://it.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://go.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zt.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cr.shxzukj.cn

Go:   func add(a, b int) int
来源：http://jr.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jh.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://su.nicolike.cn

[C14] 泛型函数
来源：http://rh.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ki.huanxung.cn

PHP:  // 无泛型
来源：http://xj.haigaiapp.cn

JS:   // 无泛型
来源：http://ip.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zf.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wc.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lm.panjiajie.cn

Ruby: # 无泛型
来源：http://zb.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ra.nszjky.cn

[C15] 解构 / 展开参数
来源：http://kl.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vy.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://ra.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pw.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://at.bjjhwx.cn

Java: // 无解构
来源：http://ik.newstarts.cn

Go:   // 无解构
来源：http://py.gzmigu.cn

Ruby: a, b = pair
来源：http://dv.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://op.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://cq.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nt.shxzukj.cn

PHP:  // 无重载
来源：http://hj.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yp.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://hq.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wu.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://rv.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://us.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vy.jctech888.com.cn

================================================================================
来源：http://jz.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://ug.huixiangedu.cn

================================================================================
来源：http://ic.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://gu.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ov.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mh.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ei.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eu.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sg.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://df.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://fg.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rh.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://oi.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hy.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gc.shtwfgs.cn

JS:   arr.push(4);
来源：http://ei.gzmigu.cn

TS:   arr.push(4);
来源：http://yt.huanxung.cn

Java: list.add(4);
来源：http://xe.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://fn.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://vw.9csxet.cn

C#:   list.Add(4);
来源：http://ad.huanxung.cn

[D03] 在指定位置插入元素
来源：http://uw.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://jz.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gh.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mj.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://hx.szsharing.cn

Java: list.add(0, 0);
来源：http://ej.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ae.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qt.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://cr.lnxyls.cn

[D04] 删除元素
来源：http://lv.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://er.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gk.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rz.colortex.cn

TS:   arr.splice(0, 1);
来源：http://ut.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aj.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mt.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xj.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sg.bjjhwx.cn

[D05] 访问与修改元素
来源：http://fg.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qn.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pf.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vb.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://to.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://qc.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://au.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vo.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wi.shtwfgs.cn

[D06] 数组长度
来源：http://fu.chemitech.net.cn

Py:   len(arr)
来源：http://bt.colortex.cn

PHP:  count($arr);
来源：http://vd.shxzukj.cn

JS:   arr.length
来源：http://gk.huixinmuqiang.cn

TS:   arr.length
来源：http://lp.hnjuh.cn

Java: list.size();
来源：http://px.yuntaijiaju.cn

Go:   len(arr)
来源：http://rn.huanxung.cn

Ruby: arr.length; arr.size
来源：http://yi.gzmigu.cn

C#:   list.Count;
来源：http://ph.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://yf.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hs.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zf.521024.cn

JS:   arr.slice(1, 4);
来源：http://bs.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://tk.szxytkj.cn

Java: list.subList(1, 4);
来源：http://mf.panjiajie.cn

Go:   arr[1:4]
来源：http://vb.newstarts.cn

Ruby: arr[1, 3]
来源：http://dy.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://ga.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://nb.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://yu.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://td.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cs.shxzskj.cn

TS:   [...a, ...b];
来源：http://az.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jm.jctech888.com.cn

Go:   append(a, b...)
来源：http://wd.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://aj.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://cm.muxihuayi.cn

[D09] 排序（升序）
来源：http://vq.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://ca.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://yp.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yw.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tr.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wp.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tf.chemitech.net.cn

Ruby: arr.sort
来源：http://rw.nszjky.cn

C#:   list.Sort();
来源：http://sm.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fd.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xg.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zy.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ic.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mv.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xg.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cx.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cx.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vp.yuntaijiaju.cn

[D11] 反转数组
来源：http://ht.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gy.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://ii.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qz.nszjky.cn

TS:   [...arr].reverse();
来源：http://qp.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://ej.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://lq.yuexingan06.cn

Ruby: arr.reverse
来源：http://iz.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://xp.9csxet.cn

[D12] 查找元素下标
来源：http://tv.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://hh.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aa.shtwfgs.cn


<!-- 参考信息 -->