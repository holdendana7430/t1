代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://tr.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yk.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://al.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://od.gzmigu.cn

[C02] 默认参数
来源：http://xn.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ul.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sb.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://di.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cv.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zq.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://en.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://op.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://gx.chemitech.net.cn

[C03] 可变参数
来源：http://hn.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://kx.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nf.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bg.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nt.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mq.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aj.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wg.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ky.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://au.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vw.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ff.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xy.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wy.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ka.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://cp.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://dy.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://pr.nszjky.cn

[C05] 返回多个值
来源：http://ok.yuexingan06.cn

Py:   return a, b
来源：http://uv.lnxyls.cn

PHP:  return [$a, $b];
来源：http://qu.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ww.szxytkj.cn

TS:   return { a, b };
来源：http://rd.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ca.haigaiapp.cn

Go:   return a, b
来源：http://mk.shxzskj.cn

Ruby: return a, b
来源：http://tb.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://dw.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://rl.nicolike.cn

Py:   square = lambda x: x * x
来源：http://jx.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xz.szxytkj.cn

JS:   const square = x => x * x;
来源：http://ay.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://bn.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zd.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tj.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://if.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gn.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://vg.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://am.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hu.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yq.wgjwhj.cn

TS:   arr.map(String)
来源：http://kx.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mf.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hr.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://uy.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iw.gzmigu.cn

[C08] 闭包
来源：http://eb.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bb.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lh.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iv.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oa.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fh.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gj.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://go.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jr.lnxyls.cn

[C09] 递归
来源：http://pk.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ij.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mh.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://no.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vo.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://js.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aq.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rb.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fg.nszjky.cn

[C10] 变量作用域
来源：http://av.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nf.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fy.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gj.nszjky.cn

TS:   同 JS
来源：http://ud.shxzukj.cn

Java: 方法内为块级作用域
来源：http://jc.asd995.cn

Go:   花括号块级作用域
来源：http://rx.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jn.szxytkj.cn

C#:   块级作用域
来源：http://cw.chemitech.net.cn

[C11] 模块导入与导出
来源：http://kf.shtwfgs.cn

Py:   from module import func
来源：http://ki.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zs.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bj.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yj.nicolike.cn

Java: import java.util.List;
来源：http://lm.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mm.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://on.gzmigu.cn

C#:   using System.Text;
来源：http://ri.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://dh.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://sj.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://wn.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://yr.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://wv.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ke.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://qr.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://zg.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://am.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://cp.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mx.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nr.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yw.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nq.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fa.hnjuh.cn

Go:   func add(a, b int) int
来源：http://dy.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zx.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gd.yuexingan06.cn

[C14] 泛型函数
来源：http://ro.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gq.szsharing.cn

PHP:  // 无泛型
来源：http://rp.colortex.cn

JS:   // 无泛型
来源：http://cy.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ok.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qe.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sp.9csxet.cn

Ruby: # 无泛型
来源：http://ss.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qh.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://cp.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vd.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://pe.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xw.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bb.jianghongdianzi.cn

Java: // 无解构
来源：http://uw.shxzskj.cn

Go:   // 无解构
来源：http://te.muxihuayi.cn

Ruby: a, b = pair
来源：http://lf.newstarts.cn

C#:   var (a, b) = pair;
来源：http://me.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://sg.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nt.hnjuh.cn

PHP:  // 无重载
来源：http://kf.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://va.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ip.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ub.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://df.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://bb.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xk.panjiajie.cn

================================================================================
来源：http://dp.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://nw.szsharing.cn

================================================================================
来源：http://mw.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://tv.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gz.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qe.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nk.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dm.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mq.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://ie.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://he.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zi.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://mp.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ir.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ra.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://ia.bookmarksfly.cn

TS:   arr.push(4);
来源：http://qa.bjjhwx.cn

Java: list.add(4);
来源：http://nr.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://ym.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://hw.huanxung.cn

C#:   list.Add(4);
来源：http://jy.huanxung.cn

[D03] 在指定位置插入元素
来源：http://xv.521024.cn

Py:   arr.insert(0, 0)
来源：http://tr.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ss.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vc.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://mw.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://nq.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yo.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://js.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://qx.szxytkj.cn

[D04] 删除元素
来源：http://yh.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uo.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mx.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ob.asd995.cn

TS:   arr.splice(0, 1);
来源：http://ds.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://po.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jr.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pi.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://td.huixiangedu.cn

[D05] 访问与修改元素
来源：http://gb.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vz.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uz.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ai.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://fn.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://dr.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://yd.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hn.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ks.yuexingan06.cn

[D06] 数组长度
来源：http://ph.gzmigu.cn

Py:   len(arr)
来源：http://mp.bookmarksfly.cn

PHP:  count($arr);
来源：http://zn.lnxyls.cn

JS:   arr.length
来源：http://ur.shxzskj.cn

TS:   arr.length
来源：http://wa.muxihuayi.cn

Java: list.size();
来源：http://uv.szxytkj.cn

Go:   len(arr)
来源：http://zb.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://ff.wgjwhj.cn

C#:   list.Count;
来源：http://ng.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://dc.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oe.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hy.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://ol.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://un.nicolike.cn

Java: list.subList(1, 4);
来源：http://gv.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://ei.hnjuh.cn

Ruby: arr[1, 3]
来源：http://lv.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://kl.wgjwhj.cn

[D08] 合并两个数组
来源：http://yk.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://ci.colortex.cn

PHP:  array_merge($a, $b);
来源：http://sb.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mm.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://ps.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oy.jctech888.com.cn

Go:   append(a, b...)
来源：http://ms.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://tj.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://gq.bookmarksfly.cn

[D09] 排序（升序）
来源：http://nw.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://an.nszjky.cn

PHP:  sort($arr);
来源：http://ds.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xh.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sf.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cl.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://al.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ro.nicolike.cn

C#:   list.Sort();
来源：http://jt.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fy.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jt.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xn.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pp.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lo.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mj.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://di.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oq.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oc.yuntaijiaju.cn

[D11] 反转数组
来源：http://if.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qu.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://xe.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ey.gzmigu.cn

TS:   [...arr].reverse();
来源：http://py.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://ao.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://bg.colortex.cn

Ruby: arr.reverse
来源：http://kq.nicolike.cn

C#:   list.Reverse();
来源：http://df.shtwfgs.cn

[D12] 查找元素下标
来源：http://hr.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://du.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yk.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ea.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fi.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wt.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://ys.muxihuayi.cn

Ruby: arr.index(x)
来源：http://ev.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://uo.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://mg.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ue.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qd.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://ij.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://tw.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ip.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wy.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jv.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ab.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ao.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wg.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hp.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://ub.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://xl.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lb.colortex.cn

Go:   // 手写循环
来源：http://xt.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ce.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jf.521024.cn

[D15] 去重
来源：http://qg.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ip.gzmigu.cn

PHP:  array_unique($arr);
来源：http://bv.nszjky.cn

JS:   [...new Set(arr)]
来源：http://nz.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ai.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xk.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nr.hahajie.cn

Ruby: arr.uniq
来源：http://br.asd995.cn

C#:   list.Distinct().ToList()
来源：http://ms.shtwfgs.cn

[D16] 求和与平均值
来源：http://vv.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tk.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qd.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vy.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://li.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vl.nicolike.cn

Go:   // 手写循环累加
来源：http://ah.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jx.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://md.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://gq.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://dl.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://fa.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pa.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://co.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bq.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kn.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://bs.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://vw.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://hi.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ii.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://hy.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zr.9csxet.cn

TS:   nested.flat();
来源：http://qp.muxihuayi.cn


<!-- 参考信息 -->