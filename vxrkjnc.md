代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://qq.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sr.szxytkj.cn

[C08] 闭包
来源：http://ah.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qs.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fw.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://es.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sm.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ml.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sg.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xd.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://as.newstarts.cn

[C09] 递归
来源：http://eg.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sl.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qf.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://al.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qc.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gr.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oz.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ob.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oh.hnjuh.cn

[C10] 变量作用域
来源：http://kv.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://di.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://at.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vs.muxihuayi.cn

TS:   同 JS
来源：http://dn.colortex.cn

Java: 方法内为块级作用域
来源：http://qm.jctech888.com.cn

Go:   花括号块级作用域
来源：http://op.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kw.wgjwhj.cn

C#:   块级作用域
来源：http://da.shxzskj.cn

[C11] 模块导入与导出
来源：http://vn.bookmarksfly.cn

Py:   from module import func
来源：http://oa.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xm.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yc.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ac.bookmarksfly.cn

Java: import java.util.List;
来源：http://ci.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ya.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://jd.hahajie.cn

C#:   using System.Text;
来源：http://wf.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://ng.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://oi.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://tv.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://dc.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://mc.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tl.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://gi.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://ah.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ui.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://uj.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sm.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bf.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gx.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eb.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ih.panjiajie.cn

Go:   func add(a, b int) int
来源：http://jm.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rq.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fw.huanxung.cn

[C14] 泛型函数
来源：http://wr.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dl.newstarts.cn

PHP:  // 无泛型
来源：http://xe.panjiajie.cn

JS:   // 无泛型
来源：http://vh.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nu.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gd.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ja.shtwfgs.cn

Ruby: # 无泛型
来源：http://xr.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wn.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://px.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ng.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://mo.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mg.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pd.shxzukj.cn

Java: // 无解构
来源：http://ig.shtwfgs.cn

Go:   // 无解构
来源：http://cc.bookmarksfly.cn

Ruby: a, b = pair
来源：http://uj.9csxet.cn

C#:   var (a, b) = pair;
来源：http://jl.colortex.cn

[C16] 函数 / 方法重载
来源：http://kt.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ag.hnjuh.cn

PHP:  // 无重载
来源：http://lh.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ju.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://vl.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nh.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://lh.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://ya.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zn.newstarts.cn

================================================================================
来源：http://hr.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://gx.jianghongdianzi.cn

================================================================================
来源：http://ab.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://ju.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bl.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zv.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://et.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sc.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sm.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://uo.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://mu.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kt.colortex.cn

[D02] 追加元素到末尾
来源：http://zn.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ny.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lr.521024.cn

JS:   arr.push(4);
来源：http://kn.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://ri.521024.cn

Java: list.add(4);
来源：http://jd.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://tl.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://ff.panjiajie.cn

C#:   list.Add(4);
来源：http://ss.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://al.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://xo.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cg.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wh.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://dh.colortex.cn

Java: list.add(0, 0);
来源：http://uu.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ie.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ps.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://ze.asd995.cn

[D04] 删除元素
来源：http://nf.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sz.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cw.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://wu.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uq.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://be.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://px.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bo.shtwfgs.cn

[D05] 访问与修改元素
来源：http://ew.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ba.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bq.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sb.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://xn.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://pz.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://ar.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xa.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gz.szsharing.cn

[D06] 数组长度
来源：http://xy.yuntaijiaju.cn

Py:   len(arr)
来源：http://rl.9csxet.cn

PHP:  count($arr);
来源：http://be.gzmigu.cn

JS:   arr.length
来源：http://km.nszjky.cn

TS:   arr.length
来源：http://qy.jctech888.com.cn

Java: list.size();
来源：http://dg.muxihuayi.cn

Go:   len(arr)
来源：http://wa.szsharing.cn

Ruby: arr.length; arr.size
来源：http://dh.szxytkj.cn

C#:   list.Count;
来源：http://uw.newstarts.cn

[D07] 切片 / 取子数组
来源：http://ue.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rc.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wr.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://ht.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://ki.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://vm.huixiangedu.cn

Go:   arr[1:4]
来源：http://uo.shxzskj.cn

Ruby: arr[1, 3]
来源：http://gt.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://wu.newstarts.cn

[D08] 合并两个数组
来源：http://cj.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://qm.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://bt.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uz.jctech888.com.cn

TS:   [...a, ...b];
来源：http://co.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sa.colortex.cn

Go:   append(a, b...)
来源：http://iq.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://jh.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://nk.chemitech.net.cn

[D09] 排序（升序）
来源：http://ti.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://sa.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://tx.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://up.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xp.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://is.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ht.yuexingan06.cn

Ruby: arr.sort
来源：http://kk.521024.cn

C#:   list.Sort();
来源：http://tj.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ud.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sm.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wq.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hy.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rh.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yw.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oe.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yu.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rn.hahajie.cn

[D11] 反转数组
来源：http://bp.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uc.huanxung.cn

PHP:  array_reverse($arr);
来源：http://se.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xx.shxzukj.cn

TS:   [...arr].reverse();
来源：http://oc.newstarts.cn

Java: Collections.reverse(list);
来源：http://di.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://fq.lnxyls.cn

Ruby: arr.reverse
来源：http://pb.szxytkj.cn

C#:   list.Reverse();
来源：http://qq.shxzskj.cn

[D12] 查找元素下标
来源：http://ty.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://uj.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ne.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gu.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iy.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eo.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://zs.newstarts.cn

Ruby: arr.index(x)
来源：http://qq.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://dv.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://sd.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iz.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nj.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://tt.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://eo.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qq.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jg.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hg.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mt.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://hm.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jk.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ip.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://cj.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://rf.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sl.shxzukj.cn

Go:   // 手写循环
来源：http://dn.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hl.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nw.huixiangedu.cn

[D15] 去重
来源：http://bu.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gn.huanxung.cn

PHP:  array_unique($arr);
来源：http://kq.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://cf.huanxung.cn

TS:   [...new Set(arr)]
来源：http://na.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nx.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ag.muxihuayi.cn

Ruby: arr.uniq
来源：http://to.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://jn.szsharing.cn

[D16] 求和与平均值
来源：http://rd.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hk.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yh.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gf.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xk.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ro.newstarts.cn

Go:   // 手写循环累加
来源：http://js.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xh.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://xf.panjiajie.cn

[D17] 最大值与最小值
来源：http://vi.521024.cn

Py:   max(arr);  min(arr)
来源：http://bl.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://xr.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rw.nicolike.cn

TS:   Math.max(...arr);
来源：http://gv.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ub.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fx.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://vc.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://zj.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://jg.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tm.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://cw.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wf.bookmarksfly.cn

TS:   nested.flat();
来源：http://dy.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ix.huixiangedu.cn

Go:   // 手写双层循环
来源：http://mh.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://sw.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vn.lnxyls.cn

[D19] 按字段分组
来源：http://sx.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rd.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qn.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lh.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pp.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ts.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://ly.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://df.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fe.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://tv.nszjky.cn

Py:   Counter(arr)
来源：http://zz.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://kq.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rv.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ju.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gi.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://dp.asd995.cn

Ruby: arr.tally
来源：http://ln.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gm.hahajie.cn

[D21] 判断是否包含某元素
来源：http://ey.jctech888.com.cn

Py:   x in arr
来源：http://xe.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://oh.lnxyls.cn

JS:   arr.includes(x)
来源：http://yg.newstarts.cn

TS:   arr.includes(x)
来源：http://ce.yuntaijiaju.cn

Java: list.contains(x)
来源：http://ox.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://vk.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://nx.nszjky.cn

C#:   list.Contains(x)
来源：http://rk.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://xo.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uh.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ft.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dl.521024.cn

TS:   [...arr];
来源：http://go.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://er.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://af.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://lt.wgjwhj.cn

C#:   new List<int>(list);
来源：http://us.bjjhwx.cn

[D23] reduce 累积计算
来源：http://gg.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wk.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ii.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cp.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tz.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vs.yuexingan06.cn

Go:   // 手写循环
来源：http://cv.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ft.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pm.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://xp.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sf.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cr.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ga.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://og.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ce.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ae.jctech888.com.cn


<!-- 参考信息 -->