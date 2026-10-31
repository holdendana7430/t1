代发 wailian999

C#:   块级作用域
来源：http://gx.jctech888.com.cn

[C11] 模块导入与导出
来源：http://bi.huanxung.cn

Py:   from module import func
来源：http://ml.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zg.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lv.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qn.hnjuh.cn

Java: import java.util.List;
来源：http://fe.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xb.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://vo.nszjky.cn

C#:   using System.Text;
来源：http://yu.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://hm.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://am.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://be.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://yq.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://dt.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bo.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://et.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://vo.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://um.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://lu.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://id.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ky.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eh.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mx.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ye.hahajie.cn

Go:   func add(a, b int) int
来源：http://zi.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uj.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rl.jianghongdianzi.cn

[C14] 泛型函数
来源：http://bz.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vl.jctech888.com.cn

PHP:  // 无泛型
来源：http://ve.nicolike.cn

JS:   // 无泛型
来源：http://pw.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zn.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pb.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ej.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://kt.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nl.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://kq.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xt.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://ja.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zy.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mp.huixiangedu.cn

Java: // 无解构
来源：http://sp.huixiangedu.cn

Go:   // 无解构
来源：http://xf.shtwfgs.cn

Ruby: a, b = pair
来源：http://si.huanxung.cn

C#:   var (a, b) = pair;
来源：http://ez.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://hu.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xp.colortex.cn

PHP:  // 无重载
来源：http://kb.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oa.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://qk.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mx.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://mh.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://ld.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jh.521024.cn

================================================================================
来源：http://tj.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://db.huixiangedu.cn

================================================================================
来源：http://dx.szsharing.cn

[D01] 创建数组 / 列表
来源：http://pf.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sk.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ta.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://na.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tb.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://do.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://gf.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://iv.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hq.lnxyls.cn

[D02] 追加元素到末尾
来源：http://xv.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fv.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cg.lnxyls.cn

JS:   arr.push(4);
来源：http://gk.shxzskj.cn

TS:   arr.push(4);
来源：http://kc.panjiajie.cn

Java: list.add(4);
来源：http://jf.asd995.cn

Go:   arr = append(arr, 4)
来源：http://dh.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://tz.jctech888.com.cn

C#:   list.Add(4);
来源：http://ed.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://zm.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://sq.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hh.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ok.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://cg.muxihuayi.cn

Java: list.add(0, 0);
来源：http://if.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://td.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tf.521024.cn

C#:   list.Insert(0, 0);
来源：http://yl.nicolike.cn

[D04] 删除元素
来源：http://rp.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gt.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tv.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nn.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://rw.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rp.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xk.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://in.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ko.9csxet.cn

[D05] 访问与修改元素
来源：http://bt.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://of.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oo.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ky.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://hj.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://le.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://bp.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xq.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hh.bookmarksfly.cn

[D06] 数组长度
来源：http://jk.muxihuayi.cn

Py:   len(arr)
来源：http://ob.shtwfgs.cn

PHP:  count($arr);
来源：http://lh.bjjhwx.cn

JS:   arr.length
来源：http://gj.jctech888.com.cn

TS:   arr.length
来源：http://wm.huixinmuqiang.cn

Java: list.size();
来源：http://mo.yuexingan06.cn

Go:   len(arr)
来源：http://rg.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://wi.nicolike.cn

C#:   list.Count;
来源：http://oh.newstarts.cn

[D07] 切片 / 取子数组
来源：http://vv.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ha.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oc.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://ti.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://zf.9csxet.cn

Java: list.subList(1, 4);
来源：http://cl.bjjhwx.cn

Go:   arr[1:4]
来源：http://jn.521024.cn

Ruby: arr[1, 3]
来源：http://qu.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://vy.wgjwhj.cn

[D08] 合并两个数组
来源：http://yc.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://ma.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://is.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ca.colortex.cn

TS:   [...a, ...b];
来源：http://eo.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pi.bjjhwx.cn

Go:   append(a, b...)
来源：http://yj.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://or.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://nc.shxzskj.cn

[D09] 排序（升序）
来源：http://wn.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://sv.hahajie.cn

PHP:  sort($arr);
来源：http://lq.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xu.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lc.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qd.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bt.asd995.cn

Ruby: arr.sort
来源：http://on.nicolike.cn

C#:   list.Sort();
来源：http://lz.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lt.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://af.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pa.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ks.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dp.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zx.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oh.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://in.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pn.muxihuayi.cn

[D11] 反转数组
来源：http://vs.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vg.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://cp.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bd.hahajie.cn

TS:   [...arr].reverse();
来源：http://ad.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://nk.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://il.yuexingan06.cn

Ruby: arr.reverse
来源：http://ov.bookmarksfly.cn

C#:   list.Reverse();
来源：http://kl.huixiangedu.cn

[D12] 查找元素下标
来源：http://ex.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://mv.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pv.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lq.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lf.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dj.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://ip.asd995.cn

Ruby: arr.index(x)
来源：http://sw.nicolike.cn

C#:   list.IndexOf(x);
来源：http://cd.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://gp.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pk.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mu.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://ax.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://my.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bx.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yc.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cp.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mg.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://tu.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oy.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gq.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://qb.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://ns.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rx.shxzskj.cn

Go:   // 手写循环
来源：http://pk.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zi.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rl.chemitech.net.cn

[D15] 去重
来源：http://gf.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oh.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://ci.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://lj.huanxung.cn

TS:   [...new Set(arr)]
来源：http://mu.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uc.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://is.asd995.cn

Ruby: arr.uniq
来源：http://zz.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://jo.chemitech.net.cn

[D16] 求和与平均值
来源：http://xv.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kx.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pp.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pu.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ef.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nd.huixiangedu.cn

Go:   // 手写循环累加
来源：http://nj.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nv.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://zx.szsharing.cn

[D17] 最大值与最小值
来源：http://qz.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://qu.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://ww.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mx.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://hc.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oc.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yf.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://is.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://ai.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://tn.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xt.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://hw.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fc.huixiangedu.cn

TS:   nested.flat();
来源：http://pv.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ua.muxihuayi.cn

Go:   // 手写双层循环
来源：http://wh.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://kv.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tv.asd995.cn

[D19] 按字段分组
来源：http://qz.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://im.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ji.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rf.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tq.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bl.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://vc.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://en.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uk.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://zs.huixiangedu.cn

Py:   Counter(arr)
来源：http://dx.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://qg.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wi.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pc.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://le.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://ax.haigaiapp.cn

Ruby: arr.tally
来源：http://vb.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ng.nszjky.cn

[D21] 判断是否包含某元素
来源：http://mg.newstarts.cn

Py:   x in arr
来源：http://uj.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://ap.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://yl.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://xb.huixinmuqiang.cn

Java: list.contains(x)
来源：http://wm.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://ka.shxzukj.cn

Ruby: arr.include?(x)
来源：http://is.shtwfgs.cn

C#:   list.Contains(x)
来源：http://nm.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://dt.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oq.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rw.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pa.panjiajie.cn

TS:   [...arr];
来源：http://uu.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://rm.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://on.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://jr.wgjwhj.cn

C#:   new List<int>(list);
来源：http://tg.gzmigu.cn

[D23] reduce 累积计算
来源：http://sx.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gs.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ce.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ee.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://op.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hf.bjjhwx.cn

Go:   // 手写循环
来源：http://cp.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xa.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hy.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://sg.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ek.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gb.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ff.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ox.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wp.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ug.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ir.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lt.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://ld.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://su.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ds.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fo.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nw.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ny.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qf.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mn.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://td.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://na.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://cr.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://rn.hnjuh.cn

JS:   arr.join(", ")
来源：http://ai.chemitech.net.cn

TS:   arr.join(", ")
来源：http://pv.lnxyls.cn

Java: String.join(", ", list)
来源：http://wg.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://ql.521024.cn

Ruby: arr.join(", ")
来源：http://zg.nszjky.cn

C#:   string.Join(", ", list)
来源：http://rd.colortex.cn

================================================================================
来源：http://le.chemitech.net.cn

E. 字符串处理
来源：http://jv.jctech888.com.cn

================================================================================
来源：http://mp.hahajie.cn

[E01] 拼接字符串
来源：http://gw.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bu.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pa.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kz.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vi.lnxyls.cn


<!-- 参考信息 -->