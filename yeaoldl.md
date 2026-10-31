代发 wailian999

[C06] 匿名函数 / lambda
来源：http://bv.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://mv.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://br.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://zt.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://gq.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jy.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://se.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://rv.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ee.9csxet.cn

[C07] 把函数作为参数传入
来源：http://bu.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://my.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ig.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bl.bjjhwx.cn

TS:   arr.map(String)
来源：http://kk.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cj.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yx.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://bq.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zn.nszjky.cn

[C08] 闭包
来源：http://pc.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dk.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yn.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qz.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ww.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ng.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://at.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uo.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://as.hahajie.cn

[C09] 递归
来源：http://kq.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fr.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://il.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kg.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uh.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xf.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lq.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pn.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hc.colortex.cn

[C10] 变量作用域
来源：http://zx.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dy.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ko.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ow.yuexingan06.cn

TS:   同 JS
来源：http://vb.szxytkj.cn

Java: 方法内为块级作用域
来源：http://rl.chemitech.net.cn

Go:   花括号块级作用域
来源：http://vf.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xd.panjiajie.cn

C#:   块级作用域
来源：http://tb.newstarts.cn

[C11] 模块导入与导出
来源：http://tu.nicolike.cn

Py:   from module import func
来源：http://dq.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pb.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qb.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mo.hahajie.cn

Java: import java.util.List;
来源：http://le.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bd.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://nh.shtwfgs.cn

C#:   using System.Text;
来源：http://ql.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://du.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://ar.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://ai.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://dw.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://zu.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bt.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://kp.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ep.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gg.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://gl.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bo.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yj.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fd.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mq.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sj.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://mh.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mq.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vn.muxihuayi.cn

[C14] 泛型函数
来源：http://ie.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ad.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://hb.huixiangedu.cn

JS:   // 无泛型
来源：http://ix.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://al.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mf.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://az.colortex.cn

Ruby: # 无泛型
来源：http://rw.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://af.nszjky.cn

[C15] 解构 / 展开参数
来源：http://tw.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ff.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://ij.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rh.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rz.yuexingan06.cn

Java: // 无解构
来源：http://ei.haigaiapp.cn

Go:   // 无解构
来源：http://ol.asd995.cn

Ruby: a, b = pair
来源：http://fl.nszjky.cn

C#:   var (a, b) = pair;
来源：http://bd.newstarts.cn

[C16] 函数 / 方法重载
来源：http://ji.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eq.hnjuh.cn

PHP:  // 无重载
来源：http://jr.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qh.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://ij.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jf.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://gn.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://fa.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bb.bjjhwx.cn

================================================================================
来源：http://sv.asd995.cn

D. 数组 / 列表 / 集合
来源：http://lc.shxzukj.cn

================================================================================
来源：http://gu.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://qx.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ae.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jv.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zg.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bl.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vw.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ee.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://vx.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fq.521024.cn

[D02] 追加元素到末尾
来源：http://wl.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fy.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ij.huanxung.cn

JS:   arr.push(4);
来源：http://oo.huanxung.cn

TS:   arr.push(4);
来源：http://px.wgjwhj.cn

Java: list.add(4);
来源：http://bi.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://xf.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://nv.haigaiapp.cn

C#:   list.Add(4);
来源：http://xr.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://xi.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://xm.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fa.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wy.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://zp.hahajie.cn

Java: list.add(0, 0);
来源：http://ih.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sx.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jj.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://ge.521024.cn

[D04] 删除元素
来源：http://py.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://md.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mh.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sw.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://va.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qd.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vy.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hv.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ez.huixiangedu.cn

[D05] 访问与修改元素
来源：http://na.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://se.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oz.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://td.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://mp.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://fj.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://rb.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uo.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://es.bookmarksfly.cn

[D06] 数组长度
来源：http://pa.huixinmuqiang.cn

Py:   len(arr)
来源：http://nv.hnjuh.cn

PHP:  count($arr);
来源：http://my.huanxung.cn

JS:   arr.length
来源：http://rn.yuexingan06.cn

TS:   arr.length
来源：http://ty.chemitech.net.cn

Java: list.size();
来源：http://pk.muxihuayi.cn

Go:   len(arr)
来源：http://og.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://wg.jctech888.com.cn

C#:   list.Count;
来源：http://gg.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://zg.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ur.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://id.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://mg.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://vw.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://xf.bjjhwx.cn

Go:   arr[1:4]
来源：http://vq.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://bl.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://gl.9csxet.cn

[D08] 合并两个数组
来源：http://fq.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://vq.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://sz.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://en.shxzukj.cn

TS:   [...a, ...b];
来源：http://lt.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ss.bookmarksfly.cn

Go:   append(a, b...)
来源：http://ne.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://ou.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://rj.wgjwhj.cn

[D09] 排序（升序）
来源：http://sh.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://fo.panjiajie.cn

PHP:  sort($arr);
来源：http://dm.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ep.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fj.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vk.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mo.shxzskj.cn

Ruby: arr.sort
来源：http://hc.wgjwhj.cn

C#:   list.Sort();
来源：http://xf.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mt.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bu.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xb.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vp.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ui.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://if.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cz.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://im.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yt.bjjhwx.cn

[D11] 反转数组
来源：http://oz.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://am.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://mp.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oo.nszjky.cn

TS:   [...arr].reverse();
来源：http://ur.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://mp.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://td.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://dz.shxzskj.cn

C#:   list.Reverse();
来源：http://jk.bookmarksfly.cn

[D12] 查找元素下标
来源：http://cg.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://pe.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sr.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jj.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jz.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xo.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://cr.szxytkj.cn

Ruby: arr.index(x)
来源：http://bx.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://xq.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://gl.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ur.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ep.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://vn.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://ny.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qz.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dt.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xq.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mq.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://sk.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://od.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rh.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://nq.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://oa.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dh.huanxung.cn

Go:   // 手写循环
来源：http://dn.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uu.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ej.nszjky.cn

[D15] 去重
来源：http://ym.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lt.shxzskj.cn

PHP:  array_unique($arr);
来源：http://cl.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://pt.9csxet.cn

TS:   [...new Set(arr)]
来源：http://vm.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://js.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sg.hnjuh.cn

Ruby: arr.uniq
来源：http://bl.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://vp.bjjhwx.cn

[D16] 求和与平均值
来源：http://zl.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qz.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wi.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kh.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ex.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hv.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://aa.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xn.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://ob.bjjhwx.cn

[D17] 最大值与最小值
来源：http://rw.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://jl.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://lb.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sg.szxytkj.cn

TS:   Math.max(...arr);
来源：http://cb.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jn.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ni.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://fu.521024.cn

C#:   list.Max();  list.Min()
来源：http://xw.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://pj.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bv.521024.cn

PHP:  array_merge(...$nested);
来源：http://om.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jg.colortex.cn

TS:   nested.flat();
来源：http://mu.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rh.chemitech.net.cn

Go:   // 手写双层循环
来源：http://an.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://bq.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tj.asd995.cn

[D19] 按字段分组
来源：http://yf.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://it.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ef.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ay.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yt.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nu.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://mo.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ep.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uc.colortex.cn

[D20] 统计每个元素出现次数
来源：http://wq.bookmarksfly.cn

Py:   Counter(arr)
来源：http://pp.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://eq.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hr.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bl.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rq.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://et.hnjuh.cn

Ruby: arr.tally
来源：http://mz.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ns.asd995.cn

[D21] 判断是否包含某元素
来源：http://zo.huanxung.cn

Py:   x in arr
来源：http://hz.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://fw.asd995.cn

JS:   arr.includes(x)
来源：http://hs.shxzukj.cn

TS:   arr.includes(x)
来源：http://jt.szsharing.cn

Java: list.contains(x)
来源：http://sv.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://qp.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://hc.haigaiapp.cn

C#:   list.Contains(x)
来源：http://dr.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://rn.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kc.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sw.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jz.chemitech.net.cn

TS:   [...arr];
来源：http://el.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://hb.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hh.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://ww.hnjuh.cn

C#:   new List<int>(list);
来源：http://ae.chemitech.net.cn


<!-- 参考信息 -->