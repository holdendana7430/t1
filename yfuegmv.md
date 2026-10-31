代发 wailian999

C#:   块级作用域
来源：http://fr.szxytkj.cn

[C11] 模块导入与导出
来源：http://la.asd995.cn

Py:   from module import func
来源：http://da.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cv.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nw.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ur.yuntaijiaju.cn

Java: import java.util.List;
来源：http://of.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tt.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://hd.huixinmuqiang.cn

C#:   using System.Text;
来源：http://um.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://sb.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://fm.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://zq.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://le.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://iq.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xf.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://oa.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://ds.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pj.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://je.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iv.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wo.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cb.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wc.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wy.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://uw.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qb.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ku.jianghongdianzi.cn

[C14] 泛型函数
来源：http://ys.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qj.shxzukj.cn

PHP:  // 无泛型
来源：http://zc.huanxung.cn

JS:   // 无泛型
来源：http://tp.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eg.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tm.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wp.huixiangedu.cn

Ruby: # 无泛型
来源：http://cd.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ts.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://zq.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hk.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://tp.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jg.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uc.szxytkj.cn

Java: // 无解构
来源：http://hb.wgjwhj.cn

Go:   // 无解构
来源：http://bb.bookmarksfly.cn

Ruby: a, b = pair
来源：http://nn.nicolike.cn

C#:   var (a, b) = pair;
来源：http://lw.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://gn.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://de.chemitech.net.cn

PHP:  // 无重载
来源：http://dx.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ls.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://tl.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://us.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://ge.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://yx.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dd.9csxet.cn

================================================================================
来源：http://ud.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://wg.lnxyls.cn

================================================================================
来源：http://le.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://ln.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://at.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mx.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ys.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gs.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dt.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://vk.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://ie.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jj.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://wr.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zm.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wt.panjiajie.cn

JS:   arr.push(4);
来源：http://dd.muxihuayi.cn

TS:   arr.push(4);
来源：http://ly.jctech888.com.cn

Java: list.add(4);
来源：http://ry.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://lr.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://sj.lnxyls.cn

C#:   list.Add(4);
来源：http://dc.hahajie.cn

[D03] 在指定位置插入元素
来源：http://pb.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://re.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xq.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vy.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://hw.jctech888.com.cn

Java: list.add(0, 0);
来源：http://ql.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yx.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rz.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://vq.hahajie.cn

[D04] 删除元素
来源：http://hl.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jm.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hl.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pp.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://wa.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cs.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://us.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nl.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://da.asd995.cn

[D05] 访问与修改元素
来源：http://de.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ru.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qs.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eg.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://lo.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ta.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://il.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gx.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vt.chemitech.net.cn

[D06] 数组长度
来源：http://sj.bookmarksfly.cn

Py:   len(arr)
来源：http://jl.521024.cn

PHP:  count($arr);
来源：http://ev.colortex.cn

JS:   arr.length
来源：http://dg.9csxet.cn

TS:   arr.length
来源：http://he.szxytkj.cn

Java: list.size();
来源：http://tc.szsharing.cn

Go:   len(arr)
来源：http://gu.9csxet.cn

Ruby: arr.length; arr.size
来源：http://iz.shxzskj.cn

C#:   list.Count;
来源：http://xi.newstarts.cn

[D07] 切片 / 取子数组
来源：http://pa.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pk.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pg.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://pa.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://od.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://lk.asd995.cn

Go:   arr[1:4]
来源：http://sl.9csxet.cn

Ruby: arr[1, 3]
来源：http://hg.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://cl.muxihuayi.cn

[D08] 合并两个数组
来源：http://qw.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://mi.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://vf.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lm.hnjuh.cn

TS:   [...a, ...b];
来源：http://km.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rh.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://hz.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://fe.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://rd.9csxet.cn

[D09] 排序（升序）
来源：http://jk.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://lf.yuexingan06.cn

PHP:  sort($arr);
来源：http://ma.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yf.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://di.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jm.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://me.nszjky.cn

Ruby: arr.sort
来源：http://fb.huanxung.cn

C#:   list.Sort();
来源：http://wu.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nz.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eb.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nq.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fi.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lr.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wu.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wl.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tp.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gw.szsharing.cn

[D11] 反转数组
来源：http://kz.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xq.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://ok.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hq.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://kw.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://np.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://hv.bookmarksfly.cn

Ruby: arr.reverse
来源：http://cj.szsharing.cn

C#:   list.Reverse();
来源：http://dp.huixiangedu.cn

[D12] 查找元素下标
来源：http://gm.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://tc.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://de.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oq.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xp.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://th.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://hv.muxihuayi.cn

Ruby: arr.index(x)
来源：http://jk.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://kg.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://zi.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vi.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hx.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://rf.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://bk.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zz.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://im.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hi.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qi.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://xd.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gf.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eo.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://ma.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://dr.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yp.bookmarksfly.cn

Go:   // 手写循环
来源：http://yq.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://it.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zd.hahajie.cn

[D15] 去重
来源：http://ry.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xa.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://ou.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://kc.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://yf.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xh.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yd.newstarts.cn

Ruby: arr.uniq
来源：http://nm.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://av.gzmigu.cn

[D16] 求和与平均值
来源：http://cw.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uf.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nd.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uu.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xr.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ol.newstarts.cn

Go:   // 手写循环累加
来源：http://wh.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mg.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://gw.shxzskj.cn

[D17] 最大值与最小值
来源：http://gd.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://kg.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://vp.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cw.huanxung.cn

TS:   Math.max(...arr);
来源：http://pz.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kt.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sj.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://yx.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://kz.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://pl.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wt.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://kx.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ma.newstarts.cn

TS:   nested.flat();
来源：http://jo.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sf.gzmigu.cn

Go:   // 手写双层循环
来源：http://eo.asd995.cn

Ruby: nested.flatten
来源：http://sn.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://af.colortex.cn

[D19] 按字段分组
来源：http://qm.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wo.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fj.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mz.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ur.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tg.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://ec.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mi.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gv.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://uo.szxytkj.cn

Py:   Counter(arr)
来源：http://nt.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://xj.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zc.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://og.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jo.hahajie.cn

Go:   // 手写 map[T]int
来源：http://mh.asd995.cn

Ruby: arr.tally
来源：http://gv.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gd.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://xv.colortex.cn

Py:   x in arr
来源：http://uv.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://ga.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://he.yuexingan06.cn

TS:   arr.includes(x)
来源：http://hq.yuntaijiaju.cn

Java: list.contains(x)
来源：http://uq.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://ky.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://tg.jctech888.com.cn

C#:   list.Contains(x)
来源：http://gw.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://sg.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://in.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://co.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://il.szxytkj.cn

TS:   [...arr];
来源：http://ga.asd995.cn

Java: new ArrayList<>(list);
来源：http://hj.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wl.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://rc.lnxyls.cn

C#:   new List<int>(list);
来源：http://gc.shtwfgs.cn

[D23] reduce 累积计算
来源：http://dy.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rh.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cl.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zv.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ry.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gi.shxzskj.cn

Go:   // 手写循环
来源：http://hj.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://el.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cm.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://dz.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mj.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rk.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pe.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rr.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wr.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kb.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ab.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://an.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://bh.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eq.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zo.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nf.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jb.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ap.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ra.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://in.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xz.lnxyls.cn

[D26] 数组转字符串
来源：http://ex.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://hr.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://pu.9csxet.cn

JS:   arr.join(", ")
来源：http://qp.colortex.cn

TS:   arr.join(", ")
来源：http://ac.chemitech.net.cn

Java: String.join(", ", list)
来源：http://ty.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://ku.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://dz.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://yu.bookmarksfly.cn

================================================================================
来源：http://tj.huixiangedu.cn

E. 字符串处理
来源：http://ss.colortex.cn

================================================================================
来源：http://os.panjiajie.cn

[E01] 拼接字符串
来源：http://zj.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qm.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zf.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eu.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gf.bookmarksfly.cn


<!-- 参考信息 -->