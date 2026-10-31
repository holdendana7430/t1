代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://ic.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wx.nszjky.cn

[B15] 布尔运算与取反
来源：http://io.huanxung.cn

Py:   a and b or not c
来源：http://wt.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://cg.huixinmuqiang.cn

JS:   a && b || !c
来源：http://dj.jctech888.com.cn

TS:   a && b || !c
来源：http://gi.chemitech.net.cn

Java: a && b || !c
来源：http://rn.huixinmuqiang.cn

Go:   a && b || !c
来源：http://hj.shtwfgs.cn

Ruby: a && b || !c
来源：http://aa.jctech888.com.cn

C#:   a && b || !c
来源：http://ty.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xr.gzmigu.cn

Py:   if not data: return
来源：http://dw.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://tn.haigaiapp.cn

JS:   if (!data) return;
来源：http://ud.yuexingan06.cn

TS:   if (!data) return;
来源：http://dk.521024.cn

Java: if (data == null) return;
来源：http://mq.jctech888.com.cn

Go:   if data == nil { return }
来源：http://jk.gzmigu.cn

Ruby: return if data.nil?
来源：http://kf.newstarts.cn

C#:   if (data == null) return;
来源：http://iu.colortex.cn

================================================================================
来源：http://ql.hnjuh.cn

C. 函数与作用域
来源：http://fs.panjiajie.cn

================================================================================
来源：http://bf.wgjwhj.cn

[C01] 定义函数
来源：http://ih.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://rf.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hd.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://sj.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ck.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rp.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lw.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://wk.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://je.szsharing.cn

[C02] 默认参数
来源：http://di.521024.cn

Py:   def greet(name="World"): return name
来源：http://dm.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jw.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://nc.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bk.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yu.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://if.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://za.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ca.huanxung.cn

[C03] 可变参数
来源：http://wy.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://wv.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kn.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kx.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kn.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pl.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cm.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kl.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jn.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://ih.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dh.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bl.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ht.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kx.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://yb.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://mz.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://nj.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://bl.bookmarksfly.cn

[C05] 返回多个值
来源：http://nc.yuntaijiaju.cn

Py:   return a, b
来源：http://mp.szsharing.cn

PHP:  return [$a, $b];
来源：http://ie.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dd.huixiangedu.cn

TS:   return { a, b };
来源：http://up.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sq.nicolike.cn

Go:   return a, b
来源：http://oe.9csxet.cn

Ruby: return a, b
来源：http://fi.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://hw.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://zp.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://ph.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cl.colortex.cn

JS:   const square = x => x * x;
来源：http://bn.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://zz.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ji.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ht.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://tr.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cb.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://vm.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ep.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eg.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ei.asd995.cn

TS:   arr.map(String)
来源：http://dc.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ta.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zb.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://ua.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zq.nszjky.cn

[C08] 闭包
来源：http://hd.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jv.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qj.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xt.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gc.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zc.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://no.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ho.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mb.panjiajie.cn

[C09] 递归
来源：http://bj.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bb.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ub.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qi.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ub.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lb.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rh.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hv.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wc.wgjwhj.cn

[C10] 变量作用域
来源：http://hy.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wf.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mc.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nn.shxzukj.cn

TS:   同 JS
来源：http://ig.szxytkj.cn

Java: 方法内为块级作用域
来源：http://jf.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://hn.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cn.huanxung.cn

C#:   块级作用域
来源：http://qi.haigaiapp.cn

[C11] 模块导入与导出
来源：http://ae.shxzskj.cn

Py:   from module import func
来源：http://nj.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ru.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iw.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fw.shtwfgs.cn

Java: import java.util.List;
来源：http://ms.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://is.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://hi.yuntaijiaju.cn

C#:   using System.Text;
来源：http://tf.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://cn.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://ux.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://nq.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://xh.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://rs.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://el.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://nb.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://wd.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://td.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://kf.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ns.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jr.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lk.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tk.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fs.asd995.cn

Go:   func add(a, b int) int
来源：http://yv.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yx.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fd.muxihuayi.cn

[C14] 泛型函数
来源：http://eb.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ye.9csxet.cn

PHP:  // 无泛型
来源：http://nx.haigaiapp.cn

JS:   // 无泛型
来源：http://tg.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lc.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xe.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jt.yuexingan06.cn

Ruby: # 无泛型
来源：http://tm.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ki.521024.cn

[C15] 解构 / 展开参数
来源：http://dq.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jj.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://ic.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ia.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://up.521024.cn

Java: // 无解构
来源：http://bt.nicolike.cn

Go:   // 无解构
来源：http://bx.colortex.cn

Ruby: a, b = pair
来源：http://pe.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://am.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://bm.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zy.bjjhwx.cn

PHP:  // 无重载
来源：http://vc.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xg.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://ci.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pt.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://dw.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://ei.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://th.hahajie.cn

================================================================================
来源：http://fc.521024.cn

D. 数组 / 列表 / 集合
来源：http://di.panjiajie.cn

================================================================================
来源：http://ss.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://vv.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bs.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ux.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vb.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bn.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sy.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://mh.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://ok.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rc.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://ng.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lj.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ka.bjjhwx.cn

JS:   arr.push(4);
来源：http://ht.lnxyls.cn

TS:   arr.push(4);
来源：http://tl.asd995.cn

Java: list.add(4);
来源：http://ov.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://cp.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://vh.hahajie.cn

C#:   list.Add(4);
来源：http://ur.newstarts.cn

[D03] 在指定位置插入元素
来源：http://go.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://ud.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nh.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iu.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://cf.shtwfgs.cn

Java: list.add(0, 0);
来源：http://br.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xf.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://na.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://he.nicolike.cn

[D04] 删除元素
来源：http://xv.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qp.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eo.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kz.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://pd.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pz.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cu.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nv.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bj.bjjhwx.cn

[D05] 访问与修改元素
来源：http://rm.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qn.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zf.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ec.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://ee.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://xb.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://cu.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yz.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pp.lnxyls.cn

[D06] 数组长度
来源：http://oj.huixinmuqiang.cn

Py:   len(arr)
来源：http://kh.bjjhwx.cn

PHP:  count($arr);
来源：http://fu.chemitech.net.cn

JS:   arr.length
来源：http://jn.huanxung.cn

TS:   arr.length
来源：http://jr.bjjhwx.cn

Java: list.size();
来源：http://xs.jianghongdianzi.cn

Go:   len(arr)
来源：http://df.huanxung.cn

Ruby: arr.length; arr.size
来源：http://bq.newstarts.cn

C#:   list.Count;
来源：http://bk.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://yu.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ve.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hv.colortex.cn

JS:   arr.slice(1, 4);
来源：http://ec.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://an.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://su.chemitech.net.cn

Go:   arr[1:4]
来源：http://wg.panjiajie.cn

Ruby: arr[1, 3]
来源：http://kt.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://wx.lnxyls.cn

[D08] 合并两个数组
来源：http://hg.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://bw.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://hj.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dp.nszjky.cn

TS:   [...a, ...b];
来源：http://zb.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fi.521024.cn

Go:   append(a, b...)
来源：http://uw.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://wr.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://va.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://is.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://vu.huanxung.cn

PHP:  sort($arr);
来源：http://ae.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://go.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yw.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sk.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rc.newstarts.cn

Ruby: arr.sort
来源：http://po.shxzukj.cn

C#:   list.Sort();
来源：http://lj.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ml.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yo.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://co.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nt.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vu.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mi.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vz.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jr.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ph.hahajie.cn

[D11] 反转数组
来源：http://qz.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://he.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://li.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rr.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://mv.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://gf.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://ws.9csxet.cn

Ruby: arr.reverse
来源：http://wt.panjiajie.cn

C#:   list.Reverse();
来源：http://em.lnxyls.cn

[D12] 查找元素下标
来源：http://qn.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://hp.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sk.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jy.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qj.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ff.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://id.haigaiapp.cn

Ruby: arr.index(x)
来源：http://ko.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://jc.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://ps.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ns.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ux.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://hd.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://to.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lz.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tb.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ha.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fq.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://ia.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rg.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kh.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://xn.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://eb.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ne.shxzukj.cn

Go:   // 手写循环
来源：http://wj.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tg.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ig.lnxyls.cn

[D15] 去重
来源：http://rs.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nu.shxzskj.cn

PHP:  array_unique($arr);
来源：http://nl.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://qe.szxytkj.cn


<!-- 参考信息 -->