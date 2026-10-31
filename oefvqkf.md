代发 wailian999

TS:   同 JS
来源：http://nr.hahajie.cn

Java: 方法内为块级作用域
来源：http://kn.9csxet.cn

Go:   花括号块级作用域
来源：http://vi.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rd.panjiajie.cn

C#:   块级作用域
来源：http://ow.gzmigu.cn

[C11] 模块导入与导出
来源：http://ru.huanxung.cn

Py:   from module import func
来源：http://kn.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cn.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tz.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zd.yuntaijiaju.cn

Java: import java.util.List;
来源：http://rv.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bh.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://zw.muxihuayi.cn

C#:   using System.Text;
来源：http://dt.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://nw.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://cg.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://nf.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://ws.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://nc.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ft.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://tr.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://dl.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fn.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://mo.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kk.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ia.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ul.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://as.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kk.lnxyls.cn

Go:   func add(a, b int) int
来源：http://vz.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://va.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oa.shtwfgs.cn

[C14] 泛型函数
来源：http://us.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sh.newstarts.cn

PHP:  // 无泛型
来源：http://wy.panjiajie.cn

JS:   // 无泛型
来源：http://oq.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nv.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ig.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bh.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://kf.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oz.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://ab.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fx.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://ej.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ye.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uc.nszjky.cn

Java: // 无解构
来源：http://tj.bookmarksfly.cn

Go:   // 无解构
来源：http://qb.521024.cn

Ruby: a, b = pair
来源：http://wj.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://ge.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://dx.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gy.jianghongdianzi.cn

PHP:  // 无重载
来源：http://ot.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://im.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://qa.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kp.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://ha.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://yl.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tr.panjiajie.cn

================================================================================
来源：http://hw.colortex.cn

D. 数组 / 列表 / 集合
来源：http://hq.chemitech.net.cn

================================================================================
来源：http://or.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://zg.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ui.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dm.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zj.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nv.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kz.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://xv.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://lq.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ps.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://um.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pq.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xv.szsharing.cn

JS:   arr.push(4);
来源：http://wh.huanxung.cn

TS:   arr.push(4);
来源：http://zf.colortex.cn

Java: list.add(4);
来源：http://ye.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://qo.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://nt.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://cg.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://zx.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://jc.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pm.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cj.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://jf.hahajie.cn

Java: list.add(0, 0);
来源：http://vl.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fp.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vy.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://uz.huanxung.cn

[D04] 删除元素
来源：http://kg.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ny.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gp.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://do.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://yd.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zf.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dz.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://es.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dj.chemitech.net.cn

[D05] 访问与修改元素
来源：http://mn.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dy.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vc.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vw.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://qq.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://pb.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://on.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jt.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lw.huixinmuqiang.cn

[D06] 数组长度
来源：http://br.jianghongdianzi.cn

Py:   len(arr)
来源：http://eu.huixiangedu.cn

PHP:  count($arr);
来源：http://yc.szxytkj.cn

JS:   arr.length
来源：http://re.nszjky.cn

TS:   arr.length
来源：http://vp.gzmigu.cn

Java: list.size();
来源：http://oq.shxzukj.cn

Go:   len(arr)
来源：http://sp.nicolike.cn

Ruby: arr.length; arr.size
来源：http://gf.shtwfgs.cn

C#:   list.Count;
来源：http://oh.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://cy.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jm.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://de.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://db.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://me.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://xd.9csxet.cn

Go:   arr[1:4]
来源：http://fd.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://yq.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://zq.gzmigu.cn

[D08] 合并两个数组
来源：http://ln.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://pa.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://lh.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ix.chemitech.net.cn

TS:   [...a, ...b];
来源：http://xm.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kq.9csxet.cn

Go:   append(a, b...)
来源：http://wu.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://rx.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://ly.gzmigu.cn

[D09] 排序（升序）
来源：http://da.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://mb.bjjhwx.cn

PHP:  sort($arr);
来源：http://eg.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://az.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ff.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ko.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ou.9csxet.cn

Ruby: arr.sort
来源：http://lk.shxzukj.cn

C#:   list.Sort();
来源：http://nq.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mv.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xk.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://du.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ew.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ue.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cy.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tg.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fb.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cf.jctech888.com.cn

[D11] 反转数组
来源：http://ow.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qd.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://ge.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://um.huanxung.cn

TS:   [...arr].reverse();
来源：http://zm.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://ur.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://if.shxzskj.cn

Ruby: arr.reverse
来源：http://ex.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://ic.jctech888.com.cn

[D12] 查找元素下标
来源：http://pu.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://xa.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zc.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hh.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pq.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sw.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://zb.huixiangedu.cn

Ruby: arr.index(x)
来源：http://lq.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://ao.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://yh.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wi.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xc.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://kp.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://oq.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ae.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sy.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eg.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ne.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://rh.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pd.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://my.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://cv.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://of.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ok.9csxet.cn

Go:   // 手写循环
来源：http://bd.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fd.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bc.shxzukj.cn

[D15] 去重
来源：http://ke.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ed.szxytkj.cn

PHP:  array_unique($arr);
来源：http://ac.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://nk.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://li.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dx.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rv.huanxung.cn

Ruby: arr.uniq
来源：http://rk.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://jn.bookmarksfly.cn

[D16] 求和与平均值
来源：http://dw.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oq.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lf.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qe.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://um.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cr.yuexingan06.cn

Go:   // 手写循环累加
来源：http://tr.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qh.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://mc.nszjky.cn

[D17] 最大值与最小值
来源：http://zr.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://af.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://qp.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bs.panjiajie.cn

TS:   Math.max(...arr);
来源：http://zv.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vh.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qp.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://ve.asd995.cn

C#:   list.Max();  list.Min()
来源：http://ip.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://zb.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bz.colortex.cn

PHP:  array_merge(...$nested);
来源：http://ab.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lm.shxzskj.cn

TS:   nested.flat();
来源：http://jj.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ef.shxzskj.cn

Go:   // 手写双层循环
来源：http://vv.szxytkj.cn

Ruby: nested.flatten
来源：http://ps.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ho.szxytkj.cn

[D19] 按字段分组
来源：http://nh.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sj.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fe.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xx.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ob.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sd.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://ip.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qu.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nj.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://ug.hahajie.cn

Py:   Counter(arr)
来源：http://we.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://gw.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ik.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ho.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fp.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://gn.hahajie.cn

Ruby: arr.tally
来源：http://jo.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hk.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://ik.gzmigu.cn

Py:   x in arr
来源：http://xl.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://wl.nicolike.cn

JS:   arr.includes(x)
来源：http://sx.szsharing.cn

TS:   arr.includes(x)
来源：http://wj.hnjuh.cn

Java: list.contains(x)
来源：http://bx.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://sy.colortex.cn

Ruby: arr.include?(x)
来源：http://po.huixiangedu.cn

C#:   list.Contains(x)
来源：http://lq.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://or.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bn.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yg.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cc.shtwfgs.cn

TS:   [...arr];
来源：http://kc.nszjky.cn

Java: new ArrayList<>(list);
来源：http://bf.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cw.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://vb.jctech888.com.cn

C#:   new List<int>(list);
来源：http://wv.shtwfgs.cn

[D23] reduce 累积计算
来源：http://mo.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://og.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xc.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vy.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oy.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qc.521024.cn

Go:   // 手写循环
来源：http://pe.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lx.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dd.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://jb.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vq.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sb.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gy.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mv.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gc.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ij.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fy.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tw.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://cv.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cw.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dd.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rw.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dc.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dx.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ok.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eb.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wu.gzmigu.cn

[D26] 数组转字符串
来源：http://cx.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://xz.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://cy.gzmigu.cn

JS:   arr.join(", ")
来源：http://zj.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://hd.nicolike.cn

Java: String.join(", ", list)
来源：http://un.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://wi.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://nf.asd995.cn

C#:   string.Join(", ", list)
来源：http://eb.huixinmuqiang.cn

================================================================================
来源：http://iq.521024.cn

E. 字符串处理
来源：http://wq.asd995.cn

================================================================================
来源：http://we.haigaiapp.cn

[E01] 拼接字符串
来源：http://yz.jctech888.com.cn


<!-- 参考信息 -->