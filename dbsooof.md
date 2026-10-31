代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://zf.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fs.jctech888.com.cn

Java: import java.util.List;
来源：http://in.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fi.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://kc.chemitech.net.cn

C#:   using System.Text;
来源：http://ni.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://sf.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://fi.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://an.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://ye.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://yy.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yw.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://gy.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://mp.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qh.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://og.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jn.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://id.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dg.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yj.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hj.nszjky.cn

Go:   func add(a, b int) int
来源：http://xv.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hi.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nq.shtwfgs.cn

[C14] 泛型函数
来源：http://ct.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lm.yuexingan06.cn

PHP:  // 无泛型
来源：http://ro.521024.cn

JS:   // 无泛型
来源：http://gk.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mg.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vt.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bq.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://uh.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jd.521024.cn

[C15] 解构 / 展开参数
来源：http://gc.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://et.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://ff.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ez.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ys.521024.cn

Java: // 无解构
来源：http://uj.jianghongdianzi.cn

Go:   // 无解构
来源：http://ee.shxzskj.cn

Ruby: a, b = pair
来源：http://wd.9csxet.cn

C#:   var (a, b) = pair;
来源：http://ko.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://px.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xc.bjjhwx.cn

PHP:  // 无重载
来源：http://vo.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ka.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://no.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sp.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://wu.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://rq.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lr.chemitech.net.cn

================================================================================
来源：http://un.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://qb.bjjhwx.cn

================================================================================
来源：http://cb.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://pl.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bj.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gt.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://la.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zf.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dh.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://yf.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://ay.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yb.asd995.cn

[D02] 追加元素到末尾
来源：http://tg.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nr.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ip.muxihuayi.cn

JS:   arr.push(4);
来源：http://vk.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://cy.newstarts.cn

Java: list.add(4);
来源：http://ei.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://zr.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://qw.jctech888.com.cn

C#:   list.Add(4);
来源：http://il.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://qa.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://ke.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ce.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://id.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://nh.yuexingan06.cn

Java: list.add(0, 0);
来源：http://og.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pl.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ep.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://hh.shtwfgs.cn

[D04] 删除元素
来源：http://lv.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yl.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nr.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rh.521024.cn

TS:   arr.splice(0, 1);
来源：http://pj.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ln.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sq.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lr.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tw.521024.cn

[D05] 访问与修改元素
来源：http://rc.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hq.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ji.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oe.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://sb.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://jj.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://xu.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://le.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ib.jianghongdianzi.cn

[D06] 数组长度
来源：http://vy.yuexingan06.cn

Py:   len(arr)
来源：http://xl.jianghongdianzi.cn

PHP:  count($arr);
来源：http://zs.521024.cn

JS:   arr.length
来源：http://fd.yuexingan06.cn

TS:   arr.length
来源：http://ce.bjjhwx.cn

Java: list.size();
来源：http://py.huixiangedu.cn

Go:   len(arr)
来源：http://tf.huanxung.cn

Ruby: arr.length; arr.size
来源：http://al.colortex.cn

C#:   list.Count;
来源：http://jz.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://ol.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tg.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yh.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://mk.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://ik.panjiajie.cn

Java: list.subList(1, 4);
来源：http://qp.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://za.lnxyls.cn

Ruby: arr[1, 3]
来源：http://hf.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://vy.hnjuh.cn

[D08] 合并两个数组
来源：http://jv.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://ow.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://dv.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gj.shxzukj.cn

TS:   [...a, ...b];
来源：http://dr.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lp.nicolike.cn

Go:   append(a, b...)
来源：http://cc.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://bf.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://pw.yuexingan06.cn

[D09] 排序（升序）
来源：http://pj.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://xu.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://px.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ua.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rm.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oz.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ge.jianghongdianzi.cn

Ruby: arr.sort
来源：http://xc.newstarts.cn

C#:   list.Sort();
来源：http://xz.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ly.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hf.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ez.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lk.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pg.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qh.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ov.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zk.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://db.jianghongdianzi.cn

[D11] 反转数组
来源：http://eq.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yh.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://xe.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dd.shxzukj.cn

TS:   [...arr].reverse();
来源：http://va.9csxet.cn

Java: Collections.reverse(list);
来源：http://yc.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://mx.huixiangedu.cn

Ruby: arr.reverse
来源：http://fi.huanxung.cn

C#:   list.Reverse();
来源：http://ub.shxzskj.cn

[D12] 查找元素下标
来源：http://ej.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://rq.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gy.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zh.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uo.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://he.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://sc.wgjwhj.cn

Ruby: arr.index(x)
来源：http://xf.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://gc.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://wu.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ky.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sa.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://yu.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://fp.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gs.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ro.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sk.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pj.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://wv.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bc.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ba.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://ay.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://uf.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iz.lnxyls.cn

Go:   // 手写循环
来源：http://fw.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uz.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oh.jianghongdianzi.cn

[D15] 去重
来源：http://sl.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nx.nszjky.cn

PHP:  array_unique($arr);
来源：http://wi.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://sr.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://gb.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bh.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gc.bjjhwx.cn

Ruby: arr.uniq
来源：http://wl.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://bx.asd995.cn

[D16] 求和与平均值
来源：http://qj.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://so.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gl.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cq.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ds.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ix.9csxet.cn

Go:   // 手写循环累加
来源：http://sx.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ie.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://nd.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://ro.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://qn.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://qy.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mj.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://ql.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://up.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yx.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://li.asd995.cn

C#:   list.Max();  list.Min()
来源：http://db.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://wn.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zg.colortex.cn

PHP:  array_merge(...$nested);
来源：http://pa.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://np.chemitech.net.cn

TS:   nested.flat();
来源：http://vq.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zf.jctech888.com.cn

Go:   // 手写双层循环
来源：http://tg.9csxet.cn

Ruby: nested.flatten
来源：http://rh.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kp.chemitech.net.cn

[D19] 按字段分组
来源：http://qr.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zy.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://id.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pv.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fr.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jp.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://uc.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://de.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://os.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://zm.szxytkj.cn

Py:   Counter(arr)
来源：http://nm.nszjky.cn

PHP:  array_count_values($arr);
来源：http://vi.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gy.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://im.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://be.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://im.nszjky.cn

Ruby: arr.tally
来源：http://hg.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ag.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://ey.huanxung.cn

Py:   x in arr
来源：http://po.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://vu.wgjwhj.cn

JS:   arr.includes(x)
来源：http://wt.colortex.cn

TS:   arr.includes(x)
来源：http://so.hnjuh.cn

Java: list.contains(x)
来源：http://cy.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://kx.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://zp.bjjhwx.cn

C#:   list.Contains(x)
来源：http://pt.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://sv.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://km.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bk.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://da.haigaiapp.cn

TS:   [...arr];
来源：http://yu.nicolike.cn

Java: new ArrayList<>(list);
来源：http://cb.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cm.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://vp.hahajie.cn

C#:   new List<int>(list);
来源：http://sw.shtwfgs.cn

[D23] reduce 累积计算
来源：http://ip.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dn.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zv.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dd.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://if.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hw.yuexingan06.cn

Go:   // 手写循环
来源：http://uk.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://um.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ec.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://yv.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zg.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yd.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ij.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zk.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uu.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mj.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ln.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fp.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://uv.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zx.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fo.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ep.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ax.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://of.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oo.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kq.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kx.jctech888.com.cn

[D26] 数组转字符串
来源：http://dv.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://ng.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://ro.panjiajie.cn

JS:   arr.join(", ")
来源：http://au.lnxyls.cn

TS:   arr.join(", ")
来源：http://lm.newstarts.cn

Java: String.join(", ", list)
来源：http://fh.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://zp.9csxet.cn

Ruby: arr.join(", ")
来源：http://rn.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://ly.bookmarksfly.cn

================================================================================
来源：http://ec.szxytkj.cn

E. 字符串处理
来源：http://vg.wgjwhj.cn

================================================================================
来源：http://sv.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://jm.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oc.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tu.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ff.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xu.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ll.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hl.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mb.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cx.muxihuayi.cn


<!-- 参考信息 -->