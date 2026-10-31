代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xb.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ok.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zs.newstarts.cn

[C09] 递归
来源：http://ch.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uw.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://it.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uz.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yc.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yk.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gy.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ld.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yj.hnjuh.cn

[C10] 变量作用域
来源：http://rw.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nn.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ua.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ak.szsharing.cn

TS:   同 JS
来源：http://pl.hnjuh.cn

Java: 方法内为块级作用域
来源：http://st.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://vj.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ql.jianghongdianzi.cn

C#:   块级作用域
来源：http://vs.bjjhwx.cn

[C11] 模块导入与导出
来源：http://hl.szxytkj.cn

Py:   from module import func
来源：http://la.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://um.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sv.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ts.huanxung.cn

Java: import java.util.List;
来源：http://az.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yq.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://dv.jianghongdianzi.cn

C#:   using System.Text;
来源：http://ke.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://lo.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://wv.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://pb.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://ae.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://nn.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ag.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://fx.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://ci.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vy.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://lm.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://za.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xd.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://da.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yt.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kx.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://sb.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ae.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fw.asd995.cn

[C14] 泛型函数
来源：http://gj.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uv.huixiangedu.cn

PHP:  // 无泛型
来源：http://dz.huixinmuqiang.cn

JS:   // 无泛型
来源：http://lt.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nl.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tg.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mu.yuexingan06.cn

Ruby: # 无泛型
来源：http://bw.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gf.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://yp.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dg.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://gs.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lt.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dm.asd995.cn

Java: // 无解构
来源：http://eq.yuexingan06.cn

Go:   // 无解构
来源：http://hl.panjiajie.cn

Ruby: a, b = pair
来源：http://tf.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://pd.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://sn.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mk.muxihuayi.cn

PHP:  // 无重载
来源：http://bu.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pp.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://br.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ic.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://qe.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://os.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ky.nicolike.cn

================================================================================
来源：http://hb.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://ah.huixiangedu.cn

================================================================================
来源：http://td.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://ct.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cc.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://so.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mm.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://br.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hn.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://aj.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://cd.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pb.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://cm.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nu.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wp.wgjwhj.cn

JS:   arr.push(4);
来源：http://qc.shxzskj.cn

TS:   arr.push(4);
来源：http://xc.newstarts.cn

Java: list.add(4);
来源：http://ty.521024.cn

Go:   arr = append(arr, 4)
来源：http://mf.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://nd.9csxet.cn

C#:   list.Add(4);
来源：http://kt.newstarts.cn

[D03] 在指定位置插入元素
来源：http://uy.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://rl.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://st.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wq.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://on.yuexingan06.cn

Java: list.add(0, 0);
来源：http://nv.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ak.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zb.521024.cn

C#:   list.Insert(0, 0);
来源：http://hk.huixiangedu.cn

[D04] 删除元素
来源：http://ab.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ve.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bd.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nb.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://ad.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ed.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uj.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ah.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gb.bjjhwx.cn

[D05] 访问与修改元素
来源：http://za.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ne.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ru.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pj.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://lf.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ur.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://sy.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ua.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uo.haigaiapp.cn

[D06] 数组长度
来源：http://pq.wgjwhj.cn

Py:   len(arr)
来源：http://pb.hahajie.cn

PHP:  count($arr);
来源：http://qm.gzmigu.cn

JS:   arr.length
来源：http://oy.shxzskj.cn

TS:   arr.length
来源：http://ht.bjjhwx.cn

Java: list.size();
来源：http://oe.nicolike.cn

Go:   len(arr)
来源：http://di.asd995.cn

Ruby: arr.length; arr.size
来源：http://bb.yuntaijiaju.cn

C#:   list.Count;
来源：http://sf.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://su.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oy.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yu.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://be.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ot.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://mr.521024.cn

Go:   arr[1:4]
来源：http://um.shxzukj.cn

Ruby: arr[1, 3]
来源：http://iu.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://pb.chemitech.net.cn

[D08] 合并两个数组
来源：http://is.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://vl.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://tz.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://de.shxzskj.cn

TS:   [...a, ...b];
来源：http://kh.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ov.newstarts.cn

Go:   append(a, b...)
来源：http://ik.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://qe.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://dc.lnxyls.cn

[D09] 排序（升序）
来源：http://dl.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://eg.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://vp.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://on.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gq.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ma.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bl.bjjhwx.cn

Ruby: arr.sort
来源：http://tj.huixinmuqiang.cn

C#:   list.Sort();
来源：http://do.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ew.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rl.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fr.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kx.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kj.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nv.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://un.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wn.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qq.hahajie.cn

[D11] 反转数组
来源：http://ru.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wv.hahajie.cn

PHP:  array_reverse($arr);
来源：http://em.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xl.521024.cn

TS:   [...arr].reverse();
来源：http://lm.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://tq.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://rc.muxihuayi.cn

Ruby: arr.reverse
来源：http://ae.newstarts.cn

C#:   list.Reverse();
来源：http://mt.jctech888.com.cn

[D12] 查找元素下标
来源：http://jx.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://sb.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://np.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xt.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jr.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oh.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://tb.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://kl.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://wb.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://bt.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ah.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kf.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://gz.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://za.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ft.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dd.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bt.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hc.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://aw.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://br.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rf.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://tq.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://ub.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fq.9csxet.cn

Go:   // 手写循环
来源：http://dm.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uo.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ww.colortex.cn

[D15] 去重
来源：http://dp.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cl.colortex.cn

PHP:  array_unique($arr);
来源：http://sf.521024.cn

JS:   [...new Set(arr)]
来源：http://cu.nszjky.cn

TS:   [...new Set(arr)]
来源：http://me.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ms.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gm.panjiajie.cn

Ruby: arr.uniq
来源：http://af.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://bz.colortex.cn

[D16] 求和与平均值
来源：http://ut.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yh.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mv.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wt.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hc.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://so.wgjwhj.cn

Go:   // 手写循环累加
来源：http://sv.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ol.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://cr.lnxyls.cn

[D17] 最大值与最小值
来源：http://iw.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://zs.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://wn.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sr.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://ly.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hy.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://on.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://zg.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://dk.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://mc.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wu.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://ns.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sr.szsharing.cn

TS:   nested.flat();
来源：http://xc.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sl.hnjuh.cn

Go:   // 手写双层循环
来源：http://va.wgjwhj.cn

Ruby: nested.flatten
来源：http://df.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ld.huixiangedu.cn

[D19] 按字段分组
来源：http://gk.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rn.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ub.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pk.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ek.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hv.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://yt.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hy.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bo.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://iv.yuexingan06.cn

Py:   Counter(arr)
来源：http://xi.huanxung.cn

PHP:  array_count_values($arr);
来源：http://hf.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bf.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gr.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xi.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://bt.9csxet.cn

Ruby: arr.tally
来源：http://em.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uy.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://fs.yuntaijiaju.cn

Py:   x in arr
来源：http://jy.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://vk.muxihuayi.cn

JS:   arr.includes(x)
来源：http://rz.hnjuh.cn

TS:   arr.includes(x)
来源：http://sm.bjjhwx.cn

Java: list.contains(x)
来源：http://wz.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://gx.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://fb.chemitech.net.cn

C#:   list.Contains(x)
来源：http://uj.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://iy.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ul.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://us.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sa.huixinmuqiang.cn

TS:   [...arr];
来源：http://ak.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://bf.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ro.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://pd.bjjhwx.cn

C#:   new List<int>(list);
来源：http://jj.shxzukj.cn

[D23] reduce 累积计算
来源：http://at.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zo.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ka.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ng.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tw.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xc.huixinmuqiang.cn

Go:   // 手写循环
来源：http://yt.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lz.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://er.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://jh.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://au.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jk.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fl.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rw.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ab.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nt.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pv.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fp.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://za.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rr.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hk.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://if.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rg.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://of.szsharing.cn


<!-- 参考信息 -->