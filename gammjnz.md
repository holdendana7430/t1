代发 wailian999

[B13] 判断是否为数字
来源：http://hu.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://pz.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://by.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ky.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rv.bjjhwx.cn

Java: x instanceof Number
来源：http://vm.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ln.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://vn.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://kk.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://pu.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ri.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rt.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://yp.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://mp.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sr.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ha.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zn.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rv.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://ua.szsharing.cn

Py:   a and b or not c
来源：http://py.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://wh.shtwfgs.cn

JS:   a && b || !c
来源：http://mk.hahajie.cn

TS:   a && b || !c
来源：http://rs.szxytkj.cn

Java: a && b || !c
来源：http://cx.hnjuh.cn

Go:   a && b || !c
来源：http://tv.huanxung.cn

Ruby: a && b || !c
来源：http://wg.szsharing.cn

C#:   a && b || !c
来源：http://cv.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tv.nszjky.cn

Py:   if not data: return
来源：http://ao.521024.cn

PHP:  if (!$data) { return; }
来源：http://oc.panjiajie.cn

JS:   if (!data) return;
来源：http://sp.szxytkj.cn

TS:   if (!data) return;
来源：http://qq.nszjky.cn

Java: if (data == null) return;
来源：http://mp.shtwfgs.cn

Go:   if data == nil { return }
来源：http://pk.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://lu.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://af.shtwfgs.cn

================================================================================
来源：http://bg.jctech888.com.cn

C. 函数与作用域
来源：http://xo.bjjhwx.cn

================================================================================
来源：http://fj.huanxung.cn

[C01] 定义函数
来源：http://rh.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://ds.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rg.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://ka.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mz.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://er.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lq.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://ps.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://la.colortex.cn

[C02] 默认参数
来源：http://bg.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://ou.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://im.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://oy.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ej.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oq.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zh.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://fw.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://gf.shxzukj.cn

[C03] 可变参数
来源：http://ot.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://og.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lq.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nx.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gd.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jx.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pb.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tu.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pe.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://sj.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zr.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xq.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nh.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xh.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://ph.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://fa.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://om.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://xk.szsharing.cn

[C05] 返回多个值
来源：http://pp.huanxung.cn

Py:   return a, b
来源：http://jp.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://vv.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xt.haigaiapp.cn

TS:   return { a, b };
来源：http://mg.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bl.haigaiapp.cn

Go:   return a, b
来源：http://lf.hahajie.cn

Ruby: return a, b
来源：http://fp.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ks.521024.cn

[C06] 匿名函数 / lambda
来源：http://xl.szsharing.cn

Py:   square = lambda x: x * x
来源：http://ja.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wh.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://zk.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://vh.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dt.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zx.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://cn.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://be.huanxung.cn

[C07] 把函数作为参数传入
来源：http://ve.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ar.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hb.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ev.nicolike.cn

TS:   arr.map(String)
来源：http://au.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hb.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gd.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://uo.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xd.hnjuh.cn

[C08] 闭包
来源：http://dd.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ug.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cy.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zf.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oh.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kf.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yp.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jz.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jo.muxihuayi.cn

[C09] 递归
来源：http://gw.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kq.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nt.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://go.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jq.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ie.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mc.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rw.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vj.shtwfgs.cn

[C10] 变量作用域
来源：http://cz.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wp.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fv.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oi.colortex.cn

TS:   同 JS
来源：http://gc.panjiajie.cn

Java: 方法内为块级作用域
来源：http://jg.chemitech.net.cn

Go:   花括号块级作用域
来源：http://sy.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ka.asd995.cn

C#:   块级作用域
来源：http://rs.haigaiapp.cn

[C11] 模块导入与导出
来源：http://dr.yuntaijiaju.cn

Py:   from module import func
来源：http://ly.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hc.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jt.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vb.shxzukj.cn

Java: import java.util.List;
来源：http://hm.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wy.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://zr.hahajie.cn

C#:   using System.Text;
来源：http://dj.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://mg.521024.cn

Py:   (lambda: print("run"))()
来源：http://zv.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://yu.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://hy.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://dp.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qr.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://fu.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://jy.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://aa.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://ps.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ac.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hv.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sk.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cu.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gy.szxytkj.cn

Go:   func add(a, b int) int
来源：http://no.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uv.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bd.yuexingan06.cn

[C14] 泛型函数
来源：http://ub.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wi.colortex.cn

PHP:  // 无泛型
来源：http://an.panjiajie.cn

JS:   // 无泛型
来源：http://ih.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yb.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ln.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://su.chemitech.net.cn

Ruby: # 无泛型
来源：http://au.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tj.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://ry.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cv.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://ry.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sl.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dp.gzmigu.cn

Java: // 无解构
来源：http://zh.nszjky.cn

Go:   // 无解构
来源：http://ne.gzmigu.cn

Ruby: a, b = pair
来源：http://dm.szsharing.cn

C#:   var (a, b) = pair;
来源：http://rj.asd995.cn

[C16] 函数 / 方法重载
来源：http://ml.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gd.shxzskj.cn

PHP:  // 无重载
来源：http://sl.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rf.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://xj.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ep.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://ct.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://pz.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://va.shxzskj.cn

================================================================================
来源：http://zc.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://et.huixiangedu.cn

================================================================================
来源：http://mg.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://ks.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gb.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hp.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://od.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gr.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://su.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://wa.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://dt.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zi.colortex.cn

[D02] 追加元素到末尾
来源：http://sl.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ej.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vt.nicolike.cn

JS:   arr.push(4);
来源：http://tq.colortex.cn

TS:   arr.push(4);
来源：http://vf.bookmarksfly.cn

Java: list.add(4);
来源：http://is.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://ew.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://ve.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://gl.nicolike.cn

[D03] 在指定位置插入元素
来源：http://ag.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://pn.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://at.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xq.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://hx.hnjuh.cn

Java: list.add(0, 0);
来源：http://sz.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yh.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mi.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://ed.huixinmuqiang.cn

[D04] 删除元素
来源：http://hn.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ym.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://po.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mu.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://bk.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mx.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yu.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ef.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qx.muxihuayi.cn

[D05] 访问与修改元素
来源：http://tl.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rx.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cx.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://em.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://wm.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://sn.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://ik.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ho.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ha.huixinmuqiang.cn

[D06] 数组长度
来源：http://fk.lnxyls.cn

Py:   len(arr)
来源：http://ul.shtwfgs.cn

PHP:  count($arr);
来源：http://in.huixiangedu.cn

JS:   arr.length
来源：http://bq.nicolike.cn

TS:   arr.length
来源：http://my.521024.cn

Java: list.size();
来源：http://vy.lnxyls.cn

Go:   len(arr)
来源：http://mx.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://yp.521024.cn

C#:   list.Count;
来源：http://xg.9csxet.cn

[D07] 切片 / 取子数组
来源：http://oz.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nk.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pn.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://ty.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://dy.hnjuh.cn

Java: list.subList(1, 4);
来源：http://ps.szxytkj.cn

Go:   arr[1:4]
来源：http://px.gzmigu.cn

Ruby: arr[1, 3]
来源：http://pp.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://zv.huixiangedu.cn

[D08] 合并两个数组
来源：http://et.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://tz.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://fy.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zs.panjiajie.cn

TS:   [...a, ...b];
来源：http://jm.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oh.asd995.cn

Go:   append(a, b...)
来源：http://li.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://aw.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://yh.521024.cn

[D09] 排序（升序）
来源：http://oc.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://ti.panjiajie.cn

PHP:  sort($arr);
来源：http://qi.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rs.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zj.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dt.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ax.huixinmuqiang.cn

Ruby: arr.sort
来源：http://wu.shtwfgs.cn

C#:   list.Sort();
来源：http://ne.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ud.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cz.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ua.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yh.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vk.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uo.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kh.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tp.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qc.panjiajie.cn

[D11] 反转数组
来源：http://mf.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pd.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://dl.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ic.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://rv.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://qg.colortex.cn

Go:   slices.Reverse(arr)
来源：http://ku.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://pj.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://gm.nicolike.cn

[D12] 查找元素下标
来源：http://su.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://pw.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lf.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fb.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jw.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vt.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://lf.szsharing.cn

Ruby: arr.index(x)
来源：http://gg.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://it.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://gk.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ws.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tg.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://nm.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://cg.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aw.wgjwhj.cn


<!-- 参考信息 -->