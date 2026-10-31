代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yo.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qh.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vk.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wa.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ea.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ff.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://il.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lo.jianghongdianzi.cn

[C10] 变量作用域
来源：http://sd.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zo.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ui.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ca.hnjuh.cn

TS:   同 JS
来源：http://we.9csxet.cn

Java: 方法内为块级作用域
来源：http://ue.nicolike.cn

Go:   花括号块级作用域
来源：http://yq.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hf.nicolike.cn

C#:   块级作用域
来源：http://bz.muxihuayi.cn

[C11] 模块导入与导出
来源：http://ot.shxzskj.cn

Py:   from module import func
来源：http://hk.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wc.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vu.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bu.jianghongdianzi.cn

Java: import java.util.List;
来源：http://rv.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ev.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://xu.colortex.cn

C#:   using System.Text;
来源：http://am.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://fv.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://qa.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://xl.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://vi.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://pz.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tm.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://yv.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://ew.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qt.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://lb.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yh.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rw.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uk.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wi.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cw.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://qa.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://md.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wr.9csxet.cn

[C14] 泛型函数
来源：http://kq.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nt.szsharing.cn

PHP:  // 无泛型
来源：http://hj.bjjhwx.cn

JS:   // 无泛型
来源：http://sg.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fq.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vj.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vs.jctech888.com.cn

Ruby: # 无泛型
来源：http://qb.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ev.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://ce.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hs.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://ss.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://up.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kt.521024.cn

Java: // 无解构
来源：http://ak.shtwfgs.cn

Go:   // 无解构
来源：http://yc.szsharing.cn

Ruby: a, b = pair
来源：http://rd.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://xf.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://gk.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fq.shtwfgs.cn

PHP:  // 无重载
来源：http://nl.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hn.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://bf.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ko.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://gu.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://xm.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fn.bookmarksfly.cn

================================================================================
来源：http://eg.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://eu.szxytkj.cn

================================================================================
来源：http://ps.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://bj.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ee.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ds.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kf.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mg.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sh.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://ra.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://as.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kz.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://bh.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://au.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wh.bjjhwx.cn

JS:   arr.push(4);
来源：http://vm.szxytkj.cn

TS:   arr.push(4);
来源：http://oe.chemitech.net.cn

Java: list.add(4);
来源：http://ef.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://ws.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://xu.haigaiapp.cn

C#:   list.Add(4);
来源：http://hu.nszjky.cn

[D03] 在指定位置插入元素
来源：http://qj.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://cc.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qp.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hh.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://mg.shxzskj.cn

Java: list.add(0, 0);
来源：http://vz.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sn.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nl.asd995.cn

C#:   list.Insert(0, 0);
来源：http://fj.lnxyls.cn

[D04] 删除元素
来源：http://gx.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cb.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ax.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://br.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://cj.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bf.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zq.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://my.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xe.bjjhwx.cn

[D05] 访问与修改元素
来源：http://jm.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uy.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fa.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dd.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://sl.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://zd.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://bf.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aj.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mq.nicolike.cn

[D06] 数组长度
来源：http://uj.haigaiapp.cn

Py:   len(arr)
来源：http://ji.jctech888.com.cn

PHP:  count($arr);
来源：http://ew.shxzskj.cn

JS:   arr.length
来源：http://by.newstarts.cn

TS:   arr.length
来源：http://hf.jctech888.com.cn

Java: list.size();
来源：http://pd.gzmigu.cn

Go:   len(arr)
来源：http://vj.huanxung.cn

Ruby: arr.length; arr.size
来源：http://qh.szxytkj.cn

C#:   list.Count;
来源：http://lr.9csxet.cn

[D07] 切片 / 取子数组
来源：http://ao.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tz.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://se.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://we.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://ca.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://sg.newstarts.cn

Go:   arr[1:4]
来源：http://jn.9csxet.cn

Ruby: arr[1, 3]
来源：http://hw.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://bm.wgjwhj.cn

[D08] 合并两个数组
来源：http://sx.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://jc.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://ws.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kf.bjjhwx.cn

TS:   [...a, ...b];
来源：http://fi.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cl.szxytkj.cn

Go:   append(a, b...)
来源：http://fo.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://zc.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://on.wgjwhj.cn

[D09] 排序（升序）
来源：http://ej.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://uc.szsharing.cn

PHP:  sort($arr);
来源：http://jq.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pp.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://et.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vb.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kq.muxihuayi.cn

Ruby: arr.sort
来源：http://ef.szxytkj.cn

C#:   list.Sort();
来源：http://uh.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kh.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mc.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jz.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gr.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bc.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wi.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ty.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ar.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mm.9csxet.cn

[D11] 反转数组
来源：http://kr.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jc.nszjky.cn

PHP:  array_reverse($arr);
来源：http://uy.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yj.521024.cn

TS:   [...arr].reverse();
来源：http://ap.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://kz.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://ko.colortex.cn

Ruby: arr.reverse
来源：http://iu.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://ik.szxytkj.cn

[D12] 查找元素下标
来源：http://fs.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://mh.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zv.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://et.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mz.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ci.colortex.cn

Go:   slices.Index(arr, x)
来源：http://bs.shtwfgs.cn

Ruby: arr.index(x)
来源：http://vg.colortex.cn

C#:   list.IndexOf(x);
来源：http://vi.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://cj.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aw.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zh.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://ed.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://oj.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gw.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ue.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mj.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yo.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://fr.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mj.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oe.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://pq.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://mq.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fu.bookmarksfly.cn

Go:   // 手写循环
来源：http://kq.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pe.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bz.szsharing.cn

[D15] 去重
来源：http://ba.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qx.szxytkj.cn

PHP:  array_unique($arr);
来源：http://vi.nszjky.cn

JS:   [...new Set(arr)]
来源：http://sw.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://ms.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yt.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ma.haigaiapp.cn

Ruby: arr.uniq
来源：http://dh.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://mw.panjiajie.cn

[D16] 求和与平均值
来源：http://ph.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nx.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iz.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://px.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bs.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xp.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://gq.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ox.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://oo.huixiangedu.cn

[D17] 最大值与最小值
来源：http://hr.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://ji.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://oj.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hm.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://ka.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qa.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gq.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://rn.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://ly.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://nk.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mk.asd995.cn

PHP:  array_merge(...$nested);
来源：http://ax.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kn.szsharing.cn

TS:   nested.flat();
来源：http://rf.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nr.chemitech.net.cn

Go:   // 手写双层循环
来源：http://so.newstarts.cn

Ruby: nested.flatten
来源：http://mw.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qt.shtwfgs.cn

[D19] 按字段分组
来源：http://nm.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oa.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cx.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zo.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bi.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yj.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://im.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bn.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jo.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://hr.nszjky.cn

Py:   Counter(arr)
来源：http://te.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://cc.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://np.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kf.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wa.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://ur.asd995.cn

Ruby: arr.tally
来源：http://ep.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fr.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://br.newstarts.cn

Py:   x in arr
来源：http://ab.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://oo.lnxyls.cn

JS:   arr.includes(x)
来源：http://qv.wgjwhj.cn

TS:   arr.includes(x)
来源：http://zq.newstarts.cn

Java: list.contains(x)
来源：http://jm.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://ot.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://tv.szsharing.cn

C#:   list.Contains(x)
来源：http://dc.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://ne.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ke.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zr.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://np.nicolike.cn

TS:   [...arr];
来源：http://gu.newstarts.cn

Java: new ArrayList<>(list);
来源：http://bo.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wg.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://qt.muxihuayi.cn

C#:   new List<int>(list);
来源：http://bp.asd995.cn

[D23] reduce 累积计算
来源：http://no.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ie.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dv.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ea.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ax.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tt.szsharing.cn

Go:   // 手写循环
来源：http://ru.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xm.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rg.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://sp.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rx.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hu.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xm.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qm.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nz.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mk.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cc.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://il.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://hv.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qn.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cd.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ce.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ax.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sc.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dr.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rm.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://de.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://cj.yuexingan06.cn


<!-- 参考信息 -->