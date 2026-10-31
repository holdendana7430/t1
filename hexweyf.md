代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://vh.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qw.chemitech.net.cn

Java: import java.util.List;
来源：http://xy.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yx.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://wz.jianghongdianzi.cn

C#:   using System.Text;
来源：http://aw.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://gq.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://bt.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://bn.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://uk.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://cy.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zc.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://pf.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://di.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jz.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://cj.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lv.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cs.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gd.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ai.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jw.9csxet.cn

Go:   func add(a, b int) int
来源：http://ip.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vt.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oo.haigaiapp.cn

[C14] 泛型函数
来源：http://zd.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qk.521024.cn

PHP:  // 无泛型
来源：http://uo.bjjhwx.cn

JS:   // 无泛型
来源：http://sj.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rk.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zq.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bv.shxzukj.cn

Ruby: # 无泛型
来源：http://oy.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ds.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://lk.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rr.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://xn.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yo.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mk.jianghongdianzi.cn

Java: // 无解构
来源：http://uo.bookmarksfly.cn

Go:   // 无解构
来源：http://if.gzmigu.cn

Ruby: a, b = pair
来源：http://ch.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://gs.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://vx.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mo.521024.cn

PHP:  // 无重载
来源：http://uu.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pj.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ii.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://if.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://wq.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://dm.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fb.shtwfgs.cn

================================================================================
来源：http://si.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://xs.huanxung.cn

================================================================================
来源：http://mc.szsharing.cn

[D01] 创建数组 / 列表
来源：http://dp.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hc.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uy.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jz.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pv.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zo.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://sp.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://oy.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ny.521024.cn

[D02] 追加元素到末尾
来源：http://hp.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jw.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ej.chemitech.net.cn

JS:   arr.push(4);
来源：http://kz.haigaiapp.cn

TS:   arr.push(4);
来源：http://rw.yuntaijiaju.cn

Java: list.add(4);
来源：http://aw.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://xu.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://pk.hahajie.cn

C#:   list.Add(4);
来源：http://qh.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://vj.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://ug.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cp.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tn.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://jt.shxzukj.cn

Java: list.add(0, 0);
来源：http://iz.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mm.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://np.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://wf.521024.cn

[D04] 删除元素
来源：http://sb.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://du.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uq.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sj.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://er.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://et.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sn.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ph.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eq.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://zq.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cm.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iq.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nr.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://lz.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://sa.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://gy.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ww.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sv.panjiajie.cn

[D06] 数组长度
来源：http://el.yuexingan06.cn

Py:   len(arr)
来源：http://zd.gzmigu.cn

PHP:  count($arr);
来源：http://wm.bookmarksfly.cn

JS:   arr.length
来源：http://ol.shxzskj.cn

TS:   arr.length
来源：http://fh.szsharing.cn

Java: list.size();
来源：http://wy.huixiangedu.cn

Go:   len(arr)
来源：http://sm.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://dx.gzmigu.cn

C#:   list.Count;
来源：http://pj.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://gs.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nx.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dq.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://jb.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://cb.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://nf.nszjky.cn

Go:   arr[1:4]
来源：http://yw.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://ed.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://sc.panjiajie.cn

[D08] 合并两个数组
来源：http://gf.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://so.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://ew.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nt.hahajie.cn

TS:   [...a, ...b];
来源：http://rr.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ct.haigaiapp.cn

Go:   append(a, b...)
来源：http://ti.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://eo.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://nm.huixiangedu.cn

[D09] 排序（升序）
来源：http://uz.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://jb.asd995.cn

PHP:  sort($arr);
来源：http://aq.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://io.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vj.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fo.hahajie.cn

Ruby: arr.sort
来源：http://nm.huanxung.cn

C#:   list.Sort();
来源：http://oa.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yv.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sn.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ma.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ys.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://me.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hy.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jl.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aa.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lb.bookmarksfly.cn

[D11] 反转数组
来源：http://wh.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pm.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://qx.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ol.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://jr.szsharing.cn

Java: Collections.reverse(list);
来源：http://ah.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://yt.colortex.cn

Ruby: arr.reverse
来源：http://yc.szxytkj.cn

C#:   list.Reverse();
来源：http://zi.yuexingan06.cn

[D12] 查找元素下标
来源：http://ky.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://ct.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ql.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wp.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qz.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://df.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://mo.newstarts.cn

Ruby: arr.index(x)
来源：http://xq.9csxet.cn

C#:   list.IndexOf(x);
来源：http://uq.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://fl.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xm.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rs.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://ne.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://ox.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mx.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://df.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://az.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fb.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://bg.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nk.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vz.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://sz.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://wt.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sb.bjjhwx.cn

Go:   // 手写循环
来源：http://rt.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://os.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://um.huixinmuqiang.cn

[D15] 去重
来源：http://ir.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wl.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://bv.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://eq.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://xs.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ys.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rl.shtwfgs.cn

Ruby: arr.uniq
来源：http://nj.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://bh.haigaiapp.cn

[D16] 求和与平均值
来源：http://nj.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://on.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pt.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vb.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nz.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fp.huixiangedu.cn

Go:   // 手写循环累加
来源：http://wc.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xq.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://pv.hahajie.cn

[D17] 最大值与最小值
来源：http://kl.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://bd.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://fn.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cm.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://jd.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lu.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kg.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://vs.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://cg.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://wd.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://li.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://ej.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fm.nszjky.cn

TS:   nested.flat();
来源：http://nw.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dm.jctech888.com.cn

Go:   // 手写双层循环
来源：http://tk.szxytkj.cn

Ruby: nested.flatten
来源：http://mc.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uw.szxytkj.cn

[D19] 按字段分组
来源：http://wx.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sd.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://od.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hi.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yu.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nd.asd995.cn

Go:   // 手写 map[string][]T
来源：http://kn.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fe.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ia.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://qc.muxihuayi.cn

Py:   Counter(arr)
来源：http://gw.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://ky.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tu.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ur.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iq.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://ti.nszjky.cn

Ruby: arr.tally
来源：http://gr.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aj.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://er.gzmigu.cn

Py:   x in arr
来源：http://vv.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://me.lnxyls.cn

JS:   arr.includes(x)
来源：http://hm.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://fl.newstarts.cn

Java: list.contains(x)
来源：http://iq.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://nx.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://gz.colortex.cn

C#:   list.Contains(x)
来源：http://vf.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://oh.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aq.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://df.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lt.lnxyls.cn

TS:   [...arr];
来源：http://ze.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://nq.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mm.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://re.gzmigu.cn

C#:   new List<int>(list);
来源：http://yd.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://vv.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cl.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kj.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uo.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vl.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lo.jianghongdianzi.cn

Go:   // 手写循环
来源：http://nv.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cj.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://su.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://im.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bt.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kx.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ex.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://li.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lv.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ya.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qw.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uo.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://kp.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rn.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://po.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fz.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hi.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://na.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rw.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bk.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ay.nszjky.cn

[D26] 数组转字符串
来源：http://fg.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://lu.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://ko.lnxyls.cn

JS:   arr.join(", ")
来源：http://oe.huixiangedu.cn

TS:   arr.join(", ")
来源：http://jc.colortex.cn

Java: String.join(", ", list)
来源：http://lp.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://hq.shxzukj.cn

Ruby: arr.join(", ")
来源：http://xq.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://iq.yuntaijiaju.cn

================================================================================
来源：http://ld.shxzskj.cn

E. 字符串处理
来源：http://ke.shxzskj.cn

================================================================================
来源：http://hn.newstarts.cn

[E01] 拼接字符串
来源：http://ge.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qy.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jx.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wd.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ku.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zj.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ei.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wz.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xe.wgjwhj.cn


<!-- 参考信息 -->