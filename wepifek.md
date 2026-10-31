代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fb.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kp.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ti.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rk.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zh.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ie.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fv.colortex.cn

[C09] 递归
来源：http://lo.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ud.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cx.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://we.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://de.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://se.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jz.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://il.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vf.hahajie.cn

[C10] 变量作用域
来源：http://ss.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cg.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fz.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://in.gzmigu.cn

TS:   同 JS
来源：http://gq.szxytkj.cn

Java: 方法内为块级作用域
来源：http://nz.chemitech.net.cn

Go:   花括号块级作用域
来源：http://ay.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pe.nszjky.cn

C#:   块级作用域
来源：http://au.521024.cn

[C11] 模块导入与导出
来源：http://wt.huixiangedu.cn

Py:   from module import func
来源：http://qq.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ie.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://su.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dr.hnjuh.cn

Java: import java.util.List;
来源：http://vs.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sg.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://mf.shxzskj.cn

C#:   using System.Text;
来源：http://dw.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://ij.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://nt.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://ph.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://zq.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://bu.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mx.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://ns.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://sj.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://no.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://si.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vy.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://au.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ax.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gm.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fs.nicolike.cn

Go:   func add(a, b int) int
来源：http://iu.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ed.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lt.huanxung.cn

[C14] 泛型函数
来源：http://yg.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ao.hnjuh.cn

PHP:  // 无泛型
来源：http://ql.wgjwhj.cn

JS:   // 无泛型
来源：http://td.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ih.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jg.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://am.huanxung.cn

Ruby: # 无泛型
来源：http://so.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wm.nszjky.cn

[C15] 解构 / 展开参数
来源：http://ud.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pq.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://kp.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://du.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vc.nszjky.cn

Java: // 无解构
来源：http://mz.hahajie.cn

Go:   // 无解构
来源：http://dx.huixiangedu.cn

Ruby: a, b = pair
来源：http://xr.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://oy.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://gd.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qp.bjjhwx.cn

PHP:  // 无重载
来源：http://ub.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rm.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://vg.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rs.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://td.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://lr.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ow.gzmigu.cn

================================================================================
来源：http://ua.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://xq.jctech888.com.cn

================================================================================
来源：http://uq.asd995.cn

[D01] 创建数组 / 列表
来源：http://qy.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cj.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://on.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://la.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oh.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://re.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://xz.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://pq.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wx.nicolike.cn

[D02] 追加元素到末尾
来源：http://rt.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dz.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ag.hahajie.cn

JS:   arr.push(4);
来源：http://xz.panjiajie.cn

TS:   arr.push(4);
来源：http://il.huixinmuqiang.cn

Java: list.add(4);
来源：http://sd.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://hi.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://or.jctech888.com.cn

C#:   list.Add(4);
来源：http://dl.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://tt.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://ap.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vi.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tf.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://dc.muxihuayi.cn

Java: list.add(0, 0);
来源：http://ru.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zy.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xn.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://hh.huixinmuqiang.cn

[D04] 删除元素
来源：http://dk.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qe.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fg.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nf.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://br.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jv.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ls.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vt.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ks.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://sz.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fs.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ud.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mj.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://xs.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://sx.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://la.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bo.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pi.szsharing.cn

[D06] 数组长度
来源：http://pk.bookmarksfly.cn

Py:   len(arr)
来源：http://kb.lnxyls.cn

PHP:  count($arr);
来源：http://hm.yuntaijiaju.cn

JS:   arr.length
来源：http://wa.huanxung.cn

TS:   arr.length
来源：http://ya.lnxyls.cn

Java: list.size();
来源：http://pb.szxytkj.cn

Go:   len(arr)
来源：http://if.hahajie.cn

Ruby: arr.length; arr.size
来源：http://qu.huixiangedu.cn

C#:   list.Count;
来源：http://hk.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://hg.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sx.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://er.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://nm.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://ik.panjiajie.cn

Java: list.subList(1, 4);
来源：http://ip.shxzukj.cn

Go:   arr[1:4]
来源：http://nl.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://kn.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://tf.szsharing.cn

[D08] 合并两个数组
来源：http://ds.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://rz.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://wm.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pq.hahajie.cn

TS:   [...a, ...b];
来源：http://ej.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ye.bjjhwx.cn

Go:   append(a, b...)
来源：http://oj.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://zd.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://de.huixiangedu.cn

[D09] 排序（升序）
来源：http://en.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://xk.hnjuh.cn

PHP:  sort($arr);
来源：http://dj.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gb.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hj.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qi.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lc.newstarts.cn

Ruby: arr.sort
来源：http://bq.haigaiapp.cn

C#:   list.Sort();
来源：http://wk.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vz.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nq.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xf.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bv.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dm.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lz.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ll.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cg.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jr.shtwfgs.cn

[D11] 反转数组
来源：http://lo.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xh.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://pt.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tm.hahajie.cn

TS:   [...arr].reverse();
来源：http://vz.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://uy.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://cd.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://ij.asd995.cn

C#:   list.Reverse();
来源：http://ls.haigaiapp.cn

[D12] 查找元素下标
来源：http://ez.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://vd.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gz.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ra.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iw.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qu.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://zl.hahajie.cn

Ruby: arr.index(x)
来源：http://kl.colortex.cn

C#:   list.IndexOf(x);
来源：http://cj.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://yu.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yk.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zl.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://gs.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://yv.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yk.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ob.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qs.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ce.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://fd.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wx.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hw.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://wg.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://rf.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lk.huanxung.cn

Go:   // 手写循环
来源：http://nu.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cp.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hu.colortex.cn

[D15] 去重
来源：http://gq.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uk.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://qp.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://li.9csxet.cn

TS:   [...new Set(arr)]
来源：http://qc.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fy.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ur.newstarts.cn

Ruby: arr.uniq
来源：http://wb.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://wi.wgjwhj.cn

[D16] 求和与平均值
来源：http://no.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qa.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nt.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cl.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rb.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tm.szxytkj.cn

Go:   // 手写循环累加
来源：http://ph.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sm.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://wn.huixiangedu.cn

[D17] 最大值与最小值
来源：http://vu.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://ge.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://sc.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xg.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://ex.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qf.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ud.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://xq.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://ed.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://cg.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lj.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://rd.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://og.bjjhwx.cn

TS:   nested.flat();
来源：http://hq.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gh.shxzskj.cn

Go:   // 手写双层循环
来源：http://my.shtwfgs.cn

Ruby: nested.flatten
来源：http://nr.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ww.colortex.cn

[D19] 按字段分组
来源：http://cj.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fp.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gt.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qm.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://am.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dy.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://iu.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fm.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ni.colortex.cn

[D20] 统计每个元素出现次数
来源：http://ah.nszjky.cn

Py:   Counter(arr)
来源：http://oc.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://qw.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wk.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cc.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://om.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://it.yuexingan06.cn

Ruby: arr.tally
来源：http://mj.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hm.huanxung.cn

[D21] 判断是否包含某元素
来源：http://wt.9csxet.cn

Py:   x in arr
来源：http://qh.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://ga.521024.cn

JS:   arr.includes(x)
来源：http://vk.szsharing.cn

TS:   arr.includes(x)
来源：http://lv.huixinmuqiang.cn

Java: list.contains(x)
来源：http://by.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://gi.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://bo.colortex.cn

C#:   list.Contains(x)
来源：http://dg.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://ys.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lh.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mm.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uo.szsharing.cn

TS:   [...arr];
来源：http://aw.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://wd.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ob.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://ij.asd995.cn

C#:   new List<int>(list);
来源：http://uv.bjjhwx.cn

[D23] reduce 累积计算
来源：http://yt.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://op.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kd.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qs.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wh.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gl.nicolike.cn

Go:   // 手写循环
来源：http://mr.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://db.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iw.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://kl.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hw.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hv.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lh.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://id.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bx.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ao.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fv.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qs.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://wz.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://no.yuexingan06.cn


<!-- 参考信息 -->