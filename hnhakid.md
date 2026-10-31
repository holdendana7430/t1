代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://tg.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tj.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://we.shxzukj.cn

Py:   a and b or not c
来源：http://gy.nicolike.cn

PHP:  $a && $b || !$c
来源：http://pf.szsharing.cn

JS:   a && b || !c
来源：http://pw.huixiangedu.cn

TS:   a && b || !c
来源：http://rb.hnjuh.cn

Java: a && b || !c
来源：http://ob.szxytkj.cn

Go:   a && b || !c
来源：http://jq.chemitech.net.cn

Ruby: a && b || !c
来源：http://ec.shtwfgs.cn

C#:   a && b || !c
来源：http://py.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://og.hnjuh.cn

Py:   if not data: return
来源：http://lu.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://vh.colortex.cn

JS:   if (!data) return;
来源：http://iw.9csxet.cn

TS:   if (!data) return;
来源：http://ya.yuexingan06.cn

Java: if (data == null) return;
来源：http://zc.panjiajie.cn

Go:   if data == nil { return }
来源：http://md.9csxet.cn

Ruby: return if data.nil?
来源：http://ve.szxytkj.cn

C#:   if (data == null) return;
来源：http://mw.panjiajie.cn

================================================================================
来源：http://ab.yuntaijiaju.cn

C. 函数与作用域
来源：http://fn.shxzukj.cn

================================================================================
来源：http://us.panjiajie.cn

[C01] 定义函数
来源：http://gj.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://qe.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lw.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://se.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dc.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://df.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dq.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://tq.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zt.chemitech.net.cn

[C02] 默认参数
来源：http://it.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://dd.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ay.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://lh.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://md.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://op.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nm.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://ul.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://cm.haigaiapp.cn

[C03] 可变参数
来源：http://zm.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://zz.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://md.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mr.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fy.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tc.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hm.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zb.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ir.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://hk.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jq.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qn.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ky.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xg.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://ng.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://ky.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://rx.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://hv.huanxung.cn

[C05] 返回多个值
来源：http://qo.panjiajie.cn

Py:   return a, b
来源：http://bg.hahajie.cn

PHP:  return [$a, $b];
来源：http://qo.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ma.521024.cn

TS:   return { a, b };
来源：http://jo.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xs.huixiangedu.cn

Go:   return a, b
来源：http://td.colortex.cn

Ruby: return a, b
来源：http://sr.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://iw.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://mb.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://sn.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ux.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://fy.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://qk.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ks.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hn.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://wy.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pr.hahajie.cn

[C07] 把函数作为参数传入
来源：http://iq.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bb.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qf.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zp.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://py.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rt.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jc.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://ai.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tg.jctech888.com.cn

[C08] 闭包
来源：http://ma.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uf.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vr.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wv.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qs.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zi.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jk.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bd.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bo.szxytkj.cn

[C09] 递归
来源：http://bl.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sx.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nd.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://si.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xo.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pg.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ky.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wj.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qe.shtwfgs.cn

[C10] 变量作用域
来源：http://ou.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ml.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://au.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tn.bjjhwx.cn

TS:   同 JS
来源：http://tp.asd995.cn

Java: 方法内为块级作用域
来源：http://vo.muxihuayi.cn

Go:   花括号块级作用域
来源：http://fa.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yl.muxihuayi.cn

C#:   块级作用域
来源：http://sz.521024.cn

[C11] 模块导入与导出
来源：http://zp.asd995.cn

Py:   from module import func
来源：http://rg.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pw.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oe.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://on.yuntaijiaju.cn

Java: import java.util.List;
来源：http://nk.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://as.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://rm.shxzskj.cn

C#:   using System.Text;
来源：http://qk.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://xe.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://rm.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://wi.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://aj.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://dp.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://am.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://cd.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://zz.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yd.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://oi.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fb.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rd.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ei.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pj.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wl.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ys.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oh.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dz.jctech888.com.cn

[C14] 泛型函数
来源：http://ax.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xk.asd995.cn

PHP:  // 无泛型
来源：http://eu.hahajie.cn

JS:   // 无泛型
来源：http://cp.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xu.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yu.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tf.shxzskj.cn

Ruby: # 无泛型
来源：http://tp.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dx.szsharing.cn

[C15] 解构 / 展开参数
来源：http://ik.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://te.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://vt.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bf.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wf.521024.cn

Java: // 无解构
来源：http://id.szxytkj.cn

Go:   // 无解构
来源：http://az.chemitech.net.cn

Ruby: a, b = pair
来源：http://fo.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://pn.colortex.cn

[C16] 函数 / 方法重载
来源：http://dr.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oh.hnjuh.cn

PHP:  // 无重载
来源：http://nd.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sv.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://bv.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gf.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://pa.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://jf.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hc.jctech888.com.cn

================================================================================
来源：http://ol.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://rq.yuexingan06.cn

================================================================================
来源：http://oe.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://bj.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://se.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sz.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ow.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sx.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ar.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://zl.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://ie.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bz.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://sj.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mh.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yd.huixiangedu.cn

JS:   arr.push(4);
来源：http://ry.chemitech.net.cn

TS:   arr.push(4);
来源：http://jo.wgjwhj.cn

Java: list.add(4);
来源：http://pa.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://wp.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://wl.521024.cn

C#:   list.Add(4);
来源：http://tv.nszjky.cn

[D03] 在指定位置插入元素
来源：http://kp.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://ys.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kg.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qm.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://oy.chemitech.net.cn

Java: list.add(0, 0);
来源：http://ua.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uw.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oi.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://os.shxzskj.cn

[D04] 删除元素
来源：http://gi.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fj.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hc.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xy.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://yr.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bn.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ik.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zz.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ma.9csxet.cn

[D05] 访问与修改元素
来源：http://hv.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wj.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ed.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mf.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://vl.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://sv.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://qz.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lx.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bv.nicolike.cn

[D06] 数组长度
来源：http://ke.bjjhwx.cn

Py:   len(arr)
来源：http://ka.hnjuh.cn

PHP:  count($arr);
来源：http://no.yuntaijiaju.cn

JS:   arr.length
来源：http://zs.newstarts.cn

TS:   arr.length
来源：http://um.huixinmuqiang.cn

Java: list.size();
来源：http://ks.jianghongdianzi.cn

Go:   len(arr)
来源：http://do.9csxet.cn

Ruby: arr.length; arr.size
来源：http://wz.bjjhwx.cn

C#:   list.Count;
来源：http://zx.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://tz.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ot.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eb.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://ti.colortex.cn

TS:   arr.slice(1, 4);
来源：http://wv.9csxet.cn

Java: list.subList(1, 4);
来源：http://uf.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://id.hahajie.cn

Ruby: arr[1, 3]
来源：http://pq.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://fl.hnjuh.cn

[D08] 合并两个数组
来源：http://zk.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://da.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://uf.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yn.521024.cn

TS:   [...a, ...b];
来源：http://gt.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sy.chemitech.net.cn

Go:   append(a, b...)
来源：http://yl.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://al.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://ak.nszjky.cn

[D09] 排序（升序）
来源：http://mc.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://dq.9csxet.cn

PHP:  sort($arr);
来源：http://hx.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rz.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sp.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ct.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ic.chemitech.net.cn

Ruby: arr.sort
来源：http://bp.szxytkj.cn

C#:   list.Sort();
来源：http://ei.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mf.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xx.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://js.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uw.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kf.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gt.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yw.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gc.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gp.jianghongdianzi.cn

[D11] 反转数组
来源：http://hk.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ed.nszjky.cn

PHP:  array_reverse($arr);
来源：http://lk.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cu.newstarts.cn

TS:   [...arr].reverse();
来源：http://zj.hnjuh.cn

Java: Collections.reverse(list);
来源：http://lr.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://rb.gzmigu.cn

Ruby: arr.reverse
来源：http://ws.colortex.cn

C#:   list.Reverse();
来源：http://yj.hnjuh.cn

[D12] 查找元素下标
来源：http://th.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://cb.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sl.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cf.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ru.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ma.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://sm.hnjuh.cn

Ruby: arr.index(x)
来源：http://ln.nszjky.cn

C#:   list.IndexOf(x);
来源：http://jx.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://yc.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gn.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gd.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://gi.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://uw.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ow.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ab.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tk.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://os.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://wr.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://er.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fv.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ln.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://nz.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fc.szsharing.cn

Go:   // 手写循环
来源：http://zl.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wy.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hi.lnxyls.cn

[D15] 去重
来源：http://oa.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kg.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://tg.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://qs.colortex.cn


<!-- 参考信息 -->