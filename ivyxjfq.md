代发 wailian999

Py:   return a, b
来源：http://fj.nicolike.cn

PHP:  return [$a, $b];
来源：http://up.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rw.panjiajie.cn

TS:   return { a, b };
来源：http://dm.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yw.chemitech.net.cn

Go:   return a, b
来源：http://ph.huanxung.cn

Ruby: return a, b
来源：http://jr.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://az.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://hr.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://qa.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wr.newstarts.cn

JS:   const square = x => x * x;
来源：http://ye.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://jw.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fo.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nz.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://rw.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ph.nszjky.cn

[C07] 把函数作为参数传入
来源：http://ai.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qp.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jx.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ea.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://df.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ux.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bg.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://kn.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wv.haigaiapp.cn

[C08] 闭包
来源：http://jv.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fr.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hf.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vk.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pt.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jl.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mk.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bv.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nl.huanxung.cn

[C09] 递归
来源：http://wo.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pi.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rf.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yg.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ej.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://le.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mg.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://by.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zv.shxzskj.cn

[C10] 变量作用域
来源：http://gf.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vp.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sv.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://et.lnxyls.cn

TS:   同 JS
来源：http://ae.9csxet.cn

Java: 方法内为块级作用域
来源：http://dd.hnjuh.cn

Go:   花括号块级作用域
来源：http://od.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rs.shxzukj.cn

C#:   块级作用域
来源：http://iv.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://mx.newstarts.cn

Py:   from module import func
来源：http://zl.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wi.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gy.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zt.yuntaijiaju.cn

Java: import java.util.List;
来源：http://lk.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://le.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://wk.newstarts.cn

C#:   using System.Text;
来源：http://ac.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://mf.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://ij.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://iq.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://xj.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://me.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xl.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://on.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://lz.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ps.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://sa.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://io.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yz.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vj.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fg.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hm.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://en.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fi.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uh.lnxyls.cn

[C14] 泛型函数
来源：http://ni.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cz.bjjhwx.cn

PHP:  // 无泛型
来源：http://kt.9csxet.cn

JS:   // 无泛型
来源：http://pz.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zi.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zj.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sy.yuexingan06.cn

Ruby: # 无泛型
来源：http://se.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sv.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://uz.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ir.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://pf.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gk.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nh.9csxet.cn

Java: // 无解构
来源：http://lk.newstarts.cn

Go:   // 无解构
来源：http://ij.shtwfgs.cn

Ruby: a, b = pair
来源：http://by.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://uc.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://gu.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gq.muxihuayi.cn

PHP:  // 无重载
来源：http://ng.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qr.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://ro.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jz.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://ts.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://xp.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yb.jianghongdianzi.cn

================================================================================
来源：http://ck.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://cz.huixinmuqiang.cn

================================================================================
来源：http://ot.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://cq.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hx.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uu.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ed.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://go.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ci.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://jx.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://ig.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yn.hahajie.cn

[D02] 追加元素到末尾
来源：http://uw.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ry.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jc.521024.cn

JS:   arr.push(4);
来源：http://hq.szxytkj.cn

TS:   arr.push(4);
来源：http://hf.nicolike.cn

Java: list.add(4);
来源：http://xb.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://wg.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://ea.shtwfgs.cn

C#:   list.Add(4);
来源：http://jx.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://fv.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://qv.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qm.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://et.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://om.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://if.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rg.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vg.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://ao.bjjhwx.cn

[D04] 删除元素
来源：http://lq.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mg.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fn.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hm.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://qy.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gp.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ms.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ts.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uy.gzmigu.cn

[D05] 访问与修改元素
来源：http://tv.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xf.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://de.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wx.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://vc.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://it.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://tv.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dn.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bg.nszjky.cn

[D06] 数组长度
来源：http://eb.521024.cn

Py:   len(arr)
来源：http://ui.jianghongdianzi.cn

PHP:  count($arr);
来源：http://fj.nicolike.cn

JS:   arr.length
来源：http://pz.521024.cn

TS:   arr.length
来源：http://sl.szsharing.cn

Java: list.size();
来源：http://tn.wgjwhj.cn

Go:   len(arr)
来源：http://pc.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://op.wgjwhj.cn

C#:   list.Count;
来源：http://mn.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://zi.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ui.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pp.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://oi.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://kd.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://mh.gzmigu.cn

Go:   arr[1:4]
来源：http://bc.szxytkj.cn

Ruby: arr[1, 3]
来源：http://wt.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://fi.shxzskj.cn

[D08] 合并两个数组
来源：http://zt.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://pj.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://sg.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mo.jctech888.com.cn

TS:   [...a, ...b];
来源：http://km.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://co.9csxet.cn

Go:   append(a, b...)
来源：http://ne.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://wx.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://fx.huixiangedu.cn

[D09] 排序（升序）
来源：http://af.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://ra.nicolike.cn

PHP:  sort($arr);
来源：http://mz.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://la.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://du.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ak.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://og.panjiajie.cn

Ruby: arr.sort
来源：http://wf.shxzskj.cn

C#:   list.Sort();
来源：http://vq.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aw.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fo.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nv.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nh.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ne.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tz.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pk.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wj.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ib.asd995.cn

[D11] 反转数组
来源：http://th.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cb.nszjky.cn

PHP:  array_reverse($arr);
来源：http://kn.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ft.newstarts.cn

TS:   [...arr].reverse();
来源：http://ak.lnxyls.cn

Java: Collections.reverse(list);
来源：http://ri.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://vr.panjiajie.cn

Ruby: arr.reverse
来源：http://kp.shxzukj.cn

C#:   list.Reverse();
来源：http://nd.wgjwhj.cn

[D12] 查找元素下标
来源：http://pr.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://gp.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gl.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yl.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sy.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yv.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://ei.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://bu.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://je.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://nq.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pp.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ej.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://ng.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://vp.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iu.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bu.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ab.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ug.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://fz.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kk.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ts.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://gh.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://gh.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tg.huixinmuqiang.cn

Go:   // 手写循环
来源：http://te.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eo.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rs.szsharing.cn

[D15] 去重
来源：http://lg.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zd.szsharing.cn

PHP:  array_unique($arr);
来源：http://yy.521024.cn

JS:   [...new Set(arr)]
来源：http://oa.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://yd.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vw.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yd.hnjuh.cn

Ruby: arr.uniq
来源：http://tf.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://xd.muxihuayi.cn

[D16] 求和与平均值
来源：http://qf.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yp.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yr.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bx.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mf.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mu.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://de.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://af.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://zb.muxihuayi.cn

[D17] 最大值与最小值
来源：http://mw.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://ra.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://sh.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jh.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://yp.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uh.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ld.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://bi.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://ww.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://xu.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tx.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://dk.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oq.szsharing.cn

TS:   nested.flat();
来源：http://jb.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rg.hahajie.cn

Go:   // 手写双层循环
来源：http://ei.521024.cn

Ruby: nested.flatten
来源：http://go.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gl.yuexingan06.cn

[D19] 按字段分组
来源：http://zf.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gm.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://un.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jo.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sf.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wy.521024.cn

Go:   // 手写 map[string][]T
来源：http://ix.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yr.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nw.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://ha.huixiangedu.cn

Py:   Counter(arr)
来源：http://am.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://dv.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zh.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bh.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wl.nicolike.cn

Go:   // 手写 map[T]int
来源：http://ql.bjjhwx.cn

Ruby: arr.tally
来源：http://om.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://es.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://ec.521024.cn

Py:   x in arr
来源：http://du.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://ru.asd995.cn

JS:   arr.includes(x)
来源：http://dw.shtwfgs.cn

TS:   arr.includes(x)
来源：http://ld.colortex.cn

Java: list.contains(x)
来源：http://ya.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://ep.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://eb.hahajie.cn

C#:   list.Contains(x)
来源：http://ha.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://xq.szxytkj.cn


<!-- 参考信息 -->