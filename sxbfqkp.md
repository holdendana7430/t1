代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://zq.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://he.nszjky.cn

[C08] 闭包
来源：http://by.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mc.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gq.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fz.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cr.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://po.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ie.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ix.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oh.colortex.cn

[C09] 递归
来源：http://nt.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sf.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zb.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ej.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ai.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kl.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bb.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kn.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kq.yuntaijiaju.cn

[C10] 变量作用域
来源：http://jo.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gh.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mk.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lw.shxzskj.cn

TS:   同 JS
来源：http://wk.asd995.cn

Java: 方法内为块级作用域
来源：http://gj.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://rk.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bo.9csxet.cn

C#:   块级作用域
来源：http://cf.jctech888.com.cn

[C11] 模块导入与导出
来源：http://kl.shtwfgs.cn

Py:   from module import func
来源：http://ox.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wa.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zk.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mq.jianghongdianzi.cn

Java: import java.util.List;
来源：http://ej.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ma.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://wy.yuexingan06.cn

C#:   using System.Text;
来源：http://gx.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://jy.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://rw.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://xi.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://kd.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://iy.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ez.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ca.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://ix.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ox.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://fq.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ux.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yq.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qm.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dq.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cv.gzmigu.cn

Go:   func add(a, b int) int
来源：http://gs.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://su.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://et.newstarts.cn

[C14] 泛型函数
来源：http://mt.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bx.gzmigu.cn

PHP:  // 无泛型
来源：http://cp.panjiajie.cn

JS:   // 无泛型
来源：http://my.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xl.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ae.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pr.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://vb.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bk.521024.cn

[C15] 解构 / 展开参数
来源：http://js.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uq.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://nd.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zy.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zy.shxzskj.cn

Java: // 无解构
来源：http://gc.haigaiapp.cn

Go:   // 无解构
来源：http://mu.muxihuayi.cn

Ruby: a, b = pair
来源：http://ne.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://hu.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://ak.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://da.9csxet.cn

PHP:  // 无重载
来源：http://dj.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sl.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ra.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zb.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://kn.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://ne.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rv.jianghongdianzi.cn

================================================================================
来源：http://gn.asd995.cn

D. 数组 / 列表 / 集合
来源：http://um.yuexingan06.cn

================================================================================
来源：http://xy.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://gx.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://az.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xd.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ri.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ut.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ou.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://to.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://bj.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qt.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://my.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kf.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nm.asd995.cn

JS:   arr.push(4);
来源：http://px.wgjwhj.cn

TS:   arr.push(4);
来源：http://bc.shxzskj.cn

Java: list.add(4);
来源：http://iu.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://fo.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://fr.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://yo.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://jq.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://fo.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gw.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fh.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://hw.haigaiapp.cn

Java: list.add(0, 0);
来源：http://pg.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vy.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yi.asd995.cn

C#:   list.Insert(0, 0);
来源：http://gm.yuntaijiaju.cn

[D04] 删除元素
来源：http://wy.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yh.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://st.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pl.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://qr.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pl.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wa.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oe.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mz.panjiajie.cn

[D05] 访问与修改元素
来源：http://pw.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ns.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vl.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mj.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://uv.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://oh.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://uu.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kr.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zj.newstarts.cn

[D06] 数组长度
来源：http://rl.lnxyls.cn

Py:   len(arr)
来源：http://vt.shtwfgs.cn

PHP:  count($arr);
来源：http://nx.521024.cn

JS:   arr.length
来源：http://nf.hahajie.cn

TS:   arr.length
来源：http://wa.hahajie.cn

Java: list.size();
来源：http://aq.huixiangedu.cn

Go:   len(arr)
来源：http://ky.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://lo.lnxyls.cn

C#:   list.Count;
来源：http://ly.nszjky.cn

[D07] 切片 / 取子数组
来源：http://kw.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bf.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://it.asd995.cn

JS:   arr.slice(1, 4);
来源：http://fr.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://xs.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://un.jctech888.com.cn

Go:   arr[1:4]
来源：http://fh.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://wk.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://tj.shxzskj.cn

[D08] 合并两个数组
来源：http://nq.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://rh.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://cu.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oy.newstarts.cn

TS:   [...a, ...b];
来源：http://ju.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vw.shxzskj.cn

Go:   append(a, b...)
来源：http://nv.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://xp.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://mh.lnxyls.cn

[D09] 排序（升序）
来源：http://dh.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://pk.nszjky.cn

PHP:  sort($arr);
来源：http://so.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wg.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vu.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://za.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rc.shxzukj.cn

Ruby: arr.sort
来源：http://so.szxytkj.cn

C#:   list.Sort();
来源：http://vq.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vb.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ni.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gn.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://it.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://up.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cv.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yh.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ac.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lz.gzmigu.cn

[D11] 反转数组
来源：http://iv.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zj.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://cs.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zp.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://kq.huanxung.cn

Java: Collections.reverse(list);
来源：http://bv.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://xz.haigaiapp.cn

Ruby: arr.reverse
来源：http://my.colortex.cn

C#:   list.Reverse();
来源：http://wt.nszjky.cn

[D12] 查找元素下标
来源：http://pv.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ru.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bq.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fj.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xz.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zh.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://rh.nicolike.cn

Ruby: arr.index(x)
来源：http://th.colortex.cn

C#:   list.IndexOf(x);
来源：http://hj.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://ll.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xo.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ob.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://sc.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://wm.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lk.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gz.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oi.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fh.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://mb.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qz.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ns.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://sw.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://ts.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sb.shxzukj.cn

Go:   // 手写循环
来源：http://uo.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ax.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vv.bjjhwx.cn

[D15] 去重
来源：http://ka.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gk.newstarts.cn

PHP:  array_unique($arr);
来源：http://lm.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://ap.asd995.cn

TS:   [...new Set(arr)]
来源：http://wu.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rz.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eh.huixiangedu.cn

Ruby: arr.uniq
来源：http://cd.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://qr.shxzskj.cn

[D16] 求和与平均值
来源：http://cz.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zq.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gj.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gk.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cb.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://op.shtwfgs.cn

Go:   // 手写循环累加
来源：http://yr.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gu.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://kc.szxytkj.cn

[D17] 最大值与最小值
来源：http://cb.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://xy.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://sg.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ez.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://ul.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ag.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nl.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://gx.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://ow.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://ce.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lg.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://jz.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gf.muxihuayi.cn

TS:   nested.flat();
来源：http://ub.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://df.bjjhwx.cn

Go:   // 手写双层循环
来源：http://wc.bjjhwx.cn

Ruby: nested.flatten
来源：http://ng.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vc.shxzskj.cn

[D19] 按字段分组
来源：http://tw.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lf.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fj.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jl.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rv.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ix.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://mo.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zn.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xd.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://jt.newstarts.cn

Py:   Counter(arr)
来源：http://os.szsharing.cn

PHP:  array_count_values($arr);
来源：http://sz.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wn.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rf.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ld.nszjky.cn

Go:   // 手写 map[T]int
来源：http://wx.huixiangedu.cn

Ruby: arr.tally
来源：http://fe.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aa.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://nc.9csxet.cn

Py:   x in arr
来源：http://yj.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://oc.asd995.cn

JS:   arr.includes(x)
来源：http://xh.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://jx.huixiangedu.cn

Java: list.contains(x)
来源：http://dr.521024.cn

Go:   slices.Contains(arr, x)
来源：http://vy.szsharing.cn

Ruby: arr.include?(x)
来源：http://zu.huixiangedu.cn

C#:   list.Contains(x)
来源：http://ju.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://dh.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wj.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rw.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://go.yuntaijiaju.cn

TS:   [...arr];
来源：http://dw.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://dk.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gc.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://aa.shxzskj.cn

C#:   new List<int>(list);
来源：http://th.bjjhwx.cn

[D23] reduce 累积计算
来源：http://yr.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qz.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ux.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://er.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ke.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pi.huixiangedu.cn

Go:   // 手写循环
来源：http://gn.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jh.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oa.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://mr.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://px.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://se.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bd.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://im.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ky.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zh.shxzukj.cn


<!-- 参考信息 -->