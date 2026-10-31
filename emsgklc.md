代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bs.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vt.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ub.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fd.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://co.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xh.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rn.asd995.cn

[C09] 递归
来源：http://nz.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ya.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jz.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ta.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pr.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uk.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hw.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kv.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iy.newstarts.cn

[C10] 变量作用域
来源：http://jh.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ad.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://we.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jr.bjjhwx.cn

TS:   同 JS
来源：http://lp.szsharing.cn

Java: 方法内为块级作用域
来源：http://pq.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://sm.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://la.gzmigu.cn

C#:   块级作用域
来源：http://sz.nszjky.cn

[C11] 模块导入与导出
来源：http://ft.huixiangedu.cn

Py:   from module import func
来源：http://ih.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ht.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xt.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tg.huixinmuqiang.cn

Java: import java.util.List;
来源：http://lv.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tl.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://si.wgjwhj.cn

C#:   using System.Text;
来源：http://xe.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://ok.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://jf.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://yx.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://ga.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://yq.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tr.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ce.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ly.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jg.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://yt.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cy.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://he.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lr.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wq.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uo.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://dj.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ri.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mj.panjiajie.cn

[C14] 泛型函数
来源：http://wp.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xm.huanxung.cn

PHP:  // 无泛型
来源：http://rn.yuntaijiaju.cn

JS:   // 无泛型
来源：http://zt.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wr.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zn.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yh.jctech888.com.cn

Ruby: # 无泛型
来源：http://jy.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hq.nicolike.cn

[C15] 解构 / 展开参数
来源：http://jh.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ol.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://yh.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sl.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gt.shxzukj.cn

Java: // 无解构
来源：http://vp.hnjuh.cn

Go:   // 无解构
来源：http://cp.lnxyls.cn

Ruby: a, b = pair
来源：http://je.521024.cn

C#:   var (a, b) = pair;
来源：http://ry.szsharing.cn

[C16] 函数 / 方法重载
来源：http://nx.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rs.huanxung.cn

PHP:  // 无重载
来源：http://ju.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vb.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://po.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rp.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://cf.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://gg.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kh.jianghongdianzi.cn

================================================================================
来源：http://lz.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://sf.jctech888.com.cn

================================================================================
来源：http://pz.9csxet.cn

[D01] 创建数组 / 列表
来源：http://hb.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yu.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dp.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dg.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jq.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mz.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://xo.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://yi.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ny.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://th.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sq.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sh.szsharing.cn

JS:   arr.push(4);
来源：http://yy.521024.cn

TS:   arr.push(4);
来源：http://co.lnxyls.cn

Java: list.add(4);
来源：http://sw.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://iy.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://nv.shxzskj.cn

C#:   list.Add(4);
来源：http://qg.szsharing.cn

[D03] 在指定位置插入元素
来源：http://me.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://bf.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fi.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ur.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://op.szsharing.cn

Java: list.add(0, 0);
来源：http://cb.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mm.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jh.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://gd.colortex.cn

[D04] 删除元素
来源：http://wx.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kd.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ma.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oc.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://jz.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cb.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gc.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dh.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lr.asd995.cn

[D05] 访问与修改元素
来源：http://aj.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cr.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ps.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qv.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://xj.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://vm.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://al.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ow.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zl.szsharing.cn

[D06] 数组长度
来源：http://pm.huixiangedu.cn

Py:   len(arr)
来源：http://jx.panjiajie.cn

PHP:  count($arr);
来源：http://af.chemitech.net.cn

JS:   arr.length
来源：http://fb.nicolike.cn

TS:   arr.length
来源：http://io.9csxet.cn

Java: list.size();
来源：http://zm.huixiangedu.cn

Go:   len(arr)
来源：http://bh.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://yd.colortex.cn

C#:   list.Count;
来源：http://it.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://aq.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cl.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pv.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://gn.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://ns.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://gs.huixiangedu.cn

Go:   arr[1:4]
来源：http://ym.colortex.cn

Ruby: arr[1, 3]
来源：http://tn.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://tx.yuexingan06.cn

[D08] 合并两个数组
来源：http://mh.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://cd.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://fh.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oh.shxzukj.cn

TS:   [...a, ...b];
来源：http://zu.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://as.hahajie.cn

Go:   append(a, b...)
来源：http://mc.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://tc.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://ne.wgjwhj.cn

[D09] 排序（升序）
来源：http://dm.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://la.gzmigu.cn

PHP:  sort($arr);
来源：http://qg.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lb.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lq.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ld.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sp.gzmigu.cn

Ruby: arr.sort
来源：http://bb.haigaiapp.cn

C#:   list.Sort();
来源：http://vs.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mh.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wi.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://az.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pf.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nj.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zv.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kx.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fa.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://as.521024.cn

[D11] 反转数组
来源：http://eq.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hd.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://aa.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vf.huanxung.cn

TS:   [...arr].reverse();
来源：http://ko.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://qm.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://yx.szsharing.cn

Ruby: arr.reverse
来源：http://do.newstarts.cn

C#:   list.Reverse();
来源：http://vi.huixiangedu.cn

[D12] 查找元素下标
来源：http://kj.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://by.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dl.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ie.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dq.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ro.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://vl.jctech888.com.cn

Ruby: arr.index(x)
来源：http://sh.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://bn.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://xy.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xr.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://td.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://vw.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://tg.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sy.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gs.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bl.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hr.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://yz.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ux.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dx.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://ku.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://ry.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sy.shtwfgs.cn

Go:   // 手写循环
来源：http://fl.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xo.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://go.szsharing.cn

[D15] 去重
来源：http://jj.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qg.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://dn.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://ha.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://qy.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tr.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uh.huanxung.cn

Ruby: arr.uniq
来源：http://jh.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://ud.huanxung.cn

[D16] 求和与平均值
来源：http://mx.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rl.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qu.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ub.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ly.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nh.gzmigu.cn

Go:   // 手写循环累加
来源：http://of.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://of.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://zd.asd995.cn

[D17] 最大值与最小值
来源：http://tz.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://vp.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://un.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gr.shxzskj.cn

TS:   Math.max(...arr);
来源：http://zh.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ch.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cp.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://lu.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://si.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://lk.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yf.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://az.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gf.521024.cn

TS:   nested.flat();
来源：http://il.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://je.colortex.cn

Go:   // 手写双层循环
来源：http://db.nicolike.cn

Ruby: nested.flatten
来源：http://vn.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qu.521024.cn

[D19] 按字段分组
来源：http://qk.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mt.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ms.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wp.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tj.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mv.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://aa.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jl.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ig.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://jn.gzmigu.cn

Py:   Counter(arr)
来源：http://xi.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://na.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gx.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xh.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vp.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://hg.panjiajie.cn

Ruby: arr.tally
来源：http://li.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zg.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://so.huixiangedu.cn

Py:   x in arr
来源：http://ke.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://he.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://lm.huanxung.cn

TS:   arr.includes(x)
来源：http://io.shxzskj.cn

Java: list.contains(x)
来源：http://cg.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://qs.colortex.cn

Ruby: arr.include?(x)
来源：http://pw.gzmigu.cn

C#:   list.Contains(x)
来源：http://tq.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://yu.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fg.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qj.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nm.colortex.cn

TS:   [...arr];
来源：http://ix.hahajie.cn

Java: new ArrayList<>(list);
来源：http://wi.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lq.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://od.gzmigu.cn

C#:   new List<int>(list);
来源：http://fq.jctech888.com.cn

[D23] reduce 累积计算
来源：http://zy.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sf.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://so.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oj.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lc.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ka.9csxet.cn

Go:   // 手写循环
来源：http://vi.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fo.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rz.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://pt.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eo.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gg.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ar.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mm.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mf.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pg.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vc.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hl.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://vl.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zd.jianghongdianzi.cn


<!-- 参考信息 -->