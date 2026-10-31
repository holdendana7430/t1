代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://ly.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bh.panjiajie.cn

Java: import java.util.List;
来源：http://oj.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dt.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://pu.bookmarksfly.cn

C#:   using System.Text;
来源：http://bi.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://ad.colortex.cn

Py:   (lambda: print("run"))()
来源：http://um.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://ja.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://ho.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://ko.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hf.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://gh.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://le.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hy.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://ip.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tz.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ej.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ey.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vj.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tx.colortex.cn

Go:   func add(a, b int) int
来源：http://sb.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eh.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fi.huixiangedu.cn

[C14] 泛型函数
来源：http://fl.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vg.newstarts.cn

PHP:  // 无泛型
来源：http://ln.wgjwhj.cn

JS:   // 无泛型
来源：http://xu.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dc.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wx.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wd.chemitech.net.cn

Ruby: # 无泛型
来源：http://ja.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pk.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://fz.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hh.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://wb.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ku.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pg.nszjky.cn

Java: // 无解构
来源：http://yq.yuexingan06.cn

Go:   // 无解构
来源：http://hy.bjjhwx.cn

Ruby: a, b = pair
来源：http://ar.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://xf.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://gl.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sn.lnxyls.cn

PHP:  // 无重载
来源：http://fw.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://di.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://xz.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oe.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://fq.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://nt.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ua.gzmigu.cn

================================================================================
来源：http://id.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://dz.shxzukj.cn

================================================================================
来源：http://tl.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://kh.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pf.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tf.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ur.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nm.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ay.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://ku.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://ce.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bn.lnxyls.cn

[D02] 追加元素到末尾
来源：http://ea.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mf.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bf.gzmigu.cn

JS:   arr.push(4);
来源：http://ag.chemitech.net.cn

TS:   arr.push(4);
来源：http://ta.shtwfgs.cn

Java: list.add(4);
来源：http://xl.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://gt.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://wh.panjiajie.cn

C#:   list.Add(4);
来源：http://hj.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://co.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://kt.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ax.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://si.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://pp.asd995.cn

Java: list.add(0, 0);
来源：http://wb.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tv.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vc.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://eq.asd995.cn

[D04] 删除元素
来源：http://jf.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xn.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://db.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yx.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://au.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hy.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ir.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ml.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xr.huanxung.cn

[D05] 访问与修改元素
来源：http://tq.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bb.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xh.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ap.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://ur.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://fh.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ib.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sq.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xh.colortex.cn

[D06] 数组长度
来源：http://jd.colortex.cn

Py:   len(arr)
来源：http://kc.newstarts.cn

PHP:  count($arr);
来源：http://hp.jctech888.com.cn

JS:   arr.length
来源：http://cw.nicolike.cn

TS:   arr.length
来源：http://sa.yuntaijiaju.cn

Java: list.size();
来源：http://is.haigaiapp.cn

Go:   len(arr)
来源：http://ow.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://ed.jianghongdianzi.cn

C#:   list.Count;
来源：http://rj.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://bh.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ax.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qq.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://hc.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://pl.lnxyls.cn

Java: list.subList(1, 4);
来源：http://rl.hnjuh.cn

Go:   arr[1:4]
来源：http://rv.colortex.cn

Ruby: arr[1, 3]
来源：http://lr.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://lg.szxytkj.cn

[D08] 合并两个数组
来源：http://ly.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://dx.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://rw.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bb.jctech888.com.cn

TS:   [...a, ...b];
来源：http://dj.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aw.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://pc.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://kd.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://lo.shxzskj.cn

[D09] 排序（升序）
来源：http://bq.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://aq.yuexingan06.cn

PHP:  sort($arr);
来源：http://xe.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tl.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rv.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ch.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://la.szxytkj.cn

Ruby: arr.sort
来源：http://za.bjjhwx.cn

C#:   list.Sort();
来源：http://nl.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vj.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ji.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kn.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fo.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wg.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ks.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bm.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zt.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ns.nszjky.cn

[D11] 反转数组
来源：http://kg.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://js.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://nq.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ck.lnxyls.cn

TS:   [...arr].reverse();
来源：http://bo.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://jp.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://oy.521024.cn

Ruby: arr.reverse
来源：http://al.9csxet.cn

C#:   list.Reverse();
来源：http://uh.shxzukj.cn

[D12] 查找元素下标
来源：http://qa.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://yu.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ru.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nx.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ai.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ob.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://zn.wgjwhj.cn

Ruby: arr.index(x)
来源：http://cq.9csxet.cn

C#:   list.IndexOf(x);
来源：http://ps.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://wh.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qc.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jn.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://ha.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://ap.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zv.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xu.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tb.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aq.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://bd.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ih.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dy.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://mz.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://vi.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cf.shtwfgs.cn

Go:   // 手写循环
来源：http://ba.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ev.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xq.nszjky.cn

[D15] 去重
来源：http://jm.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ds.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://hn.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://ld.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://fw.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mf.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rz.9csxet.cn

Ruby: arr.uniq
来源：http://vb.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://ts.nszjky.cn

[D16] 求和与平均值
来源：http://bl.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ei.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vu.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ch.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dc.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eb.haigaiapp.cn

Go:   // 手写循环累加
来源：http://vm.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ur.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://ut.hahajie.cn

[D17] 最大值与最小值
来源：http://mt.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://wp.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://xp.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dp.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://sp.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vm.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cu.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://de.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://ff.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://xi.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://am.colortex.cn

PHP:  array_merge(...$nested);
来源：http://ip.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ah.shxzskj.cn

TS:   nested.flat();
来源：http://ry.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qo.huixiangedu.cn

Go:   // 手写双层循环
来源：http://wm.bookmarksfly.cn

Ruby: nested.flatten
来源：http://ft.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jz.yuntaijiaju.cn

[D19] 按字段分组
来源：http://dt.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cb.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ro.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ug.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qu.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gh.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://ij.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ej.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xn.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://bu.bookmarksfly.cn

Py:   Counter(arr)
来源：http://wf.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://ju.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gu.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xc.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zl.szsharing.cn

Go:   // 手写 map[T]int
来源：http://sp.szsharing.cn

Ruby: arr.tally
来源：http://vz.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lu.nicolike.cn

[D21] 判断是否包含某元素
来源：http://gd.szxytkj.cn

Py:   x in arr
来源：http://us.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://mc.bjjhwx.cn

JS:   arr.includes(x)
来源：http://zk.nicolike.cn

TS:   arr.includes(x)
来源：http://sn.9csxet.cn

Java: list.contains(x)
来源：http://hq.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://dd.szsharing.cn

Ruby: arr.include?(x)
来源：http://ku.gzmigu.cn

C#:   list.Contains(x)
来源：http://df.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://hl.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fi.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sh.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fw.9csxet.cn

TS:   [...arr];
来源：http://qp.newstarts.cn

Java: new ArrayList<>(list);
来源：http://kl.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hj.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://lx.chemitech.net.cn

C#:   new List<int>(list);
来源：http://xk.gzmigu.cn

[D23] reduce 累积计算
来源：http://nm.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gb.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://my.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zv.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qk.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qr.yuntaijiaju.cn

Go:   // 手写循环
来源：http://oo.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hq.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ak.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://dr.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ts.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yq.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://di.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jw.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zf.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dj.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oz.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kp.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://lx.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ur.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://av.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bd.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kc.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ic.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gg.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ri.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ch.hnjuh.cn

[D26] 数组转字符串
来源：http://fa.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://zx.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://vh.hnjuh.cn

JS:   arr.join(", ")
来源：http://bk.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://yv.haigaiapp.cn

Java: String.join(", ", list)
来源：http://vi.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://lf.asd995.cn

Ruby: arr.join(", ")
来源：http://py.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://fb.colortex.cn

================================================================================
来源：http://uh.yuexingan06.cn

E. 字符串处理
来源：http://xm.szxytkj.cn

================================================================================
来源：http://df.bjjhwx.cn

[E01] 拼接字符串
来源：http://va.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tu.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jx.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wm.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mo.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ns.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zn.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ga.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qm.521024.cn


<!-- 参考信息 -->