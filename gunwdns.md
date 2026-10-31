代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pw.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pq.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://am.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ry.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lk.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hf.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zr.jianghongdianzi.cn

[C09] 递归
来源：http://vn.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://up.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lv.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vx.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pa.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cm.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ub.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gb.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uj.huanxung.cn

[C10] 变量作用域
来源：http://wz.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oj.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ki.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iy.asd995.cn

TS:   同 JS
来源：http://gs.hahajie.cn

Java: 方法内为块级作用域
来源：http://nm.shtwfgs.cn

Go:   花括号块级作用域
来源：http://ip.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yq.huanxung.cn

C#:   块级作用域
来源：http://hy.szxytkj.cn

[C11] 模块导入与导出
来源：http://zi.szsharing.cn

Py:   from module import func
来源：http://so.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sr.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cs.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uk.521024.cn

Java: import java.util.List;
来源：http://ml.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vz.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://an.gzmigu.cn

C#:   using System.Text;
来源：http://wy.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://xd.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://rk.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://nr.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://rt.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://dc.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kp.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://cz.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://nt.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bz.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://vy.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kt.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://db.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ge.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nr.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fl.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ov.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xe.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://px.gzmigu.cn

[C14] 泛型函数
来源：http://bj.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://it.muxihuayi.cn

PHP:  // 无泛型
来源：http://qf.huixiangedu.cn

JS:   // 无泛型
来源：http://bp.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jh.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xk.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fw.asd995.cn

Ruby: # 无泛型
来源：http://fm.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qu.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://ah.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://so.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://wh.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://of.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cg.bookmarksfly.cn

Java: // 无解构
来源：http://kp.9csxet.cn

Go:   // 无解构
来源：http://rs.huixiangedu.cn

Ruby: a, b = pair
来源：http://lt.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://et.hahajie.cn

[C16] 函数 / 方法重载
来源：http://lh.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nm.wgjwhj.cn

PHP:  // 无重载
来源：http://je.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ei.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ml.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ye.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://hz.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://ve.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xm.asd995.cn

================================================================================
来源：http://rc.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://mo.nicolike.cn

================================================================================
来源：http://fe.asd995.cn

[D01] 创建数组 / 列表
来源：http://xf.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ns.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wo.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qx.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nj.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ub.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://lf.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://hp.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rp.shxzukj.cn

[D02] 追加元素到末尾
来源：http://me.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ty.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yw.newstarts.cn

JS:   arr.push(4);
来源：http://ix.szxytkj.cn

TS:   arr.push(4);
来源：http://vb.huixinmuqiang.cn

Java: list.add(4);
来源：http://rf.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://ma.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://mf.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://mp.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://zt.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://rg.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ip.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bl.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://zp.szxytkj.cn

Java: list.add(0, 0);
来源：http://em.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sn.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ae.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://ww.yuexingan06.cn

[D04] 删除元素
来源：http://ko.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ta.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://au.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qu.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://qe.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kr.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jb.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iv.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mw.panjiajie.cn

[D05] 访问与修改元素
来源：http://mc.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jx.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yw.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vy.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://jv.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://iq.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ly.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://za.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dr.newstarts.cn

[D06] 数组长度
来源：http://no.colortex.cn

Py:   len(arr)
来源：http://ps.lnxyls.cn

PHP:  count($arr);
来源：http://iv.bjjhwx.cn

JS:   arr.length
来源：http://hp.jctech888.com.cn

TS:   arr.length
来源：http://fn.colortex.cn

Java: list.size();
来源：http://rw.szxytkj.cn

Go:   len(arr)
来源：http://jg.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://dt.colortex.cn

C#:   list.Count;
来源：http://yq.nszjky.cn

[D07] 切片 / 取子数组
来源：http://ct.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://me.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iu.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://yj.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://ff.gzmigu.cn

Java: list.subList(1, 4);
来源：http://bo.nicolike.cn

Go:   arr[1:4]
来源：http://dd.gzmigu.cn

Ruby: arr[1, 3]
来源：http://rj.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://lv.wgjwhj.cn

[D08] 合并两个数组
来源：http://rt.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://as.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://gi.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sy.muxihuayi.cn

TS:   [...a, ...b];
来源：http://kw.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://er.shxzukj.cn

Go:   append(a, b...)
来源：http://sq.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://rv.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://hu.nszjky.cn

[D09] 排序（升序）
来源：http://nv.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://kp.lnxyls.cn

PHP:  sort($arr);
来源：http://tf.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fp.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yd.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://in.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qb.shxzukj.cn

Ruby: arr.sort
来源：http://wc.szxytkj.cn

C#:   list.Sort();
来源：http://ee.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://op.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qk.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kk.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://or.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vs.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ac.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rs.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sy.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ob.szxytkj.cn

[D11] 反转数组
来源：http://vw.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rg.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://ou.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nq.shxzukj.cn

TS:   [...arr].reverse();
来源：http://by.colortex.cn

Java: Collections.reverse(list);
来源：http://iv.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://yv.wgjwhj.cn

Ruby: arr.reverse
来源：http://bx.asd995.cn

C#:   list.Reverse();
来源：http://xu.521024.cn

[D12] 查找元素下标
来源：http://eb.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://bn.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zl.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zp.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mg.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://el.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://uz.gzmigu.cn

Ruby: arr.index(x)
来源：http://ng.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://tw.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://ju.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zb.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fa.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://lq.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://sy.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tn.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://td.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nu.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qs.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://vo.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hh.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lg.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://xc.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://ce.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dg.hahajie.cn

Go:   // 手写循环
来源：http://vv.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ye.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ey.szxytkj.cn

[D15] 去重
来源：http://lv.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xh.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://os.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://kl.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://dv.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mu.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wu.jctech888.com.cn

Ruby: arr.uniq
来源：http://kp.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://oa.9csxet.cn

[D16] 求和与平均值
来源：http://pd.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uy.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oj.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qk.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kk.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eb.asd995.cn

Go:   // 手写循环累加
来源：http://zc.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bd.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://hb.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://pp.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://te.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://kf.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qv.shxzukj.cn

TS:   Math.max(...arr);
来源：http://wc.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gp.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kd.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://do.asd995.cn

C#:   list.Max();  list.Min()
来源：http://dt.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://iq.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wi.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://vt.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ul.chemitech.net.cn

TS:   nested.flat();
来源：http://xo.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cm.nszjky.cn

Go:   // 手写双层循环
来源：http://qt.gzmigu.cn

Ruby: nested.flatten
来源：http://um.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ya.jianghongdianzi.cn

[D19] 按字段分组
来源：http://ua.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ks.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gv.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zn.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wu.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vg.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://pf.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gv.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mx.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://ux.newstarts.cn

Py:   Counter(arr)
来源：http://oi.nszjky.cn

PHP:  array_count_values($arr);
来源：http://bq.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://re.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iv.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cy.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://tv.panjiajie.cn

Ruby: arr.tally
来源：http://vz.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dr.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://ui.gzmigu.cn

Py:   x in arr
来源：http://px.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://hm.colortex.cn

JS:   arr.includes(x)
来源：http://mu.huanxung.cn

TS:   arr.includes(x)
来源：http://yr.huixinmuqiang.cn

Java: list.contains(x)
来源：http://mc.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://vm.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://xi.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://it.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://nz.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qh.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pc.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qm.shxzukj.cn

TS:   [...arr];
来源：http://jb.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://su.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pv.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://oy.huixiangedu.cn

C#:   new List<int>(list);
来源：http://cj.bjjhwx.cn

[D23] reduce 累积计算
来源：http://lv.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xi.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iy.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://je.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://re.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://na.shxzskj.cn

Go:   // 手写循环
来源：http://uz.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fn.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vr.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://uh.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ju.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gx.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bk.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oi.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bq.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yz.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xi.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://se.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://ok.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bm.wgjwhj.cn


<!-- 参考信息 -->