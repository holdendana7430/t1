代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://tf.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://jc.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yh.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cx.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ha.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://aq.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ub.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oc.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://aj.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gm.chemitech.net.cn

[C08] 闭包
来源：http://ob.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tm.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xe.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qd.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://et.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zy.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hm.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lk.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uj.jctech888.com.cn

[C09] 递归
来源：http://wn.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vb.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zq.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ln.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gc.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kw.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ac.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ub.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lc.jctech888.com.cn

[C10] 变量作用域
来源：http://zf.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mb.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://do.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ft.huixinmuqiang.cn

TS:   同 JS
来源：http://jr.lnxyls.cn

Java: 方法内为块级作用域
来源：http://eq.hahajie.cn

Go:   花括号块级作用域
来源：http://if.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wl.szxytkj.cn

C#:   块级作用域
来源：http://be.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://rc.hnjuh.cn

Py:   from module import func
来源：http://kg.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eu.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kz.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ms.chemitech.net.cn

Java: import java.util.List;
来源：http://jk.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yp.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://gd.9csxet.cn

C#:   using System.Text;
来源：http://it.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://ur.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://pt.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://kz.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://ls.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://pq.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ga.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://pf.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://bu.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ar.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://cr.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jz.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uz.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dw.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sv.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bt.szxytkj.cn

Go:   func add(a, b int) int
来源：http://ek.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kp.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yf.hahajie.cn

[C14] 泛型函数
来源：http://ub.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sb.newstarts.cn

PHP:  // 无泛型
来源：http://mp.szxytkj.cn

JS:   // 无泛型
来源：http://ad.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lh.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fw.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iq.521024.cn

Ruby: # 无泛型
来源：http://sv.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://no.szsharing.cn

[C15] 解构 / 展开参数
来源：http://ga.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kn.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://zv.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://di.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xn.nicolike.cn

Java: // 无解构
来源：http://qm.hnjuh.cn

Go:   // 无解构
来源：http://jo.szsharing.cn

Ruby: a, b = pair
来源：http://jd.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://fu.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://xq.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vl.hahajie.cn

PHP:  // 无重载
来源：http://xd.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qy.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://jw.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jm.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://vq.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://ck.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mg.chemitech.net.cn

================================================================================
来源：http://gp.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://my.gzmigu.cn

================================================================================
来源：http://gk.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://mh.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oz.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rd.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vb.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ir.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yq.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://tm.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://uv.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mv.szsharing.cn

[D02] 追加元素到末尾
来源：http://cj.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wq.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qz.gzmigu.cn

JS:   arr.push(4);
来源：http://xl.nicolike.cn

TS:   arr.push(4);
来源：http://zj.bjjhwx.cn

Java: list.add(4);
来源：http://vv.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://xg.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://tb.9csxet.cn

C#:   list.Add(4);
来源：http://qa.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://vr.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://ge.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kt.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ip.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://rb.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://ae.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hk.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ab.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://lj.521024.cn

[D04] 删除元素
来源：http://et.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oq.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lt.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lp.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://mg.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ju.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uh.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://il.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ub.huanxung.cn

[D05] 访问与修改元素
来源：http://ef.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ba.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hi.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iy.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://ob.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://kh.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://xe.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ng.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ls.lnxyls.cn

[D06] 数组长度
来源：http://jx.newstarts.cn

Py:   len(arr)
来源：http://ju.wgjwhj.cn

PHP:  count($arr);
来源：http://jg.szsharing.cn

JS:   arr.length
来源：http://ei.lnxyls.cn

TS:   arr.length
来源：http://lq.szsharing.cn

Java: list.size();
来源：http://cv.lnxyls.cn

Go:   len(arr)
来源：http://sz.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://hk.hahajie.cn

C#:   list.Count;
来源：http://vk.9csxet.cn

[D07] 切片 / 取子数组
来源：http://ys.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zx.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ob.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://mw.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://nk.shxzskj.cn

Java: list.subList(1, 4);
来源：http://nv.haigaiapp.cn

Go:   arr[1:4]
来源：http://bx.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://ol.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://vk.hahajie.cn

[D08] 合并两个数组
来源：http://tj.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://yy.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://ou.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cn.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://ue.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rq.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://db.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://ck.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://cu.jctech888.com.cn

[D09] 排序（升序）
来源：http://yi.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ee.wgjwhj.cn

PHP:  sort($arr);
来源：http://jd.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://td.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xq.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ri.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hh.hnjuh.cn

Ruby: arr.sort
来源：http://zl.nicolike.cn

C#:   list.Sort();
来源：http://nu.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zk.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qf.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ei.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fv.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lt.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tf.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uy.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fu.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ge.521024.cn

[D11] 反转数组
来源：http://ew.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ll.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://gu.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jx.asd995.cn

TS:   [...arr].reverse();
来源：http://ma.szsharing.cn

Java: Collections.reverse(list);
来源：http://ow.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://ih.lnxyls.cn

Ruby: arr.reverse
来源：http://as.jctech888.com.cn

C#:   list.Reverse();
来源：http://qs.lnxyls.cn

[D12] 查找元素下标
来源：http://nh.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://ph.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vi.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jg.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fs.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qh.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://fs.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://vj.huanxung.cn

C#:   list.IndexOf(x);
来源：http://ln.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://jo.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ot.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ed.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://ie.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://kh.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xb.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://so.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lt.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dn.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://td.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ix.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mv.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://fs.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://xa.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://km.chemitech.net.cn

Go:   // 手写循环
来源：http://ml.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qv.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bu.yuexingan06.cn

[D15] 去重
来源：http://xt.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lx.szsharing.cn

PHP:  array_unique($arr);
来源：http://cl.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://ox.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://ig.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://de.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tl.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://uv.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://nt.shtwfgs.cn

[D16] 求和与平均值
来源：http://lf.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ev.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wd.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ek.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dt.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hh.bjjhwx.cn

Go:   // 手写循环累加
来源：http://ys.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ee.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://nm.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://xk.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://oi.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://nb.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cp.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://nx.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ue.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rs.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://le.asd995.cn

C#:   list.Max();  list.Min()
来源：http://qx.asd995.cn

[D18] 扁平化嵌套数组
来源：http://jl.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hk.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://iv.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ud.szxytkj.cn

TS:   nested.flat();
来源：http://mx.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fq.shxzskj.cn

Go:   // 手写双层循环
来源：http://jl.9csxet.cn

Ruby: nested.flatten
来源：http://vv.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xj.newstarts.cn

[D19] 按字段分组
来源：http://yx.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ke.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lf.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cy.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sm.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mh.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://vm.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gl.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cw.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://cc.yuexingan06.cn

Py:   Counter(arr)
来源：http://ms.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://el.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yw.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cc.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dg.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://oo.asd995.cn

Ruby: arr.tally
来源：http://ni.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rh.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://lb.szxytkj.cn

Py:   x in arr
来源：http://hi.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://rv.asd995.cn

JS:   arr.includes(x)
来源：http://hv.nicolike.cn

TS:   arr.includes(x)
来源：http://zx.bjjhwx.cn

Java: list.contains(x)
来源：http://yb.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://dn.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://ks.colortex.cn

C#:   list.Contains(x)
来源：http://jr.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://vi.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wm.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rp.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ti.huixiangedu.cn

TS:   [...arr];
来源：http://ar.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://mt.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://if.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://yb.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://br.haigaiapp.cn

[D23] reduce 累积计算
来源：http://wj.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oj.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jg.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iu.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://su.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ss.shtwfgs.cn

Go:   // 手写循环
来源：http://ph.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://os.chemitech.net.cn


<!-- 参考信息 -->