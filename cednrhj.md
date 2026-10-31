代发 wailian999

TS:   同 JS
来源：http://no.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://go.9csxet.cn

Go:   花括号块级作用域
来源：http://qv.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ld.9csxet.cn

C#:   块级作用域
来源：http://ga.shtwfgs.cn

[C11] 模块导入与导出
来源：http://cq.chemitech.net.cn

Py:   from module import func
来源：http://og.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vh.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cq.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ol.newstarts.cn

Java: import java.util.List;
来源：http://of.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://os.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://st.haigaiapp.cn

C#:   using System.Text;
来源：http://jx.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://xi.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://fh.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://bv.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://vy.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://wk.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zk.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://sw.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://nj.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://at.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://hh.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mi.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sv.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ye.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mo.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cf.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://it.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tm.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bx.bookmarksfly.cn

[C14] 泛型函数
来源：http://yk.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xa.panjiajie.cn

PHP:  // 无泛型
来源：http://dz.huixinmuqiang.cn

JS:   // 无泛型
来源：http://ku.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uw.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ne.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vu.9csxet.cn

Ruby: # 无泛型
来源：http://oo.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jx.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://qy.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ne.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://oa.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ob.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dp.yuntaijiaju.cn

Java: // 无解构
来源：http://zo.nszjky.cn

Go:   // 无解构
来源：http://yn.szxytkj.cn

Ruby: a, b = pair
来源：http://kf.nszjky.cn

C#:   var (a, b) = pair;
来源：http://fy.hahajie.cn

[C16] 函数 / 方法重载
来源：http://ib.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://us.huixiangedu.cn

PHP:  // 无重载
来源：http://ui.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hh.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://tf.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ba.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://xb.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://ir.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oz.asd995.cn

================================================================================
来源：http://ex.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://ud.huixinmuqiang.cn

================================================================================
来源：http://qd.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://fd.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://du.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mq.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tr.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mb.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vb.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://ev.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://qa.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gq.huanxung.cn

[D02] 追加元素到末尾
来源：http://dq.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tk.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rr.newstarts.cn

JS:   arr.push(4);
来源：http://yv.shtwfgs.cn

TS:   arr.push(4);
来源：http://ua.521024.cn

Java: list.add(4);
来源：http://wx.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://la.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ny.newstarts.cn

C#:   list.Add(4);
来源：http://wj.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://zp.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://oz.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aa.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://da.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://jm.9csxet.cn

Java: list.add(0, 0);
来源：http://hw.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vb.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bt.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://mz.521024.cn

[D04] 删除元素
来源：http://xh.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://td.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pd.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pn.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://ia.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zg.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ud.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bg.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xx.lnxyls.cn

[D05] 访问与修改元素
来源：http://jm.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://it.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hs.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://be.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://kz.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://rn.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://ma.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ns.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ia.chemitech.net.cn

[D06] 数组长度
来源：http://kv.asd995.cn

Py:   len(arr)
来源：http://ch.gzmigu.cn

PHP:  count($arr);
来源：http://sj.nicolike.cn

JS:   arr.length
来源：http://ny.wgjwhj.cn

TS:   arr.length
来源：http://yc.nszjky.cn

Java: list.size();
来源：http://tj.shtwfgs.cn

Go:   len(arr)
来源：http://yl.9csxet.cn

Ruby: arr.length; arr.size
来源：http://ng.nicolike.cn

C#:   list.Count;
来源：http://bg.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://zy.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gs.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fx.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://et.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://ex.hahajie.cn

Java: list.subList(1, 4);
来源：http://ho.colortex.cn

Go:   arr[1:4]
来源：http://xx.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://eu.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://dj.chemitech.net.cn

[D08] 合并两个数组
来源：http://lv.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://qg.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://tz.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qe.panjiajie.cn

TS:   [...a, ...b];
来源：http://xp.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eo.szxytkj.cn

Go:   append(a, b...)
来源：http://bn.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://kw.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://lr.panjiajie.cn

[D09] 排序（升序）
来源：http://iv.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://bl.yuexingan06.cn

PHP:  sort($arr);
来源：http://cl.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sj.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oh.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ag.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://by.huanxung.cn

Ruby: arr.sort
来源：http://dg.nszjky.cn

C#:   list.Sort();
来源：http://ec.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fp.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yg.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xr.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rx.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lz.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xn.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wt.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dl.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ag.bookmarksfly.cn

[D11] 反转数组
来源：http://gj.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wq.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://se.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://to.9csxet.cn

TS:   [...arr].reverse();
来源：http://uk.521024.cn

Java: Collections.reverse(list);
来源：http://tv.asd995.cn

Go:   slices.Reverse(arr)
来源：http://wu.nszjky.cn

Ruby: arr.reverse
来源：http://nq.gzmigu.cn

C#:   list.Reverse();
来源：http://py.chemitech.net.cn

[D12] 查找元素下标
来源：http://uk.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://vd.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lc.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://or.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bv.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://su.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://gi.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://rj.9csxet.cn

C#:   list.IndexOf(x);
来源：http://qt.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://oo.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iw.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://of.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://qy.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://sr.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cs.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hp.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ox.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kh.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://qe.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yc.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jz.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://tx.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://bw.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bs.shxzukj.cn

Go:   // 手写循环
来源：http://pq.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gl.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lz.9csxet.cn

[D15] 去重
来源：http://hk.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bx.newstarts.cn

PHP:  array_unique($arr);
来源：http://bq.newstarts.cn

JS:   [...new Set(arr)]
来源：http://qa.newstarts.cn

TS:   [...new Set(arr)]
来源：http://ld.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dt.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pu.bjjhwx.cn

Ruby: arr.uniq
来源：http://tm.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://lk.yuexingan06.cn

[D16] 求和与平均值
来源：http://uf.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ob.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yy.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yi.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oi.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lz.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://er.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ea.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://fl.panjiajie.cn

[D17] 最大值与最小值
来源：http://dh.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://kh.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://vt.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hs.nszjky.cn

TS:   Math.max(...arr);
来源：http://bu.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kf.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zj.asd995.cn

Ruby: arr.max;  arr.min
来源：http://mz.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://jt.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://bv.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wo.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://sm.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://km.muxihuayi.cn

TS:   nested.flat();
来源：http://kw.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sd.jctech888.com.cn

Go:   // 手写双层循环
来源：http://ye.jctech888.com.cn

Ruby: nested.flatten
来源：http://bl.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gr.wgjwhj.cn

[D19] 按字段分组
来源：http://pn.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lu.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tj.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://os.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hr.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fe.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://yv.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bg.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hd.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://bg.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://lt.colortex.cn

PHP:  array_count_values($arr);
来源：http://da.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xp.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ny.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xq.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://ux.bookmarksfly.cn

Ruby: arr.tally
来源：http://or.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://de.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://am.bookmarksfly.cn

Py:   x in arr
来源：http://zm.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://ro.haigaiapp.cn

JS:   arr.includes(x)
来源：http://wy.shxzukj.cn

TS:   arr.includes(x)
来源：http://mh.colortex.cn

Java: list.contains(x)
来源：http://qi.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://xq.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://on.9csxet.cn

C#:   list.Contains(x)
来源：http://vz.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://qt.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mi.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qc.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ny.yuexingan06.cn

TS:   [...arr];
来源：http://fu.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://nx.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bk.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://yf.szsharing.cn

C#:   new List<int>(list);
来源：http://in.asd995.cn

[D23] reduce 累积计算
来源：http://yf.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ni.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xs.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dq.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ju.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tm.huixinmuqiang.cn

Go:   // 手写循环
来源：http://tp.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fx.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ry.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://yb.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jj.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uk.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ko.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tl.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ev.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://do.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xv.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rl.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://xv.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bz.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zx.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zj.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xe.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kb.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fw.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ng.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mx.wgjwhj.cn

[D26] 数组转字符串
来源：http://hg.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://xp.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://mm.shtwfgs.cn

JS:   arr.join(", ")
来源：http://ar.shxzukj.cn

TS:   arr.join(", ")
来源：http://vl.gzmigu.cn

Java: String.join(", ", list)
来源：http://lo.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://uw.shxzskj.cn

Ruby: arr.join(", ")
来源：http://nd.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://rz.huanxung.cn

================================================================================
来源：http://fm.yuexingan06.cn

E. 字符串处理
来源：http://is.panjiajie.cn

================================================================================
来源：http://dp.bookmarksfly.cn

[E01] 拼接字符串
来源：http://qn.hnjuh.cn


<!-- 参考信息 -->