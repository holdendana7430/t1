代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://ye.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://zj.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hp.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kk.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kd.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://ew.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qr.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ic.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://uh.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gd.haigaiapp.cn

[C08] 闭包
来源：http://yn.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kp.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xa.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oh.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mi.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fz.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hn.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ox.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ka.hahajie.cn

[C09] 递归
来源：http://wv.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://un.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ze.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cm.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fm.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yn.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uc.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qa.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hr.haigaiapp.cn

[C10] 变量作用域
来源：http://gu.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nj.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://el.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ar.asd995.cn

TS:   同 JS
来源：http://gu.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://dh.asd995.cn

Go:   花括号块级作用域
来源：http://vc.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://le.huanxung.cn

C#:   块级作用域
来源：http://kc.shxzukj.cn

[C11] 模块导入与导出
来源：http://tl.nszjky.cn

Py:   from module import func
来源：http://ml.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bc.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sg.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zg.gzmigu.cn

Java: import java.util.List;
来源：http://fi.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://za.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://mf.9csxet.cn

C#:   using System.Text;
来源：http://yh.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://zx.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://zq.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://ue.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://ox.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://bg.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ko.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ts.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://rc.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pi.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://qb.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dg.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ek.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sc.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hv.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wl.shxzukj.cn

Go:   func add(a, b int) int
来源：http://cp.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vr.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://to.bookmarksfly.cn

[C14] 泛型函数
来源：http://uk.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://li.9csxet.cn

PHP:  // 无泛型
来源：http://bv.gzmigu.cn

JS:   // 无泛型
来源：http://nl.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ic.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qm.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bq.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://ph.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yt.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://wf.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://th.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://tt.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://es.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jj.asd995.cn

Java: // 无解构
来源：http://iq.huanxung.cn

Go:   // 无解构
来源：http://bd.jctech888.com.cn

Ruby: a, b = pair
来源：http://er.hahajie.cn

C#:   var (a, b) = pair;
来源：http://rf.nszjky.cn

[C16] 函数 / 方法重载
来源：http://ga.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wd.huixiangedu.cn

PHP:  // 无重载
来源：http://gs.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sh.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://ca.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wx.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://bz.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://ap.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kt.jianghongdianzi.cn

================================================================================
来源：http://ol.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://fm.9csxet.cn

================================================================================
来源：http://wi.huanxung.cn

[D01] 创建数组 / 列表
来源：http://ps.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pb.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yp.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://en.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dc.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://od.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://ff.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://ty.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xq.colortex.cn

[D02] 追加元素到末尾
来源：http://bv.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oo.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sd.nicolike.cn

JS:   arr.push(4);
来源：http://at.521024.cn

TS:   arr.push(4);
来源：http://jw.muxihuayi.cn

Java: list.add(4);
来源：http://if.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://vb.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://tn.colortex.cn

C#:   list.Add(4);
来源：http://mi.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://mo.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://uj.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zy.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ps.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://is.wgjwhj.cn

Java: list.add(0, 0);
来源：http://pu.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ef.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://la.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://ce.bookmarksfly.cn

[D04] 删除元素
来源：http://va.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jf.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fy.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sa.colortex.cn

TS:   arr.splice(0, 1);
来源：http://aa.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dt.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lh.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kf.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nu.9csxet.cn

[D05] 访问与修改元素
来源：http://tn.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gy.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kj.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mh.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://gw.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://po.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://tu.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xr.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ls.yuntaijiaju.cn

[D06] 数组长度
来源：http://yv.bookmarksfly.cn

Py:   len(arr)
来源：http://oc.hahajie.cn

PHP:  count($arr);
来源：http://yq.huixiangedu.cn

JS:   arr.length
来源：http://il.shxzskj.cn

TS:   arr.length
来源：http://oa.chemitech.net.cn

Java: list.size();
来源：http://yb.hnjuh.cn

Go:   len(arr)
来源：http://kb.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://hv.jctech888.com.cn

C#:   list.Count;
来源：http://ro.521024.cn

[D07] 切片 / 取子数组
来源：http://qa.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jw.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iu.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://tv.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://nh.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://rt.521024.cn

Go:   arr[1:4]
来源：http://xm.nszjky.cn

Ruby: arr[1, 3]
来源：http://ec.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://ct.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://dz.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://fr.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://dj.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kd.asd995.cn

TS:   [...a, ...b];
来源：http://gw.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://el.asd995.cn

Go:   append(a, b...)
来源：http://au.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://ue.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://ne.gzmigu.cn

[D09] 排序（升序）
来源：http://hr.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://rh.chemitech.net.cn

PHP:  sort($arr);
来源：http://mm.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hr.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vk.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sy.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wn.shtwfgs.cn

Ruby: arr.sort
来源：http://te.newstarts.cn

C#:   list.Sort();
来源：http://oc.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yu.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lf.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ry.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://op.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pm.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zj.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ym.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://go.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ao.nicolike.cn

[D11] 反转数组
来源：http://pi.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eh.szsharing.cn

PHP:  array_reverse($arr);
来源：http://uw.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://va.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://ts.colortex.cn

Java: Collections.reverse(list);
来源：http://ww.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://gz.huixiangedu.cn

Ruby: arr.reverse
来源：http://fw.colortex.cn

C#:   list.Reverse();
来源：http://cl.newstarts.cn

[D12] 查找元素下标
来源：http://mv.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://mw.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ky.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://py.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sm.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lc.colortex.cn

Go:   slices.Index(arr, x)
来源：http://ea.huanxung.cn

Ruby: arr.index(x)
来源：http://hn.nicolike.cn

C#:   list.IndexOf(x);
来源：http://gk.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://dl.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://au.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xt.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://yz.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://ek.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ex.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cu.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://of.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lc.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://go.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lk.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qg.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://ju.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://ci.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yl.9csxet.cn

Go:   // 手写循环
来源：http://dg.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rw.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vs.chemitech.net.cn

[D15] 去重
来源：http://ow.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kh.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://mh.nicolike.cn

JS:   [...new Set(arr)]
来源：http://gs.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://ut.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hw.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lh.nszjky.cn

Ruby: arr.uniq
来源：http://at.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://rf.shxzukj.cn

[D16] 求和与平均值
来源：http://ah.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pe.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yg.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fz.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ke.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cp.shxzskj.cn

Go:   // 手写循环累加
来源：http://em.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ge.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://pa.shxzukj.cn

[D17] 最大值与最小值
来源：http://ou.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://ab.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://qz.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://so.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://mi.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cp.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yl.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://pw.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://sn.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://ja.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vd.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://if.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ef.shtwfgs.cn

TS:   nested.flat();
来源：http://bz.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ii.nicolike.cn

Go:   // 手写双层循环
来源：http://vu.huanxung.cn

Ruby: nested.flatten
来源：http://zr.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xj.jctech888.com.cn

[D19] 按字段分组
来源：http://jk.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wv.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xg.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rc.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hs.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vf.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://dd.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bc.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://os.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://xp.shxzukj.cn

Py:   Counter(arr)
来源：http://ji.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://gt.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vi.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sz.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yl.nicolike.cn

Go:   // 手写 map[T]int
来源：http://ep.shtwfgs.cn

Ruby: arr.tally
来源：http://wl.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cs.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://pe.huixinmuqiang.cn

Py:   x in arr
来源：http://up.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://mh.panjiajie.cn

JS:   arr.includes(x)
来源：http://xw.haigaiapp.cn

TS:   arr.includes(x)
来源：http://kd.yuntaijiaju.cn

Java: list.contains(x)
来源：http://zn.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://gb.colortex.cn

Ruby: arr.include?(x)
来源：http://ar.shtwfgs.cn

C#:   list.Contains(x)
来源：http://qy.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://ct.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xu.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ri.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xi.newstarts.cn

TS:   [...arr];
来源：http://tg.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://mi.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tz.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://jl.shxzskj.cn

C#:   new List<int>(list);
来源：http://dv.huanxung.cn

[D23] reduce 累积计算
来源：http://je.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ao.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rx.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bn.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ip.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ic.nszjky.cn

Go:   // 手写循环
来源：http://em.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uk.huixiangedu.cn


<!-- 参考信息 -->