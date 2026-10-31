代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://kz.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dh.huixinmuqiang.cn

Java: import java.util.List;
来源：http://ni.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qu.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://vd.huanxung.cn

C#:   using System.Text;
来源：http://ff.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://tf.asd995.cn

Py:   (lambda: print("run"))()
来源：http://ql.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://mp.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://xf.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://wz.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ar.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://js.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://nt.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rf.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://es.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ho.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://az.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ju.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kj.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wc.shxzukj.cn

Go:   func add(a, b int) int
来源：http://za.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lw.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ca.shxzskj.cn

[C14] 泛型函数
来源：http://dm.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://th.shxzukj.cn

PHP:  // 无泛型
来源：http://al.szsharing.cn

JS:   // 无泛型
来源：http://qa.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://if.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bv.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oq.muxihuayi.cn

Ruby: # 无泛型
来源：http://dy.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://as.9csxet.cn

[C15] 解构 / 展开参数
来源：http://dp.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ap.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://kb.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fl.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hm.yuexingan06.cn

Java: // 无解构
来源：http://tx.asd995.cn

Go:   // 无解构
来源：http://db.wgjwhj.cn

Ruby: a, b = pair
来源：http://fy.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://ed.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://gr.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ln.haigaiapp.cn

PHP:  // 无重载
来源：http://vb.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rr.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://kp.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cg.521024.cn

Go:   // 无重载：用不同函数名
来源：http://im.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://hg.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fx.nicolike.cn

================================================================================
来源：http://oj.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://ua.panjiajie.cn

================================================================================
来源：http://wu.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://sf.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yo.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://el.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://af.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://px.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ji.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ex.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://cz.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nn.szsharing.cn

[D02] 追加元素到末尾
来源：http://ui.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ac.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bx.szxytkj.cn

JS:   arr.push(4);
来源：http://cx.muxihuayi.cn

TS:   arr.push(4);
来源：http://iq.521024.cn

Java: list.add(4);
来源：http://iu.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://op.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://nx.huanxung.cn

C#:   list.Add(4);
来源：http://on.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://hp.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://sc.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gp.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cc.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://sh.gzmigu.cn

Java: list.add(0, 0);
来源：http://hq.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fj.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fe.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ht.yuexingan06.cn

[D04] 删除元素
来源：http://oq.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://my.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://st.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yv.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://cl.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hn.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ou.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qt.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bu.9csxet.cn

[D05] 访问与修改元素
来源：http://to.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dy.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ca.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qg.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://tm.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://eh.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://qd.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ip.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wu.asd995.cn

[D06] 数组长度
来源：http://ox.haigaiapp.cn

Py:   len(arr)
来源：http://jh.panjiajie.cn

PHP:  count($arr);
来源：http://yo.newstarts.cn

JS:   arr.length
来源：http://yj.lnxyls.cn

TS:   arr.length
来源：http://ao.newstarts.cn

Java: list.size();
来源：http://rn.panjiajie.cn

Go:   len(arr)
来源：http://yd.asd995.cn

Ruby: arr.length; arr.size
来源：http://jn.jctech888.com.cn

C#:   list.Count;
来源：http://xz.newstarts.cn

[D07] 切片 / 取子数组
来源：http://ey.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fu.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://ib.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://ke.asd995.cn

Java: list.subList(1, 4);
来源：http://sa.nszjky.cn

Go:   arr[1:4]
来源：http://do.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://vi.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://fc.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://cy.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://vx.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://lg.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nm.jctech888.com.cn

TS:   [...a, ...b];
来源：http://yf.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uq.haigaiapp.cn

Go:   append(a, b...)
来源：http://md.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://zo.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://bt.shtwfgs.cn

[D09] 排序（升序）
来源：http://br.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://jq.yuexingan06.cn

PHP:  sort($arr);
来源：http://jb.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vk.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ju.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ue.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nh.huixinmuqiang.cn

Ruby: arr.sort
来源：http://yi.hahajie.cn

C#:   list.Sort();
来源：http://le.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ic.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uh.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jy.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://al.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hy.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://om.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ue.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nd.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kb.szsharing.cn

[D11] 反转数组
来源：http://nf.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ox.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://ws.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ln.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://dk.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://oi.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://nr.wgjwhj.cn

Ruby: arr.reverse
来源：http://ln.chemitech.net.cn

C#:   list.Reverse();
来源：http://cz.haigaiapp.cn

[D12] 查找元素下标
来源：http://lb.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://vq.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zd.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://on.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sq.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vy.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://um.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://ze.huanxung.cn

C#:   list.IndexOf(x);
来源：http://nh.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://sr.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hq.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://em.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://pu.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://tg.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lm.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cp.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jm.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oa.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://as.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ag.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kf.521024.cn

JS:   arr.map(x => x * 2)
来源：http://dp.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://et.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xn.shtwfgs.cn

Go:   // 手写循环
来源：http://bv.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vw.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ss.wgjwhj.cn

[D15] 去重
来源：http://hm.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bi.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://bi.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://yd.asd995.cn

TS:   [...new Set(arr)]
来源：http://zi.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rj.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zj.9csxet.cn

Ruby: arr.uniq
来源：http://lp.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://rc.hnjuh.cn

[D16] 求和与平均值
来源：http://rw.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ck.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bc.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wb.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sb.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qc.panjiajie.cn

Go:   // 手写循环累加
来源：http://ct.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pz.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://ad.hahajie.cn

[D17] 最大值与最小值
来源：http://dx.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://um.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://yc.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uv.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://sh.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hv.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kq.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://yr.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://it.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://ei.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ba.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://yg.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hv.jctech888.com.cn

TS:   nested.flat();
来源：http://jp.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://be.yuexingan06.cn

Go:   // 手写双层循环
来源：http://bm.wgjwhj.cn

Ruby: nested.flatten
来源：http://ty.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qy.newstarts.cn

[D19] 按字段分组
来源：http://id.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uj.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://if.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ja.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rz.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rm.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://fp.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hi.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kd.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://ey.muxihuayi.cn

Py:   Counter(arr)
来源：http://bp.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://dz.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eh.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tz.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://do.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://tp.szsharing.cn

Ruby: arr.tally
来源：http://cx.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jl.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://wy.bjjhwx.cn

Py:   x in arr
来源：http://qk.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://kb.hahajie.cn

JS:   arr.includes(x)
来源：http://yx.gzmigu.cn

TS:   arr.includes(x)
来源：http://my.shtwfgs.cn

Java: list.contains(x)
来源：http://on.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://on.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://pk.jctech888.com.cn

C#:   list.Contains(x)
来源：http://cp.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://uo.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gc.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yj.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lm.wgjwhj.cn

TS:   [...arr];
来源：http://wi.nszjky.cn

Java: new ArrayList<>(list);
来源：http://vh.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ld.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://sf.chemitech.net.cn

C#:   new List<int>(list);
来源：http://cm.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://co.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ai.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ti.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ws.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ee.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sb.colortex.cn

Go:   // 手写循环
来源：http://xy.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zn.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hs.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://xh.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ua.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uf.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xz.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ux.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lw.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cu.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hd.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qt.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://ls.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sr.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sr.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qt.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://os.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ch.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gj.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pf.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rx.haigaiapp.cn

[D26] 数组转字符串
来源：http://zg.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://ey.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://la.9csxet.cn

JS:   arr.join(", ")
来源：http://jm.huanxung.cn

TS:   arr.join(", ")
来源：http://zf.wgjwhj.cn

Java: String.join(", ", list)
来源：http://mg.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://bi.shxzukj.cn

Ruby: arr.join(", ")
来源：http://ot.colortex.cn

C#:   string.Join(", ", list)
来源：http://kh.colortex.cn

================================================================================
来源：http://yp.yuntaijiaju.cn

E. 字符串处理
来源：http://ss.muxihuayi.cn

================================================================================
来源：http://mg.haigaiapp.cn

[E01] 拼接字符串
来源：http://ze.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wq.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ta.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ie.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://js.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ek.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qa.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wn.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gf.szsharing.cn


<!-- 参考信息 -->