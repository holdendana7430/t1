代发 wailian999

[C10] 变量作用域
来源：http://fi.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://de.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ee.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nb.huixinmuqiang.cn

TS:   同 JS
来源：http://lt.szsharing.cn

Java: 方法内为块级作用域
来源：http://td.gzmigu.cn

Go:   花括号块级作用域
来源：http://bn.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ad.bookmarksfly.cn

C#:   块级作用域
来源：http://ty.yuexingan06.cn

[C11] 模块导入与导出
来源：http://gj.nicolike.cn

Py:   from module import func
来源：http://nu.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uo.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gr.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://co.shxzskj.cn

Java: import java.util.List;
来源：http://ru.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dp.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://xz.jctech888.com.cn

C#:   using System.Text;
来源：http://jz.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://ju.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://py.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://xm.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://pc.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://gx.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qc.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://gm.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://qw.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ls.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://cb.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dz.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qt.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kb.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qh.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ug.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://en.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ic.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zp.muxihuayi.cn

[C14] 泛型函数
来源：http://yv.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://as.wgjwhj.cn

PHP:  // 无泛型
来源：http://us.panjiajie.cn

JS:   // 无泛型
来源：http://ii.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yp.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yv.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oa.chemitech.net.cn

Ruby: # 无泛型
来源：http://mx.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lz.asd995.cn

[C15] 解构 / 展开参数
来源：http://cj.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://om.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://xp.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gm.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tk.wgjwhj.cn

Java: // 无解构
来源：http://do.shtwfgs.cn

Go:   // 无解构
来源：http://lg.hahajie.cn

Ruby: a, b = pair
来源：http://zu.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://kf.521024.cn

[C16] 函数 / 方法重载
来源：http://km.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://up.shxzskj.cn

PHP:  // 无重载
来源：http://gq.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qr.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://ef.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zr.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://zs.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://qo.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fh.9csxet.cn

================================================================================
来源：http://ju.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://ru.yuexingan06.cn

================================================================================
来源：http://wr.521024.cn

[D01] 创建数组 / 列表
来源：http://af.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hi.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rb.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ps.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ar.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://il.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://pq.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://ea.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iu.szxytkj.cn

[D02] 追加元素到末尾
来源：http://ps.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ov.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://an.huixiangedu.cn

JS:   arr.push(4);
来源：http://ew.9csxet.cn

TS:   arr.push(4);
来源：http://cr.yuntaijiaju.cn

Java: list.add(4);
来源：http://te.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://nm.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://mm.lnxyls.cn

C#:   list.Add(4);
来源：http://iw.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://vq.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://mc.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lr.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sp.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://cl.shxzskj.cn

Java: list.add(0, 0);
来源：http://hr.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://us.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yx.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://nz.hnjuh.cn

[D04] 删除元素
来源：http://um.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rs.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ik.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fw.521024.cn

TS:   arr.splice(0, 1);
来源：http://oe.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://of.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aj.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://br.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://on.shtwfgs.cn

[D05] 访问与修改元素
来源：http://he.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://th.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ct.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eb.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://xv.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://uc.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://lt.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yc.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ey.shxzskj.cn

[D06] 数组长度
来源：http://uo.521024.cn

Py:   len(arr)
来源：http://dn.hnjuh.cn

PHP:  count($arr);
来源：http://yh.hnjuh.cn

JS:   arr.length
来源：http://bd.521024.cn

TS:   arr.length
来源：http://lh.9csxet.cn

Java: list.size();
来源：http://mx.yuntaijiaju.cn

Go:   len(arr)
来源：http://no.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://oa.shxzukj.cn

C#:   list.Count;
来源：http://jo.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://lw.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kr.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vx.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://oz.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://nj.szxytkj.cn

Java: list.subList(1, 4);
来源：http://ie.nicolike.cn

Go:   arr[1:4]
来源：http://ro.9csxet.cn

Ruby: arr[1, 3]
来源：http://kb.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://ya.asd995.cn

[D08] 合并两个数组
来源：http://ua.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://mr.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://mi.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://st.shtwfgs.cn

TS:   [...a, ...b];
来源：http://kb.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hs.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://nd.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://wm.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://pj.panjiajie.cn

[D09] 排序（升序）
来源：http://tt.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ow.521024.cn

PHP:  sort($arr);
来源：http://eo.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zx.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jk.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lk.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ko.hahajie.cn

Ruby: arr.sort
来源：http://oc.bookmarksfly.cn

C#:   list.Sort();
来源：http://ke.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mq.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://we.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nz.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iz.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aj.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://om.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gs.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sg.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pw.gzmigu.cn

[D11] 反转数组
来源：http://ep.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rl.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://zn.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ch.szsharing.cn

TS:   [...arr].reverse();
来源：http://pn.nszjky.cn

Java: Collections.reverse(list);
来源：http://br.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://oj.szxytkj.cn

Ruby: arr.reverse
来源：http://kj.nszjky.cn

C#:   list.Reverse();
来源：http://cp.wgjwhj.cn

[D12] 查找元素下标
来源：http://sa.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://ii.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vv.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ab.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wz.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bd.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://ug.huixiangedu.cn

Ruby: arr.index(x)
来源：http://lb.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://au.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ad.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rg.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ep.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://rb.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://vt.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iq.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://im.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uz.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://fc.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sw.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wl.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://tl.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://bw.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://et.huixinmuqiang.cn

Go:   // 手写循环
来源：http://lz.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gd.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xk.asd995.cn

[D15] 去重
来源：http://ep.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sm.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://zi.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://ce.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://gv.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bt.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jw.muxihuayi.cn

Ruby: arr.uniq
来源：http://iq.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://hv.bookmarksfly.cn

[D16] 求和与平均值
来源：http://fg.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pw.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ad.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lo.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wm.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ng.521024.cn

Go:   // 手写循环累加
来源：http://vp.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jt.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://cq.panjiajie.cn

[D17] 最大值与最小值
来源：http://vy.asd995.cn

Py:   max(arr);  min(arr)
来源：http://pd.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://ct.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ey.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://eo.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jn.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yn.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://ku.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://dg.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://ma.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sy.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://bs.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bu.shxzukj.cn

TS:   nested.flat();
来源：http://cz.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qy.colortex.cn

Go:   // 手写双层循环
来源：http://oa.nszjky.cn

Ruby: nested.flatten
来源：http://jd.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lo.huanxung.cn

[D19] 按字段分组
来源：http://ui.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ou.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mc.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://li.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yh.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mw.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://eh.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://et.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wl.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://qd.szxytkj.cn

Py:   Counter(arr)
来源：http://fy.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://gj.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rd.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ga.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mo.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://ge.panjiajie.cn

Ruby: arr.tally
来源：http://ss.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gw.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://xu.lnxyls.cn

Py:   x in arr
来源：http://tm.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://ee.wgjwhj.cn

JS:   arr.includes(x)
来源：http://xp.lnxyls.cn

TS:   arr.includes(x)
来源：http://sw.colortex.cn

Java: list.contains(x)
来源：http://bw.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://mc.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://vd.nszjky.cn

C#:   list.Contains(x)
来源：http://pr.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://xd.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gr.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://za.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ss.haigaiapp.cn

TS:   [...arr];
来源：http://bg.521024.cn

Java: new ArrayList<>(list);
来源：http://mr.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hy.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://lc.yuexingan06.cn

C#:   new List<int>(list);
来源：http://qn.shxzskj.cn

[D23] reduce 累积计算
来源：http://zp.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pv.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mo.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pg.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sy.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fx.lnxyls.cn

Go:   // 手写循环
来源：http://ee.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iy.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kk.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://hz.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ee.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rt.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uq.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sb.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jn.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sj.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qz.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dr.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://ok.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nq.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hk.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gi.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ly.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ut.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ww.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wy.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://my.szxytkj.cn

[D26] 数组转字符串
来源：http://fw.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://yj.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://xc.gzmigu.cn

JS:   arr.join(", ")
来源：http://fc.shxzukj.cn

TS:   arr.join(", ")
来源：http://av.colortex.cn

Java: String.join(", ", list)
来源：http://on.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://nj.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://ns.newstarts.cn

C#:   string.Join(", ", list)
来源：http://zo.bookmarksfly.cn


<!-- 参考信息 -->