代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ei.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://md.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ey.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ae.521024.cn

[B13] 判断是否为数字
来源：http://ua.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://mr.521024.cn

PHP:  is_numeric($x)
来源：http://eh.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wp.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fy.bjjhwx.cn

Java: x instanceof Number
来源：http://jt.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zw.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://zd.panjiajie.cn

C#:   x is int or double or decimal
来源：http://uv.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://ps.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hx.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://li.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://vq.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://on.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ft.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ci.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cf.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nd.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://yo.gzmigu.cn

Py:   a and b or not c
来源：http://ml.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://uj.szsharing.cn

JS:   a && b || !c
来源：http://cx.shtwfgs.cn

TS:   a && b || !c
来源：http://vi.muxihuayi.cn

Java: a && b || !c
来源：http://cv.hahajie.cn

Go:   a && b || !c
来源：http://zz.shxzukj.cn

Ruby: a && b || !c
来源：http://rp.lnxyls.cn

C#:   a && b || !c
来源：http://yu.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yf.hnjuh.cn

Py:   if not data: return
来源：http://nx.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://rp.gzmigu.cn

JS:   if (!data) return;
来源：http://fs.521024.cn

TS:   if (!data) return;
来源：http://dx.nszjky.cn

Java: if (data == null) return;
来源：http://ja.bjjhwx.cn

Go:   if data == nil { return }
来源：http://gw.jctech888.com.cn

Ruby: return if data.nil?
来源：http://ei.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://la.9csxet.cn

================================================================================
来源：http://tp.huixinmuqiang.cn

C. 函数与作用域
来源：http://tg.szsharing.cn

================================================================================
来源：http://nd.yuntaijiaju.cn

[C01] 定义函数
来源：http://qi.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://cr.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zj.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://rx.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ul.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kf.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ko.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://zc.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hi.shxzukj.cn

[C02] 默认参数
来源：http://sf.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://ff.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wx.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://sy.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hx.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wj.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fd.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://bt.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://xf.newstarts.cn

[C03] 可变参数
来源：http://xl.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://gz.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xc.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mx.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vd.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kw.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tx.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://du.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kc.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ef.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zr.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qu.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mg.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://el.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://ur.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ng.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://so.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://mh.szxytkj.cn

[C05] 返回多个值
来源：http://lj.asd995.cn

Py:   return a, b
来源：http://jw.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://wa.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sc.yuntaijiaju.cn

TS:   return { a, b };
来源：http://dk.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vs.newstarts.cn

Go:   return a, b
来源：http://lb.muxihuayi.cn

Ruby: return a, b
来源：http://bi.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://tk.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://wq.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://jp.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pp.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://gm.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://gx.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://px.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mi.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://gs.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ze.521024.cn

[C07] 把函数作为参数传入
来源：http://vz.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fa.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bg.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kk.shtwfgs.cn

TS:   arr.map(String)
来源：http://fr.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dh.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iv.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://oy.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eo.huanxung.cn

[C08] 闭包
来源：http://tp.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vw.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bj.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dz.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sm.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gi.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ww.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nd.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qx.jianghongdianzi.cn

[C09] 递归
来源：http://ae.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wo.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ee.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jq.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pk.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oo.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qt.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cp.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wu.haigaiapp.cn

[C10] 变量作用域
来源：http://sn.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://km.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eb.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ic.shxzukj.cn

TS:   同 JS
来源：http://ct.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://fb.lnxyls.cn

Go:   花括号块级作用域
来源：http://at.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tm.hnjuh.cn

C#:   块级作用域
来源：http://yh.jctech888.com.cn

[C11] 模块导入与导出
来源：http://ya.haigaiapp.cn

Py:   from module import func
来源：http://zp.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pe.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cv.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hp.hahajie.cn

Java: import java.util.List;
来源：http://ev.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eg.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://jl.yuexingan06.cn

C#:   using System.Text;
来源：http://yw.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://eo.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://um.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://rt.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://kp.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://lb.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cx.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://bi.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://pg.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gp.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://om.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://in.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tv.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rt.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vp.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yi.hahajie.cn

Go:   func add(a, b int) int
来源：http://ob.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://co.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oo.szxytkj.cn

[C14] 泛型函数
来源：http://dc.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ut.haigaiapp.cn

PHP:  // 无泛型
来源：http://bf.shxzukj.cn

JS:   // 无泛型
来源：http://iy.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ob.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kh.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hr.muxihuayi.cn

Ruby: # 无泛型
来源：http://nf.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jw.nszjky.cn

[C15] 解构 / 展开参数
来源：http://np.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yc.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://hw.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wq.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ib.shtwfgs.cn

Java: // 无解构
来源：http://pj.shxzskj.cn

Go:   // 无解构
来源：http://hu.muxihuayi.cn

Ruby: a, b = pair
来源：http://bf.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://hj.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://pw.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://er.panjiajie.cn

PHP:  // 无重载
来源：http://lc.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lu.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://ct.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://is.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://cx.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://nt.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nw.jianghongdianzi.cn

================================================================================
来源：http://dy.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ae.shtwfgs.cn

================================================================================
来源：http://mv.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://ee.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dk.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ug.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ei.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zc.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ex.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://im.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://of.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xl.colortex.cn

[D02] 追加元素到末尾
来源：http://mu.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pw.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pm.521024.cn

JS:   arr.push(4);
来源：http://vg.hahajie.cn

TS:   arr.push(4);
来源：http://fe.huixinmuqiang.cn

Java: list.add(4);
来源：http://qp.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://cb.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://mb.huanxung.cn

C#:   list.Add(4);
来源：http://da.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://ww.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://xo.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yc.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://af.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://ti.colortex.cn

Java: list.add(0, 0);
来源：http://he.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kx.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rm.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://tt.huixiangedu.cn

[D04] 删除元素
来源：http://yb.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://am.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://th.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uv.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://pz.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nz.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jc.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nl.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dw.hahajie.cn

[D05] 访问与修改元素
来源：http://wx.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uy.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dy.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qs.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://bx.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ru.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://aq.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bu.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://et.muxihuayi.cn

[D06] 数组长度
来源：http://ez.nszjky.cn

Py:   len(arr)
来源：http://ts.nicolike.cn

PHP:  count($arr);
来源：http://ih.newstarts.cn

JS:   arr.length
来源：http://ea.huanxung.cn

TS:   arr.length
来源：http://ir.szxytkj.cn

Java: list.size();
来源：http://ff.szsharing.cn

Go:   len(arr)
来源：http://ry.nicolike.cn

Ruby: arr.length; arr.size
来源：http://dl.huixinmuqiang.cn

C#:   list.Count;
来源：http://ql.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://zd.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gd.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pe.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://qu.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://rb.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://lq.9csxet.cn

Go:   arr[1:4]
来源：http://jw.huanxung.cn

Ruby: arr[1, 3]
来源：http://cy.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://dq.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://yi.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://wt.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://in.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ew.colortex.cn

TS:   [...a, ...b];
来源：http://rd.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mh.shtwfgs.cn

Go:   append(a, b...)
来源：http://qi.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://ne.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://tg.newstarts.cn

[D09] 排序（升序）
来源：http://ls.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://rw.haigaiapp.cn

PHP:  sort($arr);
来源：http://ye.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tw.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wd.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aw.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vp.colortex.cn

Ruby: arr.sort
来源：http://ha.nicolike.cn

C#:   list.Sort();
来源：http://oa.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bz.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lm.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qf.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qe.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lr.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dw.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jg.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ah.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rn.nszjky.cn

[D11] 反转数组
来源：http://by.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yb.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://ko.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://si.521024.cn

TS:   [...arr].reverse();
来源：http://ib.gzmigu.cn

Java: Collections.reverse(list);
来源：http://xy.521024.cn

Go:   slices.Reverse(arr)
来源：http://lo.lnxyls.cn

Ruby: arr.reverse
来源：http://eq.yuexingan06.cn

C#:   list.Reverse();
来源：http://om.gzmigu.cn

[D12] 查找元素下标
来源：http://us.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://wn.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rg.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xo.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fn.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gd.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://mp.colortex.cn

Ruby: arr.index(x)
来源：http://up.9csxet.cn

C#:   list.IndexOf(x);
来源：http://ge.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://im.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ft.huixinmuqiang.cn


<!-- 参考信息 -->