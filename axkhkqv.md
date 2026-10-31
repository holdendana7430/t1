代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://xx.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ef.szsharing.cn

Java: import java.util.List;
来源：http://on.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yh.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://ik.huixinmuqiang.cn

C#:   using System.Text;
来源：http://ow.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://xl.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://ye.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://ja.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://pp.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://uh.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vy.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://qy.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://pj.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zh.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://kg.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ys.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ko.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://df.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://le.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fa.panjiajie.cn

Go:   func add(a, b int) int
来源：http://mm.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xh.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qw.colortex.cn

[C14] 泛型函数
来源：http://tr.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dz.hahajie.cn

PHP:  // 无泛型
来源：http://da.muxihuayi.cn

JS:   // 无泛型
来源：http://pz.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qa.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cc.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xz.szsharing.cn

Ruby: # 无泛型
来源：http://lv.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zz.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://lz.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pq.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://in.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wy.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ha.hnjuh.cn

Java: // 无解构
来源：http://gc.haigaiapp.cn

Go:   // 无解构
来源：http://zx.bookmarksfly.cn

Ruby: a, b = pair
来源：http://am.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://rj.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://cz.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uv.9csxet.cn

PHP:  // 无重载
来源：http://zc.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://di.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://jc.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ra.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://ci.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://kr.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yz.jctech888.com.cn

================================================================================
来源：http://ar.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://hi.hahajie.cn

================================================================================
来源：http://sn.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://cf.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ud.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xr.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ig.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fz.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dw.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://ko.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://nk.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ae.hnjuh.cn

[D02] 追加元素到末尾
来源：http://aw.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jq.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hk.szxytkj.cn

JS:   arr.push(4);
来源：http://wl.yuexingan06.cn

TS:   arr.push(4);
来源：http://tf.nszjky.cn

Java: list.add(4);
来源：http://hq.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://zz.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://qv.nszjky.cn

C#:   list.Add(4);
来源：http://kj.colortex.cn

[D03] 在指定位置插入元素
来源：http://xe.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://xk.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rq.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dk.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://sd.bjjhwx.cn

Java: list.add(0, 0);
来源：http://yz.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rd.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vy.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://pt.szsharing.cn

[D04] 删除元素
来源：http://ew.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jr.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://az.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ck.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://nw.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jn.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tb.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vm.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ie.colortex.cn

[D05] 访问与修改元素
来源：http://bi.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://et.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ao.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dr.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://to.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://xo.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://tv.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zn.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pj.panjiajie.cn

[D06] 数组长度
来源：http://na.newstarts.cn

Py:   len(arr)
来源：http://tf.chemitech.net.cn

PHP:  count($arr);
来源：http://gf.huixinmuqiang.cn

JS:   arr.length
来源：http://jp.huixinmuqiang.cn

TS:   arr.length
来源：http://ok.nszjky.cn

Java: list.size();
来源：http://oa.newstarts.cn

Go:   len(arr)
来源：http://jg.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://hn.nicolike.cn

C#:   list.Count;
来源：http://dq.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://qr.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bp.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hq.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://nf.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://as.nszjky.cn

Java: list.subList(1, 4);
来源：http://jc.yuexingan06.cn

Go:   arr[1:4]
来源：http://oj.asd995.cn

Ruby: arr[1, 3]
来源：http://rs.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://rj.521024.cn

[D08] 合并两个数组
来源：http://kw.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://sg.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://db.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gn.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://cy.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wt.shxzukj.cn

Go:   append(a, b...)
来源：http://pz.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://dv.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://qj.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://xx.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://kz.colortex.cn

PHP:  sort($arr);
来源：http://ji.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yc.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uh.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://js.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dn.hnjuh.cn

Ruby: arr.sort
来源：http://oe.shtwfgs.cn

C#:   list.Sort();
来源：http://oo.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://da.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jx.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hk.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pk.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cm.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vq.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://js.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bv.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gb.huixiangedu.cn

[D11] 反转数组
来源：http://yb.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://we.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://dz.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lc.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://rf.szxytkj.cn

Java: Collections.reverse(list);
来源：http://zj.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://lv.jctech888.com.cn

Ruby: arr.reverse
来源：http://vm.yuexingan06.cn

C#:   list.Reverse();
来源：http://pl.wgjwhj.cn

[D12] 查找元素下标
来源：http://lv.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://ie.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zj.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hr.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sz.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mv.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://gy.shxzukj.cn

Ruby: arr.index(x)
来源：http://nv.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://on.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://nj.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rh.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ff.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://vz.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://yr.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ui.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jm.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qd.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qb.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://de.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pw.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hf.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://cs.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://fi.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bk.nszjky.cn

Go:   // 手写循环
来源：http://pp.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xy.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cl.huixiangedu.cn

[D15] 去重
来源：http://gd.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jv.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://bw.szsharing.cn

JS:   [...new Set(arr)]
来源：http://df.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://ep.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bw.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hg.hnjuh.cn

Ruby: arr.uniq
来源：http://eu.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://tu.asd995.cn

[D16] 求和与平均值
来源：http://gm.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lw.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zp.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wa.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tp.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kf.9csxet.cn

Go:   // 手写循环累加
来源：http://kt.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ay.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://hl.newstarts.cn

[D17] 最大值与最小值
来源：http://ah.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://sd.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://ik.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mg.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://ru.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eq.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://gq.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://jy.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://sj.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rb.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://mi.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dn.newstarts.cn

TS:   nested.flat();
来源：http://yl.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wx.shxzukj.cn

Go:   // 手写双层循环
来源：http://gx.nszjky.cn

Ruby: nested.flatten
来源：http://fn.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tm.newstarts.cn

[D19] 按字段分组
来源：http://ho.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sa.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://im.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://go.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ef.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oc.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://wo.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oj.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ad.colortex.cn

[D20] 统计每个元素出现次数
来源：http://wr.9csxet.cn

Py:   Counter(arr)
来源：http://jx.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://cs.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ib.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gq.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qx.asd995.cn

Go:   // 手写 map[T]int
来源：http://nt.nicolike.cn

Ruby: arr.tally
来源：http://ig.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xk.hahajie.cn

[D21] 判断是否包含某元素
来源：http://zl.hahajie.cn

Py:   x in arr
来源：http://tw.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://vd.shxzskj.cn

JS:   arr.includes(x)
来源：http://qx.shxzskj.cn

TS:   arr.includes(x)
来源：http://ll.jctech888.com.cn

Java: list.contains(x)
来源：http://db.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://hf.szsharing.cn

Ruby: arr.include?(x)
来源：http://cx.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://nx.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://mq.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ob.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jl.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dk.szxytkj.cn

TS:   [...arr];
来源：http://jm.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://qf.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://az.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://ns.shxzskj.cn

C#:   new List<int>(list);
来源：http://wb.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://xu.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yg.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ta.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zb.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yq.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qq.panjiajie.cn

Go:   // 手写循环
来源：http://or.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vx.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sn.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://fi.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rz.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ht.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wx.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://se.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cb.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rv.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vm.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hh.asd995.cn

[D25] Set 集合去重与交并差
来源：http://eq.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xb.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ha.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bh.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uv.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sn.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mm.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://so.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nl.panjiajie.cn

[D26] 数组转字符串
来源：http://is.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://bf.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://tn.haigaiapp.cn

JS:   arr.join(", ")
来源：http://lu.hahajie.cn

TS:   arr.join(", ")
来源：http://vq.jctech888.com.cn

Java: String.join(", ", list)
来源：http://sp.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://ke.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://my.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://zy.huixinmuqiang.cn

================================================================================
来源：http://lb.newstarts.cn

E. 字符串处理
来源：http://ew.shtwfgs.cn

================================================================================
来源：http://df.jctech888.com.cn

[E01] 拼接字符串
来源：http://fs.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eg.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bf.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vp.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gy.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lr.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oi.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ra.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yq.colortex.cn


<!-- 参考信息 -->