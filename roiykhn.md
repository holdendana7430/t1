代发 wailian999

TS:   同 JS
来源：http://bx.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://gd.shtwfgs.cn

Go:   花括号块级作用域
来源：http://mg.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kw.shxzukj.cn

C#:   块级作用域
来源：http://ss.521024.cn

[C11] 模块导入与导出
来源：http://qg.szxytkj.cn

Py:   from module import func
来源：http://mf.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jh.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hx.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nj.hnjuh.cn

Java: import java.util.List;
来源：http://do.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fh.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://sb.shxzskj.cn

C#:   using System.Text;
来源：http://jf.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://kk.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://ar.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://jw.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://fx.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://ay.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rd.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://op.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://nh.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fd.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://os.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eg.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rf.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ex.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qp.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tj.szxytkj.cn

Go:   func add(a, b int) int
来源：http://jb.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yj.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cm.shxzukj.cn

[C14] 泛型函数
来源：http://qm.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ma.huanxung.cn

PHP:  // 无泛型
来源：http://uy.nszjky.cn

JS:   // 无泛型
来源：http://tl.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yh.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ab.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ke.szsharing.cn

Ruby: # 无泛型
来源：http://ev.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dn.nicolike.cn

[C15] 解构 / 展开参数
来源：http://fq.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kv.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://dq.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zn.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ev.szsharing.cn

Java: // 无解构
来源：http://qe.jianghongdianzi.cn

Go:   // 无解构
来源：http://ut.panjiajie.cn

Ruby: a, b = pair
来源：http://ng.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://za.nszjky.cn

[C16] 函数 / 方法重载
来源：http://yl.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://px.jianghongdianzi.cn

PHP:  // 无重载
来源：http://gn.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lx.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://aw.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yz.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://wd.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://fk.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ju.yuexingan06.cn

================================================================================
来源：http://nv.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://ca.jianghongdianzi.cn

================================================================================
来源：http://gy.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://wv.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ou.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ov.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ys.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://aj.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mi.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://mx.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://uz.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tt.szsharing.cn

[D02] 追加元素到末尾
来源：http://ox.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tt.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mt.shtwfgs.cn

JS:   arr.push(4);
来源：http://ks.bookmarksfly.cn

TS:   arr.push(4);
来源：http://zl.asd995.cn

Java: list.add(4);
来源：http://vz.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://du.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://qo.huixiangedu.cn

C#:   list.Add(4);
来源：http://fv.huanxung.cn

[D03] 在指定位置插入元素
来源：http://rt.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://ki.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sl.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jb.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://lg.shxzukj.cn

Java: list.add(0, 0);
来源：http://zc.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ck.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gw.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://zv.szxytkj.cn

[D04] 删除元素
来源：http://hj.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ct.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iz.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tu.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://he.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mb.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ve.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wf.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ef.lnxyls.cn

[D05] 访问与修改元素
来源：http://jt.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wc.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yw.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fz.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://nx.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://as.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://as.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yx.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ls.asd995.cn

[D06] 数组长度
来源：http://im.chemitech.net.cn

Py:   len(arr)
来源：http://ch.newstarts.cn

PHP:  count($arr);
来源：http://cd.haigaiapp.cn

JS:   arr.length
来源：http://jk.nszjky.cn

TS:   arr.length
来源：http://lk.huixiangedu.cn

Java: list.size();
来源：http://kk.nszjky.cn

Go:   len(arr)
来源：http://zx.nszjky.cn

Ruby: arr.length; arr.size
来源：http://oh.newstarts.cn

C#:   list.Count;
来源：http://do.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://vq.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dv.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nh.colortex.cn

JS:   arr.slice(1, 4);
来源：http://zm.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://xr.asd995.cn

Java: list.subList(1, 4);
来源：http://ko.nszjky.cn

Go:   arr[1:4]
来源：http://bz.9csxet.cn

Ruby: arr[1, 3]
来源：http://nx.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://tt.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://qq.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://pm.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://vf.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lf.asd995.cn

TS:   [...a, ...b];
来源：http://iw.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hh.nicolike.cn

Go:   append(a, b...)
来源：http://qz.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://mu.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://kb.bookmarksfly.cn

[D09] 排序（升序）
来源：http://ss.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://hm.nicolike.cn

PHP:  sort($arr);
来源：http://dg.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zg.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://op.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wz.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nm.bjjhwx.cn

Ruby: arr.sort
来源：http://qt.yuexingan06.cn

C#:   list.Sort();
来源：http://qk.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ee.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rq.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fe.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sl.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vs.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cb.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ss.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vs.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nx.shtwfgs.cn

[D11] 反转数组
来源：http://an.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ry.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://tv.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rv.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://jt.hnjuh.cn

Java: Collections.reverse(list);
来源：http://tl.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://uj.lnxyls.cn

Ruby: arr.reverse
来源：http://za.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://bh.colortex.cn

[D12] 查找元素下标
来源：http://is.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://wi.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zg.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kc.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pm.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vb.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://ij.chemitech.net.cn

Ruby: arr.index(x)
来源：http://km.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://kn.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://qw.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mt.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bh.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://np.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://ox.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jo.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yg.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ub.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ia.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://ql.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tk.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ij.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://rv.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://sr.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vm.nicolike.cn

Go:   // 手写循环
来源：http://az.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fw.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kf.jianghongdianzi.cn

[D15] 去重
来源：http://cr.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zx.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://mc.newstarts.cn

JS:   [...new Set(arr)]
来源：http://zf.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://mm.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mr.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vh.wgjwhj.cn

Ruby: arr.uniq
来源：http://yi.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://bq.nicolike.cn

[D16] 求和与平均值
来源：http://st.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ts.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tw.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sw.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oi.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ga.hahajie.cn

Go:   // 手写循环累加
来源：http://vl.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fx.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://ci.hnjuh.cn

[D17] 最大值与最小值
来源：http://xz.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://zn.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://ni.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fp.hnjuh.cn

TS:   Math.max(...arr);
来源：http://ct.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mf.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dm.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ri.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://gd.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://mz.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tw.asd995.cn

PHP:  array_merge(...$nested);
来源：http://wo.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yq.yuntaijiaju.cn

TS:   nested.flat();
来源：http://zy.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wx.asd995.cn

Go:   // 手写双层循环
来源：http://ue.haigaiapp.cn

Ruby: nested.flatten
来源：http://or.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hb.jctech888.com.cn

[D19] 按字段分组
来源：http://bx.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bh.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kl.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gu.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://az.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qh.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://rs.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zv.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jx.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://we.newstarts.cn

Py:   Counter(arr)
来源：http://xi.9csxet.cn

PHP:  array_count_values($arr);
来源：http://lz.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sa.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wf.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wy.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://ps.shxzukj.cn

Ruby: arr.tally
来源：http://ls.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dw.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://iq.huixiangedu.cn

Py:   x in arr
来源：http://yb.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://ff.haigaiapp.cn

JS:   arr.includes(x)
来源：http://jv.colortex.cn

TS:   arr.includes(x)
来源：http://qj.shxzukj.cn

Java: list.contains(x)
来源：http://ys.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://mj.nicolike.cn

Ruby: arr.include?(x)
来源：http://wc.shtwfgs.cn

C#:   list.Contains(x)
来源：http://mn.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://ay.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dy.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://az.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nx.nicolike.cn

TS:   [...arr];
来源：http://gz.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://lh.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vr.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://xq.haigaiapp.cn

C#:   new List<int>(list);
来源：http://wl.nszjky.cn

[D23] reduce 累积计算
来源：http://ap.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pa.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ha.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ab.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lv.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tq.jctech888.com.cn

Go:   // 手写循环
来源：http://zm.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bf.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pv.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://hh.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://br.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cn.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gy.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xl.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uu.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mu.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gp.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bu.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://ko.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://od.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qu.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ec.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xn.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yk.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sj.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pt.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jo.muxihuayi.cn

[D26] 数组转字符串
来源：http://ja.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://cp.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://xi.chemitech.net.cn

JS:   arr.join(", ")
来源：http://ma.chemitech.net.cn

TS:   arr.join(", ")
来源：http://la.hnjuh.cn

Java: String.join(", ", list)
来源：http://sp.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://qw.hnjuh.cn

Ruby: arr.join(", ")
来源：http://mq.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://qh.shxzukj.cn

================================================================================
来源：http://xm.nszjky.cn

E. 字符串处理
来源：http://qo.szxytkj.cn

================================================================================
来源：http://wf.hahajie.cn

[E01] 拼接字符串
来源：http://qi.521024.cn


<!-- 参考信息 -->