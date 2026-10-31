代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tm.gzmigu.cn

Go:   return a, b
来源：http://sm.nicolike.cn

Ruby: return a, b
来源：http://ym.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://hp.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://ms.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://jd.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://au.szxytkj.cn

JS:   const square = x => x * x;
来源：http://jz.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://js.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nt.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mc.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://qn.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lr.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://qf.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mn.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lq.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wi.nicolike.cn

TS:   arr.map(String)
来源：http://eh.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xh.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jq.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://sb.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bo.shxzukj.cn

[C08] 闭包
来源：http://fj.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wy.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xj.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pb.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dk.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xu.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bk.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dh.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zg.hnjuh.cn

[C09] 递归
来源：http://bi.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ny.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dy.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vh.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ux.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nh.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://il.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://il.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kq.szsharing.cn

[C10] 变量作用域
来源：http://pm.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ez.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mj.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nh.shtwfgs.cn

TS:   同 JS
来源：http://zq.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://mc.huanxung.cn

Go:   花括号块级作用域
来源：http://yh.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ko.muxihuayi.cn

C#:   块级作用域
来源：http://eb.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://ke.newstarts.cn

Py:   from module import func
来源：http://qx.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wb.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ny.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nd.hnjuh.cn

Java: import java.util.List;
来源：http://rg.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zl.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://xg.huixinmuqiang.cn

C#:   using System.Text;
来源：http://mt.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://nb.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://be.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://hj.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://jq.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://kb.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jt.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://cp.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://gw.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bb.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://lq.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eo.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ic.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zg.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yl.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ma.panjiajie.cn

Go:   func add(a, b int) int
来源：http://ee.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zm.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vz.newstarts.cn

[C14] 泛型函数
来源：http://tg.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fh.colortex.cn

PHP:  // 无泛型
来源：http://ec.asd995.cn

JS:   // 无泛型
来源：http://fx.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ov.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aj.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fq.nszjky.cn

Ruby: # 无泛型
来源：http://ih.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yo.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://aw.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://js.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://pi.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://of.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cx.wgjwhj.cn

Java: // 无解构
来源：http://wy.haigaiapp.cn

Go:   // 无解构
来源：http://kr.szsharing.cn

Ruby: a, b = pair
来源：http://vz.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://fk.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://qc.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fw.huanxung.cn

PHP:  // 无重载
来源：http://kl.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lm.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://fl.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sd.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://fa.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://su.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://th.bjjhwx.cn

================================================================================
来源：http://ce.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://cz.hahajie.cn

================================================================================
来源：http://bj.9csxet.cn

[D01] 创建数组 / 列表
来源：http://ot.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rm.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dm.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vg.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fd.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jn.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://bx.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://sq.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dg.hnjuh.cn

[D02] 追加元素到末尾
来源：http://ok.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gf.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tz.521024.cn

JS:   arr.push(4);
来源：http://cs.asd995.cn

TS:   arr.push(4);
来源：http://ou.521024.cn

Java: list.add(4);
来源：http://ug.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://dj.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://nn.bjjhwx.cn

C#:   list.Add(4);
来源：http://gz.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://aj.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://es.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://us.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ma.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://io.szxytkj.cn

Java: list.add(0, 0);
来源：http://ek.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://og.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ir.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://ws.lnxyls.cn

[D04] 删除元素
来源：http://oz.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qt.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gp.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ks.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://af.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cs.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ji.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yq.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mi.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://bn.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ih.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vv.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kk.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://py.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://mm.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://uk.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kh.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mx.hnjuh.cn

[D06] 数组长度
来源：http://gi.bookmarksfly.cn

Py:   len(arr)
来源：http://vp.yuntaijiaju.cn

PHP:  count($arr);
来源：http://ki.9csxet.cn

JS:   arr.length
来源：http://jz.bookmarksfly.cn

TS:   arr.length
来源：http://hs.panjiajie.cn

Java: list.size();
来源：http://uk.jctech888.com.cn

Go:   len(arr)
来源：http://ao.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://fd.yuntaijiaju.cn

C#:   list.Count;
来源：http://fl.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://ne.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wl.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mq.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://pv.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://ci.panjiajie.cn

Java: list.subList(1, 4);
来源：http://qd.yuexingan06.cn

Go:   arr[1:4]
来源：http://uj.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://tq.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://mt.bjjhwx.cn

[D08] 合并两个数组
来源：http://yb.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://ii.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://sh.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vm.asd995.cn

TS:   [...a, ...b];
来源：http://rz.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kn.colortex.cn

Go:   append(a, b...)
来源：http://ra.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://ar.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://ke.nicolike.cn

[D09] 排序（升序）
来源：http://gb.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://iv.9csxet.cn

PHP:  sort($arr);
来源：http://ah.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://px.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jx.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://si.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://av.jctech888.com.cn

Ruby: arr.sort
来源：http://vv.muxihuayi.cn

C#:   list.Sort();
来源：http://an.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://db.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://or.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sz.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pq.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ig.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nj.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fh.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nb.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bz.hnjuh.cn

[D11] 反转数组
来源：http://xw.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qp.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://ja.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ee.huanxung.cn

TS:   [...arr].reverse();
来源：http://xb.colortex.cn

Java: Collections.reverse(list);
来源：http://lt.colortex.cn

Go:   slices.Reverse(arr)
来源：http://io.521024.cn

Ruby: arr.reverse
来源：http://ap.asd995.cn

C#:   list.Reverse();
来源：http://qi.9csxet.cn

[D12] 查找元素下标
来源：http://hg.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://cf.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sw.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rq.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dh.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ft.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://et.shxzukj.cn

Ruby: arr.index(x)
来源：http://es.huanxung.cn

C#:   list.IndexOf(x);
来源：http://pc.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://vb.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ov.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ox.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://qd.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://tq.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ru.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://io.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kb.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hq.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://sa.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hp.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cp.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://je.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://fz.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ju.shtwfgs.cn

Go:   // 手写循环
来源：http://ax.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nh.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://el.hahajie.cn

[D15] 去重
来源：http://zk.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jb.gzmigu.cn

PHP:  array_unique($arr);
来源：http://os.huanxung.cn

JS:   [...new Set(arr)]
来源：http://th.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://xh.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kj.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fz.wgjwhj.cn

Ruby: arr.uniq
来源：http://sa.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://qm.muxihuayi.cn

[D16] 求和与平均值
来源：http://pd.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hv.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kg.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oe.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ju.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mq.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://yj.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ea.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://qq.gzmigu.cn

[D17] 最大值与最小值
来源：http://kg.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://en.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://qa.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wo.hnjuh.cn

TS:   Math.max(...arr);
来源：http://yd.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://an.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lj.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://zo.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://em.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://pn.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://va.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://zq.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xb.asd995.cn

TS:   nested.flat();
来源：http://iu.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ox.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://ue.szsharing.cn

Ruby: nested.flatten
来源：http://bc.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pr.521024.cn

[D19] 按字段分组
来源：http://pv.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://su.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://np.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nf.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mx.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oi.521024.cn

Go:   // 手写 map[string][]T
来源：http://zy.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cw.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vm.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://nq.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://ya.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://le.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vn.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mc.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zb.hahajie.cn

Go:   // 手写 map[T]int
来源：http://zm.521024.cn

Ruby: arr.tally
来源：http://gf.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://em.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://qy.colortex.cn

Py:   x in arr
来源：http://go.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://ev.shxzskj.cn

JS:   arr.includes(x)
来源：http://iz.muxihuayi.cn

TS:   arr.includes(x)
来源：http://ou.yuexingan06.cn

Java: list.contains(x)
来源：http://jl.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://qe.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://az.bjjhwx.cn

C#:   list.Contains(x)
来源：http://bl.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://vo.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://do.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dj.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ap.huixiangedu.cn

TS:   [...arr];
来源：http://gk.nicolike.cn


<!-- 参考信息 -->