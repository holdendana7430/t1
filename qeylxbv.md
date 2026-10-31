代发 wailian999

Py:   return a, b
来源：http://lt.gzmigu.cn

PHP:  return [$a, $b];
来源：http://qd.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ci.szsharing.cn

TS:   return { a, b };
来源：http://sl.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lp.jianghongdianzi.cn

Go:   return a, b
来源：http://ox.newstarts.cn

Ruby: return a, b
来源：http://lm.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://yp.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://ga.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://xi.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ab.nszjky.cn

JS:   const square = x => x * x;
来源：http://dg.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://xr.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ka.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://az.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://jl.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hj.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://fl.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qr.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://em.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qj.521024.cn

TS:   arr.map(String)
来源：http://dr.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://up.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jp.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://qa.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qo.gzmigu.cn

[C08] 闭包
来源：http://uv.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yf.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ep.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qn.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nc.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ij.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cz.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://il.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ig.wgjwhj.cn

[C09] 递归
来源：http://sx.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ix.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lv.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gd.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gd.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sj.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kt.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rt.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hs.panjiajie.cn

[C10] 变量作用域
来源：http://nh.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dm.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hd.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lo.hnjuh.cn

TS:   同 JS
来源：http://je.newstarts.cn

Java: 方法内为块级作用域
来源：http://he.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://gg.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ba.yuexingan06.cn

C#:   块级作用域
来源：http://of.szxytkj.cn

[C11] 模块导入与导出
来源：http://cn.yuntaijiaju.cn

Py:   from module import func
来源：http://lo.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pa.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nc.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pw.huixinmuqiang.cn

Java: import java.util.List;
来源：http://yb.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cu.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://jp.nszjky.cn

C#:   using System.Text;
来源：http://le.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://ur.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://rg.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://hs.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://aw.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://nc.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yw.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://xc.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://jq.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rs.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://la.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bv.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sj.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wg.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ai.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xm.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://hs.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fo.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://by.hahajie.cn

[C14] 泛型函数
来源：http://ft.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://li.shxzskj.cn

PHP:  // 无泛型
来源：http://ij.lnxyls.cn

JS:   // 无泛型
来源：http://tq.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pe.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xi.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xc.colortex.cn

Ruby: # 无泛型
来源：http://qv.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rz.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://dy.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mn.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://oc.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xi.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ju.wgjwhj.cn

Java: // 无解构
来源：http://wi.asd995.cn

Go:   // 无解构
来源：http://fm.lnxyls.cn

Ruby: a, b = pair
来源：http://ch.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://tv.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://fj.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hr.huanxung.cn

PHP:  // 无重载
来源：http://jq.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ws.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://za.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tr.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://fh.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://ix.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wc.nicolike.cn

================================================================================
来源：http://gm.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://yx.lnxyls.cn

================================================================================
来源：http://on.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://xf.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oo.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ho.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ya.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uv.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vj.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ph.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://mm.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dr.nicolike.cn

[D02] 追加元素到末尾
来源：http://tf.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dq.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pk.nicolike.cn

JS:   arr.push(4);
来源：http://cf.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://xe.newstarts.cn

Java: list.add(4);
来源：http://pw.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://xr.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://dw.hahajie.cn

C#:   list.Add(4);
来源：http://zc.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://av.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://ux.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kn.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bj.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://kw.huanxung.cn

Java: list.add(0, 0);
来源：http://mn.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vq.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rx.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://qh.huanxung.cn

[D04] 删除元素
来源：http://ru.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zs.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bq.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ka.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://gc.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ws.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dt.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cm.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hg.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://xx.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xp.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bg.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rk.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://hw.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ku.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://if.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ra.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eb.colortex.cn

[D06] 数组长度
来源：http://nu.szsharing.cn

Py:   len(arr)
来源：http://sa.haigaiapp.cn

PHP:  count($arr);
来源：http://do.521024.cn

JS:   arr.length
来源：http://fk.jctech888.com.cn

TS:   arr.length
来源：http://zg.hnjuh.cn

Java: list.size();
来源：http://pn.jctech888.com.cn

Go:   len(arr)
来源：http://pm.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://yu.521024.cn

C#:   list.Count;
来源：http://rq.521024.cn

[D07] 切片 / 取子数组
来源：http://ds.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nd.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lu.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://xc.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://kk.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://ua.huanxung.cn

Go:   arr[1:4]
来源：http://aa.nicolike.cn

Ruby: arr[1, 3]
来源：http://jq.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://wy.jctech888.com.cn

[D08] 合并两个数组
来源：http://ok.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://iy.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://ig.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yq.gzmigu.cn

TS:   [...a, ...b];
来源：http://ve.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fa.jctech888.com.cn

Go:   append(a, b...)
来源：http://lh.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://mg.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://vu.wgjwhj.cn

[D09] 排序（升序）
来源：http://ns.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://jy.chemitech.net.cn

PHP:  sort($arr);
来源：http://ej.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zl.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jg.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ig.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uh.wgjwhj.cn

Ruby: arr.sort
来源：http://zn.szsharing.cn

C#:   list.Sort();
来源：http://pq.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pv.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://es.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zg.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yx.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://az.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://at.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://it.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pb.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://km.yuntaijiaju.cn

[D11] 反转数组
来源：http://jy.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wp.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://kh.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vs.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://um.shxzukj.cn

Java: Collections.reverse(list);
来源：http://gp.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://kk.gzmigu.cn

Ruby: arr.reverse
来源：http://zu.9csxet.cn

C#:   list.Reverse();
来源：http://gh.muxihuayi.cn

[D12] 查找元素下标
来源：http://fl.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://iq.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://so.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mi.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lc.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mn.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://sg.haigaiapp.cn

Ruby: arr.index(x)
来源：http://kg.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://vz.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://gn.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sy.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wy.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://zk.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://yv.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ds.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vi.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xh.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lu.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://xm.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ne.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ji.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://pa.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://xo.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ks.hahajie.cn

Go:   // 手写循环
来源：http://rr.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vh.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jf.yuexingan06.cn

[D15] 去重
来源：http://bl.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vj.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://qs.hahajie.cn

JS:   [...new Set(arr)]
来源：http://gc.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://ta.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hg.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tb.wgjwhj.cn

Ruby: arr.uniq
来源：http://mn.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://uf.nicolike.cn

[D16] 求和与平均值
来源：http://wv.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ig.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://so.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dc.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qa.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ib.9csxet.cn

Go:   // 手写循环累加
来源：http://oz.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zi.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://wh.szsharing.cn

[D17] 最大值与最小值
来源：http://rx.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://yy.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://uh.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cg.nszjky.cn

TS:   Math.max(...arr);
来源：http://cg.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://to.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ar.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://yi.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://nu.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://qr.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lc.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://bf.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gj.panjiajie.cn

TS:   nested.flat();
来源：http://qo.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mj.gzmigu.cn

Go:   // 手写双层循环
来源：http://gs.huixiangedu.cn

Ruby: nested.flatten
来源：http://sb.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ak.jctech888.com.cn

[D19] 按字段分组
来源：http://qd.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://va.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vc.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wn.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fc.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rv.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://ji.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ka.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uy.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://qo.9csxet.cn

Py:   Counter(arr)
来源：http://yj.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://dl.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vi.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ta.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ox.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://rc.shxzukj.cn

Ruby: arr.tally
来源：http://vh.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xs.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://bp.bjjhwx.cn

Py:   x in arr
来源：http://fh.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://mg.nszjky.cn

JS:   arr.includes(x)
来源：http://mf.szsharing.cn

TS:   arr.includes(x)
来源：http://bv.huixiangedu.cn

Java: list.contains(x)
来源：http://yn.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://hv.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://ny.haigaiapp.cn

C#:   list.Contains(x)
来源：http://jg.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://mr.yuexingan06.cn


<!-- 参考信息 -->