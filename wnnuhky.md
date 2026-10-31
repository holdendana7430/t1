代发 wailian999

C#:   块级作用域
来源：http://sl.colortex.cn

[C11] 模块导入与导出
来源：http://gc.chemitech.net.cn

Py:   from module import func
来源：http://wm.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rp.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gy.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://od.shtwfgs.cn

Java: import java.util.List;
来源：http://fi.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oy.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://cl.bookmarksfly.cn

C#:   using System.Text;
来源：http://jr.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://bl.521024.cn

Py:   (lambda: print("run"))()
来源：http://qn.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://vo.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://lx.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://az.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gi.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://zr.521024.cn

Ruby: -> { puts "run" }.call
来源：http://ak.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ab.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://so.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jq.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gp.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pe.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zp.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kr.nicolike.cn

Go:   func add(a, b int) int
来源：http://ex.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qm.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ps.chemitech.net.cn

[C14] 泛型函数
来源：http://sl.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rr.hnjuh.cn

PHP:  // 无泛型
来源：http://ey.yuexingan06.cn

JS:   // 无泛型
来源：http://mb.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://es.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://es.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hh.shtwfgs.cn

Ruby: # 无泛型
来源：http://ml.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lh.colortex.cn

[C15] 解构 / 展开参数
来源：http://uc.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hu.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://xu.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://el.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://os.jianghongdianzi.cn

Java: // 无解构
来源：http://qd.nicolike.cn

Go:   // 无解构
来源：http://rk.newstarts.cn

Ruby: a, b = pair
来源：http://dh.nicolike.cn

C#:   var (a, b) = pair;
来源：http://ju.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://om.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sw.huixiangedu.cn

PHP:  // 无重载
来源：http://yv.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://di.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://uq.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wk.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://ji.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://xp.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://my.nszjky.cn

================================================================================
来源：http://ey.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://ja.shxzukj.cn

================================================================================
来源：http://bn.colortex.cn

[D01] 创建数组 / 列表
来源：http://dg.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pj.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pb.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mc.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ev.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ju.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://ef.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://fm.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jc.asd995.cn

[D02] 追加元素到末尾
来源：http://qs.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bw.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://to.chemitech.net.cn

JS:   arr.push(4);
来源：http://vg.shtwfgs.cn

TS:   arr.push(4);
来源：http://ic.wgjwhj.cn

Java: list.add(4);
来源：http://rz.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://ab.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://kl.lnxyls.cn

C#:   list.Add(4);
来源：http://vg.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://hy.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://kd.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ww.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wn.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://gk.huixiangedu.cn

Java: list.add(0, 0);
来源：http://wi.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hr.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hy.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://os.bjjhwx.cn

[D04] 删除元素
来源：http://cy.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mq.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fi.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fh.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://kz.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jh.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nj.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wd.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ia.chemitech.net.cn

[D05] 访问与修改元素
来源：http://zp.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://td.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hw.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ft.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://iw.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://ru.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://ri.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ct.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ek.szxytkj.cn

[D06] 数组长度
来源：http://vg.newstarts.cn

Py:   len(arr)
来源：http://bn.muxihuayi.cn

PHP:  count($arr);
来源：http://ve.jianghongdianzi.cn

JS:   arr.length
来源：http://ae.jctech888.com.cn

TS:   arr.length
来源：http://hn.wgjwhj.cn

Java: list.size();
来源：http://fl.yuntaijiaju.cn

Go:   len(arr)
来源：http://mr.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://ag.szxytkj.cn

C#:   list.Count;
来源：http://wx.nicolike.cn

[D07] 切片 / 取子数组
来源：http://cc.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pk.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ro.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://uz.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://th.newstarts.cn

Java: list.subList(1, 4);
来源：http://ef.chemitech.net.cn

Go:   arr[1:4]
来源：http://mn.9csxet.cn

Ruby: arr[1, 3]
来源：http://wi.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://vg.szxytkj.cn

[D08] 合并两个数组
来源：http://rh.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://pb.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://mf.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pw.nszjky.cn

TS:   [...a, ...b];
来源：http://mq.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qd.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://mp.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://vw.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://jt.9csxet.cn

[D09] 排序（升序）
来源：http://zx.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://aa.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://ov.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ff.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xg.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bq.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kt.hnjuh.cn

Ruby: arr.sort
来源：http://rg.shxzukj.cn

C#:   list.Sort();
来源：http://yr.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eu.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bc.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cb.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ru.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zx.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zl.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zk.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oh.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xs.wgjwhj.cn

[D11] 反转数组
来源：http://ai.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cq.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://nw.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vq.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://mc.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://zg.asd995.cn

Go:   slices.Reverse(arr)
来源：http://de.shxzskj.cn

Ruby: arr.reverse
来源：http://zq.nszjky.cn

C#:   list.Reverse();
来源：http://if.muxihuayi.cn

[D12] 查找元素下标
来源：http://lx.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://hx.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vh.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ji.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vw.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://no.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://wj.colortex.cn

Ruby: arr.index(x)
来源：http://wl.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://kt.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://xx.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dq.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jp.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://dg.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://xv.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ic.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eb.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ll.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ub.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://ur.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://md.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uk.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://vg.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://av.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mc.shxzukj.cn

Go:   // 手写循环
来源：http://yo.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kd.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hy.colortex.cn

[D15] 去重
来源：http://js.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dy.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://lt.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://tz.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://dd.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hm.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ig.chemitech.net.cn

Ruby: arr.uniq
来源：http://tj.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://rj.panjiajie.cn

[D16] 求和与平均值
来源：http://gm.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iv.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nx.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yf.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rk.9csxet.cn

Go:   // 手写循环累加
来源：http://np.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bk.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://je.521024.cn

[D17] 最大值与最小值
来源：http://gi.521024.cn

Py:   max(arr);  min(arr)
来源：http://in.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://um.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xd.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://rm.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oz.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fe.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://ye.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://wb.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://ia.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zr.colortex.cn

PHP:  array_merge(...$nested);
来源：http://pq.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yq.huanxung.cn

TS:   nested.flat();
来源：http://iq.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ve.wgjwhj.cn

Go:   // 手写双层循环
来源：http://rk.lnxyls.cn

Ruby: nested.flatten
来源：http://ld.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fk.yuntaijiaju.cn

[D19] 按字段分组
来源：http://gh.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wt.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rg.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ed.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ru.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fa.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://du.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rj.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iq.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://ge.wgjwhj.cn

Py:   Counter(arr)
来源：http://gc.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://bt.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yb.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zb.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yg.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://qi.haigaiapp.cn

Ruby: arr.tally
来源：http://ws.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cz.9csxet.cn

[D21] 判断是否包含某元素
来源：http://xk.9csxet.cn

Py:   x in arr
来源：http://wg.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://xw.bjjhwx.cn

JS:   arr.includes(x)
来源：http://rd.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://qy.haigaiapp.cn

Java: list.contains(x)
来源：http://jf.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://lv.shxzskj.cn

Ruby: arr.include?(x)
来源：http://tf.huanxung.cn

C#:   list.Contains(x)
来源：http://bf.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://bn.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ig.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gr.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rj.szxytkj.cn

TS:   [...arr];
来源：http://en.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://ut.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sv.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://oe.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://sf.lnxyls.cn

[D23] reduce 累积计算
来源：http://di.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ht.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zb.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://is.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mk.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dn.muxihuayi.cn

Go:   // 手写循环
来源：http://vx.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rl.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jk.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://tx.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lg.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://am.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mo.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hv.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wp.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rm.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ym.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xd.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://gm.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cj.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rr.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mx.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fs.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ti.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wz.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ny.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ke.hnjuh.cn

[D26] 数组转字符串
来源：http://st.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://yh.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://cs.szxytkj.cn

JS:   arr.join(", ")
来源：http://jp.nszjky.cn

TS:   arr.join(", ")
来源：http://xi.hahajie.cn

Java: String.join(", ", list)
来源：http://pm.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://zj.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://ah.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://hg.szsharing.cn

================================================================================
来源：http://ig.nszjky.cn

E. 字符串处理
来源：http://vk.colortex.cn

================================================================================
来源：http://ax.szsharing.cn

[E01] 拼接字符串
来源：http://kt.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eq.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cd.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qi.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bb.huixinmuqiang.cn


<!-- 参考信息 -->