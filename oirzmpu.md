代发 wailian999

[C10] 变量作用域
来源：http://io.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rn.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bf.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ta.521024.cn

TS:   同 JS
来源：http://iz.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ta.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://rb.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://la.shxzukj.cn

C#:   块级作用域
来源：http://ag.shxzukj.cn

[C11] 模块导入与导出
来源：http://zh.chemitech.net.cn

Py:   from module import func
来源：http://pp.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ya.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ng.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hd.nicolike.cn

Java: import java.util.List;
来源：http://oj.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iw.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://vt.newstarts.cn

C#:   using System.Text;
来源：http://bh.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ay.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://za.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://bk.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://fz.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://zv.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gg.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://tz.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://sm.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ls.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://ex.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zq.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lf.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://il.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://no.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cs.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://sw.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hw.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://te.wgjwhj.cn

[C14] 泛型函数
来源：http://ug.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rs.nszjky.cn

PHP:  // 无泛型
来源：http://hc.bookmarksfly.cn

JS:   // 无泛型
来源：http://vg.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ht.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qs.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ew.asd995.cn

Ruby: # 无泛型
来源：http://gk.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tg.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://qa.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ax.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://zg.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wc.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ro.jctech888.com.cn

Java: // 无解构
来源：http://bf.huixinmuqiang.cn

Go:   // 无解构
来源：http://mb.jctech888.com.cn

Ruby: a, b = pair
来源：http://gj.9csxet.cn

C#:   var (a, b) = pair;
来源：http://md.newstarts.cn

[C16] 函数 / 方法重载
来源：http://mv.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kp.asd995.cn

PHP:  // 无重载
来源：http://pc.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eo.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://xj.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fa.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://tj.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://ls.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yo.9csxet.cn

================================================================================
来源：http://kd.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://qi.shxzskj.cn

================================================================================
来源：http://px.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://cv.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kw.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ww.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://of.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://km.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aw.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://dy.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://oc.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qq.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://vy.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vj.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://in.szxytkj.cn

JS:   arr.push(4);
来源：http://fi.wgjwhj.cn

TS:   arr.push(4);
来源：http://aa.muxihuayi.cn

Java: list.add(4);
来源：http://jb.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://cz.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://su.shtwfgs.cn

C#:   list.Add(4);
来源：http://yr.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://gh.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://pe.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://co.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xz.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://rc.asd995.cn

Java: list.add(0, 0);
来源：http://hr.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vx.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gn.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://aa.huixiangedu.cn

[D04] 删除元素
来源：http://rt.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ue.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://in.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://bg.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fv.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lj.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yy.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wz.lnxyls.cn

[D05] 访问与修改元素
来源：http://tr.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://io.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vb.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nx.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://jh.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://zr.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://vs.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kb.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ap.gzmigu.cn

[D06] 数组长度
来源：http://cv.panjiajie.cn

Py:   len(arr)
来源：http://dg.shxzskj.cn

PHP:  count($arr);
来源：http://wl.szxytkj.cn

JS:   arr.length
来源：http://ni.gzmigu.cn

TS:   arr.length
来源：http://cu.wgjwhj.cn

Java: list.size();
来源：http://hx.yuntaijiaju.cn

Go:   len(arr)
来源：http://jc.9csxet.cn

Ruby: arr.length; arr.size
来源：http://eu.nszjky.cn

C#:   list.Count;
来源：http://nh.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://jt.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xq.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mm.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://pi.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://zo.gzmigu.cn

Java: list.subList(1, 4);
来源：http://fh.shxzskj.cn

Go:   arr[1:4]
来源：http://ox.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://vb.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://uk.lnxyls.cn

[D08] 合并两个数组
来源：http://qp.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://mt.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://eg.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ga.bjjhwx.cn

TS:   [...a, ...b];
来源：http://ld.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ti.chemitech.net.cn

Go:   append(a, b...)
来源：http://yv.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://yd.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://ya.gzmigu.cn

[D09] 排序（升序）
来源：http://ww.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://kg.chemitech.net.cn

PHP:  sort($arr);
来源：http://jb.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vf.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yx.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ge.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://th.shtwfgs.cn

Ruby: arr.sort
来源：http://jf.muxihuayi.cn

C#:   list.Sort();
来源：http://vg.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zg.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vp.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bh.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jz.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kq.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://en.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ic.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cd.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lr.lnxyls.cn

[D11] 反转数组
来源：http://dz.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ek.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://ai.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jw.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://jk.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://mc.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://re.bookmarksfly.cn

Ruby: arr.reverse
来源：http://cr.lnxyls.cn

C#:   list.Reverse();
来源：http://bp.shtwfgs.cn

[D12] 查找元素下标
来源：http://lf.521024.cn

Py:   arr.index(x);  x in arr
来源：http://uv.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://az.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fz.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://on.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ke.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://ew.bjjhwx.cn

Ruby: arr.index(x)
来源：http://my.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://vj.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://cu.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kq.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yy.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://dq.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://mo.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kv.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kd.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kz.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cs.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://lq.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ll.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qp.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://qn.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://vs.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mc.colortex.cn

Go:   // 手写循环
来源：http://lh.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ls.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bt.muxihuayi.cn

[D15] 去重
来源：http://jm.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fu.huanxung.cn

PHP:  array_unique($arr);
来源：http://yx.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://aa.szsharing.cn

TS:   [...new Set(arr)]
来源：http://lk.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://um.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ka.bookmarksfly.cn

Ruby: arr.uniq
来源：http://ts.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://en.hahajie.cn

[D16] 求和与平均值
来源：http://ev.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ac.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ex.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rm.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kx.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lz.huanxung.cn

Go:   // 手写循环累加
来源：http://sq.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dx.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://uw.hahajie.cn

[D17] 最大值与最小值
来源：http://sd.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://in.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://rh.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rt.shxzskj.cn

TS:   Math.max(...arr);
来源：http://zh.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jb.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://da.asd995.cn

Ruby: arr.max;  arr.min
来源：http://qa.colortex.cn

C#:   list.Max();  list.Min()
来源：http://ji.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://pz.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vj.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://lb.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rd.521024.cn

TS:   nested.flat();
来源：http://fe.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sn.newstarts.cn

Go:   // 手写双层循环
来源：http://np.521024.cn

Ruby: nested.flatten
来源：http://lo.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://un.szxytkj.cn

[D19] 按字段分组
来源：http://vr.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ab.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ko.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dy.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://af.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sq.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://tm.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jy.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://py.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://ja.hnjuh.cn

Py:   Counter(arr)
来源：http://qp.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://nj.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qa.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fw.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://aq.hnjuh.cn

Ruby: arr.tally
来源：http://qs.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wj.521024.cn

[D21] 判断是否包含某元素
来源：http://ny.shtwfgs.cn

Py:   x in arr
来源：http://ld.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://fm.shxzskj.cn

JS:   arr.includes(x)
来源：http://dr.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://vj.huixiangedu.cn

Java: list.contains(x)
来源：http://np.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://qs.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://zx.huanxung.cn

C#:   list.Contains(x)
来源：http://um.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://bw.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ft.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lh.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qe.haigaiapp.cn

TS:   [...arr];
来源：http://yc.9csxet.cn

Java: new ArrayList<>(list);
来源：http://xu.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cl.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://oz.nicolike.cn

C#:   new List<int>(list);
来源：http://mu.muxihuayi.cn

[D23] reduce 累积计算
来源：http://ve.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iw.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mh.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sb.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fg.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vu.szxytkj.cn

Go:   // 手写循环
来源：http://gr.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mx.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mx.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://tp.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ao.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tw.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yd.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wl.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pj.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xs.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mq.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gy.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://wi.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nc.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://of.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pu.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ik.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mm.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wu.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qp.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xp.shtwfgs.cn

[D26] 数组转字符串
来源：http://ox.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ng.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://ic.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://us.hahajie.cn

TS:   arr.join(", ")
来源：http://ie.huanxung.cn

Java: String.join(", ", list)
来源：http://ew.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://ad.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://sb.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://cq.panjiajie.cn


<!-- 参考信息 -->