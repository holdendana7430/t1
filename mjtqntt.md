代发 wailian999

TS:   同 JS
来源：http://hy.shxzukj.cn

Java: 方法内为块级作用域
来源：http://mu.huixiangedu.cn

Go:   花括号块级作用域
来源：http://fw.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ye.wgjwhj.cn

C#:   块级作用域
来源：http://yg.szxytkj.cn

[C11] 模块导入与导出
来源：http://qn.haigaiapp.cn

Py:   from module import func
来源：http://dr.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dy.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wz.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nf.jctech888.com.cn

Java: import java.util.List;
来源：http://pu.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oq.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://kj.nszjky.cn

C#:   using System.Text;
来源：http://od.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://jf.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://gd.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://by.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://fu.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://zx.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hk.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://cd.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://go.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ll.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://so.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qy.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mq.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gs.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ac.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sr.szsharing.cn

Go:   func add(a, b int) int
来源：http://mo.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ik.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://td.chemitech.net.cn

[C14] 泛型函数
来源：http://uj.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bc.hahajie.cn

PHP:  // 无泛型
来源：http://ex.colortex.cn

JS:   // 无泛型
来源：http://sa.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://of.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cw.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tn.muxihuayi.cn

Ruby: # 无泛型
来源：http://jr.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gn.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://ae.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xb.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://cw.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fs.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ok.asd995.cn

Java: // 无解构
来源：http://ky.szsharing.cn

Go:   // 无解构
来源：http://gt.newstarts.cn

Ruby: a, b = pair
来源：http://gm.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://km.521024.cn

[C16] 函数 / 方法重载
来源：http://jx.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rg.szxytkj.cn

PHP:  // 无重载
来源：http://pp.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lb.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://ue.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ax.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://ay.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://dl.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pd.lnxyls.cn

================================================================================
来源：http://ib.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://ut.jctech888.com.cn

================================================================================
来源：http://bc.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://kd.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kh.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xp.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cf.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jr.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xq.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://gy.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://ow.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ns.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://zj.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xt.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hl.nicolike.cn

JS:   arr.push(4);
来源：http://jp.nicolike.cn

TS:   arr.push(4);
来源：http://jk.szxytkj.cn

Java: list.add(4);
来源：http://wf.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://ep.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://mj.haigaiapp.cn

C#:   list.Add(4);
来源：http://rb.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://gs.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://wv.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sd.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dz.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://du.muxihuayi.cn

Java: list.add(0, 0);
来源：http://sn.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jm.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://an.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://te.wgjwhj.cn

[D04] 删除元素
来源：http://qr.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xe.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qr.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hu.asd995.cn

TS:   arr.splice(0, 1);
来源：http://zy.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rn.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://um.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vd.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lw.panjiajie.cn

[D05] 访问与修改元素
来源：http://lx.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ov.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qg.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uc.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://jr.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://vo.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://sh.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fq.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cl.yuexingan06.cn

[D06] 数组长度
来源：http://ct.newstarts.cn

Py:   len(arr)
来源：http://ix.hnjuh.cn

PHP:  count($arr);
来源：http://rp.hnjuh.cn

JS:   arr.length
来源：http://kn.yuexingan06.cn

TS:   arr.length
来源：http://ej.haigaiapp.cn

Java: list.size();
来源：http://an.asd995.cn

Go:   len(arr)
来源：http://xh.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://su.jctech888.com.cn

C#:   list.Count;
来源：http://tp.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://jt.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uw.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ct.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://sk.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://ay.9csxet.cn

Java: list.subList(1, 4);
来源：http://gr.muxihuayi.cn

Go:   arr[1:4]
来源：http://zv.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://vs.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://qq.muxihuayi.cn

[D08] 合并两个数组
来源：http://vq.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://nl.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://kf.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gq.huixiangedu.cn

TS:   [...a, ...b];
来源：http://hi.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mq.shxzskj.cn

Go:   append(a, b...)
来源：http://yu.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://rl.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://bo.hnjuh.cn

[D09] 排序（升序）
来源：http://bx.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://uq.wgjwhj.cn

PHP:  sort($arr);
来源：http://pa.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zc.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ln.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ow.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pp.bjjhwx.cn

Ruby: arr.sort
来源：http://kx.shxzukj.cn

C#:   list.Sort();
来源：http://xt.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tg.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ld.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eg.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pb.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hv.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zc.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uu.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lb.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hw.haigaiapp.cn

[D11] 反转数组
来源：http://mv.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ga.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://bh.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iu.hahajie.cn

TS:   [...arr].reverse();
来源：http://pf.newstarts.cn

Java: Collections.reverse(list);
来源：http://ci.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://dg.asd995.cn

Ruby: arr.reverse
来源：http://zv.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://wj.nszjky.cn

[D12] 查找元素下标
来源：http://px.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://vl.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ne.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ts.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uv.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jj.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://fy.panjiajie.cn

Ruby: arr.index(x)
来源：http://ty.nicolike.cn

C#:   list.IndexOf(x);
来源：http://dc.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://cl.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bf.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uc.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://oa.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://ye.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yb.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lp.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://du.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jp.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://zq.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lb.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vd.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://ui.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://zk.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cp.asd995.cn

Go:   // 手写循环
来源：http://wy.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://op.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rs.bjjhwx.cn

[D15] 去重
来源：http://kl.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xp.panjiajie.cn

PHP:  array_unique($arr);
来源：http://fi.nszjky.cn

JS:   [...new Set(arr)]
来源：http://xm.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://yg.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rt.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jm.colortex.cn

Ruby: arr.uniq
来源：http://jt.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://ng.wgjwhj.cn

[D16] 求和与平均值
来源：http://tp.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rz.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lt.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mo.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wc.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mp.szsharing.cn

Go:   // 手写循环累加
来源：http://mv.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ui.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://iw.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://ql.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://ag.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ss.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ct.nszjky.cn

TS:   Math.max(...arr);
来源：http://fh.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ve.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cz.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://nt.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://hs.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://ml.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hv.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://ty.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wc.bjjhwx.cn

TS:   nested.flat();
来源：http://wa.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fv.shxzskj.cn

Go:   // 手写双层循环
来源：http://nn.bookmarksfly.cn

Ruby: nested.flatten
来源：http://re.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hy.nszjky.cn

[D19] 按字段分组
来源：http://lr.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://da.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kd.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xz.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xq.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wd.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://fo.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sb.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yg.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://lu.shxzukj.cn

Py:   Counter(arr)
来源：http://uq.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://ra.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iv.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gf.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bj.hahajie.cn

Go:   // 手写 map[T]int
来源：http://rn.huixiangedu.cn

Ruby: arr.tally
来源：http://np.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ws.szsharing.cn

[D21] 判断是否包含某元素
来源：http://ad.huixiangedu.cn

Py:   x in arr
来源：http://xt.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://oa.chemitech.net.cn

JS:   arr.includes(x)
来源：http://ja.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://fo.chemitech.net.cn

Java: list.contains(x)
来源：http://oz.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://zo.hahajie.cn

Ruby: arr.include?(x)
来源：http://ek.szxytkj.cn

C#:   list.Contains(x)
来源：http://qw.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://uv.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yx.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bu.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://px.yuntaijiaju.cn

TS:   [...arr];
来源：http://du.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://hr.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cb.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://mp.huixiangedu.cn

C#:   new List<int>(list);
来源：http://vw.chemitech.net.cn

[D23] reduce 累积计算
来源：http://mt.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jp.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://es.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cj.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uv.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ku.muxihuayi.cn

Go:   // 手写循环
来源：http://tw.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wk.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hg.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://bq.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pb.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gx.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wl.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://js.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ex.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xl.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zw.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xb.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://ge.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ed.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ie.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nz.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iu.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bk.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oi.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tq.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nt.haigaiapp.cn

[D26] 数组转字符串
来源：http://gr.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://ce.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://zg.wgjwhj.cn

JS:   arr.join(", ")
来源：http://mn.yuexingan06.cn

TS:   arr.join(", ")
来源：http://ax.nicolike.cn

Java: String.join(", ", list)
来源：http://nr.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://cb.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://rh.nszjky.cn

C#:   string.Join(", ", list)
来源：http://uc.9csxet.cn

================================================================================
来源：http://zf.yuexingan06.cn

E. 字符串处理
来源：http://du.521024.cn

================================================================================
来源：http://um.szxytkj.cn

[E01] 拼接字符串
来源：http://wm.bjjhwx.cn


<!-- 参考信息 -->