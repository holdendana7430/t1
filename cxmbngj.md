代发 wailian999

TS:   同 JS
来源：http://sj.huanxung.cn

Java: 方法内为块级作用域
来源：http://ow.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://lj.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xw.colortex.cn

C#:   块级作用域
来源：http://sg.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://wy.newstarts.cn

Py:   from module import func
来源：http://lo.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bg.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tf.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fr.nicolike.cn

Java: import java.util.List;
来源：http://ap.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yr.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://kq.huixiangedu.cn

C#:   using System.Text;
来源：http://hn.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://jf.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://sy.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://my.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://fd.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://xf.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ru.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://bp.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://an.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ba.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://dd.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hw.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wo.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ik.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gp.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zg.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://ax.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aa.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yq.521024.cn

[C14] 泛型函数
来源：http://oi.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hi.colortex.cn

PHP:  // 无泛型
来源：http://eh.bookmarksfly.cn

JS:   // 无泛型
来源：http://ev.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hc.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://km.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xc.lnxyls.cn

Ruby: # 无泛型
来源：http://aj.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fh.huanxung.cn

[C15] 解构 / 展开参数
来源：http://xf.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nh.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://ab.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wg.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://td.szsharing.cn

Java: // 无解构
来源：http://mk.newstarts.cn

Go:   // 无解构
来源：http://or.521024.cn

Ruby: a, b = pair
来源：http://vi.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://pd.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://cp.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uk.szsharing.cn

PHP:  // 无重载
来源：http://yc.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zd.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://ek.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iy.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://py.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://gl.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rv.shxzskj.cn

================================================================================
来源：http://vy.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://nv.colortex.cn

================================================================================
来源：http://wt.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://fg.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gk.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ds.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lt.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yk.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gl.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://gl.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://gk.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oz.shxzukj.cn

[D02] 追加元素到末尾
来源：http://je.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xx.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zk.asd995.cn

JS:   arr.push(4);
来源：http://xj.wgjwhj.cn

TS:   arr.push(4);
来源：http://wl.chemitech.net.cn

Java: list.add(4);
来源：http://bu.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://xy.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://te.521024.cn

C#:   list.Add(4);
来源：http://dn.9csxet.cn

[D03] 在指定位置插入元素
来源：http://lp.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://cw.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qy.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iq.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://om.nszjky.cn

Java: list.add(0, 0);
来源：http://mb.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jn.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hq.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://js.haigaiapp.cn

[D04] 删除元素
来源：http://fo.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yr.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ia.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lw.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://pd.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bi.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://du.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xh.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pf.huixiangedu.cn

[D05] 访问与修改元素
来源：http://zr.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dt.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://du.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hk.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://qc.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://lu.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://vm.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wv.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vv.bjjhwx.cn

[D06] 数组长度
来源：http://mv.huixiangedu.cn

Py:   len(arr)
来源：http://ls.huixiangedu.cn

PHP:  count($arr);
来源：http://hq.wgjwhj.cn

JS:   arr.length
来源：http://eu.szxytkj.cn

TS:   arr.length
来源：http://ep.yuntaijiaju.cn

Java: list.size();
来源：http://uk.huixiangedu.cn

Go:   len(arr)
来源：http://zn.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://li.chemitech.net.cn

C#:   list.Count;
来源：http://bc.hahajie.cn

[D07] 切片 / 取子数组
来源：http://xj.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dw.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://id.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://bo.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://ts.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://ru.huixiangedu.cn

Go:   arr[1:4]
来源：http://fk.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://gb.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://ab.521024.cn

[D08] 合并两个数组
来源：http://vy.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://ch.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://px.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://da.huanxung.cn

TS:   [...a, ...b];
来源：http://gm.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qo.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://et.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://mu.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://mk.shtwfgs.cn

[D09] 排序（升序）
来源：http://lt.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://wg.521024.cn

PHP:  sort($arr);
来源：http://oc.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pm.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dz.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gj.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uc.muxihuayi.cn

Ruby: arr.sort
来源：http://pz.szsharing.cn

C#:   list.Sort();
来源：http://yw.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vt.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ik.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lo.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oa.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lk.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xz.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yv.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ft.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://co.shxzukj.cn

[D11] 反转数组
来源：http://lp.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://je.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://ka.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://am.newstarts.cn

TS:   [...arr].reverse();
来源：http://ie.colortex.cn

Java: Collections.reverse(list);
来源：http://su.colortex.cn

Go:   slices.Reverse(arr)
来源：http://fu.521024.cn

Ruby: arr.reverse
来源：http://yj.muxihuayi.cn

C#:   list.Reverse();
来源：http://rh.nicolike.cn

[D12] 查找元素下标
来源：http://tc.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://hp.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lh.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sb.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ds.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://er.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://es.hnjuh.cn

Ruby: arr.index(x)
来源：http://lw.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://ka.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://ew.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pd.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://at.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://mq.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://uz.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lj.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sy.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tw.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ap.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://pt.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oo.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wl.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://rw.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://al.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ad.shxzskj.cn

Go:   // 手写循环
来源：http://sl.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fc.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oy.nicolike.cn

[D15] 去重
来源：http://sl.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wm.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://cq.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://ft.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://hg.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lc.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://an.shxzukj.cn

Ruby: arr.uniq
来源：http://bp.colortex.cn

C#:   list.Distinct().ToList()
来源：http://oo.gzmigu.cn

[D16] 求和与平均值
来源：http://il.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qu.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zp.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ga.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zo.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sk.shxzskj.cn

Go:   // 手写循环累加
来源：http://rs.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fh.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://ui.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://zq.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://so.521024.cn

PHP:  max($arr);  min($arr);
来源：http://ns.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rd.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://ky.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jz.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gd.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ub.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://oc.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://xm.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zi.colortex.cn

PHP:  array_merge(...$nested);
来源：http://mo.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ho.lnxyls.cn

TS:   nested.flat();
来源：http://ia.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lo.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://yk.asd995.cn

Ruby: nested.flatten
来源：http://ny.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ps.nszjky.cn

[D19] 按字段分组
来源：http://pd.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fp.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sg.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lp.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jw.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://un.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://ex.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yg.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iv.asd995.cn

[D20] 统计每个元素出现次数
来源：http://ub.chemitech.net.cn

Py:   Counter(arr)
来源：http://po.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://pz.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ys.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ex.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qn.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://fq.colortex.cn

Ruby: arr.tally
来源：http://qp.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bn.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://jd.panjiajie.cn

Py:   x in arr
来源：http://ia.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://hw.gzmigu.cn

JS:   arr.includes(x)
来源：http://ud.panjiajie.cn

TS:   arr.includes(x)
来源：http://ol.huixiangedu.cn

Java: list.contains(x)
来源：http://fp.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://xp.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://sf.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://oi.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://fv.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gz.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sa.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pw.gzmigu.cn

TS:   [...arr];
来源：http://md.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ib.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://is.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://pv.nicolike.cn

C#:   new List<int>(list);
来源：http://cl.newstarts.cn

[D23] reduce 累积计算
来源：http://la.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://py.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zd.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dc.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ig.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ha.newstarts.cn

Go:   // 手写循环
来源：http://qd.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://md.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xs.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://mt.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ok.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ff.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bi.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sq.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yz.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tp.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tr.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dw.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://xr.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dp.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hk.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jy.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dz.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jh.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uw.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qi.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qf.shxzskj.cn

[D26] 数组转字符串
来源：http://gv.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://av.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://yy.hahajie.cn

JS:   arr.join(", ")
来源：http://jn.shxzukj.cn

TS:   arr.join(", ")
来源：http://sk.yuexingan06.cn

Java: String.join(", ", list)
来源：http://zw.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://zv.huanxung.cn

Ruby: arr.join(", ")
来源：http://lg.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://gx.bookmarksfly.cn

================================================================================
来源：http://zt.shxzukj.cn

E. 字符串处理
来源：http://sk.asd995.cn

================================================================================
来源：http://po.huanxung.cn

[E01] 拼接字符串
来源：http://mg.colortex.cn


<!-- 参考信息 -->