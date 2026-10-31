代发 wailian999

[C06] 匿名函数 / lambda
来源：http://rt.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://kc.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ae.colortex.cn

JS:   const square = x => x * x;
来源：http://vu.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://qy.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lx.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jl.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://ru.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zu.hahajie.cn

[C07] 把函数作为参数传入
来源：http://tn.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nw.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ml.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yp.bjjhwx.cn

TS:   arr.map(String)
来源：http://ix.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ei.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hu.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ot.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ir.shtwfgs.cn

[C08] 闭包
来源：http://ne.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kp.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yw.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qb.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nb.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hf.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ki.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zz.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ze.jctech888.com.cn

[C09] 递归
来源：http://zg.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pb.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ob.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mf.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kz.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vj.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lz.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://da.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kr.panjiajie.cn

[C10] 变量作用域
来源：http://yj.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ch.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hw.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ky.huixinmuqiang.cn

TS:   同 JS
来源：http://ds.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://qp.szsharing.cn

Go:   花括号块级作用域
来源：http://qw.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gx.nszjky.cn

C#:   块级作用域
来源：http://eu.huanxung.cn

[C11] 模块导入与导出
来源：http://oz.nszjky.cn

Py:   from module import func
来源：http://ui.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sa.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rb.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jm.huixinmuqiang.cn

Java: import java.util.List;
来源：http://rk.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wd.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://ks.nszjky.cn

C#:   using System.Text;
来源：http://og.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://yz.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://fz.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://tq.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://hx.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://ec.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://au.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://xa.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://mr.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uf.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://uu.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ok.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ns.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hd.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ty.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vd.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://bn.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://by.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://br.bookmarksfly.cn

[C14] 泛型函数
来源：http://cf.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mj.shxzukj.cn

PHP:  // 无泛型
来源：http://gp.lnxyls.cn

JS:   // 无泛型
来源：http://ee.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tq.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eq.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oa.shtwfgs.cn

Ruby: # 无泛型
来源：http://kj.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://se.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://ba.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gh.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ut.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zg.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ha.shxzskj.cn

Java: // 无解构
来源：http://tz.haigaiapp.cn

Go:   // 无解构
来源：http://mp.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://xg.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://vc.colortex.cn

[C16] 函数 / 方法重载
来源：http://ze.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gt.huixinmuqiang.cn

PHP:  // 无重载
来源：http://zq.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://og.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://ks.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ea.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://vi.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://bv.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wc.asd995.cn

================================================================================
来源：http://wn.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://pd.yuntaijiaju.cn

================================================================================
来源：http://ic.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://ru.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://az.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://us.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rz.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://st.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ik.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://rk.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://er.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hl.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://kk.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vv.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lr.nicolike.cn

JS:   arr.push(4);
来源：http://ge.chemitech.net.cn

TS:   arr.push(4);
来源：http://az.lnxyls.cn

Java: list.add(4);
来源：http://qo.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://zc.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ic.jctech888.com.cn

C#:   list.Add(4);
来源：http://lp.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://br.colortex.cn

Py:   arr.insert(0, 0)
来源：http://lc.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kv.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cr.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://es.yuexingan06.cn

Java: list.add(0, 0);
来源：http://qh.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dh.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nt.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://nf.shtwfgs.cn

[D04] 删除元素
来源：http://pz.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ri.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ue.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ul.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://vc.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://la.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mo.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nr.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sg.shxzukj.cn

[D05] 访问与修改元素
来源：http://ke.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rs.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ai.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tu.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://iu.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://tq.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://em.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://at.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fn.yuexingan06.cn

[D06] 数组长度
来源：http://sy.hnjuh.cn

Py:   len(arr)
来源：http://xz.newstarts.cn

PHP:  count($arr);
来源：http://ps.jianghongdianzi.cn

JS:   arr.length
来源：http://ut.huixinmuqiang.cn

TS:   arr.length
来源：http://tg.shtwfgs.cn

Java: list.size();
来源：http://gt.yuntaijiaju.cn

Go:   len(arr)
来源：http://zj.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://fl.newstarts.cn

C#:   list.Count;
来源：http://xq.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://sz.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ev.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ek.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://kq.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://ys.lnxyls.cn

Java: list.subList(1, 4);
来源：http://ad.muxihuayi.cn

Go:   arr[1:4]
来源：http://qa.521024.cn

Ruby: arr[1, 3]
来源：http://oq.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://fa.lnxyls.cn

[D08] 合并两个数组
来源：http://da.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://yo.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://vh.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dz.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://mq.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ij.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://pm.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://vb.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://pj.hnjuh.cn

[D09] 排序（升序）
来源：http://ik.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ft.szsharing.cn

PHP:  sort($arr);
来源：http://fp.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dm.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ip.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://br.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hn.bookmarksfly.cn

Ruby: arr.sort
来源：http://kb.jctech888.com.cn

C#:   list.Sort();
来源：http://wc.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yg.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gr.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bn.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hw.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bt.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lg.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sj.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yx.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gj.gzmigu.cn

[D11] 反转数组
来源：http://fr.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ca.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://sh.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ms.shxzskj.cn

TS:   [...arr].reverse();
来源：http://iw.nszjky.cn

Java: Collections.reverse(list);
来源：http://el.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://bd.bjjhwx.cn

Ruby: arr.reverse
来源：http://gt.shtwfgs.cn

C#:   list.Reverse();
来源：http://kd.haigaiapp.cn

[D12] 查找元素下标
来源：http://vz.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://pk.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ep.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://on.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zc.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wn.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://lo.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://yv.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://ot.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://il.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ye.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vl.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://og.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://bj.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kg.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vk.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ja.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wx.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://sx.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jg.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iq.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://tv.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://gf.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qw.9csxet.cn

Go:   // 手写循环
来源：http://sc.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://md.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cv.bjjhwx.cn

[D15] 去重
来源：http://hh.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jf.szsharing.cn

PHP:  array_unique($arr);
来源：http://rz.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://dx.hahajie.cn

TS:   [...new Set(arr)]
来源：http://ma.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wp.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mr.nszjky.cn

Ruby: arr.uniq
来源：http://ex.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://cx.chemitech.net.cn

[D16] 求和与平均值
来源：http://oa.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ym.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ab.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ij.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://au.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vs.521024.cn

Go:   // 手写循环累加
来源：http://nh.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ap.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://ag.asd995.cn

[D17] 最大值与最小值
来源：http://gh.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://dh.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://gc.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ul.newstarts.cn

TS:   Math.max(...arr);
来源：http://gn.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bb.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ep.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://zz.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://wo.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://or.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://og.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://vb.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mw.colortex.cn

TS:   nested.flat();
来源：http://qu.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ad.nicolike.cn

Go:   // 手写双层循环
来源：http://as.yuexingan06.cn

Ruby: nested.flatten
来源：http://tl.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qr.panjiajie.cn

[D19] 按字段分组
来源：http://jz.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vc.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uc.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kg.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://td.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qq.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://xt.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ch.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wy.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://rw.huanxung.cn

Py:   Counter(arr)
来源：http://gr.nicolike.cn

PHP:  array_count_values($arr);
来源：http://hz.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qs.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ul.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zm.newstarts.cn

Go:   // 手写 map[T]int
来源：http://yz.hnjuh.cn

Ruby: arr.tally
来源：http://wu.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://br.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://gh.shxzukj.cn

Py:   x in arr
来源：http://zj.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://yc.9csxet.cn

JS:   arr.includes(x)
来源：http://qk.shtwfgs.cn

TS:   arr.includes(x)
来源：http://jc.colortex.cn

Java: list.contains(x)
来源：http://jw.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://hx.huanxung.cn

Ruby: arr.include?(x)
来源：http://pd.lnxyls.cn

C#:   list.Contains(x)
来源：http://gj.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://ko.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wr.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dr.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ql.panjiajie.cn

TS:   [...arr];
来源：http://vd.asd995.cn

Java: new ArrayList<>(list);
来源：http://gl.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xi.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://zs.colortex.cn

C#:   new List<int>(list);
来源：http://zw.yuntaijiaju.cn


<!-- 参考信息 -->