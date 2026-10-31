代发 wailian999

[C10] 变量作用域
来源：http://cd.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://se.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vu.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rx.szsharing.cn

TS:   同 JS
来源：http://hr.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://jh.hnjuh.cn

Go:   花括号块级作用域
来源：http://wc.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hx.jctech888.com.cn

C#:   块级作用域
来源：http://cf.9csxet.cn

[C11] 模块导入与导出
来源：http://lb.huixiangedu.cn

Py:   from module import func
来源：http://bl.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://du.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://et.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ah.shtwfgs.cn

Java: import java.util.List;
来源：http://ly.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uw.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://mi.bjjhwx.cn

C#:   using System.Text;
来源：http://zf.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://zt.521024.cn

Py:   (lambda: print("run"))()
来源：http://xj.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://xq.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://br.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://fc.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yy.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://hk.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://yj.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ij.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://tv.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gi.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ui.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tx.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://so.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lf.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://zw.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uf.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wu.jctech888.com.cn

[C14] 泛型函数
来源：http://fw.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yf.shtwfgs.cn

PHP:  // 无泛型
来源：http://mj.yuntaijiaju.cn

JS:   // 无泛型
来源：http://dc.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ka.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ni.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dg.szsharing.cn

Ruby: # 无泛型
来源：http://br.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yc.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://oi.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://im.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://uj.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gt.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ou.huanxung.cn

Java: // 无解构
来源：http://pc.jianghongdianzi.cn

Go:   // 无解构
来源：http://xr.hnjuh.cn

Ruby: a, b = pair
来源：http://hb.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://aq.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://pz.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yi.jianghongdianzi.cn

PHP:  // 无重载
来源：http://hr.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zq.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://gq.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rm.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://mv.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://zd.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sh.521024.cn

================================================================================
来源：http://gh.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://bc.shtwfgs.cn

================================================================================
来源：http://if.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://ld.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pa.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sw.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zo.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://au.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://af.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://sv.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://it.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tb.shxzskj.cn

[D02] 追加元素到末尾
来源：http://qx.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ql.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kf.muxihuayi.cn

JS:   arr.push(4);
来源：http://ja.panjiajie.cn

TS:   arr.push(4);
来源：http://fj.nicolike.cn

Java: list.add(4);
来源：http://vr.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://hy.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://nt.yuexingan06.cn

C#:   list.Add(4);
来源：http://pw.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://ea.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://xb.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yt.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kl.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://bg.chemitech.net.cn

Java: list.add(0, 0);
来源：http://jz.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://of.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rx.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://ib.shtwfgs.cn

[D04] 删除元素
来源：http://nx.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pf.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jy.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sj.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://wd.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://av.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qo.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bj.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ea.nicolike.cn

[D05] 访问与修改元素
来源：http://xi.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://so.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://at.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rh.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://rj.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://lt.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://rr.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xy.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ht.gzmigu.cn

[D06] 数组长度
来源：http://eb.yuexingan06.cn

Py:   len(arr)
来源：http://tk.huanxung.cn

PHP:  count($arr);
来源：http://pg.yuexingan06.cn

JS:   arr.length
来源：http://mb.chemitech.net.cn

TS:   arr.length
来源：http://td.shxzskj.cn

Java: list.size();
来源：http://bb.hnjuh.cn

Go:   len(arr)
来源：http://fz.hahajie.cn

Ruby: arr.length; arr.size
来源：http://ao.asd995.cn

C#:   list.Count;
来源：http://kb.521024.cn

[D07] 切片 / 取子数组
来源：http://hn.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oo.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gz.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://zp.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://wk.gzmigu.cn

Java: list.subList(1, 4);
来源：http://zo.shtwfgs.cn

Go:   arr[1:4]
来源：http://kk.nicolike.cn

Ruby: arr[1, 3]
来源：http://vu.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://rq.asd995.cn

[D08] 合并两个数组
来源：http://rd.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://ol.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://rq.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zk.asd995.cn

TS:   [...a, ...b];
来源：http://ec.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xl.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://pj.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://th.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://ob.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://av.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://hn.huixiangedu.cn

PHP:  sort($arr);
来源：http://uk.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ap.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lo.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zy.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bb.huanxung.cn

Ruby: arr.sort
来源：http://sq.shxzskj.cn

C#:   list.Sort();
来源：http://gc.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pr.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dy.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vv.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kg.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pi.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nd.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bf.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yl.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yl.jianghongdianzi.cn

[D11] 反转数组
来源：http://rt.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jn.521024.cn

PHP:  array_reverse($arr);
来源：http://md.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cl.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://ux.asd995.cn

Java: Collections.reverse(list);
来源：http://nn.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://me.521024.cn

Ruby: arr.reverse
来源：http://ak.hnjuh.cn

C#:   list.Reverse();
来源：http://dz.wgjwhj.cn

[D12] 查找元素下标
来源：http://kx.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://qy.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pb.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://va.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eg.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nu.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://ge.nszjky.cn

Ruby: arr.index(x)
来源：http://ra.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://xi.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://bp.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sp.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iu.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://bb.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://qa.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hy.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cl.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uq.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jc.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://qe.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sl.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dz.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://fq.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://wi.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wi.muxihuayi.cn

Go:   // 手写循环
来源：http://ki.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tq.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://db.colortex.cn

[D15] 去重
来源：http://zp.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zq.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://ey.huanxung.cn

JS:   [...new Set(arr)]
来源：http://qr.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://ky.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://od.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qm.shtwfgs.cn

Ruby: arr.uniq
来源：http://lx.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://ej.muxihuayi.cn

[D16] 求和与平均值
来源：http://mi.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hx.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oh.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://le.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eo.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fk.9csxet.cn

Go:   // 手写循环累加
来源：http://zw.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lu.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://qz.huanxung.cn

[D17] 最大值与最小值
来源：http://iv.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://yx.521024.cn

PHP:  max($arr);  min($arr);
来源：http://oi.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cc.521024.cn

TS:   Math.max(...arr);
来源：http://yx.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ew.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://br.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://tx.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://kr.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ff.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wd.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://xf.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eb.shxzukj.cn

TS:   nested.flat();
来源：http://oi.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tn.haigaiapp.cn

Go:   // 手写双层循环
来源：http://mr.huixiangedu.cn

Ruby: nested.flatten
来源：http://mc.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qy.shxzskj.cn

[D19] 按字段分组
来源：http://og.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pl.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://th.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://by.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://by.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ih.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://tk.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ca.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gx.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://vx.szxytkj.cn

Py:   Counter(arr)
来源：http://ko.szsharing.cn

PHP:  array_count_values($arr);
来源：http://ky.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fy.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uq.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ix.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://xq.shxzukj.cn

Ruby: arr.tally
来源：http://yf.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wu.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://ys.shxzukj.cn

Py:   x in arr
来源：http://yk.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://nh.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://iv.panjiajie.cn

TS:   arr.includes(x)
来源：http://zz.huixiangedu.cn

Java: list.contains(x)
来源：http://yb.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://rz.nszjky.cn

Ruby: arr.include?(x)
来源：http://wy.9csxet.cn

C#:   list.Contains(x)
来源：http://ni.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://je.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eh.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jc.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yj.lnxyls.cn

TS:   [...arr];
来源：http://pj.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://yk.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ul.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://vq.jctech888.com.cn

C#:   new List<int>(list);
来源：http://hd.lnxyls.cn

[D23] reduce 累积计算
来源：http://me.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oy.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://me.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bw.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ye.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ql.521024.cn

Go:   // 手写循环
来源：http://aa.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ge.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wo.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://wb.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kg.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ag.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tr.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ei.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cy.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pw.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fx.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ls.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://ae.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oz.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://np.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://er.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://no.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vg.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://am.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fj.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://as.bjjhwx.cn

[D26] 数组转字符串
来源：http://cu.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://un.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://kz.colortex.cn

JS:   arr.join(", ")
来源：http://va.shxzukj.cn

TS:   arr.join(", ")
来源：http://qk.huanxung.cn

Java: String.join(", ", list)
来源：http://ng.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://zz.nszjky.cn

Ruby: arr.join(", ")
来源：http://ik.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://uw.szsharing.cn


<!-- 参考信息 -->