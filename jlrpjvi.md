代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://av.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qn.muxihuayi.cn

Java: import java.util.List;
来源：http://hl.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qw.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://gm.jctech888.com.cn

C#:   using System.Text;
来源：http://wk.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://ki.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://ju.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://wd.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://oc.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://nq.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://du.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://nj.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://wo.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://df.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://ji.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vk.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tu.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://of.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eh.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yy.newstarts.cn

Go:   func add(a, b int) int
来源：http://iw.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kp.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iq.panjiajie.cn

[C14] 泛型函数
来源：http://xu.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gv.chemitech.net.cn

PHP:  // 无泛型
来源：http://ga.colortex.cn

JS:   // 无泛型
来源：http://bh.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pu.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mj.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qv.haigaiapp.cn

Ruby: # 无泛型
来源：http://rv.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zj.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://xs.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nf.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://ve.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tx.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ej.szsharing.cn

Java: // 无解构
来源：http://gu.9csxet.cn

Go:   // 无解构
来源：http://ti.wgjwhj.cn

Ruby: a, b = pair
来源：http://rn.9csxet.cn

C#:   var (a, b) = pair;
来源：http://hu.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://ug.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pu.muxihuayi.cn

PHP:  // 无重载
来源：http://cu.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wd.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://tg.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mm.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://zm.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://km.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zd.hahajie.cn

================================================================================
来源：http://ix.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://lq.panjiajie.cn

================================================================================
来源：http://yk.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://ig.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qt.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qd.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jo.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ci.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ob.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://oc.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://uw.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mo.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://af.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zz.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ar.chemitech.net.cn

JS:   arr.push(4);
来源：http://qd.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://az.shxzukj.cn

Java: list.add(4);
来源：http://ik.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://ql.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ib.muxihuayi.cn

C#:   list.Add(4);
来源：http://yy.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://as.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://dh.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ux.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wm.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://fc.hahajie.cn

Java: list.add(0, 0);
来源：http://ff.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gv.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bc.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://nh.jctech888.com.cn

[D04] 删除元素
来源：http://ok.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://my.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sm.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pk.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://vx.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qe.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wh.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://we.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cz.jctech888.com.cn

[D05] 访问与修改元素
来源：http://tf.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ed.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ho.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yt.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://bv.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://zo.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://jy.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ja.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vy.bjjhwx.cn

[D06] 数组长度
来源：http://ma.chemitech.net.cn

Py:   len(arr)
来源：http://gh.asd995.cn

PHP:  count($arr);
来源：http://aw.hahajie.cn

JS:   arr.length
来源：http://na.521024.cn

TS:   arr.length
来源：http://pa.haigaiapp.cn

Java: list.size();
来源：http://yi.yuntaijiaju.cn

Go:   len(arr)
来源：http://cj.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://cu.chemitech.net.cn

C#:   list.Count;
来源：http://yl.szsharing.cn

[D07] 切片 / 取子数组
来源：http://qn.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ks.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uo.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://jx.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://sv.asd995.cn

Java: list.subList(1, 4);
来源：http://yr.nszjky.cn

Go:   arr[1:4]
来源：http://oc.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://mw.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://qs.yuexingan06.cn

[D08] 合并两个数组
来源：http://qj.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://jn.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://rr.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oz.lnxyls.cn

TS:   [...a, ...b];
来源：http://pl.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://od.9csxet.cn

Go:   append(a, b...)
来源：http://cy.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://zu.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://ua.hnjuh.cn

[D09] 排序（升序）
来源：http://cx.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://tc.huixiangedu.cn

PHP:  sort($arr);
来源：http://st.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xk.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ih.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bk.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ps.521024.cn

Ruby: arr.sort
来源：http://od.jianghongdianzi.cn

C#:   list.Sort();
来源：http://xr.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kj.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rs.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qt.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xa.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tr.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://os.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nl.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bb.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://es.shxzskj.cn

[D11] 反转数组
来源：http://oa.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ui.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://pd.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zh.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://tu.521024.cn

Java: Collections.reverse(list);
来源：http://gl.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://ve.asd995.cn

Ruby: arr.reverse
来源：http://id.muxihuayi.cn

C#:   list.Reverse();
来源：http://iw.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://ak.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://vb.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wc.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xi.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://va.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zy.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://uu.huixiangedu.cn

Ruby: arr.index(x)
来源：http://sp.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://vj.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://mr.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://im.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qo.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://fs.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://qf.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pf.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zk.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rw.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vg.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://co.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vc.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fz.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://hu.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://yd.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sj.521024.cn

Go:   // 手写循环
来源：http://hm.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zv.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zn.lnxyls.cn

[D15] 去重
来源：http://la.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lg.lnxyls.cn

PHP:  array_unique($arr);
来源：http://ag.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://am.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://mp.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uh.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wp.shtwfgs.cn

Ruby: arr.uniq
来源：http://ku.asd995.cn

C#:   list.Distinct().ToList()
来源：http://rj.newstarts.cn

[D16] 求和与平均值
来源：http://vn.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sy.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ef.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sc.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cz.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rr.wgjwhj.cn

Go:   // 手写循环累加
来源：http://eo.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://va.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://bf.yuexingan06.cn

[D17] 最大值与最小值
来源：http://kk.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://qy.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://sh.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vg.gzmigu.cn

TS:   Math.max(...arr);
来源：http://ds.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yj.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://as.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://tw.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://gi.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://bq.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dm.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://te.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hb.huixiangedu.cn

TS:   nested.flat();
来源：http://iz.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ki.wgjwhj.cn

Go:   // 手写双层循环
来源：http://wc.shxzskj.cn

Ruby: nested.flatten
来源：http://wp.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oy.hahajie.cn

[D19] 按字段分组
来源：http://xy.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cs.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kl.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ob.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ze.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yi.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://ib.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sp.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iv.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://qj.wgjwhj.cn

Py:   Counter(arr)
来源：http://wy.asd995.cn

PHP:  array_count_values($arr);
来源：http://pj.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ui.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rb.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sr.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://fz.lnxyls.cn

Ruby: arr.tally
来源：http://sg.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ti.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://yq.newstarts.cn

Py:   x in arr
来源：http://pb.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://jf.huanxung.cn

JS:   arr.includes(x)
来源：http://zk.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://et.hnjuh.cn

Java: list.contains(x)
来源：http://ju.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://bt.panjiajie.cn

Ruby: arr.include?(x)
来源：http://un.newstarts.cn

C#:   list.Contains(x)
来源：http://om.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://tf.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kg.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bz.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ck.521024.cn

TS:   [...arr];
来源：http://wp.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://vd.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yd.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://ny.chemitech.net.cn

C#:   new List<int>(list);
来源：http://ia.szsharing.cn

[D23] reduce 累积计算
来源：http://cz.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ix.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://io.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xd.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tf.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bv.chemitech.net.cn

Go:   // 手写循环
来源：http://vg.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qj.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kc.521024.cn

[D24] 字典 / Map 基本操作
来源：http://gb.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ac.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hs.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xk.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vl.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sa.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ks.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kp.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vl.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://bh.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yi.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pe.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rz.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ea.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vh.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mm.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ki.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jk.hahajie.cn

[D26] 数组转字符串
来源：http://vn.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://wj.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://cl.jctech888.com.cn

JS:   arr.join(", ")
来源：http://ek.jctech888.com.cn

TS:   arr.join(", ")
来源：http://iv.wgjwhj.cn

Java: String.join(", ", list)
来源：http://mt.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://kg.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://te.asd995.cn

C#:   string.Join(", ", list)
来源：http://jh.hnjuh.cn

================================================================================
来源：http://yi.nicolike.cn

E. 字符串处理
来源：http://wx.yuexingan06.cn

================================================================================
来源：http://fm.haigaiapp.cn

[E01] 拼接字符串
来源：http://ke.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://co.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qo.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cl.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://re.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tt.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zk.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lf.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lr.yuntaijiaju.cn


<!-- 参考信息 -->