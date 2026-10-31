代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://zk.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pd.szxytkj.cn

Java: import java.util.List;
来源：http://vn.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fk.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://yj.wgjwhj.cn

C#:   using System.Text;
来源：http://uz.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://nd.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://kv.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://dh.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://vl.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://el.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lf.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://nw.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://nj.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uj.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://lu.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uv.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vt.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jw.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ro.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zw.9csxet.cn

Go:   func add(a, b int) int
来源：http://zz.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qp.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zx.nszjky.cn

[C14] 泛型函数
来源：http://ii.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rn.521024.cn

PHP:  // 无泛型
来源：http://wc.gzmigu.cn

JS:   // 无泛型
来源：http://fa.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kw.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mt.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ol.gzmigu.cn

Ruby: # 无泛型
来源：http://gw.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ph.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://at.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zh.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://jr.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://so.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cn.asd995.cn

Java: // 无解构
来源：http://dd.shxzukj.cn

Go:   // 无解构
来源：http://fb.szxytkj.cn

Ruby: a, b = pair
来源：http://xk.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://cp.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://du.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kk.hnjuh.cn

PHP:  // 无重载
来源：http://of.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ln.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://zd.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fv.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://yl.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://ep.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xq.huixinmuqiang.cn

================================================================================
来源：http://ay.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://bu.yuexingan06.cn

================================================================================
来源：http://tz.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://ro.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fp.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rw.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bm.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wm.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mu.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://yd.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://va.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wb.panjiajie.cn

[D02] 追加元素到末尾
来源：http://to.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://us.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dj.huanxung.cn

JS:   arr.push(4);
来源：http://ym.huanxung.cn

TS:   arr.push(4);
来源：http://sy.newstarts.cn

Java: list.add(4);
来源：http://oq.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://vs.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://sx.huanxung.cn

C#:   list.Add(4);
来源：http://hb.newstarts.cn

[D03] 在指定位置插入元素
来源：http://fo.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://lg.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hx.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dv.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://ej.jctech888.com.cn

Java: list.add(0, 0);
来源：http://bn.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ug.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cx.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://ij.huixinmuqiang.cn

[D04] 删除元素
来源：http://pu.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pl.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gc.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jn.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://ip.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ge.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://js.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xk.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zt.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://wm.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jn.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://as.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kg.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://ke.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://sy.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://nm.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://th.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mf.muxihuayi.cn

[D06] 数组长度
来源：http://wi.jctech888.com.cn

Py:   len(arr)
来源：http://ey.wgjwhj.cn

PHP:  count($arr);
来源：http://ch.huixiangedu.cn

JS:   arr.length
来源：http://sl.bookmarksfly.cn

TS:   arr.length
来源：http://fm.huixinmuqiang.cn

Java: list.size();
来源：http://rz.jctech888.com.cn

Go:   len(arr)
来源：http://ua.newstarts.cn

Ruby: arr.length; arr.size
来源：http://eu.huixinmuqiang.cn

C#:   list.Count;
来源：http://js.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://ml.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kb.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mf.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://bm.colortex.cn

TS:   arr.slice(1, 4);
来源：http://nx.521024.cn

Java: list.subList(1, 4);
来源：http://fo.521024.cn

Go:   arr[1:4]
来源：http://dj.newstarts.cn

Ruby: arr[1, 3]
来源：http://eq.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://ia.huixiangedu.cn

[D08] 合并两个数组
来源：http://jl.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://jh.521024.cn

PHP:  array_merge($a, $b);
来源：http://ya.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pg.muxihuayi.cn

TS:   [...a, ...b];
来源：http://vj.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qx.newstarts.cn

Go:   append(a, b...)
来源：http://pa.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://fg.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://js.szsharing.cn

[D09] 排序（升序）
来源：http://qk.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://pp.hnjuh.cn

PHP:  sort($arr);
来源：http://ax.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xd.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vq.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xl.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vn.lnxyls.cn

Ruby: arr.sort
来源：http://lv.colortex.cn

C#:   list.Sort();
来源：http://zv.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://up.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://al.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mr.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://is.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bm.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jt.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gd.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ac.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gx.hnjuh.cn

[D11] 反转数组
来源：http://bc.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zs.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://xt.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rc.shxzukj.cn

TS:   [...arr].reverse();
来源：http://qk.colortex.cn

Java: Collections.reverse(list);
来源：http://xk.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://ig.huixiangedu.cn

Ruby: arr.reverse
来源：http://xy.9csxet.cn

C#:   list.Reverse();
来源：http://kf.wgjwhj.cn

[D12] 查找元素下标
来源：http://rm.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://yf.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ng.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aa.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://go.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cy.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://cs.wgjwhj.cn

Ruby: arr.index(x)
来源：http://zj.nszjky.cn

C#:   list.IndexOf(x);
来源：http://dg.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://dm.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zm.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dy.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://hg.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://rq.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yp.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kp.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nv.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zh.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://hi.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fd.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://br.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://gn.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://sh.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ta.hahajie.cn

Go:   // 手写循环
来源：http://jo.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mh.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ym.jianghongdianzi.cn

[D15] 去重
来源：http://qz.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mp.asd995.cn

PHP:  array_unique($arr);
来源：http://af.colortex.cn

JS:   [...new Set(arr)]
来源：http://le.9csxet.cn

TS:   [...new Set(arr)]
来源：http://ru.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iv.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lb.asd995.cn

Ruby: arr.uniq
来源：http://re.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://ea.muxihuayi.cn

[D16] 求和与平均值
来源：http://un.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pp.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xn.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pu.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uu.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://io.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://dd.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qt.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://kf.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://qw.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://ir.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://ru.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xa.panjiajie.cn

TS:   Math.max(...arr);
来源：http://xb.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://je.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gh.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://df.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://xi.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://qp.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yz.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://km.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ua.bookmarksfly.cn

TS:   nested.flat();
来源：http://zt.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yx.nszjky.cn

Go:   // 手写双层循环
来源：http://du.hahajie.cn

Ruby: nested.flatten
来源：http://up.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ze.szsharing.cn

[D19] 按字段分组
来源：http://ui.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dz.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nb.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qo.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tb.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://ih.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ji.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nj.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://ft.yuexingan06.cn

Py:   Counter(arr)
来源：http://eo.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://ri.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cr.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hf.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ua.asd995.cn

Go:   // 手写 map[T]int
来源：http://nc.haigaiapp.cn

Ruby: arr.tally
来源：http://af.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yq.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://qk.asd995.cn

Py:   x in arr
来源：http://ev.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://uk.haigaiapp.cn

JS:   arr.includes(x)
来源：http://il.lnxyls.cn

TS:   arr.includes(x)
来源：http://ll.9csxet.cn

Java: list.contains(x)
来源：http://ir.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://bw.9csxet.cn

Ruby: arr.include?(x)
来源：http://ta.huixiangedu.cn

C#:   list.Contains(x)
来源：http://qe.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://iz.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://to.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://es.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xv.chemitech.net.cn

TS:   [...arr];
来源：http://iw.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://qe.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vc.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://hp.panjiajie.cn

C#:   new List<int>(list);
来源：http://hy.hnjuh.cn

[D23] reduce 累积计算
来源：http://nt.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gl.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ao.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://io.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sq.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ez.hahajie.cn

Go:   // 手写循环
来源：http://gd.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ch.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ov.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://yo.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://em.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eu.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kz.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://la.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cp.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vj.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gy.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vv.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://bd.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ge.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ka.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wb.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lo.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yf.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nx.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rg.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://le.521024.cn

[D26] 数组转字符串
来源：http://oc.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://jm.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://ox.huanxung.cn

JS:   arr.join(", ")
来源：http://uk.colortex.cn

TS:   arr.join(", ")
来源：http://xd.shxzskj.cn

Java: String.join(", ", list)
来源：http://du.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://ld.nszjky.cn

Ruby: arr.join(", ")
来源：http://yg.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://kq.9csxet.cn

================================================================================
来源：http://og.szxytkj.cn

E. 字符串处理
来源：http://hp.panjiajie.cn

================================================================================
来源：http://pm.shxzskj.cn

[E01] 拼接字符串
来源：http://wt.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ir.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dy.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://it.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yi.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nt.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wa.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sf.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bn.gzmigu.cn


<!-- 参考信息 -->