代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://zj.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vx.521024.cn

Java: import java.util.List;
来源：http://wp.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ue.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://jh.shxzskj.cn

C#:   using System.Text;
来源：http://rp.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://te.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://ia.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://mn.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://rm.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://mr.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pe.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://bf.521024.cn

Ruby: -> { puts "run" }.call
来源：http://tl.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wx.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://fv.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wx.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uz.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jt.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nk.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rv.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://ip.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://in.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yh.nicolike.cn

[C14] 泛型函数
来源：http://aq.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lg.yuexingan06.cn

PHP:  // 无泛型
来源：http://id.bookmarksfly.cn

JS:   // 无泛型
来源：http://cb.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qg.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ef.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oo.jctech888.com.cn

Ruby: # 无泛型
来源：http://lc.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ns.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://az.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xn.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://dn.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wk.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pc.yuexingan06.cn

Java: // 无解构
来源：http://cv.bookmarksfly.cn

Go:   // 无解构
来源：http://au.hahajie.cn

Ruby: a, b = pair
来源：http://hq.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://jz.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://sy.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bt.chemitech.net.cn

PHP:  // 无重载
来源：http://rv.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fq.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://yz.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jq.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://ah.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://qf.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qg.asd995.cn

================================================================================
来源：http://dk.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://kt.huixiangedu.cn

================================================================================
来源：http://dp.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://su.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://le.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pa.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ia.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qa.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wp.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://pb.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://yj.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ib.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://sc.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lc.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hc.colortex.cn

JS:   arr.push(4);
来源：http://lx.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://xb.haigaiapp.cn

Java: list.add(4);
来源：http://mw.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://lb.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://mv.9csxet.cn

C#:   list.Add(4);
来源：http://eh.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://nl.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://ay.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ec.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ra.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://bt.newstarts.cn

Java: list.add(0, 0);
来源：http://ml.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nc.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ta.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://zh.gzmigu.cn

[D04] 删除元素
来源：http://qt.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ox.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kc.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tz.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://xr.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://je.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cs.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qy.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wj.shxzskj.cn

[D05] 访问与修改元素
来源：http://qm.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gh.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wl.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://td.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://tx.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://cx.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://ou.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lp.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rf.shxzskj.cn

[D06] 数组长度
来源：http://ou.gzmigu.cn

Py:   len(arr)
来源：http://qd.shtwfgs.cn

PHP:  count($arr);
来源：http://qd.lnxyls.cn

JS:   arr.length
来源：http://cf.szxytkj.cn

TS:   arr.length
来源：http://qg.huixiangedu.cn

Java: list.size();
来源：http://rz.panjiajie.cn

Go:   len(arr)
来源：http://up.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://ez.yuexingan06.cn

C#:   list.Count;
来源：http://jq.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://pt.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nm.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zx.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://mu.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://on.lnxyls.cn

Java: list.subList(1, 4);
来源：http://vo.haigaiapp.cn

Go:   arr[1:4]
来源：http://rz.huanxung.cn

Ruby: arr[1, 3]
来源：http://jm.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://rg.chemitech.net.cn

[D08] 合并两个数组
来源：http://ui.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://el.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://fv.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jw.shtwfgs.cn

TS:   [...a, ...b];
来源：http://he.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://od.lnxyls.cn

Go:   append(a, b...)
来源：http://tc.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://yd.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://rv.colortex.cn

[D09] 排序（升序）
来源：http://bb.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://hh.asd995.cn

PHP:  sort($arr);
来源：http://cp.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ro.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://po.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bz.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jn.huixinmuqiang.cn

Ruby: arr.sort
来源：http://fz.lnxyls.cn

C#:   list.Sort();
来源：http://ob.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oi.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rx.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pk.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lk.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sq.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pe.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tm.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bz.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wl.newstarts.cn

[D11] 反转数组
来源：http://rh.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ry.szsharing.cn

PHP:  array_reverse($arr);
来源：http://ya.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ic.shxzskj.cn

TS:   [...arr].reverse();
来源：http://bk.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://xs.asd995.cn

Go:   slices.Reverse(arr)
来源：http://mx.bookmarksfly.cn

Ruby: arr.reverse
来源：http://jt.hnjuh.cn

C#:   list.Reverse();
来源：http://kq.muxihuayi.cn

[D12] 查找元素下标
来源：http://qa.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://zj.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mq.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rb.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qj.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fk.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://zp.hnjuh.cn

Ruby: arr.index(x)
来源：http://ye.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://ca.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://nl.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ln.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ck.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://vr.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://kb.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wr.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qk.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://il.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qp.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://nv.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ph.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yx.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ux.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://ff.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://si.shxzukj.cn

Go:   // 手写循环
来源：http://yj.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tw.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mi.panjiajie.cn

[D15] 去重
来源：http://zw.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cz.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://gu.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://xh.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://ik.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ro.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wx.newstarts.cn

Ruby: arr.uniq
来源：http://fz.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://yb.hahajie.cn

[D16] 求和与平均值
来源：http://dx.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hf.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xj.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dd.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gq.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://au.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://ym.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yp.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://jt.huixiangedu.cn

[D17] 最大值与最小值
来源：http://ji.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://ym.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://li.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wa.colortex.cn

TS:   Math.max(...arr);
来源：http://an.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ub.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bb.521024.cn

Ruby: arr.max;  arr.min
来源：http://yp.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://xf.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://vf.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bf.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://pe.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bp.shtwfgs.cn

TS:   nested.flat();
来源：http://hk.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rr.jctech888.com.cn

Go:   // 手写双层循环
来源：http://aj.hnjuh.cn

Ruby: nested.flatten
来源：http://hj.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aa.gzmigu.cn

[D19] 按字段分组
来源：http://yq.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ld.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://od.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gu.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://et.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mp.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://tq.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ul.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://js.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://pa.jctech888.com.cn

Py:   Counter(arr)
来源：http://lx.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://oo.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ur.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xu.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yg.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://bf.panjiajie.cn

Ruby: arr.tally
来源：http://cm.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rj.newstarts.cn

[D21] 判断是否包含某元素
来源：http://kq.muxihuayi.cn

Py:   x in arr
来源：http://zd.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://yj.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://rm.gzmigu.cn

TS:   arr.includes(x)
来源：http://vh.huanxung.cn

Java: list.contains(x)
来源：http://ly.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://sm.nszjky.cn

Ruby: arr.include?(x)
来源：http://qb.asd995.cn

C#:   list.Contains(x)
来源：http://mz.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://pf.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kd.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vo.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://px.newstarts.cn

TS:   [...arr];
来源：http://nk.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://aq.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cf.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://ux.hnjuh.cn

C#:   new List<int>(list);
来源：http://ng.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://xk.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ue.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kd.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lj.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://er.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yc.huixinmuqiang.cn

Go:   // 手写循环
来源：http://le.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cb.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ne.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://yo.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mi.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://au.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nu.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aq.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rx.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aq.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fb.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://as.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://oc.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rd.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://os.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yp.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ld.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hk.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pf.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cz.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hs.chemitech.net.cn

[D26] 数组转字符串
来源：http://dt.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://mx.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://mv.huixiangedu.cn

JS:   arr.join(", ")
来源：http://bx.szxytkj.cn

TS:   arr.join(", ")
来源：http://dw.wgjwhj.cn

Java: String.join(", ", list)
来源：http://hy.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://vg.panjiajie.cn

Ruby: arr.join(", ")
来源：http://fn.asd995.cn

C#:   string.Join(", ", list)
来源：http://wg.521024.cn

================================================================================
来源：http://cn.chemitech.net.cn

E. 字符串处理
来源：http://ae.szxytkj.cn

================================================================================
来源：http://su.huanxung.cn

[E01] 拼接字符串
来源：http://kq.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wl.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ub.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://am.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gg.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zt.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cw.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hs.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zc.szxytkj.cn


<!-- 参考信息 -->