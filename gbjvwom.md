代发 wailian999

[C10] 变量作用域
来源：http://bt.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wu.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ql.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://js.9csxet.cn

TS:   同 JS
来源：http://gk.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ox.huixiangedu.cn

Go:   花括号块级作用域
来源：http://ih.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ui.panjiajie.cn

C#:   块级作用域
来源：http://gp.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://td.gzmigu.cn

Py:   from module import func
来源：http://yu.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sn.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vm.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qs.asd995.cn

Java: import java.util.List;
来源：http://mq.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xk.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://lb.panjiajie.cn

C#:   using System.Text;
来源：http://rv.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://gy.colortex.cn

Py:   (lambda: print("run"))()
来源：http://aa.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://xb.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://eo.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://jj.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fl.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://qc.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://fw.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zf.521024.cn

[C13] 类型声明 / 类型注解
来源：http://zo.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ph.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ch.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fj.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gy.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qn.shxzukj.cn

Go:   func add(a, b int) int
来源：http://wv.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qu.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://df.huixinmuqiang.cn

[C14] 泛型函数
来源：http://xb.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hn.shtwfgs.cn

PHP:  // 无泛型
来源：http://yc.asd995.cn

JS:   // 无泛型
来源：http://ed.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gj.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zh.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bu.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://he.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ke.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://gi.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mm.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://qn.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zh.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pu.huanxung.cn

Java: // 无解构
来源：http://dt.haigaiapp.cn

Go:   // 无解构
来源：http://my.szsharing.cn

Ruby: a, b = pair
来源：http://si.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://pd.9csxet.cn

[C16] 函数 / 方法重载
来源：http://ep.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ff.chemitech.net.cn

PHP:  // 无重载
来源：http://gu.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tb.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://wa.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rq.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://eh.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://nh.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vz.hnjuh.cn

================================================================================
来源：http://fr.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://df.hnjuh.cn

================================================================================
来源：http://kl.hahajie.cn

[D01] 创建数组 / 列表
来源：http://lc.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bg.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aw.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iw.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ng.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ch.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://rd.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://gb.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zd.asd995.cn

[D02] 追加元素到末尾
来源：http://jl.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rd.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ye.muxihuayi.cn

JS:   arr.push(4);
来源：http://kk.hahajie.cn

TS:   arr.push(4);
来源：http://as.gzmigu.cn

Java: list.add(4);
来源：http://uj.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://no.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://zh.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://hw.colortex.cn

[D03] 在指定位置插入元素
来源：http://pb.colortex.cn

Py:   arr.insert(0, 0)
来源：http://vv.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://an.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tk.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://wo.nszjky.cn

Java: list.add(0, 0);
来源：http://tl.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://de.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ss.colortex.cn

C#:   list.Insert(0, 0);
来源：http://mo.jctech888.com.cn

[D04] 删除元素
来源：http://vr.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://si.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qx.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yx.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://ce.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zx.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bp.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://om.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eb.huanxung.cn

[D05] 访问与修改元素
来源：http://qk.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oi.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hm.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xt.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://nb.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://bi.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://aw.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ad.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cp.bjjhwx.cn

[D06] 数组长度
来源：http://pa.nicolike.cn

Py:   len(arr)
来源：http://bp.muxihuayi.cn

PHP:  count($arr);
来源：http://sf.muxihuayi.cn

JS:   arr.length
来源：http://tu.wgjwhj.cn

TS:   arr.length
来源：http://zw.shxzukj.cn

Java: list.size();
来源：http://fl.muxihuayi.cn

Go:   len(arr)
来源：http://gb.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://tj.nicolike.cn

C#:   list.Count;
来源：http://fr.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://yy.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sp.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ad.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://rf.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://va.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://zr.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://bx.shxzukj.cn

Ruby: arr[1, 3]
来源：http://yz.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://dq.huanxung.cn

[D08] 合并两个数组
来源：http://la.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://rg.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://lt.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tm.nicolike.cn

TS:   [...a, ...b];
来源：http://xr.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wa.yuexingan06.cn

Go:   append(a, b...)
来源：http://qv.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://cg.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://up.521024.cn

[D09] 排序（升序）
来源：http://fv.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://kc.shxzskj.cn

PHP:  sort($arr);
来源：http://lf.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vj.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tn.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hx.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ja.newstarts.cn

Ruby: arr.sort
来源：http://ml.bjjhwx.cn

C#:   list.Sort();
来源：http://xs.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eb.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nz.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wd.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zs.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zl.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jx.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hd.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://un.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tn.colortex.cn

[D11] 反转数组
来源：http://wc.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zd.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://sf.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xw.szxytkj.cn

TS:   [...arr].reverse();
来源：http://ag.colortex.cn

Java: Collections.reverse(list);
来源：http://qe.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://kx.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://td.chemitech.net.cn

C#:   list.Reverse();
来源：http://rf.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://qu.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://bg.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nu.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mr.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tz.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vk.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://oo.lnxyls.cn

Ruby: arr.index(x)
来源：http://lu.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://ob.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://lq.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oq.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gk.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://ow.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://fn.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hm.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ej.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tl.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://im.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://rk.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wz.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ys.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://zr.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://br.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ch.muxihuayi.cn

Go:   // 手写循环
来源：http://sf.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ay.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rr.gzmigu.cn

[D15] 去重
来源：http://zn.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ed.newstarts.cn

PHP:  array_unique($arr);
来源：http://ix.szsharing.cn

JS:   [...new Set(arr)]
来源：http://iv.nicolike.cn

TS:   [...new Set(arr)]
来源：http://sp.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ra.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vl.521024.cn

Ruby: arr.uniq
来源：http://xc.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://lp.newstarts.cn

[D16] 求和与平均值
来源：http://pv.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ev.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dv.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mg.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bs.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://la.haigaiapp.cn

Go:   // 手写循环累加
来源：http://ue.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://od.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://br.shxzukj.cn

[D17] 最大值与最小值
来源：http://is.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://pt.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://qf.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wy.nicolike.cn

TS:   Math.max(...arr);
来源：http://yi.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vi.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vq.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://jr.521024.cn

C#:   list.Max();  list.Min()
来源：http://od.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://jt.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wz.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://ql.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://od.521024.cn

TS:   nested.flat();
来源：http://lo.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jh.szsharing.cn

Go:   // 手写双层循环
来源：http://yh.haigaiapp.cn

Ruby: nested.flatten
来源：http://gy.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wp.bookmarksfly.cn

[D19] 按字段分组
来源：http://xj.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ua.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ko.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cs.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bb.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ca.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://tw.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ui.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mj.colortex.cn

[D20] 统计每个元素出现次数
来源：http://xw.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://jk.521024.cn

PHP:  array_count_values($arr);
来源：http://me.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qr.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oe.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zh.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://hk.nicolike.cn

Ruby: arr.tally
来源：http://si.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nn.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://se.haigaiapp.cn

Py:   x in arr
来源：http://we.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://hz.huanxung.cn

JS:   arr.includes(x)
来源：http://rm.newstarts.cn

TS:   arr.includes(x)
来源：http://xf.bookmarksfly.cn

Java: list.contains(x)
来源：http://dk.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://ic.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://aj.szsharing.cn

C#:   list.Contains(x)
来源：http://fd.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://ye.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://we.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gh.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yl.521024.cn

TS:   [...arr];
来源：http://zx.colortex.cn

Java: new ArrayList<>(list);
来源：http://st.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rc.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://vb.gzmigu.cn

C#:   new List<int>(list);
来源：http://ol.nicolike.cn

[D23] reduce 累积计算
来源：http://qm.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mb.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eb.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ud.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://np.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ge.panjiajie.cn

Go:   // 手写循环
来源：http://on.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fw.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ag.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://ak.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://da.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jl.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tm.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ih.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tm.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gh.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zw.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gc.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://ue.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yu.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yb.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ae.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dw.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://an.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ly.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://as.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oh.shxzukj.cn

[D26] 数组转字符串
来源：http://vt.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://vc.asd995.cn

PHP:  implode(", ", $arr);
来源：http://mu.shtwfgs.cn

JS:   arr.join(", ")
来源：http://kh.haigaiapp.cn

TS:   arr.join(", ")
来源：http://qv.asd995.cn

Java: String.join(", ", list)
来源：http://jx.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://oc.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://jm.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://le.jianghongdianzi.cn


<!-- 参考信息 -->