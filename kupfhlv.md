代发 wailian999

TS:   同 JS
来源：http://up.panjiajie.cn

Java: 方法内为块级作用域
来源：http://nt.chemitech.net.cn

Go:   花括号块级作用域
来源：http://xf.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eu.bookmarksfly.cn

C#:   块级作用域
来源：http://uy.lnxyls.cn

[C11] 模块导入与导出
来源：http://go.yuntaijiaju.cn

Py:   from module import func
来源：http://ta.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://di.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mu.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://by.asd995.cn

Java: import java.util.List;
来源：http://lb.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sn.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ox.shtwfgs.cn

C#:   using System.Text;
来源：http://nk.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://jl.521024.cn

Py:   (lambda: print("run"))()
来源：http://ew.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://bq.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://jp.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://wh.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yw.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://pd.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://du.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://as.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://ql.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://si.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ca.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jg.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bb.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mp.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://gb.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qg.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ey.wgjwhj.cn

[C14] 泛型函数
来源：http://kz.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wc.huixiangedu.cn

PHP:  // 无泛型
来源：http://qs.shxzukj.cn

JS:   // 无泛型
来源：http://bc.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zf.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eu.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ub.shxzukj.cn

Ruby: # 无泛型
来源：http://dc.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eg.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://xw.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://me.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://ai.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://av.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yc.colortex.cn

Java: // 无解构
来源：http://lz.bookmarksfly.cn

Go:   // 无解构
来源：http://hr.shxzukj.cn

Ruby: a, b = pair
来源：http://ne.hahajie.cn

C#:   var (a, b) = pair;
来源：http://jb.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ai.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gj.szsharing.cn

PHP:  // 无重载
来源：http://gy.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qa.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://xi.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pw.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://gx.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://ij.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://np.haigaiapp.cn

================================================================================
来源：http://vp.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://al.huixinmuqiang.cn

================================================================================
来源：http://ln.colortex.cn

[D01] 创建数组 / 列表
来源：http://qh.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://va.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lm.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zw.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wk.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vc.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://lz.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://kk.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gu.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://xo.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vq.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ev.nszjky.cn

JS:   arr.push(4);
来源：http://he.muxihuayi.cn

TS:   arr.push(4);
来源：http://sk.nszjky.cn

Java: list.add(4);
来源：http://ss.521024.cn

Go:   arr = append(arr, 4)
来源：http://vw.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://co.521024.cn

C#:   list.Add(4);
来源：http://wz.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://hj.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://fp.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uy.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oh.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://om.bjjhwx.cn

Java: list.add(0, 0);
来源：http://jw.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lu.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dp.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://ka.huanxung.cn

[D04] 删除元素
来源：http://cv.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gh.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sq.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ny.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://xh.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yl.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sw.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yj.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nd.muxihuayi.cn

[D05] 访问与修改元素
来源：http://bi.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rp.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bn.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rp.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://cu.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://pa.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://jp.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hm.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mi.nszjky.cn

[D06] 数组长度
来源：http://np.gzmigu.cn

Py:   len(arr)
来源：http://xo.szsharing.cn

PHP:  count($arr);
来源：http://de.asd995.cn

JS:   arr.length
来源：http://hw.huanxung.cn

TS:   arr.length
来源：http://mk.nicolike.cn

Java: list.size();
来源：http://hi.lnxyls.cn

Go:   len(arr)
来源：http://ux.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://zx.jianghongdianzi.cn

C#:   list.Count;
来源：http://bj.asd995.cn

[D07] 切片 / 取子数组
来源：http://vm.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://me.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fn.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://jk.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://sb.szsharing.cn

Java: list.subList(1, 4);
来源：http://mf.wgjwhj.cn

Go:   arr[1:4]
来源：http://it.hnjuh.cn

Ruby: arr[1, 3]
来源：http://so.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://yd.9csxet.cn

[D08] 合并两个数组
来源：http://eg.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://zx.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://xp.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ci.hahajie.cn

TS:   [...a, ...b];
来源：http://gr.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ze.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://ay.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://zm.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://hz.hnjuh.cn

[D09] 排序（升序）
来源：http://fm.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://ne.bookmarksfly.cn

PHP:  sort($arr);
来源：http://rg.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aq.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wd.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qs.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://da.chemitech.net.cn

Ruby: arr.sort
来源：http://bo.haigaiapp.cn

C#:   list.Sort();
来源：http://dn.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pi.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tq.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vo.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sn.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eo.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ah.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pv.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sz.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://po.szxytkj.cn

[D11] 反转数组
来源：http://qu.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bg.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://kv.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vm.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://hx.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://un.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://aj.bookmarksfly.cn

Ruby: arr.reverse
来源：http://dd.521024.cn

C#:   list.Reverse();
来源：http://xr.chemitech.net.cn

[D12] 查找元素下标
来源：http://by.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://vo.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zh.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kh.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://is.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sg.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://zo.gzmigu.cn

Ruby: arr.index(x)
来源：http://sx.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://bf.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://no.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xk.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oj.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://gn.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://hb.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jx.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bi.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iq.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bs.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://ym.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tw.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xo.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://ds.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://dg.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://va.nszjky.cn

Go:   // 手写循环
来源：http://qc.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nk.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://en.huanxung.cn

[D15] 去重
来源：http://ca.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dq.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://bo.asd995.cn

JS:   [...new Set(arr)]
来源：http://fv.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://qt.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kq.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nt.colortex.cn

Ruby: arr.uniq
来源：http://lk.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://ei.szsharing.cn

[D16] 求和与平均值
来源：http://va.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://en.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oq.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dz.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ez.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aj.chemitech.net.cn

Go:   // 手写循环累加
来源：http://cd.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fv.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://ta.szsharing.cn

[D17] 最大值与最小值
来源：http://tu.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://td.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://gw.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nm.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://be.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vw.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ks.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://zb.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://aw.colortex.cn

[D18] 扁平化嵌套数组
来源：http://lu.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nn.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://rw.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sz.yuntaijiaju.cn

TS:   nested.flat();
来源：http://av.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fc.muxihuayi.cn

Go:   // 手写双层循环
来源：http://hd.shxzskj.cn

Ruby: nested.flatten
来源：http://do.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wr.lnxyls.cn

[D19] 按字段分组
来源：http://cp.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hc.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vz.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hi.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bs.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qk.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://mv.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bt.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ie.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://mh.nicolike.cn

Py:   Counter(arr)
来源：http://xz.521024.cn

PHP:  array_count_values($arr);
来源：http://pj.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rr.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ek.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ys.szsharing.cn

Go:   // 手写 map[T]int
来源：http://ij.hnjuh.cn

Ruby: arr.tally
来源：http://dr.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zj.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://bf.yuntaijiaju.cn

Py:   x in arr
来源：http://fd.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://we.bjjhwx.cn

JS:   arr.includes(x)
来源：http://rv.szsharing.cn

TS:   arr.includes(x)
来源：http://ka.gzmigu.cn

Java: list.contains(x)
来源：http://mp.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://cj.szxytkj.cn

Ruby: arr.include?(x)
来源：http://sy.jctech888.com.cn

C#:   list.Contains(x)
来源：http://wa.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://yq.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qv.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bz.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bc.shxzskj.cn

TS:   [...arr];
来源：http://lt.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://zo.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vz.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://jd.szxytkj.cn

C#:   new List<int>(list);
来源：http://zo.haigaiapp.cn

[D23] reduce 累积计算
来源：http://se.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pn.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yk.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tp.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wb.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jq.szsharing.cn

Go:   // 手写循环
来源：http://rq.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ie.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kw.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://rw.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ak.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://re.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ku.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rd.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://og.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bd.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gz.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vt.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://jz.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yx.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lb.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aa.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bn.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nk.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yw.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xi.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hs.newstarts.cn

[D26] 数组转字符串
来源：http://uj.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://zn.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://nh.szxytkj.cn

JS:   arr.join(", ")
来源：http://ne.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://ev.yuexingan06.cn

Java: String.join(", ", list)
来源：http://qo.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://aj.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://zj.newstarts.cn

C#:   string.Join(", ", list)
来源：http://tv.nicolike.cn

================================================================================
来源：http://ea.hahajie.cn

E. 字符串处理
来源：http://ar.yuexingan06.cn

================================================================================
来源：http://fu.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://hh.lnxyls.cn


<!-- 参考信息 -->