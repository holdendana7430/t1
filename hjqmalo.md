代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://na.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vj.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ir.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://at.huanxung.cn

[B13] 判断是否为数字
来源：http://uo.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://fe.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://gd.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iy.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ti.yuntaijiaju.cn

Java: x instanceof Number
来源：http://mg.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dh.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://mp.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://ud.newstarts.cn

[B14] 判断值是否在集合内
来源：http://eq.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oh.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://us.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://xt.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://wc.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sn.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ot.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dk.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ew.szxytkj.cn

[B15] 布尔运算与取反
来源：http://gz.hnjuh.cn

Py:   a and b or not c
来源：http://hm.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://te.jctech888.com.cn

JS:   a && b || !c
来源：http://ez.gzmigu.cn

TS:   a && b || !c
来源：http://jj.lnxyls.cn

Java: a && b || !c
来源：http://rm.szxytkj.cn

Go:   a && b || !c
来源：http://fc.gzmigu.cn

Ruby: a && b || !c
来源：http://hk.newstarts.cn

C#:   a && b || !c
来源：http://ce.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://le.wgjwhj.cn

Py:   if not data: return
来源：http://uv.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://ar.shtwfgs.cn

JS:   if (!data) return;
来源：http://du.szsharing.cn

TS:   if (!data) return;
来源：http://jp.colortex.cn

Java: if (data == null) return;
来源：http://mx.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://pn.panjiajie.cn

Ruby: return if data.nil?
来源：http://in.shtwfgs.cn

C#:   if (data == null) return;
来源：http://dp.szxytkj.cn

================================================================================
来源：http://ao.huanxung.cn

C. 函数与作用域
来源：http://gf.nicolike.cn

================================================================================
来源：http://yr.huanxung.cn

[C01] 定义函数
来源：http://ey.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://eg.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zk.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ge.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vo.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lr.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jv.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://al.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nk.lnxyls.cn

[C02] 默认参数
来源：http://qz.asd995.cn

Py:   def greet(name="World"): return name
来源：http://ed.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fo.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://dy.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ln.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sl.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rx.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://ym.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://yx.lnxyls.cn

[C03] 可变参数
来源：http://db.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://sk.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oy.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cj.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uc.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jj.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jd.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wt.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rw.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://gd.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hr.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ia.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sq.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ft.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://wg.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://iz.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://jg.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://wu.haigaiapp.cn

[C05] 返回多个值
来源：http://lu.yuntaijiaju.cn

Py:   return a, b
来源：http://da.nicolike.cn

PHP:  return [$a, $b];
来源：http://sd.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ah.chemitech.net.cn

TS:   return { a, b };
来源：http://dy.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xl.nszjky.cn

Go:   return a, b
来源：http://ci.bookmarksfly.cn

Ruby: return a, b
来源：http://of.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://td.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://md.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://lv.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aa.shxzskj.cn

JS:   const square = x => x * x;
来源：http://ue.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://uv.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fp.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kt.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://oe.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mx.hahajie.cn

[C07] 把函数作为参数传入
来源：http://aq.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iz.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vi.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yp.bookmarksfly.cn

TS:   arr.map(String)
来源：http://lv.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sp.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jr.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://zr.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iw.chemitech.net.cn

[C08] 闭包
来源：http://eo.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oy.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://th.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cm.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rd.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nh.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tz.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://co.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ee.nicolike.cn

[C09] 递归
来源：http://ng.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qk.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kx.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mv.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qa.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qk.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ev.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://un.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ol.yuntaijiaju.cn

[C10] 变量作用域
来源：http://ax.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dj.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dv.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dc.shtwfgs.cn

TS:   同 JS
来源：http://in.szxytkj.cn

Java: 方法内为块级作用域
来源：http://wo.gzmigu.cn

Go:   花括号块级作用域
来源：http://xv.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qn.jianghongdianzi.cn

C#:   块级作用域
来源：http://gb.huanxung.cn

[C11] 模块导入与导出
来源：http://nx.szsharing.cn

Py:   from module import func
来源：http://ch.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qx.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ax.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sp.shxzukj.cn

Java: import java.util.List;
来源：http://cy.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xq.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://bu.gzmigu.cn

C#:   using System.Text;
来源：http://hb.521024.cn

[C12] 立即执行函数 IIFE
来源：http://sm.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://wd.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://pw.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://iv.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://ba.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sh.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://qz.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://ly.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jx.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://hc.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ez.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://am.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mf.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ex.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ts.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://tz.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cr.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gg.haigaiapp.cn

[C14] 泛型函数
来源：http://bv.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ai.9csxet.cn

PHP:  // 无泛型
来源：http://he.nszjky.cn

JS:   // 无泛型
来源：http://uv.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yy.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hx.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ct.9csxet.cn

Ruby: # 无泛型
来源：http://xz.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mg.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://rv.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wm.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://fv.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qz.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ps.gzmigu.cn

Java: // 无解构
来源：http://sm.huixinmuqiang.cn

Go:   // 无解构
来源：http://io.newstarts.cn

Ruby: a, b = pair
来源：http://mx.hahajie.cn

C#:   var (a, b) = pair;
来源：http://kn.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://ri.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yr.panjiajie.cn

PHP:  // 无重载
来源：http://bt.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jg.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://dg.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xq.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://ry.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://kf.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mg.nszjky.cn

================================================================================
来源：http://my.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://wp.muxihuayi.cn

================================================================================
来源：http://qt.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://vw.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cp.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pd.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wf.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pw.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ep.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://xr.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://bh.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lg.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://zj.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fj.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cb.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://jd.521024.cn

TS:   arr.push(4);
来源：http://yh.newstarts.cn

Java: list.add(4);
来源：http://ky.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://xl.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://wn.yuexingan06.cn

C#:   list.Add(4);
来源：http://yc.nszjky.cn

[D03] 在指定位置插入元素
来源：http://bm.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://cp.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vh.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lr.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://uw.szsharing.cn

Java: list.add(0, 0);
来源：http://aj.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kk.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xb.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://xp.yuexingan06.cn

[D04] 删除元素
来源：http://db.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://au.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qw.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ga.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://fp.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fh.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ao.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bn.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uf.jctech888.com.cn

[D05] 访问与修改元素
来源：http://yf.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vk.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bp.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zc.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://tc.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://wv.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://ku.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ie.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://px.shtwfgs.cn

[D06] 数组长度
来源：http://gr.yuexingan06.cn

Py:   len(arr)
来源：http://ey.nszjky.cn

PHP:  count($arr);
来源：http://zo.shxzskj.cn

JS:   arr.length
来源：http://zs.huanxung.cn

TS:   arr.length
来源：http://rk.huanxung.cn

Java: list.size();
来源：http://qy.panjiajie.cn

Go:   len(arr)
来源：http://yu.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://xd.huixinmuqiang.cn

C#:   list.Count;
来源：http://or.nszjky.cn

[D07] 切片 / 取子数组
来源：http://mh.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zh.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aj.521024.cn

JS:   arr.slice(1, 4);
来源：http://ne.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://wc.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://yo.szsharing.cn

Go:   arr[1:4]
来源：http://sb.shxzukj.cn

Ruby: arr[1, 3]
来源：http://bh.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://am.9csxet.cn

[D08] 合并两个数组
来源：http://xh.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://kn.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://km.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pt.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://ws.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yh.jctech888.com.cn

Go:   append(a, b...)
来源：http://bv.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://qm.521024.cn

C#:   a.Concat(b).ToList()
来源：http://wj.muxihuayi.cn

[D09] 排序（升序）
来源：http://rg.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://fc.haigaiapp.cn

PHP:  sort($arr);
来源：http://yv.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gz.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ae.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jt.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vu.jctech888.com.cn

Ruby: arr.sort
来源：http://gy.szsharing.cn

C#:   list.Sort();
来源：http://ig.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oq.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ym.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vn.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sv.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ju.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ws.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sx.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tw.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://er.newstarts.cn

[D11] 反转数组
来源：http://tt.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wm.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://vd.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mt.asd995.cn

TS:   [...arr].reverse();
来源：http://ou.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://vn.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://ml.szsharing.cn

Ruby: arr.reverse
来源：http://uk.szsharing.cn

C#:   list.Reverse();
来源：http://vi.nicolike.cn

[D12] 查找元素下标
来源：http://zl.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://ky.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ed.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ys.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qc.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nx.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://vp.chemitech.net.cn

Ruby: arr.index(x)
来源：http://mc.9csxet.cn

C#:   list.IndexOf(x);
来源：http://le.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://om.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yu.jianghongdianzi.cn


<!-- 参考信息 -->