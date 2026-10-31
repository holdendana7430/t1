代发 wailian999

[C10] 变量作用域
来源：http://xa.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kt.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ia.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sx.hahajie.cn

TS:   同 JS
来源：http://vg.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://mq.hahajie.cn

Go:   花括号块级作用域
来源：http://qi.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gy.wgjwhj.cn

C#:   块级作用域
来源：http://ej.chemitech.net.cn

[C11] 模块导入与导出
来源：http://zw.panjiajie.cn

Py:   from module import func
来源：http://yd.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yy.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zs.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dv.jianghongdianzi.cn

Java: import java.util.List;
来源：http://fo.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ra.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://ef.asd995.cn

C#:   using System.Text;
来源：http://vk.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://yz.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://rt.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://ru.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://ih.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://ui.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://if.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://zf.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://zs.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://js.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://ll.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bi.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bf.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ny.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ya.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ku.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://ke.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xo.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lz.shtwfgs.cn

[C14] 泛型函数
来源：http://na.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ju.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://nr.nszjky.cn

JS:   // 无泛型
来源：http://ld.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jy.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sf.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lj.nicolike.cn

Ruby: # 无泛型
来源：http://lr.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fb.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://zp.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mt.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://go.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ik.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gi.haigaiapp.cn

Java: // 无解构
来源：http://xh.jctech888.com.cn

Go:   // 无解构
来源：http://az.yuexingan06.cn

Ruby: a, b = pair
来源：http://pg.nicolike.cn

C#:   var (a, b) = pair;
来源：http://bj.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://fg.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wq.hahajie.cn

PHP:  // 无重载
来源：http://ju.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ug.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://je.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hm.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://ae.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://ad.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nb.gzmigu.cn

================================================================================
来源：http://ii.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://dp.wgjwhj.cn

================================================================================
来源：http://dy.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://rl.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eu.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ut.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dw.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zt.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fw.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://dk.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://qv.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xa.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://gx.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gt.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lj.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://pd.newstarts.cn

TS:   arr.push(4);
来源：http://oa.bookmarksfly.cn

Java: list.add(4);
来源：http://xg.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://ta.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://mp.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://yf.asd995.cn

[D03] 在指定位置插入元素
来源：http://jx.521024.cn

Py:   arr.insert(0, 0)
来源：http://ns.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://es.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oz.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://kh.huixiangedu.cn

Java: list.add(0, 0);
来源：http://db.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ku.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wv.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://xs.bookmarksfly.cn

[D04] 删除元素
来源：http://tr.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pc.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dh.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qn.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://xo.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bx.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qn.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uv.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hl.hahajie.cn

[D05] 访问与修改元素
来源：http://dd.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://am.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jb.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nz.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://dj.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://aj.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://cd.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qp.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qn.szxytkj.cn

[D06] 数组长度
来源：http://sy.huixiangedu.cn

Py:   len(arr)
来源：http://oa.shtwfgs.cn

PHP:  count($arr);
来源：http://eg.yuntaijiaju.cn

JS:   arr.length
来源：http://zo.asd995.cn

TS:   arr.length
来源：http://vy.jctech888.com.cn

Java: list.size();
来源：http://js.nszjky.cn

Go:   len(arr)
来源：http://wv.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://dr.jianghongdianzi.cn

C#:   list.Count;
来源：http://oc.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://tb.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cr.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eu.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://jc.colortex.cn

TS:   arr.slice(1, 4);
来源：http://sn.nszjky.cn

Java: list.subList(1, 4);
来源：http://yi.haigaiapp.cn

Go:   arr[1:4]
来源：http://yg.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://ff.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://ip.muxihuayi.cn

[D08] 合并两个数组
来源：http://iu.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://mk.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://hk.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://um.panjiajie.cn

TS:   [...a, ...b];
来源：http://go.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fr.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://lz.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://og.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://kx.bookmarksfly.cn

[D09] 排序（升序）
来源：http://nu.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://eg.gzmigu.cn

PHP:  sort($arr);
来源：http://uc.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hs.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fr.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ch.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xc.muxihuayi.cn

Ruby: arr.sort
来源：http://zb.hnjuh.cn

C#:   list.Sort();
来源：http://bz.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cq.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://px.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://df.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gt.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ya.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ou.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qe.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ep.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mf.yuntaijiaju.cn

[D11] 反转数组
来源：http://xc.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://an.9csxet.cn

PHP:  array_reverse($arr);
来源：http://fu.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hb.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://er.shxzskj.cn

Java: Collections.reverse(list);
来源：http://fn.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://pi.szsharing.cn

Ruby: arr.reverse
来源：http://xc.muxihuayi.cn

C#:   list.Reverse();
来源：http://us.gzmigu.cn

[D12] 查找元素下标
来源：http://xx.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://ph.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gt.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lo.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uf.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jn.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://wk.shxzukj.cn

Ruby: arr.index(x)
来源：http://dz.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://wk.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://rj.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://je.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hi.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://vb.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://ut.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bt.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xr.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jq.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dx.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://sr.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kf.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uj.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://ay.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://ro.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pm.wgjwhj.cn

Go:   // 手写循环
来源：http://xf.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nm.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xi.521024.cn

[D15] 去重
来源：http://nx.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oc.nicolike.cn

PHP:  array_unique($arr);
来源：http://ln.szsharing.cn

JS:   [...new Set(arr)]
来源：http://rf.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://fp.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cg.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ba.haigaiapp.cn

Ruby: arr.uniq
来源：http://fb.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://xp.bjjhwx.cn

[D16] 求和与平均值
来源：http://jn.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sd.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zx.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bt.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://da.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rw.lnxyls.cn

Go:   // 手写循环累加
来源：http://mv.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nj.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://aa.wgjwhj.cn

[D17] 最大值与最小值
来源：http://cz.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://on.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://ck.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fz.lnxyls.cn

TS:   Math.max(...arr);
来源：http://ag.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wm.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iw.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://lf.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://og.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://op.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fl.colortex.cn

PHP:  array_merge(...$nested);
来源：http://za.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ac.huixinmuqiang.cn

TS:   nested.flat();
来源：http://ib.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cg.szxytkj.cn

Go:   // 手写双层循环
来源：http://hw.gzmigu.cn

Ruby: nested.flatten
来源：http://og.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yd.bookmarksfly.cn

[D19] 按字段分组
来源：http://yu.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gv.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ss.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oc.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://az.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uu.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://pi.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sa.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lv.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://wc.lnxyls.cn

Py:   Counter(arr)
来源：http://kv.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://gl.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fb.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uh.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hn.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://qv.muxihuayi.cn

Ruby: arr.tally
来源：http://uw.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wz.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://xj.colortex.cn

Py:   x in arr
来源：http://wi.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://su.shtwfgs.cn

JS:   arr.includes(x)
来源：http://jc.newstarts.cn

TS:   arr.includes(x)
来源：http://de.hahajie.cn

Java: list.contains(x)
来源：http://cy.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://py.hahajie.cn

Ruby: arr.include?(x)
来源：http://bb.shtwfgs.cn

C#:   list.Contains(x)
来源：http://qp.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://ms.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fs.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lu.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uf.huixiangedu.cn

TS:   [...arr];
来源：http://yb.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://jz.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sn.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://xu.gzmigu.cn

C#:   new List<int>(list);
来源：http://yg.haigaiapp.cn

[D23] reduce 累积计算
来源：http://cp.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://de.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ht.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pa.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://im.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tu.shxzukj.cn

Go:   // 手写循环
来源：http://kf.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ey.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gg.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://ox.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ki.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fc.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fb.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ip.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dx.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xy.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fs.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pn.521024.cn

[D25] Set 集合去重与交并差
来源：http://yg.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pk.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cc.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://va.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sp.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jv.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qh.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://li.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zu.nicolike.cn

[D26] 数组转字符串
来源：http://bh.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://bo.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://lz.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://sj.shxzukj.cn

TS:   arr.join(", ")
来源：http://qh.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://mm.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://yr.521024.cn

Ruby: arr.join(", ")
来源：http://ty.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://eb.jianghongdianzi.cn


<!-- 参考信息 -->