代发 wailian999

C#:   块级作用域
来源：http://gg.bjjhwx.cn

[C11] 模块导入与导出
来源：http://mx.9csxet.cn

Py:   from module import func
来源：http://fe.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oy.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kx.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xa.bjjhwx.cn

Java: import java.util.List;
来源：http://wj.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fo.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://xk.huixiangedu.cn

C#:   using System.Text;
来源：http://nz.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://un.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://ql.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://qj.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://xq.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://od.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://at.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://na.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://fp.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xy.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://ln.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ma.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cv.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yl.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rs.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ju.lnxyls.cn

Go:   func add(a, b int) int
来源：http://nr.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://du.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mc.huixiangedu.cn

[C14] 泛型函数
来源：http://tb.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ay.nicolike.cn

PHP:  // 无泛型
来源：http://nt.jctech888.com.cn

JS:   // 无泛型
来源：http://hy.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://su.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iq.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tk.huanxung.cn

Ruby: # 无泛型
来源：http://ob.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cl.nszjky.cn

[C15] 解构 / 展开参数
来源：http://jz.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://px.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://bd.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nn.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hc.colortex.cn

Java: // 无解构
来源：http://ax.shxzskj.cn

Go:   // 无解构
来源：http://rb.gzmigu.cn

Ruby: a, b = pair
来源：http://hb.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://ur.521024.cn

[C16] 函数 / 方法重载
来源：http://np.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pm.yuexingan06.cn

PHP:  // 无重载
来源：http://je.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bg.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://cq.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fg.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://sj.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://fe.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jz.newstarts.cn

================================================================================
来源：http://en.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://zc.yuntaijiaju.cn

================================================================================
来源：http://fw.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://yw.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hm.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bl.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qr.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ma.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gf.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://qh.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://lq.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zk.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://xe.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gm.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ly.asd995.cn

JS:   arr.push(4);
来源：http://fz.muxihuayi.cn

TS:   arr.push(4);
来源：http://xv.muxihuayi.cn

Java: list.add(4);
来源：http://rn.521024.cn

Go:   arr = append(arr, 4)
来源：http://mb.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://ha.muxihuayi.cn

C#:   list.Add(4);
来源：http://kp.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://xp.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://pp.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wa.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vy.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://ap.nicolike.cn

Java: list.add(0, 0);
来源：http://me.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gp.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sw.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://rt.wgjwhj.cn

[D04] 删除元素
来源：http://lv.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kp.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dx.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lw.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://ib.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rn.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tk.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vu.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lo.nszjky.cn

[D05] 访问与修改元素
来源：http://nt.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pw.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rc.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ia.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://rw.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://rh.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://kx.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dt.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fa.nszjky.cn

[D06] 数组长度
来源：http://ed.hahajie.cn

Py:   len(arr)
来源：http://gz.asd995.cn

PHP:  count($arr);
来源：http://jg.wgjwhj.cn

JS:   arr.length
来源：http://gz.shxzskj.cn

TS:   arr.length
来源：http://ag.bookmarksfly.cn

Java: list.size();
来源：http://uu.yuntaijiaju.cn

Go:   len(arr)
来源：http://ls.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://wp.shxzukj.cn

C#:   list.Count;
来源：http://os.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://cg.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qv.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://la.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://nk.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://wu.colortex.cn

Java: list.subList(1, 4);
来源：http://vf.nszjky.cn

Go:   arr[1:4]
来源：http://ck.521024.cn

Ruby: arr[1, 3]
来源：http://fa.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://qr.nicolike.cn

[D08] 合并两个数组
来源：http://ha.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://ov.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://oa.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xl.muxihuayi.cn

TS:   [...a, ...b];
来源：http://ac.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lm.szxytkj.cn

Go:   append(a, b...)
来源：http://fh.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://pr.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://py.asd995.cn

[D09] 排序（升序）
来源：http://cz.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://mc.yuexingan06.cn

PHP:  sort($arr);
来源：http://ml.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wf.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wo.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jq.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mg.chemitech.net.cn

Ruby: arr.sort
来源：http://nt.huixinmuqiang.cn

C#:   list.Sort();
来源：http://mi.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rb.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tb.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://av.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ea.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ov.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://au.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lr.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xk.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jb.huanxung.cn

[D11] 反转数组
来源：http://kg.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oc.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://wv.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rl.nszjky.cn

TS:   [...arr].reverse();
来源：http://wa.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://iu.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://vh.huanxung.cn

Ruby: arr.reverse
来源：http://rx.lnxyls.cn

C#:   list.Reverse();
来源：http://lt.jctech888.com.cn

[D12] 查找元素下标
来源：http://uv.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://kq.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vz.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yg.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nd.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ue.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://us.szsharing.cn

Ruby: arr.index(x)
来源：http://ah.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://zo.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://ga.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://if.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sw.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://kz.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://pf.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nc.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aa.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qs.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nj.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://uu.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fv.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://su.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://tr.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://vh.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pq.hnjuh.cn

Go:   // 手写循环
来源：http://wn.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jx.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ke.shtwfgs.cn

[D15] 去重
来源：http://of.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nq.hnjuh.cn

PHP:  array_unique($arr);
来源：http://kr.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://re.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ax.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ok.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ib.szsharing.cn

Ruby: arr.uniq
来源：http://zc.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://uh.huanxung.cn

[D16] 求和与平均值
来源：http://er.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zx.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xq.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vb.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bv.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pw.bjjhwx.cn

Go:   // 手写循环累加
来源：http://sx.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rq.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://qm.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://cf.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://di.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://fw.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://za.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://dz.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bm.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fj.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://pt.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://qv.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://jz.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xu.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://br.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qb.bookmarksfly.cn

TS:   nested.flat();
来源：http://qb.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qz.huanxung.cn

Go:   // 手写双层循环
来源：http://lf.shxzskj.cn

Ruby: nested.flatten
来源：http://ek.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fq.shtwfgs.cn

[D19] 按字段分组
来源：http://zv.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gn.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sy.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eb.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ni.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hi.colortex.cn

Go:   // 手写 map[string][]T
来源：http://yn.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gd.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vw.521024.cn

[D20] 统计每个元素出现次数
来源：http://xb.szsharing.cn

Py:   Counter(arr)
来源：http://mq.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://ey.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zs.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wt.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mt.asd995.cn

Go:   // 手写 map[T]int
来源：http://mi.jianghongdianzi.cn

Ruby: arr.tally
来源：http://op.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ai.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://mf.nicolike.cn

Py:   x in arr
来源：http://uh.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://bk.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://td.nicolike.cn

TS:   arr.includes(x)
来源：http://vl.szxytkj.cn

Java: list.contains(x)
来源：http://ya.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://cx.huanxung.cn

Ruby: arr.include?(x)
来源：http://ks.521024.cn

C#:   list.Contains(x)
来源：http://bt.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://ng.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gt.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nw.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oj.wgjwhj.cn

TS:   [...arr];
来源：http://ei.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://vi.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ee.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://og.hahajie.cn

C#:   new List<int>(list);
来源：http://mo.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://qh.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://in.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mh.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fh.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sn.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pq.shxzskj.cn

Go:   // 手写循环
来源：http://zr.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uf.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xu.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://je.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gj.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zu.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wh.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://se.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vs.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yy.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qa.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rj.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://gv.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qj.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://is.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://em.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dq.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://px.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mv.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nv.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ii.colortex.cn

[D26] 数组转字符串
来源：http://kh.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://xj.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://hv.szsharing.cn

JS:   arr.join(", ")
来源：http://ih.lnxyls.cn

TS:   arr.join(", ")
来源：http://nd.lnxyls.cn

Java: String.join(", ", list)
来源：http://br.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://we.521024.cn

Ruby: arr.join(", ")
来源：http://ss.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://wa.yuexingan06.cn

================================================================================
来源：http://yi.jctech888.com.cn

E. 字符串处理
来源：http://dx.yuexingan06.cn

================================================================================
来源：http://kz.szxytkj.cn

[E01] 拼接字符串
来源：http://oy.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dp.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vu.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ob.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oi.shxzukj.cn


<!-- 参考信息 -->