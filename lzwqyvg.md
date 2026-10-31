代发 wailian999

C#:   块级作用域
来源：http://yh.lnxyls.cn

[C11] 模块导入与导出
来源：http://kl.chemitech.net.cn

Py:   from module import func
来源：http://zi.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rh.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wp.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kj.bjjhwx.cn

Java: import java.util.List;
来源：http://wh.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sv.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://it.haigaiapp.cn

C#:   using System.Text;
来源：http://ve.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://hd.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://vd.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://nm.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://xi.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://xa.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lw.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://bl.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://dd.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ec.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://dl.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qy.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://us.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vr.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://os.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vv.colortex.cn

Go:   func add(a, b int) int
来源：http://wg.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ez.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wu.panjiajie.cn

[C14] 泛型函数
来源：http://hb.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jh.muxihuayi.cn

PHP:  // 无泛型
来源：http://qc.bjjhwx.cn

JS:   // 无泛型
来源：http://pm.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fn.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zk.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ru.bookmarksfly.cn

Ruby: # 无泛型
来源：http://fb.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rw.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://zg.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ti.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://jx.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ar.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bj.haigaiapp.cn

Java: // 无解构
来源：http://yc.521024.cn

Go:   // 无解构
来源：http://pn.lnxyls.cn

Ruby: a, b = pair
来源：http://hb.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://mo.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://pi.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wr.huixiangedu.cn

PHP:  // 无重载
来源：http://gd.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ev.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://xh.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qh.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://rh.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://mi.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://im.shtwfgs.cn

================================================================================
来源：http://rl.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://dt.muxihuayi.cn

================================================================================
来源：http://yd.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://ms.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sx.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jd.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://di.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ba.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ne.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://ea.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://vw.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://un.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://dp.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bl.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jb.huixiangedu.cn

JS:   arr.push(4);
来源：http://nq.gzmigu.cn

TS:   arr.push(4);
来源：http://mw.huixiangedu.cn

Java: list.add(4);
来源：http://is.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://jl.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://wd.muxihuayi.cn

C#:   list.Add(4);
来源：http://rh.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://pf.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://wo.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ub.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dw.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://ja.newstarts.cn

Java: list.add(0, 0);
来源：http://gk.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vg.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bi.colortex.cn

C#:   list.Insert(0, 0);
来源：http://ha.521024.cn

[D04] 删除元素
来源：http://yx.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ro.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vk.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mg.asd995.cn

TS:   arr.splice(0, 1);
来源：http://eo.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qi.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pv.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qm.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kx.panjiajie.cn

[D05] 访问与修改元素
来源：http://ns.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zw.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rd.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zk.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://mp.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://kg.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://vn.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ur.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zm.lnxyls.cn

[D06] 数组长度
来源：http://nl.jctech888.com.cn

Py:   len(arr)
来源：http://eh.jctech888.com.cn

PHP:  count($arr);
来源：http://zw.panjiajie.cn

JS:   arr.length
来源：http://hk.nszjky.cn

TS:   arr.length
来源：http://nc.shxzskj.cn

Java: list.size();
来源：http://gb.nicolike.cn

Go:   len(arr)
来源：http://rj.huanxung.cn

Ruby: arr.length; arr.size
来源：http://gw.hahajie.cn

C#:   list.Count;
来源：http://hk.asd995.cn

[D07] 切片 / 取子数组
来源：http://pn.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uq.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wl.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://iw.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://dl.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://ge.szsharing.cn

Go:   arr[1:4]
来源：http://rp.shxzukj.cn

Ruby: arr[1, 3]
来源：http://pr.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://ru.huixiangedu.cn

[D08] 合并两个数组
来源：http://pj.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://nr.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://ky.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ni.bjjhwx.cn

TS:   [...a, ...b];
来源：http://ce.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dc.wgjwhj.cn

Go:   append(a, b...)
来源：http://dg.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://nh.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://ge.nicolike.cn

[D09] 排序（升序）
来源：http://rw.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://br.szxytkj.cn

PHP:  sort($arr);
来源：http://jg.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kj.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sb.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xi.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://da.szsharing.cn

Ruby: arr.sort
来源：http://zk.shtwfgs.cn

C#:   list.Sort();
来源：http://ay.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nh.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jg.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tl.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mx.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://to.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qx.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dj.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yf.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lv.newstarts.cn

[D11] 反转数组
来源：http://xl.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nh.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://wj.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pz.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://zl.nicolike.cn

Java: Collections.reverse(list);
来源：http://up.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://bo.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://eb.szsharing.cn

C#:   list.Reverse();
来源：http://xs.hahajie.cn

[D12] 查找元素下标
来源：http://bs.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://zr.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vi.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://it.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yg.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cw.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://kt.hnjuh.cn

Ruby: arr.index(x)
来源：http://sb.asd995.cn

C#:   list.IndexOf(x);
来源：http://jh.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://nm.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lk.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cv.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://bp.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://wx.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://my.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://on.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ry.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://as.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://zm.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dc.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zb.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://zl.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://bz.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://np.huixinmuqiang.cn

Go:   // 手写循环
来源：http://xh.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ms.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tq.colortex.cn

[D15] 去重
来源：http://ru.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://md.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://ow.nszjky.cn

JS:   [...new Set(arr)]
来源：http://za.nicolike.cn

TS:   [...new Set(arr)]
来源：http://ti.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xx.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zt.hnjuh.cn

Ruby: arr.uniq
来源：http://ky.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://bt.huanxung.cn

[D16] 求和与平均值
来源：http://vm.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kp.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vj.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cg.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tg.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zp.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://wu.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hv.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://fk.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://ij.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://ee.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://bp.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zw.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://pu.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ps.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vf.521024.cn

Ruby: arr.max;  arr.min
来源：http://qg.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://ir.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://mh.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bg.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://bo.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jk.nszjky.cn

TS:   nested.flat();
来源：http://mh.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dr.bjjhwx.cn

Go:   // 手写双层循环
来源：http://zr.shxzukj.cn

Ruby: nested.flatten
来源：http://oq.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hk.shtwfgs.cn

[D19] 按字段分组
来源：http://vu.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bp.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lp.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qp.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yy.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qr.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://ob.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ci.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kb.asd995.cn

[D20] 统计每个元素出现次数
来源：http://ap.huanxung.cn

Py:   Counter(arr)
来源：http://qm.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://tw.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rw.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nb.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lq.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://yl.bjjhwx.cn

Ruby: arr.tally
来源：http://wu.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mw.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://ia.panjiajie.cn

Py:   x in arr
来源：http://vt.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://kk.hnjuh.cn

JS:   arr.includes(x)
来源：http://jg.9csxet.cn

TS:   arr.includes(x)
来源：http://we.yuexingan06.cn

Java: list.contains(x)
来源：http://hn.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://kw.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://wm.gzmigu.cn

C#:   list.Contains(x)
来源：http://vy.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://rc.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fp.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dl.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ol.jctech888.com.cn

TS:   [...arr];
来源：http://zu.szsharing.cn

Java: new ArrayList<>(list);
来源：http://nw.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uy.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://rs.colortex.cn

C#:   new List<int>(list);
来源：http://un.jctech888.com.cn

[D23] reduce 累积计算
来源：http://os.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yr.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lw.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iw.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gy.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dk.yuntaijiaju.cn

Go:   // 手写循环
来源：http://bb.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ve.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mf.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://mm.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zo.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://in.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wk.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zb.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hg.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ye.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lc.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dh.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://cu.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sn.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pw.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gq.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ml.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ot.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gm.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sp.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tu.szxytkj.cn

[D26] 数组转字符串
来源：http://fa.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://wj.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://ux.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://el.newstarts.cn

TS:   arr.join(", ")
来源：http://wt.gzmigu.cn

Java: String.join(", ", list)
来源：http://cg.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://es.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://oi.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://ch.bookmarksfly.cn

================================================================================
来源：http://wc.jctech888.com.cn

E. 字符串处理
来源：http://tq.521024.cn

================================================================================
来源：http://bz.gzmigu.cn

[E01] 拼接字符串
来源：http://uo.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ls.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mo.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yg.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ye.newstarts.cn


<!-- 参考信息 -->