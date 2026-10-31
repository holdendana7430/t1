代发 wailian999

Py:   return a, b
来源：http://ae.szxytkj.cn

PHP:  return [$a, $b];
来源：http://ii.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tj.shxzskj.cn

TS:   return { a, b };
来源：http://xd.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vh.asd995.cn

Go:   return a, b
来源：http://he.jctech888.com.cn

Ruby: return a, b
来源：http://zw.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://cp.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://bm.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://uv.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sz.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://pw.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://kz.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bf.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vy.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://uy.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oc.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://eq.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fz.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nn.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ra.chemitech.net.cn

TS:   arr.map(String)
来源：http://sb.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ah.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qh.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://fl.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sa.colortex.cn

[C08] 闭包
来源：http://yk.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pi.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://um.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qb.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bp.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lx.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sy.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rx.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qb.panjiajie.cn

[C09] 递归
来源：http://ww.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cp.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sl.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ie.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zo.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://az.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wb.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gu.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://me.jianghongdianzi.cn

[C10] 变量作用域
来源：http://zk.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zv.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ox.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uw.szxytkj.cn

TS:   同 JS
来源：http://tq.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://bs.shxzskj.cn

Go:   花括号块级作用域
来源：http://xo.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zl.9csxet.cn

C#:   块级作用域
来源：http://ua.shtwfgs.cn

[C11] 模块导入与导出
来源：http://mf.huixiangedu.cn

Py:   from module import func
来源：http://em.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sy.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ck.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xi.chemitech.net.cn

Java: import java.util.List;
来源：http://ry.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jm.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ay.haigaiapp.cn

C#:   using System.Text;
来源：http://lq.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://oc.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://gi.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://la.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://zd.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ke.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vs.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://lc.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://nw.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://by.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://gf.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hj.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xt.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xb.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dd.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bp.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://vk.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://un.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fv.panjiajie.cn

[C14] 泛型函数
来源：http://sz.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kn.newstarts.cn

PHP:  // 无泛型
来源：http://cb.shxzskj.cn

JS:   // 无泛型
来源：http://iz.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sr.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ei.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lx.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://hp.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fz.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://fu.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zp.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://dq.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bv.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qd.yuexingan06.cn

Java: // 无解构
来源：http://pq.newstarts.cn

Go:   // 无解构
来源：http://xd.lnxyls.cn

Ruby: a, b = pair
来源：http://gs.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://ms.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://ho.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ly.wgjwhj.cn

PHP:  // 无重载
来源：http://si.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ny.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://qb.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://or.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://mu.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://si.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://op.bjjhwx.cn

================================================================================
来源：http://ue.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://wa.szsharing.cn

================================================================================
来源：http://dn.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://wq.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nr.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xl.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vk.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oc.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oq.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://ni.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://pk.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bw.lnxyls.cn

[D02] 追加元素到末尾
来源：http://kv.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nm.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ll.hnjuh.cn

JS:   arr.push(4);
来源：http://ht.jctech888.com.cn

TS:   arr.push(4);
来源：http://zd.lnxyls.cn

Java: list.add(4);
来源：http://jo.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://ot.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://hp.hnjuh.cn

C#:   list.Add(4);
来源：http://le.hahajie.cn

[D03] 在指定位置插入元素
来源：http://gv.colortex.cn

Py:   arr.insert(0, 0)
来源：http://ho.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jk.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tr.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://mt.wgjwhj.cn

Java: list.add(0, 0);
来源：http://lj.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wz.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vd.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://gg.newstarts.cn

[D04] 删除元素
来源：http://oi.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://au.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mk.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gi.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://to.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://an.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tg.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ck.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://to.haigaiapp.cn

[D05] 访问与修改元素
来源：http://lh.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kx.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yo.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pu.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://wr.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://im.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ej.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bt.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wg.haigaiapp.cn

[D06] 数组长度
来源：http://tz.gzmigu.cn

Py:   len(arr)
来源：http://ar.jianghongdianzi.cn

PHP:  count($arr);
来源：http://al.nicolike.cn

JS:   arr.length
来源：http://lp.huixinmuqiang.cn

TS:   arr.length
来源：http://su.huixiangedu.cn

Java: list.size();
来源：http://by.szxytkj.cn

Go:   len(arr)
来源：http://uh.asd995.cn

Ruby: arr.length; arr.size
来源：http://ip.nicolike.cn

C#:   list.Count;
来源：http://xt.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://ad.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://um.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eg.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://uk.521024.cn

TS:   arr.slice(1, 4);
来源：http://ji.szxytkj.cn

Java: list.subList(1, 4);
来源：http://se.newstarts.cn

Go:   arr[1:4]
来源：http://zz.szsharing.cn

Ruby: arr[1, 3]
来源：http://gn.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://vk.shxzskj.cn

[D08] 合并两个数组
来源：http://ce.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://ci.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://bc.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ny.szsharing.cn

TS:   [...a, ...b];
来源：http://dn.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ho.521024.cn

Go:   append(a, b...)
来源：http://kj.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://yr.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://sz.521024.cn

[D09] 排序（升序）
来源：http://oe.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://ep.yuexingan06.cn

PHP:  sort($arr);
来源：http://gn.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zn.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wk.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pw.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gd.chemitech.net.cn

Ruby: arr.sort
来源：http://kb.wgjwhj.cn

C#:   list.Sort();
来源：http://zj.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ow.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tc.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ik.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://je.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kn.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nn.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ua.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gf.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lv.nszjky.cn

[D11] 反转数组
来源：http://jr.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gw.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://qd.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gx.shxzskj.cn

TS:   [...arr].reverse();
来源：http://op.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://pg.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://za.colortex.cn

Ruby: arr.reverse
来源：http://po.jctech888.com.cn

C#:   list.Reverse();
来源：http://tf.wgjwhj.cn

[D12] 查找元素下标
来源：http://er.521024.cn

Py:   arr.index(x);  x in arr
来源：http://vh.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xe.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ag.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iw.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://on.colortex.cn

Go:   slices.Index(arr, x)
来源：http://oh.szxytkj.cn

Ruby: arr.index(x)
来源：http://et.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://bt.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://ni.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://db.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://er.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://cg.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oe.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sq.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vu.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fe.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://so.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fc.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fi.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://gf.521024.cn

TS:   arr.map(x => x * 2)
来源：http://ek.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ac.huixinmuqiang.cn

Go:   // 手写循环
来源：http://dm.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hl.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ag.wgjwhj.cn

[D15] 去重
来源：http://hf.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lb.szsharing.cn

PHP:  array_unique($arr);
来源：http://xh.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://yy.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://rn.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xi.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yd.huanxung.cn

Ruby: arr.uniq
来源：http://vt.colortex.cn

C#:   list.Distinct().ToList()
来源：http://it.bjjhwx.cn

[D16] 求和与平均值
来源：http://su.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ly.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yt.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://np.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qj.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qz.shtwfgs.cn

Go:   // 手写循环累加
来源：http://sn.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ab.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://pu.gzmigu.cn

[D17] 最大值与最小值
来源：http://ub.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://ve.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://jv.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ej.hahajie.cn

TS:   Math.max(...arr);
来源：http://pn.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nc.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gd.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://rh.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://bt.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://xa.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xg.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://xz.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pu.yuntaijiaju.cn

TS:   nested.flat();
来源：http://dx.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zr.haigaiapp.cn

Go:   // 手写双层循环
来源：http://hy.haigaiapp.cn

Ruby: nested.flatten
来源：http://re.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ud.panjiajie.cn

[D19] 按字段分组
来源：http://qc.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sl.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://it.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ov.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sj.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oe.521024.cn

Go:   // 手写 map[string][]T
来源：http://ic.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bf.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gd.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://qn.wgjwhj.cn

Py:   Counter(arr)
来源：http://qv.521024.cn

PHP:  array_count_values($arr);
来源：http://el.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vs.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ze.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oj.szsharing.cn

Go:   // 手写 map[T]int
来源：http://bo.gzmigu.cn

Ruby: arr.tally
来源：http://qy.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://to.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://go.9csxet.cn

Py:   x in arr
来源：http://rx.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://xf.9csxet.cn

JS:   arr.includes(x)
来源：http://bf.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://xy.huanxung.cn

Java: list.contains(x)
来源：http://kq.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://fm.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://ez.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://nk.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://gp.521024.cn


<!-- 参考信息 -->