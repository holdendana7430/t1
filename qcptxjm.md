代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://fz.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yy.jctech888.com.cn

Java: import java.util.List;
来源：http://ij.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bw.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://gd.szsharing.cn

C#:   using System.Text;
来源：http://fp.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://jg.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://fx.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://zr.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://ur.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://to.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://an.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://hf.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://sk.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yh.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://px.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kn.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ro.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yh.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yb.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uh.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://jy.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ah.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://to.yuexingan06.cn

[C14] 泛型函数
来源：http://mw.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ay.bookmarksfly.cn

PHP:  // 无泛型
来源：http://so.wgjwhj.cn

JS:   // 无泛型
来源：http://yw.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nw.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mw.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://im.panjiajie.cn

Ruby: # 无泛型
来源：http://vm.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xj.huanxung.cn

[C15] 解构 / 展开参数
来源：http://ih.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://io.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://hz.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pt.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ml.yuexingan06.cn

Java: // 无解构
来源：http://eq.newstarts.cn

Go:   // 无解构
来源：http://oo.shtwfgs.cn

Ruby: a, b = pair
来源：http://aj.nicolike.cn

C#:   var (a, b) = pair;
来源：http://oj.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://rq.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zp.haigaiapp.cn

PHP:  // 无重载
来源：http://my.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ee.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://ao.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://es.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://gy.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://ur.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pq.haigaiapp.cn

================================================================================
来源：http://en.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://dl.nicolike.cn

================================================================================
来源：http://qs.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://xy.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wv.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ct.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cw.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://by.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ek.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://su.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://io.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uj.lnxyls.cn

[D02] 追加元素到末尾
来源：http://jd.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sl.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gz.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://fk.shxzukj.cn

TS:   arr.push(4);
来源：http://gw.yuexingan06.cn

Java: list.add(4);
来源：http://rq.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://eu.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://sq.jctech888.com.cn

C#:   list.Add(4);
来源：http://vi.521024.cn

[D03] 在指定位置插入元素
来源：http://kj.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://ad.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tj.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://if.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://tp.colortex.cn

Java: list.add(0, 0);
来源：http://xg.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://to.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nh.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://gp.yuntaijiaju.cn

[D04] 删除元素
来源：http://nf.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qc.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nd.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bp.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://hs.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jb.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hb.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mc.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ij.huanxung.cn

[D05] 访问与修改元素
来源：http://yu.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wf.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wn.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nq.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://ff.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://dr.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://fl.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ir.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wh.chemitech.net.cn

[D06] 数组长度
来源：http://ke.asd995.cn

Py:   len(arr)
来源：http://cl.jianghongdianzi.cn

PHP:  count($arr);
来源：http://px.jctech888.com.cn

JS:   arr.length
来源：http://xi.yuntaijiaju.cn

TS:   arr.length
来源：http://mm.shtwfgs.cn

Java: list.size();
来源：http://rt.9csxet.cn

Go:   len(arr)
来源：http://xs.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://ay.szsharing.cn

C#:   list.Count;
来源：http://rr.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://cq.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qd.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cn.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://oc.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://xc.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://xq.nicolike.cn

Go:   arr[1:4]
来源：http://ht.newstarts.cn

Ruby: arr[1, 3]
来源：http://dr.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://eo.yuexingan06.cn

[D08] 合并两个数组
来源：http://qd.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://xb.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://zm.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qd.shtwfgs.cn

TS:   [...a, ...b];
来源：http://mi.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uw.huanxung.cn

Go:   append(a, b...)
来源：http://rq.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://vp.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://ah.huixiangedu.cn

[D09] 排序（升序）
来源：http://nx.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ng.panjiajie.cn

PHP:  sort($arr);
来源：http://ph.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ae.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xe.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ut.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://di.jctech888.com.cn

Ruby: arr.sort
来源：http://ho.nszjky.cn

C#:   list.Sort();
来源：http://wi.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cp.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vb.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gn.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yh.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nb.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xq.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ex.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://in.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ur.szsharing.cn

[D11] 反转数组
来源：http://xp.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hc.nicolike.cn

PHP:  array_reverse($arr);
来源：http://wt.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://un.newstarts.cn

TS:   [...arr].reverse();
来源：http://sl.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://vc.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://zi.521024.cn

Ruby: arr.reverse
来源：http://bt.hnjuh.cn

C#:   list.Reverse();
来源：http://rg.chemitech.net.cn

[D12] 查找元素下标
来源：http://rc.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://yj.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ay.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lg.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gk.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://li.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://fy.hnjuh.cn

Ruby: arr.index(x)
来源：http://in.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://ju.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://bh.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nt.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lb.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://rh.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://wt.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fd.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sh.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sr.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qj.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://fk.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jp.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uh.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://dc.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://tv.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qs.gzmigu.cn

Go:   // 手写循环
来源：http://vv.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gt.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xg.shxzukj.cn

[D15] 去重
来源：http://io.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vp.521024.cn

PHP:  array_unique($arr);
来源：http://hg.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://ru.huanxung.cn

TS:   [...new Set(arr)]
来源：http://sk.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ya.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ju.wgjwhj.cn

Ruby: arr.uniq
来源：http://fp.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://cu.panjiajie.cn

[D16] 求和与平均值
来源：http://lx.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ls.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ky.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sj.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pm.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rh.panjiajie.cn

Go:   // 手写循环累加
来源：http://ll.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hf.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://sj.huixiangedu.cn

[D17] 最大值与最小值
来源：http://ex.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://pr.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://qb.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ta.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://cw.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hk.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://un.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://hd.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://rd.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://cw.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zj.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://pg.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hv.shxzskj.cn

TS:   nested.flat();
来源：http://rx.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xg.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://ia.bjjhwx.cn

Ruby: nested.flatten
来源：http://ub.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kg.hahajie.cn

[D19] 按字段分组
来源：http://nb.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ml.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kz.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zo.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oy.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gh.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://lq.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jz.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yu.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://ym.newstarts.cn

Py:   Counter(arr)
来源：http://pa.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://xb.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mb.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qf.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xr.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://tn.jianghongdianzi.cn

Ruby: arr.tally
来源：http://uz.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xv.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://rz.wgjwhj.cn

Py:   x in arr
来源：http://jq.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://xh.chemitech.net.cn

JS:   arr.includes(x)
来源：http://eg.muxihuayi.cn

TS:   arr.includes(x)
来源：http://iz.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ri.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://lt.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://wq.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://xq.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://pa.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sq.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ay.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zv.asd995.cn

TS:   [...arr];
来源：http://de.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://os.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://az.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://gv.shxzskj.cn

C#:   new List<int>(list);
来源：http://qa.haigaiapp.cn

[D23] reduce 累积计算
来源：http://cp.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yh.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zj.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://am.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ex.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ed.jianghongdianzi.cn

Go:   // 手写循环
来源：http://xj.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://na.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ha.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://bp.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kc.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ua.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gr.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zo.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sh.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ei.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aa.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rh.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://we.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ca.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rc.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oi.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vl.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lb.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ak.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nr.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qx.wgjwhj.cn

[D26] 数组转字符串
来源：http://bx.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://aj.521024.cn

PHP:  implode(", ", $arr);
来源：http://ag.chemitech.net.cn

JS:   arr.join(", ")
来源：http://qg.jctech888.com.cn

TS:   arr.join(", ")
来源：http://me.asd995.cn

Java: String.join(", ", list)
来源：http://sv.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://pw.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://ld.nicolike.cn

C#:   string.Join(", ", list)
来源：http://on.yuntaijiaju.cn

================================================================================
来源：http://fb.hahajie.cn

E. 字符串处理
来源：http://pd.panjiajie.cn

================================================================================
来源：http://ah.muxihuayi.cn

[E01] 拼接字符串
来源：http://zv.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tl.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sd.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xm.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ew.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pm.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jz.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ci.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dg.huanxung.cn


<!-- 参考信息 -->