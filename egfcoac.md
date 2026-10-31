代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://yk.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qt.shtwfgs.cn

Java: import java.util.List;
来源：http://os.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ig.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://bg.shtwfgs.cn

C#:   using System.Text;
来源：http://ia.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://au.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://zo.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://ya.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://wy.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://gf.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ri.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://lb.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://dc.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ow.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://fp.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hm.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fd.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nu.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iu.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ut.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://jq.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gi.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ue.lnxyls.cn

[C14] 泛型函数
来源：http://ld.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nx.colortex.cn

PHP:  // 无泛型
来源：http://ys.shxzukj.cn

JS:   // 无泛型
来源：http://gh.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ls.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nb.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gl.chemitech.net.cn

Ruby: # 无泛型
来源：http://dk.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pa.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://un.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ae.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://fq.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://en.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ca.jctech888.com.cn

Java: // 无解构
来源：http://uy.newstarts.cn

Go:   // 无解构
来源：http://aq.panjiajie.cn

Ruby: a, b = pair
来源：http://xl.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://jh.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://hp.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mr.hahajie.cn

PHP:  // 无重载
来源：http://pi.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zx.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://lx.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dv.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://ad.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://um.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yl.shxzukj.cn

================================================================================
来源：http://bl.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ae.jianghongdianzi.cn

================================================================================
来源：http://iy.9csxet.cn

[D01] 创建数组 / 列表
来源：http://wh.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ww.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fn.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ij.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xh.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zi.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://qe.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://lc.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mx.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://wh.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ja.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kd.huixiangedu.cn

JS:   arr.push(4);
来源：http://cs.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://go.nszjky.cn

Java: list.add(4);
来源：http://ft.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://fy.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://xo.szxytkj.cn

C#:   list.Add(4);
来源：http://qk.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://hp.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://vi.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oa.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xj.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://xg.gzmigu.cn

Java: list.add(0, 0);
来源：http://ql.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://de.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cu.521024.cn

C#:   list.Insert(0, 0);
来源：http://xy.newstarts.cn

[D04] 删除元素
来源：http://tt.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fb.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qq.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xp.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://qy.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ov.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qp.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://el.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://un.huixiangedu.cn

[D05] 访问与修改元素
来源：http://te.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cg.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kq.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ho.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://da.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://bc.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://ye.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sk.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jy.colortex.cn

[D06] 数组长度
来源：http://wq.panjiajie.cn

Py:   len(arr)
来源：http://by.szsharing.cn

PHP:  count($arr);
来源：http://jr.szsharing.cn

JS:   arr.length
来源：http://sq.9csxet.cn

TS:   arr.length
来源：http://pl.shxzskj.cn

Java: list.size();
来源：http://mg.hahajie.cn

Go:   len(arr)
来源：http://di.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://lb.bjjhwx.cn

C#:   list.Count;
来源：http://aw.huanxung.cn

[D07] 切片 / 取子数组
来源：http://dr.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bd.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zp.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://mm.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://mj.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://po.yuexingan06.cn

Go:   arr[1:4]
来源：http://xk.hahajie.cn

Ruby: arr[1, 3]
来源：http://pw.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://uf.huixiangedu.cn

[D08] 合并两个数组
来源：http://ks.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://xt.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://jq.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zp.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://lv.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kj.muxihuayi.cn

Go:   append(a, b...)
来源：http://jp.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://eb.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://yy.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://iq.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://sj.9csxet.cn

PHP:  sort($arr);
来源：http://bj.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ny.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yq.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ky.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zj.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ij.asd995.cn

C#:   list.Sort();
来源：http://wl.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xi.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yr.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jy.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fk.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pr.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://og.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fq.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://am.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mi.haigaiapp.cn

[D11] 反转数组
来源：http://ru.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iq.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://tp.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ln.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://he.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://rg.asd995.cn

Go:   slices.Reverse(arr)
来源：http://aa.chemitech.net.cn

Ruby: arr.reverse
来源：http://mn.hahajie.cn

C#:   list.Reverse();
来源：http://al.szxytkj.cn

[D12] 查找元素下标
来源：http://od.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://qh.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uc.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zp.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sn.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rv.521024.cn

Go:   slices.Index(arr, x)
来源：http://pw.jctech888.com.cn

Ruby: arr.index(x)
来源：http://nz.521024.cn

C#:   list.IndexOf(x);
来源：http://aq.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://fp.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sw.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pf.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://zo.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://ch.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wj.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ts.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bo.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rf.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://sk.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://do.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tm.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://ou.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://oh.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kr.haigaiapp.cn

Go:   // 手写循环
来源：http://ve.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rk.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ah.panjiajie.cn

[D15] 去重
来源：http://ve.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jt.gzmigu.cn

PHP:  array_unique($arr);
来源：http://ol.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://xs.colortex.cn

TS:   [...new Set(arr)]
来源：http://xl.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ij.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vx.shxzskj.cn

Ruby: arr.uniq
来源：http://mh.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://jj.shxzskj.cn

[D16] 求和与平均值
来源：http://pl.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ij.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gn.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://de.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dj.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aq.yuexingan06.cn

Go:   // 手写循环累加
来源：http://qq.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ln.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://cj.shxzukj.cn

[D17] 最大值与最小值
来源：http://kv.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://fh.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://wx.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://en.szxytkj.cn

TS:   Math.max(...arr);
来源：http://pr.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jd.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ud.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://os.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://ge.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://jr.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lq.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://xj.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pm.szxytkj.cn

TS:   nested.flat();
来源：http://ap.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lj.shtwfgs.cn

Go:   // 手写双层循环
来源：http://jq.szxytkj.cn

Ruby: nested.flatten
来源：http://dq.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yc.yuexingan06.cn

[D19] 按字段分组
来源：http://nt.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nd.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rf.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yl.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rx.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yk.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://bu.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mi.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zr.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://ov.huanxung.cn

Py:   Counter(arr)
来源：http://nk.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://bl.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gn.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lc.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://np.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://yc.asd995.cn

Ruby: arr.tally
来源：http://ld.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rd.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://dz.muxihuayi.cn

Py:   x in arr
来源：http://nh.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://as.wgjwhj.cn

JS:   arr.includes(x)
来源：http://cu.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://ye.szxytkj.cn

Java: list.contains(x)
来源：http://uw.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://kl.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://kk.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://vk.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://pt.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nl.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yq.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yj.hahajie.cn

TS:   [...arr];
来源：http://jd.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://gu.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://up.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://rb.shxzskj.cn

C#:   new List<int>(list);
来源：http://sg.gzmigu.cn

[D23] reduce 累积计算
来源：http://hr.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ng.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zz.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rl.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kv.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sh.muxihuayi.cn

Go:   // 手写循环
来源：http://na.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vk.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jk.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://df.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qd.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ej.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cr.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ie.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fv.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fq.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ri.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aw.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://wg.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ai.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://if.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://av.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gz.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://at.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tw.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://je.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cn.asd995.cn

[D26] 数组转字符串
来源：http://zu.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://wg.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://zn.szsharing.cn

JS:   arr.join(", ")
来源：http://cy.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://wd.gzmigu.cn

Java: String.join(", ", list)
来源：http://ys.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://pz.lnxyls.cn

Ruby: arr.join(", ")
来源：http://qe.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://vc.yuntaijiaju.cn

================================================================================
来源：http://hq.jianghongdianzi.cn

E. 字符串处理
来源：http://da.521024.cn

================================================================================
来源：http://hs.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://zt.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gt.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jx.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yx.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lx.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cx.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ck.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tz.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qv.asd995.cn


<!-- 参考信息 -->