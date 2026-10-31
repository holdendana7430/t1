代发 wailian999

[C10] 变量作用域
来源：http://az.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wu.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jv.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xn.chemitech.net.cn

TS:   同 JS
来源：http://qs.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://of.hahajie.cn

Go:   花括号块级作用域
来源：http://ta.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wg.huixinmuqiang.cn

C#:   块级作用域
来源：http://zf.lnxyls.cn

[C11] 模块导入与导出
来源：http://tr.colortex.cn

Py:   from module import func
来源：http://va.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jn.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gs.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ag.jianghongdianzi.cn

Java: import java.util.List;
来源：http://qt.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pn.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://aq.panjiajie.cn

C#:   using System.Text;
来源：http://le.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://le.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://ip.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://bu.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://ij.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://jm.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ly.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://xw.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://wu.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rr.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://un.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ia.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jm.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kj.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ec.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hl.panjiajie.cn

Go:   func add(a, b int) int
来源：http://fx.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ww.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pr.bookmarksfly.cn

[C14] 泛型函数
来源：http://ui.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dn.gzmigu.cn

PHP:  // 无泛型
来源：http://xw.jctech888.com.cn

JS:   // 无泛型
来源：http://oh.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jn.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cw.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ft.shxzukj.cn

Ruby: # 无泛型
来源：http://ep.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ak.521024.cn

[C15] 解构 / 展开参数
来源：http://pn.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ct.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://ix.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cd.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zv.jianghongdianzi.cn

Java: // 无解构
来源：http://cs.colortex.cn

Go:   // 无解构
来源：http://fx.hahajie.cn

Ruby: a, b = pair
来源：http://as.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://qs.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://pd.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rg.asd995.cn

PHP:  // 无重载
来源：http://gh.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vz.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://sr.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zs.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://na.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://hh.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://va.colortex.cn

================================================================================
来源：http://ti.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://pj.jctech888.com.cn

================================================================================
来源：http://px.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://kn.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tf.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ux.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ws.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gp.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nu.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://zi.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://dx.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gn.szxytkj.cn

[D02] 追加元素到末尾
来源：http://ez.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pg.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zi.hahajie.cn

JS:   arr.push(4);
来源：http://nr.yuexingan06.cn

TS:   arr.push(4);
来源：http://em.huixiangedu.cn

Java: list.add(4);
来源：http://qs.521024.cn

Go:   arr = append(arr, 4)
来源：http://go.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://vm.muxihuayi.cn

C#:   list.Add(4);
来源：http://mn.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://nl.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://zf.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oo.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fr.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://wi.nicolike.cn

Java: list.add(0, 0);
来源：http://xp.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qp.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pq.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://qw.haigaiapp.cn

[D04] 删除元素
来源：http://dq.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gt.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rk.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lt.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://wf.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xf.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ih.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ky.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bv.nszjky.cn

[D05] 访问与修改元素
来源：http://mg.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gg.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oc.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fa.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://rf.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://nx.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://gl.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://di.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lx.yuexingan06.cn

[D06] 数组长度
来源：http://jk.muxihuayi.cn

Py:   len(arr)
来源：http://dh.wgjwhj.cn

PHP:  count($arr);
来源：http://ti.bjjhwx.cn

JS:   arr.length
来源：http://sp.gzmigu.cn

TS:   arr.length
来源：http://im.huixinmuqiang.cn

Java: list.size();
来源：http://fz.haigaiapp.cn

Go:   len(arr)
来源：http://gu.hahajie.cn

Ruby: arr.length; arr.size
来源：http://tu.nszjky.cn

C#:   list.Count;
来源：http://ig.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://sb.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gy.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yc.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://sj.521024.cn

TS:   arr.slice(1, 4);
来源：http://dn.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://ch.shxzskj.cn

Go:   arr[1:4]
来源：http://ab.shxzskj.cn

Ruby: arr[1, 3]
来源：http://dl.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://vj.521024.cn

[D08] 合并两个数组
来源：http://ig.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://fg.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://yx.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cd.shtwfgs.cn

TS:   [...a, ...b];
来源：http://cj.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xf.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://oz.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://qc.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://js.hahajie.cn

[D09] 排序（升序）
来源：http://ma.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://gt.bookmarksfly.cn

PHP:  sort($arr);
来源：http://nl.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gk.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uo.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cz.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yj.hahajie.cn

Ruby: arr.sort
来源：http://fu.asd995.cn

C#:   list.Sort();
来源：http://fu.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ky.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yl.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ls.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yk.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wm.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ju.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dp.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uo.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cf.szxytkj.cn

[D11] 反转数组
来源：http://ei.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gz.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://mc.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hs.shxzukj.cn

TS:   [...arr].reverse();
来源：http://wj.hahajie.cn

Java: Collections.reverse(list);
来源：http://yn.asd995.cn

Go:   slices.Reverse(arr)
来源：http://sk.lnxyls.cn

Ruby: arr.reverse
来源：http://he.521024.cn

C#:   list.Reverse();
来源：http://zs.521024.cn

[D12] 查找元素下标
来源：http://pr.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://fw.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ip.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://go.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fp.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cd.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://au.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://qb.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://kl.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://oo.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jo.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dk.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://xc.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://jy.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iq.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eu.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dq.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uy.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://xy.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pm.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ep.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://hq.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://be.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://us.jianghongdianzi.cn

Go:   // 手写循环
来源：http://ub.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ne.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bp.nszjky.cn

[D15] 去重
来源：http://qq.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qu.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://sz.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://df.nszjky.cn

TS:   [...new Set(arr)]
来源：http://pr.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://px.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ci.9csxet.cn

Ruby: arr.uniq
来源：http://zy.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://oz.bjjhwx.cn

[D16] 求和与平均值
来源：http://qh.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fs.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zg.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://an.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gy.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kn.muxihuayi.cn

Go:   // 手写循环累加
来源：http://ep.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://on.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://mz.nszjky.cn

[D17] 最大值与最小值
来源：http://jn.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://kn.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://pa.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rq.shxzukj.cn

TS:   Math.max(...arr);
来源：http://zt.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oi.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jr.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://pa.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://bp.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://zd.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pe.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://cv.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pi.gzmigu.cn

TS:   nested.flat();
来源：http://ba.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jr.nszjky.cn

Go:   // 手写双层循环
来源：http://uk.haigaiapp.cn

Ruby: nested.flatten
来源：http://nc.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iy.lnxyls.cn

[D19] 按字段分组
来源：http://zm.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pq.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fo.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tn.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lh.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qe.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://xk.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bn.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pi.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://uu.bookmarksfly.cn

Py:   Counter(arr)
来源：http://tm.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://hg.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lp.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://az.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xa.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://ja.wgjwhj.cn

Ruby: arr.tally
来源：http://ni.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://da.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://ib.nicolike.cn

Py:   x in arr
来源：http://fw.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://xk.jctech888.com.cn

JS:   arr.includes(x)
来源：http://qr.asd995.cn

TS:   arr.includes(x)
来源：http://ct.wgjwhj.cn

Java: list.contains(x)
来源：http://wk.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://os.521024.cn

Ruby: arr.include?(x)
来源：http://zh.jctech888.com.cn

C#:   list.Contains(x)
来源：http://cj.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://qo.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://is.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ow.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jd.nicolike.cn

TS:   [...arr];
来源：http://uc.szsharing.cn

Java: new ArrayList<>(list);
来源：http://cv.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vr.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://iy.jctech888.com.cn

C#:   new List<int>(list);
来源：http://gm.shxzukj.cn

[D23] reduce 累积计算
来源：http://le.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lq.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://er.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ze.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://il.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ly.haigaiapp.cn

Go:   // 手写循环
来源：http://ie.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ag.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lb.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://ip.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bw.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bq.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xn.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kc.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pm.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ou.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ds.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ri.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://af.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kr.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://np.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yj.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hf.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xt.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ts.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rb.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hk.huixiangedu.cn

[D26] 数组转字符串
来源：http://es.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://eq.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://qm.521024.cn

JS:   arr.join(", ")
来源：http://jv.colortex.cn

TS:   arr.join(", ")
来源：http://mg.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://is.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://wi.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://eb.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://ky.lnxyls.cn


<!-- 参考信息 -->