代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://mg.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ou.muxihuayi.cn

Java: import java.util.List;
来源：http://uo.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rc.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://xn.shxzukj.cn

C#:   using System.Text;
来源：http://lt.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://uj.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://dl.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://bh.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://kw.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://pj.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zz.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://oj.521024.cn

Ruby: -> { puts "run" }.call
来源：http://cy.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jk.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://lq.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tr.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fr.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eo.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vv.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://go.asd995.cn

Go:   func add(a, b int) int
来源：http://mc.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fj.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wc.asd995.cn

[C14] 泛型函数
来源：http://qp.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zz.szxytkj.cn

PHP:  // 无泛型
来源：http://qa.haigaiapp.cn

JS:   // 无泛型
来源：http://lg.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sm.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kc.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zf.hahajie.cn

Ruby: # 无泛型
来源：http://yc.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jv.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://jo.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rn.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://cm.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fw.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kr.yuntaijiaju.cn

Java: // 无解构
来源：http://sb.szsharing.cn

Go:   // 无解构
来源：http://pb.lnxyls.cn

Ruby: a, b = pair
来源：http://fe.huanxung.cn

C#:   var (a, b) = pair;
来源：http://eb.colortex.cn

[C16] 函数 / 方法重载
来源：http://bb.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gu.jctech888.com.cn

PHP:  // 无重载
来源：http://bk.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zp.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://ia.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rv.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://et.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://dt.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gy.bookmarksfly.cn

================================================================================
来源：http://pv.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://oq.szxytkj.cn

================================================================================
来源：http://cg.newstarts.cn

[D01] 创建数组 / 列表
来源：http://rl.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zx.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://od.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qs.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rt.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wt.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://iq.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://mu.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wm.521024.cn

[D02] 追加元素到末尾
来源：http://yi.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qj.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pd.shtwfgs.cn

JS:   arr.push(4);
来源：http://nw.huixiangedu.cn

TS:   arr.push(4);
来源：http://ci.wgjwhj.cn

Java: list.add(4);
来源：http://ra.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://bx.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ii.9csxet.cn

C#:   list.Add(4);
来源：http://hm.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://be.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://th.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://db.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qc.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://cq.521024.cn

Java: list.add(0, 0);
来源：http://ti.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ku.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xy.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://ar.huanxung.cn

[D04] 删除元素
来源：http://vc.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mh.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://az.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lk.colortex.cn

TS:   arr.splice(0, 1);
来源：http://sv.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ga.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vx.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oj.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ut.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://ck.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fw.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lf.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ua.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://sz.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://iq.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://ku.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://or.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://px.shtwfgs.cn

[D06] 数组长度
来源：http://le.wgjwhj.cn

Py:   len(arr)
来源：http://vu.bookmarksfly.cn

PHP:  count($arr);
来源：http://ug.jianghongdianzi.cn

JS:   arr.length
来源：http://el.9csxet.cn

TS:   arr.length
来源：http://gz.shxzskj.cn

Java: list.size();
来源：http://be.yuexingan06.cn

Go:   len(arr)
来源：http://li.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://xl.shxzskj.cn

C#:   list.Count;
来源：http://an.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://gi.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ui.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bg.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://ub.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://xv.newstarts.cn

Java: list.subList(1, 4);
来源：http://le.asd995.cn

Go:   arr[1:4]
来源：http://nz.huanxung.cn

Ruby: arr[1, 3]
来源：http://xu.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://ar.shxzskj.cn

[D08] 合并两个数组
来源：http://os.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://yl.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://oy.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://my.haigaiapp.cn

TS:   [...a, ...b];
来源：http://qf.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ce.colortex.cn

Go:   append(a, b...)
来源：http://ak.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://mh.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://qc.lnxyls.cn

[D09] 排序（升序）
来源：http://fd.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://el.haigaiapp.cn

PHP:  sort($arr);
来源：http://wm.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yn.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oy.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aq.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qz.hahajie.cn

Ruby: arr.sort
来源：http://nj.szsharing.cn

C#:   list.Sort();
来源：http://nd.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lf.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://op.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ec.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bs.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://md.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ro.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dh.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://py.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sx.nszjky.cn

[D11] 反转数组
来源：http://xb.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zq.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://vn.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jn.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://wf.shxzskj.cn

Java: Collections.reverse(list);
来源：http://sy.asd995.cn

Go:   slices.Reverse(arr)
来源：http://qm.chemitech.net.cn

Ruby: arr.reverse
来源：http://lj.521024.cn

C#:   list.Reverse();
来源：http://ga.asd995.cn

[D12] 查找元素下标
来源：http://vb.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://ou.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xi.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eg.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://je.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tw.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://qx.521024.cn

Ruby: arr.index(x)
来源：http://gd.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://sz.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://ik.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hv.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yy.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://ji.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://zg.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://he.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bz.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uz.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ob.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://yg.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xl.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wz.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://br.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://hc.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wx.wgjwhj.cn

Go:   // 手写循环
来源：http://nj.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ap.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hy.huixiangedu.cn

[D15] 去重
来源：http://el.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qi.521024.cn

PHP:  array_unique($arr);
来源：http://sq.huanxung.cn

JS:   [...new Set(arr)]
来源：http://tu.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://pa.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jd.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sv.bookmarksfly.cn

Ruby: arr.uniq
来源：http://lm.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://hr.521024.cn

[D16] 求和与平均值
来源：http://dk.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vb.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rk.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tp.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bz.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://al.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://gt.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dp.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://kb.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://mr.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://ri.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://ir.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fx.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://aw.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zp.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nv.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://tl.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://rx.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://iv.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fw.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://pa.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sf.wgjwhj.cn

TS:   nested.flat();
来源：http://nf.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cu.haigaiapp.cn

Go:   // 手写双层循环
来源：http://gf.szxytkj.cn

Ruby: nested.flatten
来源：http://ir.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qp.yuexingan06.cn

[D19] 按字段分组
来源：http://os.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bq.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jd.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rh.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xi.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fb.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://lz.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kk.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ai.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://dc.newstarts.cn

Py:   Counter(arr)
来源：http://de.szsharing.cn

PHP:  array_count_values($arr);
来源：http://nl.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iz.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yx.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ig.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://xu.yuexingan06.cn

Ruby: arr.tally
来源：http://dv.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bs.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://fn.chemitech.net.cn

Py:   x in arr
来源：http://iv.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://cf.521024.cn

JS:   arr.includes(x)
来源：http://od.jctech888.com.cn

TS:   arr.includes(x)
来源：http://qv.haigaiapp.cn

Java: list.contains(x)
来源：http://ow.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://ol.panjiajie.cn

Ruby: arr.include?(x)
来源：http://rn.colortex.cn

C#:   list.Contains(x)
来源：http://jk.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://vm.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qg.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wr.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vj.muxihuayi.cn

TS:   [...arr];
来源：http://pq.nszjky.cn

Java: new ArrayList<>(list);
来源：http://my.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gm.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://xe.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://sq.shxzukj.cn

[D23] reduce 累积计算
来源：http://dr.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://df.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ym.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ix.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fq.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ph.haigaiapp.cn

Go:   // 手写循环
来源：http://ng.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ww.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nx.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://ti.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mr.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kv.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://me.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aw.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jg.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hb.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dk.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ow.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://pb.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bv.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pw.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zf.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zf.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cv.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://he.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xz.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ao.bjjhwx.cn

[D26] 数组转字符串
来源：http://cq.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://ws.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://qr.wgjwhj.cn

JS:   arr.join(", ")
来源：http://wj.wgjwhj.cn

TS:   arr.join(", ")
来源：http://fc.huixiangedu.cn

Java: String.join(", ", list)
来源：http://hm.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://kz.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://tw.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://gz.bjjhwx.cn

================================================================================
来源：http://aj.muxihuayi.cn

E. 字符串处理
来源：http://uq.jctech888.com.cn

================================================================================
来源：http://rw.muxihuayi.cn

[E01] 拼接字符串
来源：http://ts.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://py.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cr.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mg.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wv.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mq.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nf.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vh.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ae.9csxet.cn


<!-- 参考信息 -->