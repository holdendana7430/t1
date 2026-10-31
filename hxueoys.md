代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://ip.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yh.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://ep.wgjwhj.cn

Py:   a and b or not c
来源：http://ya.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://zh.yuexingan06.cn

JS:   a && b || !c
来源：http://yo.muxihuayi.cn

TS:   a && b || !c
来源：http://su.hahajie.cn

Java: a && b || !c
来源：http://nx.hahajie.cn

Go:   a && b || !c
来源：http://dl.asd995.cn

Ruby: a && b || !c
来源：http://eo.nszjky.cn

C#:   a && b || !c
来源：http://uy.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jo.yuexingan06.cn

Py:   if not data: return
来源：http://ao.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://gw.bjjhwx.cn

JS:   if (!data) return;
来源：http://jg.jctech888.com.cn

TS:   if (!data) return;
来源：http://ca.hahajie.cn

Java: if (data == null) return;
来源：http://di.9csxet.cn

Go:   if data == nil { return }
来源：http://eo.chemitech.net.cn

Ruby: return if data.nil?
来源：http://iu.9csxet.cn

C#:   if (data == null) return;
来源：http://zm.shtwfgs.cn

================================================================================
来源：http://iy.bookmarksfly.cn

C. 函数与作用域
来源：http://gj.asd995.cn

================================================================================
来源：http://nb.yuexingan06.cn

[C01] 定义函数
来源：http://xk.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://wz.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ps.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://ju.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iz.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fc.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gx.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://ly.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sb.9csxet.cn

[C02] 默认参数
来源：http://yb.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://iy.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gj.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://pc.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qq.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lv.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dp.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://tj.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://zt.huixinmuqiang.cn

[C03] 可变参数
来源：http://ze.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://bv.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rc.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eu.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ub.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dk.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mg.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zl.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nc.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://ol.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://on.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lp.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lm.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jf.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://ba.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://iw.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://vy.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://ig.hnjuh.cn

[C05] 返回多个值
来源：http://jr.jianghongdianzi.cn

Py:   return a, b
来源：http://ni.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://gc.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tq.haigaiapp.cn

TS:   return { a, b };
来源：http://mi.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lc.jianghongdianzi.cn

Go:   return a, b
来源：http://zk.huixiangedu.cn

Ruby: return a, b
来源：http://wj.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://sy.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://eq.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://qr.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xh.szsharing.cn

JS:   const square = x => x * x;
来源：http://we.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ty.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dy.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://is.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://ic.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wy.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://ky.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://if.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://og.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bb.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://dz.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hf.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ku.521024.cn

Ruby: arr.map(&:upcase)
来源：http://ar.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wi.yuntaijiaju.cn

[C08] 闭包
来源：http://if.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jh.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rd.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ek.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tr.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dr.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hg.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jc.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oj.jianghongdianzi.cn

[C09] 递归
来源：http://ye.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://va.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xb.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qf.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tm.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zb.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pg.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xw.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://km.newstarts.cn

[C10] 变量作用域
来源：http://bx.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ii.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gv.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fu.wgjwhj.cn

TS:   同 JS
来源：http://ev.9csxet.cn

Java: 方法内为块级作用域
来源：http://tz.bjjhwx.cn

Go:   花括号块级作用域
来源：http://qt.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vg.9csxet.cn

C#:   块级作用域
来源：http://rn.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://gv.colortex.cn

Py:   from module import func
来源：http://im.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mm.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ef.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ze.yuntaijiaju.cn

Java: import java.util.List;
来源：http://wx.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jj.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://fc.jianghongdianzi.cn

C#:   using System.Text;
来源：http://lm.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://eo.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://wv.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://qb.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://ag.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ul.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kp.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://xc.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://bt.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ya.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://ya.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sd.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ty.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ra.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eb.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rj.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://bd.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tn.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://be.wgjwhj.cn

[C14] 泛型函数
来源：http://ca.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uw.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://ed.bjjhwx.cn

JS:   // 无泛型
来源：http://md.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://or.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rj.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sz.gzmigu.cn

Ruby: # 无泛型
来源：http://au.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xa.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://yn.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zi.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://du.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wp.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qp.huixinmuqiang.cn

Java: // 无解构
来源：http://ur.nszjky.cn

Go:   // 无解构
来源：http://sc.haigaiapp.cn

Ruby: a, b = pair
来源：http://qd.colortex.cn

C#:   var (a, b) = pair;
来源：http://ti.9csxet.cn

[C16] 函数 / 方法重载
来源：http://kn.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ct.yuntaijiaju.cn

PHP:  // 无重载
来源：http://xs.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kn.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://xk.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hj.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://mg.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://tu.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ym.lnxyls.cn

================================================================================
来源：http://su.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://jr.nicolike.cn

================================================================================
来源：http://sj.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://rf.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sg.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hy.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oh.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fn.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yi.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://rp.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://pl.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yu.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://qs.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dg.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qc.asd995.cn

JS:   arr.push(4);
来源：http://qq.521024.cn

TS:   arr.push(4);
来源：http://ll.hahajie.cn

Java: list.add(4);
来源：http://ce.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://ry.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://cp.shtwfgs.cn

C#:   list.Add(4);
来源：http://eg.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://rw.asd995.cn

Py:   arr.insert(0, 0)
来源：http://pz.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kc.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hr.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://wd.wgjwhj.cn

Java: list.add(0, 0);
来源：http://ef.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://id.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zz.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://dz.newstarts.cn

[D04] 删除元素
来源：http://jt.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xy.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pg.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kw.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://yb.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ka.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qt.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://au.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mf.9csxet.cn

[D05] 访问与修改元素
来源：http://pf.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xo.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uk.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zd.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://zh.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://hc.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://nd.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tj.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kp.jctech888.com.cn

[D06] 数组长度
来源：http://nz.szsharing.cn

Py:   len(arr)
来源：http://xq.wgjwhj.cn

PHP:  count($arr);
来源：http://tx.shtwfgs.cn

JS:   arr.length
来源：http://mg.huixiangedu.cn

TS:   arr.length
来源：http://aa.haigaiapp.cn

Java: list.size();
来源：http://cx.huixiangedu.cn

Go:   len(arr)
来源：http://os.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://ba.nicolike.cn

C#:   list.Count;
来源：http://dc.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://vf.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mf.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xh.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://ps.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://lf.hnjuh.cn

Java: list.subList(1, 4);
来源：http://wm.hnjuh.cn

Go:   arr[1:4]
来源：http://iz.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://co.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://dr.521024.cn

[D08] 合并两个数组
来源：http://us.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://gl.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://cx.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fg.wgjwhj.cn

TS:   [...a, ...b];
来源：http://rz.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ia.szxytkj.cn

Go:   append(a, b...)
来源：http://oq.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://gy.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://vj.asd995.cn

[D09] 排序（升序）
来源：http://ra.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zo.jctech888.com.cn

PHP:  sort($arr);
来源：http://bp.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nt.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wg.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ww.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rs.huixinmuqiang.cn

Ruby: arr.sort
来源：http://nu.hnjuh.cn

C#:   list.Sort();
来源：http://ux.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mj.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kq.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aq.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ds.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pq.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ra.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yp.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qc.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bj.hnjuh.cn

[D11] 反转数组
来源：http://cq.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://al.nszjky.cn

PHP:  array_reverse($arr);
来源：http://ln.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://la.9csxet.cn

TS:   [...arr].reverse();
来源：http://rv.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://gt.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://yj.muxihuayi.cn

Ruby: arr.reverse
来源：http://qf.shxzukj.cn

C#:   list.Reverse();
来源：http://cl.lnxyls.cn

[D12] 查找元素下标
来源：http://fo.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://cs.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kf.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://do.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kl.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gp.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://fu.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://ou.huanxung.cn

C#:   list.IndexOf(x);
来源：http://sc.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://vk.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ny.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ut.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://hi.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://rl.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kl.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iv.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dk.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hr.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://it.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nr.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uw.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://sf.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://xb.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vb.nicolike.cn

Go:   // 手写循环
来源：http://hb.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fx.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cs.bjjhwx.cn

[D15] 去重
来源：http://ma.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ny.gzmigu.cn

PHP:  array_unique($arr);
来源：http://vi.hahajie.cn

JS:   [...new Set(arr)]
来源：http://mg.hahajie.cn


<!-- 参考信息 -->