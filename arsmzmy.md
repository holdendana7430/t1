代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://ej.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://ku.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zh.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iy.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ii.panjiajie.cn

TS:   arr.map(String)
来源：http://hh.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dr.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yq.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://ex.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nv.bookmarksfly.cn

[C08] 闭包
来源：http://kl.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fa.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mb.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ra.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nj.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mx.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iy.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qy.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cq.shxzskj.cn

[C09] 递归
来源：http://yq.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tr.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ag.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://im.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aj.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ay.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ma.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mf.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xf.colortex.cn

[C10] 变量作用域
来源：http://tn.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ln.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wb.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ww.wgjwhj.cn

TS:   同 JS
来源：http://qt.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://vg.bjjhwx.cn

Go:   花括号块级作用域
来源：http://ew.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zj.panjiajie.cn

C#:   块级作用域
来源：http://gx.nszjky.cn

[C11] 模块导入与导出
来源：http://pi.wgjwhj.cn

Py:   from module import func
来源：http://sh.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pq.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ex.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oe.521024.cn

Java: import java.util.List;
来源：http://ph.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wg.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://bg.nicolike.cn

C#:   using System.Text;
来源：http://zu.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://xo.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://uu.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://nd.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://kd.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://yh.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ha.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://vi.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://nw.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ry.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://co.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bv.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vi.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ly.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ay.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://np.colortex.cn

Go:   func add(a, b int) int
来源：http://yg.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ap.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rd.hnjuh.cn

[C14] 泛型函数
来源：http://bq.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gc.huixiangedu.cn

PHP:  // 无泛型
来源：http://ed.wgjwhj.cn

JS:   // 无泛型
来源：http://cx.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ca.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hp.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cz.newstarts.cn

Ruby: # 无泛型
来源：http://vy.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vi.newstarts.cn

[C15] 解构 / 展开参数
来源：http://gq.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ik.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://ya.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uc.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ga.huixiangedu.cn

Java: // 无解构
来源：http://gm.shtwfgs.cn

Go:   // 无解构
来源：http://nu.nicolike.cn

Ruby: a, b = pair
来源：http://wf.hahajie.cn

C#:   var (a, b) = pair;
来源：http://hn.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://xm.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hx.shtwfgs.cn

PHP:  // 无重载
来源：http://vw.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qt.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://pj.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uf.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://gu.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://mi.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bl.szxytkj.cn

================================================================================
来源：http://vp.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://xa.huanxung.cn

================================================================================
来源：http://iq.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://rp.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wu.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rg.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mi.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bs.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vw.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://jj.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://yr.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ok.lnxyls.cn

[D02] 追加元素到末尾
来源：http://cn.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uq.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vx.shtwfgs.cn

JS:   arr.push(4);
来源：http://wj.wgjwhj.cn

TS:   arr.push(4);
来源：http://rq.lnxyls.cn

Java: list.add(4);
来源：http://wj.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://po.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://km.chemitech.net.cn

C#:   list.Add(4);
来源：http://fx.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://xo.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://nc.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wx.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ls.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://om.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://zq.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fa.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lb.colortex.cn

C#:   list.Insert(0, 0);
来源：http://fv.asd995.cn

[D04] 删除元素
来源：http://ji.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wg.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://un.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vl.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://dg.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nj.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qp.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ow.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eb.chemitech.net.cn

[D05] 访问与修改元素
来源：http://ca.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mh.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rr.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fl.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://qt.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://sz.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://xb.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cb.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fw.wgjwhj.cn

[D06] 数组长度
来源：http://yw.nicolike.cn

Py:   len(arr)
来源：http://vi.yuexingan06.cn

PHP:  count($arr);
来源：http://em.bjjhwx.cn

JS:   arr.length
来源：http://xj.chemitech.net.cn

TS:   arr.length
来源：http://dz.szsharing.cn

Java: list.size();
来源：http://ba.haigaiapp.cn

Go:   len(arr)
来源：http://sv.hahajie.cn

Ruby: arr.length; arr.size
来源：http://zu.szxytkj.cn

C#:   list.Count;
来源：http://ie.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://ow.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nn.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hn.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://pl.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://xu.gzmigu.cn

Java: list.subList(1, 4);
来源：http://ny.jctech888.com.cn

Go:   arr[1:4]
来源：http://xr.nszjky.cn

Ruby: arr[1, 3]
来源：http://ga.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://hz.hnjuh.cn

[D08] 合并两个数组
来源：http://ey.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://dm.colortex.cn

PHP:  array_merge($a, $b);
来源：http://kg.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xy.muxihuayi.cn

TS:   [...a, ...b];
来源：http://bn.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jp.asd995.cn

Go:   append(a, b...)
来源：http://xv.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://ri.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://tn.9csxet.cn

[D09] 排序（升序）
来源：http://qs.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vx.wgjwhj.cn

PHP:  sort($arr);
来源：http://cj.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pr.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yz.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kg.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ak.9csxet.cn

Ruby: arr.sort
来源：http://gd.panjiajie.cn

C#:   list.Sort();
来源：http://ch.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gg.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ij.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ty.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wv.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hs.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pt.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jk.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wl.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mu.chemitech.net.cn

[D11] 反转数组
来源：http://cb.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oa.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://iq.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qr.nszjky.cn

TS:   [...arr].reverse();
来源：http://kt.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://hc.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://il.gzmigu.cn

Ruby: arr.reverse
来源：http://fh.panjiajie.cn

C#:   list.Reverse();
来源：http://lr.chemitech.net.cn

[D12] 查找元素下标
来源：http://fe.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://tz.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ep.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rz.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nf.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sa.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://dk.521024.cn

Ruby: arr.index(x)
来源：http://at.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://qt.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://ds.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vj.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ac.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ap.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://dl.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://po.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xn.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pv.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gp.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://kl.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xt.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dn.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://tp.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://xs.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cd.bjjhwx.cn

Go:   // 手写循环
来源：http://uu.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rz.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lm.nicolike.cn

[D15] 去重
来源：http://zz.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jv.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://pr.huanxung.cn

JS:   [...new Set(arr)]
来源：http://tx.newstarts.cn

TS:   [...new Set(arr)]
来源：http://ls.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cm.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gi.nicolike.cn

Ruby: arr.uniq
来源：http://sn.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://na.huixiangedu.cn

[D16] 求和与平均值
来源：http://xl.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ms.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eu.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mv.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://do.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pu.bjjhwx.cn

Go:   // 手写循环累加
来源：http://lf.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eu.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://sl.colortex.cn

[D17] 最大值与最小值
来源：http://sb.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://el.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://rq.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pn.newstarts.cn

TS:   Math.max(...arr);
来源：http://tj.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ck.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fu.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://jb.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://es.521024.cn

[D18] 扁平化嵌套数组
来源：http://pe.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://in.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://pq.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kl.nszjky.cn

TS:   nested.flat();
来源：http://bt.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cw.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://kb.asd995.cn

Ruby: nested.flatten
来源：http://az.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ip.bjjhwx.cn

[D19] 按字段分组
来源：http://er.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://id.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kg.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zy.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rc.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tf.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://gb.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hx.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kg.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://bj.bookmarksfly.cn

Py:   Counter(arr)
来源：http://yx.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://jq.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vj.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lo.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tt.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://af.yuexingan06.cn

Ruby: arr.tally
来源：http://dx.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uu.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://ah.huixiangedu.cn

Py:   x in arr
来源：http://jt.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://co.huanxung.cn

JS:   arr.includes(x)
来源：http://fe.gzmigu.cn

TS:   arr.includes(x)
来源：http://sm.hnjuh.cn

Java: list.contains(x)
来源：http://sd.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://jr.gzmigu.cn

Ruby: arr.include?(x)
来源：http://lv.hahajie.cn

C#:   list.Contains(x)
来源：http://rk.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://sj.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nq.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wt.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pt.lnxyls.cn

TS:   [...arr];
来源：http://zt.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://jn.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://un.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://zx.nszjky.cn

C#:   new List<int>(list);
来源：http://oe.hahajie.cn

[D23] reduce 累积计算
来源：http://nj.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mu.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zc.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tb.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pa.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rz.newstarts.cn

Go:   // 手写循环
来源：http://qq.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hi.szxytkj.cn


<!-- 参考信息 -->