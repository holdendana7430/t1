代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wt.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://go.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ph.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oe.gzmigu.cn

[C10] 变量作用域
来源：http://ty.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dd.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kr.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vs.asd995.cn

TS:   同 JS
来源：http://cr.nicolike.cn

Java: 方法内为块级作用域
来源：http://ux.szsharing.cn

Go:   花括号块级作用域
来源：http://cf.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ip.hahajie.cn

C#:   块级作用域
来源：http://ww.hnjuh.cn

[C11] 模块导入与导出
来源：http://av.szxytkj.cn

Py:   from module import func
来源：http://ha.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vk.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ci.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uy.bjjhwx.cn

Java: import java.util.List;
来源：http://au.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ik.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://rq.bookmarksfly.cn

C#:   using System.Text;
来源：http://ep.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://tl.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://lo.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://tu.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://fo.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://je.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gq.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://rr.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://zo.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yn.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://on.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ij.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uy.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qe.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wz.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ha.newstarts.cn

Go:   func add(a, b int) int
来源：http://pa.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fd.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ej.nicolike.cn

[C14] 泛型函数
来源：http://fa.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ab.shxzskj.cn

PHP:  // 无泛型
来源：http://mz.521024.cn

JS:   // 无泛型
来源：http://ns.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tr.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ba.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yr.521024.cn

Ruby: # 无泛型
来源：http://nl.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nx.szsharing.cn

[C15] 解构 / 展开参数
来源：http://nk.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zp.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://ry.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pv.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mi.szsharing.cn

Java: // 无解构
来源：http://nh.gzmigu.cn

Go:   // 无解构
来源：http://pn.wgjwhj.cn

Ruby: a, b = pair
来源：http://pg.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://sa.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://xy.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cz.9csxet.cn

PHP:  // 无重载
来源：http://cb.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pr.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://uh.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mn.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://fn.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://iv.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wm.huixiangedu.cn

================================================================================
来源：http://pv.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://co.colortex.cn

================================================================================
来源：http://qx.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://ja.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pl.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ev.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://za.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hr.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tp.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ug.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://np.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hm.asd995.cn

[D02] 追加元素到末尾
来源：http://xr.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://as.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bn.hnjuh.cn

JS:   arr.push(4);
来源：http://ms.colortex.cn

TS:   arr.push(4);
来源：http://sc.huixinmuqiang.cn

Java: list.add(4);
来源：http://ui.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://zx.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://xh.nicolike.cn

C#:   list.Add(4);
来源：http://nm.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://ov.asd995.cn

Py:   arr.insert(0, 0)
来源：http://rf.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bc.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oy.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://rs.bjjhwx.cn

Java: list.add(0, 0);
来源：http://xv.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kf.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://va.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://ie.haigaiapp.cn

[D04] 删除元素
来源：http://mx.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://po.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jw.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ib.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://ca.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ju.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cx.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ef.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://no.chemitech.net.cn

[D05] 访问与修改元素
来源：http://ye.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hj.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cf.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ul.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://wt.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://ft.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://sy.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vp.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aq.huixinmuqiang.cn

[D06] 数组长度
来源：http://ef.lnxyls.cn

Py:   len(arr)
来源：http://we.panjiajie.cn

PHP:  count($arr);
来源：http://me.yuntaijiaju.cn

JS:   arr.length
来源：http://ul.521024.cn

TS:   arr.length
来源：http://hl.hnjuh.cn

Java: list.size();
来源：http://xk.9csxet.cn

Go:   len(arr)
来源：http://cz.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://kl.muxihuayi.cn

C#:   list.Count;
来源：http://nm.szsharing.cn

[D07] 切片 / 取子数组
来源：http://nq.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ls.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hm.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://in.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://fw.hahajie.cn

Java: list.subList(1, 4);
来源：http://vq.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://jq.huanxung.cn

Ruby: arr[1, 3]
来源：http://pi.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://bi.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://cb.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://cr.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://ej.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rl.haigaiapp.cn

TS:   [...a, ...b];
来源：http://fu.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qj.colortex.cn

Go:   append(a, b...)
来源：http://os.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://ob.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://df.muxihuayi.cn

[D09] 排序（升序）
来源：http://tf.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://rp.bjjhwx.cn

PHP:  sort($arr);
来源：http://ur.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rb.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fa.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pv.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zv.jianghongdianzi.cn

Ruby: arr.sort
来源：http://ws.asd995.cn

C#:   list.Sort();
来源：http://ii.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vg.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hr.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iz.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rq.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wk.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yr.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dn.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eh.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tm.nszjky.cn

[D11] 反转数组
来源：http://eg.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nr.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://fp.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xs.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://lw.szxytkj.cn

Java: Collections.reverse(list);
来源：http://nk.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://vr.newstarts.cn

Ruby: arr.reverse
来源：http://ks.gzmigu.cn

C#:   list.Reverse();
来源：http://vy.nszjky.cn

[D12] 查找元素下标
来源：http://ar.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://hc.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yq.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://va.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bb.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qw.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://cs.huanxung.cn

Ruby: arr.index(x)
来源：http://cm.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://ep.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://ky.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gm.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://la.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://io.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://wd.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jd.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qf.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ie.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ad.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://ad.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ow.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zc.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://hp.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://gm.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ko.bjjhwx.cn

Go:   // 手写循环
来源：http://ga.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://th.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uj.shxzskj.cn

[D15] 去重
来源：http://mj.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://au.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://mf.szsharing.cn

JS:   [...new Set(arr)]
来源：http://ev.nszjky.cn

TS:   [...new Set(arr)]
来源：http://fz.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ap.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gi.huixiangedu.cn

Ruby: arr.uniq
来源：http://bi.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://kz.panjiajie.cn

[D16] 求和与平均值
来源：http://ds.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wc.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tu.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cj.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ye.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://my.asd995.cn

Go:   // 手写循环累加
来源：http://tm.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ko.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://dl.chemitech.net.cn

[D17] 最大值与最小值
来源：http://uf.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://fa.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://ns.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hx.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://ul.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kk.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jy.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://iy.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://on.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://vr.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cf.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://bm.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cj.shtwfgs.cn

TS:   nested.flat();
来源：http://ff.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ey.colortex.cn

Go:   // 手写双层循环
来源：http://iw.bjjhwx.cn

Ruby: nested.flatten
来源：http://mi.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pl.newstarts.cn

[D19] 按字段分组
来源：http://xf.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://by.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jt.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hr.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rw.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ij.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://zs.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yt.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fm.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://wi.hnjuh.cn

Py:   Counter(arr)
来源：http://zu.nicolike.cn

PHP:  array_count_values($arr);
来源：http://sa.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bj.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ff.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ss.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://gq.newstarts.cn

Ruby: arr.tally
来源：http://xi.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iq.9csxet.cn

[D21] 判断是否包含某元素
来源：http://wt.bjjhwx.cn

Py:   x in arr
来源：http://bw.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://he.521024.cn

JS:   arr.includes(x)
来源：http://zs.nicolike.cn

TS:   arr.includes(x)
来源：http://hr.bjjhwx.cn

Java: list.contains(x)
来源：http://ly.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://ah.nicolike.cn

Ruby: arr.include?(x)
来源：http://jx.shxzukj.cn

C#:   list.Contains(x)
来源：http://xb.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://lv.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vv.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oa.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tb.colortex.cn

TS:   [...arr];
来源：http://fi.521024.cn

Java: new ArrayList<>(list);
来源：http://ux.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://du.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://co.panjiajie.cn

C#:   new List<int>(list);
来源：http://ju.huanxung.cn

[D23] reduce 累积计算
来源：http://xx.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tc.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xd.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jj.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cr.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://un.szsharing.cn

Go:   // 手写循环
来源：http://sv.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gx.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pf.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://fx.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cp.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sm.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xr.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://op.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pc.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://of.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uj.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://li.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://wz.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qd.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yd.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fj.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://au.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wm.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gt.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ii.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zx.521024.cn

[D26] 数组转字符串
来源：http://qc.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://lo.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://co.bjjhwx.cn

JS:   arr.join(", ")
来源：http://lb.newstarts.cn

TS:   arr.join(", ")
来源：http://nz.szsharing.cn


<!-- 参考信息 -->