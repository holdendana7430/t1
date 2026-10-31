代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://ed.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gq.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hv.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://uu.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eu.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://ju.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nh.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uk.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dt.haigaiapp.cn

TS:   arr.map(String)
来源：http://cg.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zq.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cw.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://ns.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://il.9csxet.cn

[C08] 闭包
来源：http://yv.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://na.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wo.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hi.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nm.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qn.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xc.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bk.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vi.nicolike.cn

[C09] 递归
来源：http://yf.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nb.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rl.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oe.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xs.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bd.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://am.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://br.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qr.chemitech.net.cn

[C10] 变量作用域
来源：http://jx.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qc.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ke.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ea.szsharing.cn

TS:   同 JS
来源：http://mk.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://fr.gzmigu.cn

Go:   花括号块级作用域
来源：http://yb.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vx.lnxyls.cn

C#:   块级作用域
来源：http://dq.chemitech.net.cn

[C11] 模块导入与导出
来源：http://al.shtwfgs.cn

Py:   from module import func
来源：http://ya.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gj.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ez.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ip.nszjky.cn

Java: import java.util.List;
来源：http://pa.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tk.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://ma.szxytkj.cn

C#:   using System.Text;
来源：http://ho.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://qp.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://wl.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://jy.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://jm.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://gz.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zn.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://sl.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://ao.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sd.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://xp.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yt.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://va.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gk.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dt.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jd.huanxung.cn

Go:   func add(a, b int) int
来源：http://lj.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pl.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nb.hahajie.cn

[C14] 泛型函数
来源：http://zz.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ch.szxytkj.cn

PHP:  // 无泛型
来源：http://xh.jctech888.com.cn

JS:   // 无泛型
来源：http://fm.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zi.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ou.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vg.panjiajie.cn

Ruby: # 无泛型
来源：http://gn.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zb.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://rj.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ml.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://jf.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dt.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bm.hahajie.cn

Java: // 无解构
来源：http://xg.muxihuayi.cn

Go:   // 无解构
来源：http://uf.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://wi.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://sh.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://kp.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qt.yuntaijiaju.cn

PHP:  // 无重载
来源：http://ts.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ni.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://bg.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://js.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://zu.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://qm.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tc.yuntaijiaju.cn

================================================================================
来源：http://ol.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://gj.haigaiapp.cn

================================================================================
来源：http://mo.521024.cn

[D01] 创建数组 / 列表
来源：http://uo.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rj.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sw.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ie.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bu.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zu.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://wo.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://nl.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fu.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://gg.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fz.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lw.newstarts.cn

JS:   arr.push(4);
来源：http://kr.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://ww.hahajie.cn

Java: list.add(4);
来源：http://os.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://gh.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://sd.asd995.cn

C#:   list.Add(4);
来源：http://vk.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://hb.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://zw.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bk.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zp.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://wg.shxzukj.cn

Java: list.add(0, 0);
来源：http://rs.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nc.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yx.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://zy.colortex.cn

[D04] 删除元素
来源：http://nr.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ni.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hf.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yn.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://de.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nu.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ws.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://is.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lw.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://yj.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gz.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gi.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qb.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://gz.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://tz.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://ov.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://na.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hd.huanxung.cn

[D06] 数组长度
来源：http://kl.hahajie.cn

Py:   len(arr)
来源：http://ej.yuexingan06.cn

PHP:  count($arr);
来源：http://nz.huixiangedu.cn

JS:   arr.length
来源：http://pz.lnxyls.cn

TS:   arr.length
来源：http://kk.nszjky.cn

Java: list.size();
来源：http://qd.bjjhwx.cn

Go:   len(arr)
来源：http://tw.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://js.muxihuayi.cn

C#:   list.Count;
来源：http://ki.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://et.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ch.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pl.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://ni.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://tk.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://vg.hahajie.cn

Go:   arr[1:4]
来源：http://gj.gzmigu.cn

Ruby: arr[1, 3]
来源：http://hy.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://pv.haigaiapp.cn

[D08] 合并两个数组
来源：http://lj.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://be.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://eq.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oj.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://ux.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fn.shxzskj.cn

Go:   append(a, b...)
来源：http://oo.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://mj.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://fu.shxzskj.cn

[D09] 排序（升序）
来源：http://hd.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://qx.huanxung.cn

PHP:  sort($arr);
来源：http://oh.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wt.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://za.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xs.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nj.wgjwhj.cn

Ruby: arr.sort
来源：http://or.nicolike.cn

C#:   list.Sort();
来源：http://ku.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xt.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pe.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vb.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dc.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xy.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pr.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vm.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cx.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tt.haigaiapp.cn

[D11] 反转数组
来源：http://uk.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xw.9csxet.cn

PHP:  array_reverse($arr);
来源：http://th.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aq.lnxyls.cn

TS:   [...arr].reverse();
来源：http://bj.9csxet.cn

Java: Collections.reverse(list);
来源：http://pr.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://cr.shxzskj.cn

Ruby: arr.reverse
来源：http://hh.lnxyls.cn

C#:   list.Reverse();
来源：http://sd.9csxet.cn

[D12] 查找元素下标
来源：http://kg.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://nm.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://om.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aw.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cz.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dr.colortex.cn

Go:   slices.Index(arr, x)
来源：http://bw.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://ve.nszjky.cn

C#:   list.IndexOf(x);
来源：http://gw.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://gf.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ta.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gw.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://eh.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://fb.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rw.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qv.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tv.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uj.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://bz.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ca.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sp.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://ws.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://uh.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lt.colortex.cn

Go:   // 手写循环
来源：http://sl.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iq.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fa.muxihuayi.cn

[D15] 去重
来源：http://rd.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fl.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://tq.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://lu.9csxet.cn

TS:   [...new Set(arr)]
来源：http://tk.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uj.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pi.bookmarksfly.cn

Ruby: arr.uniq
来源：http://ep.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://yz.chemitech.net.cn

[D16] 求和与平均值
来源：http://eh.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://it.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://du.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ts.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fr.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sb.hnjuh.cn

Go:   // 手写循环累加
来源：http://un.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dt.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://mh.9csxet.cn

[D17] 最大值与最小值
来源：http://xs.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://mq.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://py.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qu.shxzskj.cn

TS:   Math.max(...arr);
来源：http://si.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sm.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zz.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://ms.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://gg.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://xc.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pw.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://jg.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ul.asd995.cn

TS:   nested.flat();
来源：http://ra.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xd.lnxyls.cn

Go:   // 手写双层循环
来源：http://hf.shxzukj.cn

Ruby: nested.flatten
来源：http://yh.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tt.yuexingan06.cn

[D19] 按字段分组
来源：http://um.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jb.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wo.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yg.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bq.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zv.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://hk.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ei.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cl.asd995.cn

[D20] 统计每个元素出现次数
来源：http://fl.nszjky.cn

Py:   Counter(arr)
来源：http://ub.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://ol.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rc.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ht.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fl.szsharing.cn

Go:   // 手写 map[T]int
来源：http://ae.gzmigu.cn

Ruby: arr.tally
来源：http://ib.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uy.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://rf.bjjhwx.cn

Py:   x in arr
来源：http://gg.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://vd.wgjwhj.cn

JS:   arr.includes(x)
来源：http://fh.shtwfgs.cn

TS:   arr.includes(x)
来源：http://br.shxzskj.cn

Java: list.contains(x)
来源：http://jl.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://on.panjiajie.cn

Ruby: arr.include?(x)
来源：http://jc.bjjhwx.cn

C#:   list.Contains(x)
来源：http://nh.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://vr.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tz.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bm.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bv.lnxyls.cn

TS:   [...arr];
来源：http://xp.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://qm.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://id.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://tc.wgjwhj.cn

C#:   new List<int>(list);
来源：http://up.shxzskj.cn

[D23] reduce 累积计算
来源：http://jz.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hd.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://au.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ml.yuntaijiaju.cn


<!-- 参考信息 -->