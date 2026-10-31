代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://xm.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://ni.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fp.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pk.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ra.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oh.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://hv.haigaiapp.cn

Py:   a and b or not c
来源：http://qf.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://uh.muxihuayi.cn

JS:   a && b || !c
来源：http://cv.panjiajie.cn

TS:   a && b || !c
来源：http://ek.bjjhwx.cn

Java: a && b || !c
来源：http://qe.bookmarksfly.cn

Go:   a && b || !c
来源：http://ky.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://yn.newstarts.cn

C#:   a && b || !c
来源：http://bw.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wy.szxytkj.cn

Py:   if not data: return
来源：http://io.521024.cn

PHP:  if (!$data) { return; }
来源：http://wx.szxytkj.cn

JS:   if (!data) return;
来源：http://sn.huixiangedu.cn

TS:   if (!data) return;
来源：http://ji.asd995.cn

Java: if (data == null) return;
来源：http://rs.huanxung.cn

Go:   if data == nil { return }
来源：http://co.hnjuh.cn

Ruby: return if data.nil?
来源：http://dr.nicolike.cn

C#:   if (data == null) return;
来源：http://ln.yuntaijiaju.cn

================================================================================
来源：http://gf.bookmarksfly.cn

C. 函数与作用域
来源：http://uv.9csxet.cn

================================================================================
来源：http://lc.jctech888.com.cn

[C01] 定义函数
来源：http://tq.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://ee.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gk.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://cd.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qx.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gc.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xz.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://ue.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mf.bjjhwx.cn

[C02] 默认参数
来源：http://bm.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://te.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dz.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://lk.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://in.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hx.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://it.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://sa.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://mi.bjjhwx.cn

[C03] 可变参数
来源：http://lv.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://xd.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://my.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lb.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yo.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qv.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hh.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rv.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nb.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://av.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sk.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bu.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ql.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wo.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://qn.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://he.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://kr.521024.cn

C#:   f(a: 1, b: 2)
来源：http://xz.yuexingan06.cn

[C05] 返回多个值
来源：http://ev.wgjwhj.cn

Py:   return a, b
来源：http://fa.newstarts.cn

PHP:  return [$a, $b];
来源：http://pt.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nu.nicolike.cn

TS:   return { a, b };
来源：http://ur.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dq.jctech888.com.cn

Go:   return a, b
来源：http://qt.hnjuh.cn

Ruby: return a, b
来源：http://up.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://xk.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://mz.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://fl.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://du.521024.cn

JS:   const square = x => x * x;
来源：http://dn.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://za.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ss.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://no.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://ac.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mf.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://lb.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yb.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xj.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kx.hnjuh.cn

TS:   arr.map(String)
来源：http://an.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ef.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tb.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://lu.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gb.szsharing.cn

[C08] 闭包
来源：http://hp.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bs.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://km.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aq.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yy.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jy.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hh.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wh.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mz.haigaiapp.cn

[C09] 递归
来源：http://gf.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xt.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fq.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cp.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fd.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jt.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pk.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dh.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ts.hnjuh.cn

[C10] 变量作用域
来源：http://um.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ov.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nm.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xz.lnxyls.cn

TS:   同 JS
来源：http://ob.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://wv.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://gr.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yx.jianghongdianzi.cn

C#:   块级作用域
来源：http://bn.bjjhwx.cn

[C11] 模块导入与导出
来源：http://nf.shtwfgs.cn

Py:   from module import func
来源：http://ll.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cp.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://un.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gq.asd995.cn

Java: import java.util.List;
来源：http://oa.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hu.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://zn.yuntaijiaju.cn

C#:   using System.Text;
来源：http://th.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://kv.521024.cn

Py:   (lambda: print("run"))()
来源：http://cn.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://fd.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://qj.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://pv.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kt.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://wp.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://py.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fv.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://bf.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sn.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kj.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lj.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iy.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://go.nszjky.cn

Go:   func add(a, b int) int
来源：http://hn.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ze.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dl.jianghongdianzi.cn

[C14] 泛型函数
来源：http://wo.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gw.colortex.cn

PHP:  // 无泛型
来源：http://ej.shxzukj.cn

JS:   // 无泛型
来源：http://ar.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pt.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jo.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pu.shxzskj.cn

Ruby: # 无泛型
来源：http://hd.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xc.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://yy.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jy.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://gg.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vl.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://af.panjiajie.cn

Java: // 无解构
来源：http://fu.szsharing.cn

Go:   // 无解构
来源：http://rs.huanxung.cn

Ruby: a, b = pair
来源：http://nm.nicolike.cn

C#:   var (a, b) = pair;
来源：http://pw.521024.cn

[C16] 函数 / 方法重载
来源：http://jp.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ba.bookmarksfly.cn

PHP:  // 无重载
来源：http://ix.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zx.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://nb.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pk.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://op.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://wg.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pc.shtwfgs.cn

================================================================================
来源：http://ta.521024.cn

D. 数组 / 列表 / 集合
来源：http://wp.shxzukj.cn

================================================================================
来源：http://ox.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://dd.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xd.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oj.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ma.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ah.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lc.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://cl.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://io.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kb.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://gm.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ht.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mr.hahajie.cn

JS:   arr.push(4);
来源：http://xf.asd995.cn

TS:   arr.push(4);
来源：http://ky.yuexingan06.cn

Java: list.add(4);
来源：http://dl.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://er.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://in.wgjwhj.cn

C#:   list.Add(4);
来源：http://lf.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://rd.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://at.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://di.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vg.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://zj.nszjky.cn

Java: list.add(0, 0);
来源：http://mo.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pi.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wv.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://nz.bookmarksfly.cn

[D04] 删除元素
来源：http://is.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pe.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pc.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jv.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://qf.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://my.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ql.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yl.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jg.szxytkj.cn

[D05] 访问与修改元素
来源：http://yw.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yy.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gx.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://az.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://fm.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://tc.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://of.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cl.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ay.hnjuh.cn

[D06] 数组长度
来源：http://cs.huixinmuqiang.cn

Py:   len(arr)
来源：http://nn.9csxet.cn

PHP:  count($arr);
来源：http://va.jianghongdianzi.cn

JS:   arr.length
来源：http://cj.hahajie.cn

TS:   arr.length
来源：http://cj.wgjwhj.cn

Java: list.size();
来源：http://ng.521024.cn

Go:   len(arr)
来源：http://sp.asd995.cn

Ruby: arr.length; arr.size
来源：http://qd.huanxung.cn

C#:   list.Count;
来源：http://fm.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://ks.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gi.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vn.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://se.asd995.cn

TS:   arr.slice(1, 4);
来源：http://mv.asd995.cn

Java: list.subList(1, 4);
来源：http://cs.lnxyls.cn

Go:   arr[1:4]
来源：http://po.colortex.cn

Ruby: arr[1, 3]
来源：http://wr.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://ah.colortex.cn

[D08] 合并两个数组
来源：http://ko.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://mh.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://oq.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oc.shxzukj.cn

TS:   [...a, ...b];
来源：http://mj.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zu.shxzukj.cn

Go:   append(a, b...)
来源：http://lb.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://rh.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://hh.shxzskj.cn

[D09] 排序（升序）
来源：http://az.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://md.huixiangedu.cn

PHP:  sort($arr);
来源：http://dn.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pk.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sz.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vj.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mc.hnjuh.cn

Ruby: arr.sort
来源：http://fh.colortex.cn

C#:   list.Sort();
来源：http://un.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zq.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mz.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lw.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tw.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tk.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cf.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bb.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zk.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ic.asd995.cn

[D11] 反转数组
来源：http://el.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tu.szsharing.cn

PHP:  array_reverse($arr);
来源：http://js.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fe.nszjky.cn

TS:   [...arr].reverse();
来源：http://ai.shxzukj.cn

Java: Collections.reverse(list);
来源：http://sx.asd995.cn

Go:   slices.Reverse(arr)
来源：http://me.panjiajie.cn

Ruby: arr.reverse
来源：http://eg.jctech888.com.cn

C#:   list.Reverse();
来源：http://sy.chemitech.net.cn

[D12] 查找元素下标
来源：http://as.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://fh.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kb.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ec.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mz.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iv.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://sx.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://iv.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://fp.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://bf.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hr.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zh.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://wo.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://dp.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gu.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lj.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sj.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vz.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://vl.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ih.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nr.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://gz.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://ha.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ay.shxzskj.cn

Go:   // 手写循环
来源：http://qp.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vh.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oz.szsharing.cn


<!-- 参考信息 -->