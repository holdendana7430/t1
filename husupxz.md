代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ed.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sv.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sm.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oh.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sx.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wl.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tk.szxytkj.cn

[C09] 递归
来源：http://av.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pl.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jl.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hm.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nt.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mo.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://or.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pz.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kw.wgjwhj.cn

[C10] 变量作用域
来源：http://yl.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bd.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qf.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ie.newstarts.cn

TS:   同 JS
来源：http://mc.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://aa.colortex.cn

Go:   花括号块级作用域
来源：http://xw.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://en.gzmigu.cn

C#:   块级作用域
来源：http://xr.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://uy.nicolike.cn

Py:   from module import func
来源：http://at.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xo.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dk.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eg.jctech888.com.cn

Java: import java.util.List;
来源：http://yu.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rx.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://bx.yuntaijiaju.cn

C#:   using System.Text;
来源：http://bm.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://aw.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://pd.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://oy.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://uk.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://wd.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wz.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://fx.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://lw.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xs.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://um.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tv.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ec.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gu.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xf.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qv.9csxet.cn

Go:   func add(a, b int) int
来源：http://tp.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zx.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bg.bookmarksfly.cn

[C14] 泛型函数
来源：http://ue.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ty.gzmigu.cn

PHP:  // 无泛型
来源：http://nr.shxzskj.cn

JS:   // 无泛型
来源：http://rn.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tz.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ex.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wy.nszjky.cn

Ruby: # 无泛型
来源：http://ib.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gn.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://ju.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://na.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://so.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://br.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://om.huanxung.cn

Java: // 无解构
来源：http://np.szsharing.cn

Go:   // 无解构
来源：http://nc.newstarts.cn

Ruby: a, b = pair
来源：http://pf.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://uk.newstarts.cn

[C16] 函数 / 方法重载
来源：http://mg.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uc.colortex.cn

PHP:  // 无重载
来源：http://hb.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sq.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://lk.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://st.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://hc.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://az.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cd.shtwfgs.cn

================================================================================
来源：http://nw.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://fy.521024.cn

================================================================================
来源：http://yv.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://md.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://np.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://at.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gu.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pk.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bw.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://zq.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://lm.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://il.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://ue.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mt.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lk.shtwfgs.cn

JS:   arr.push(4);
来源：http://dd.lnxyls.cn

TS:   arr.push(4);
来源：http://rn.bjjhwx.cn

Java: list.add(4);
来源：http://im.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://qx.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://rw.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://ok.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://zp.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://bz.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ge.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ie.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ik.huixiangedu.cn

Java: list.add(0, 0);
来源：http://op.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pw.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bb.colortex.cn

C#:   list.Insert(0, 0);
来源：http://fm.huixinmuqiang.cn

[D04] 删除元素
来源：http://pf.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fo.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ve.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hk.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://in.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qb.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xp.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xj.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vs.asd995.cn

[D05] 访问与修改元素
来源：http://lu.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wu.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://va.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xl.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://fo.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://er.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ee.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bb.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yw.chemitech.net.cn

[D06] 数组长度
来源：http://hj.521024.cn

Py:   len(arr)
来源：http://re.muxihuayi.cn

PHP:  count($arr);
来源：http://vd.chemitech.net.cn

JS:   arr.length
来源：http://je.huixinmuqiang.cn

TS:   arr.length
来源：http://cz.panjiajie.cn

Java: list.size();
来源：http://ab.9csxet.cn

Go:   len(arr)
来源：http://ds.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://ql.gzmigu.cn

C#:   list.Count;
来源：http://dl.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://gs.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://is.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yf.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://sc.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://lw.9csxet.cn

Java: list.subList(1, 4);
来源：http://ii.bjjhwx.cn

Go:   arr[1:4]
来源：http://np.szxytkj.cn

Ruby: arr[1, 3]
来源：http://dv.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://ag.gzmigu.cn

[D08] 合并两个数组
来源：http://ku.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://np.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://wa.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xv.nicolike.cn

TS:   [...a, ...b];
来源：http://lz.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://th.asd995.cn

Go:   append(a, b...)
来源：http://zy.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://zq.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://im.szsharing.cn

[D09] 排序（升序）
来源：http://jo.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://pg.bookmarksfly.cn

PHP:  sort($arr);
来源：http://gy.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ls.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lt.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://np.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ll.panjiajie.cn

Ruby: arr.sort
来源：http://tq.nicolike.cn

C#:   list.Sort();
来源：http://pt.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qy.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://en.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uo.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kn.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xg.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kv.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fp.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eq.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jq.jctech888.com.cn

[D11] 反转数组
来源：http://yv.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wg.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://cz.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nc.szxytkj.cn

TS:   [...arr].reverse();
来源：http://ri.shxzukj.cn

Java: Collections.reverse(list);
来源：http://tb.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://ly.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://bo.muxihuayi.cn

C#:   list.Reverse();
来源：http://cm.jctech888.com.cn

[D12] 查找元素下标
来源：http://pw.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://lj.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pw.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jj.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qn.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gt.colortex.cn

Go:   slices.Index(arr, x)
来源：http://mw.szsharing.cn

Ruby: arr.index(x)
来源：http://qf.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://en.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://gj.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rw.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lq.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://bi.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://vn.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xe.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ra.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://on.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wf.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://tk.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kz.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kj.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://um.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://la.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yg.newstarts.cn

Go:   // 手写循环
来源：http://xl.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://de.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tm.9csxet.cn

[D15] 去重
来源：http://re.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gr.nszjky.cn

PHP:  array_unique($arr);
来源：http://sh.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://mf.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://rg.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gx.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iv.huanxung.cn

Ruby: arr.uniq
来源：http://ur.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://pr.newstarts.cn

[D16] 求和与平均值
来源：http://eg.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nz.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gy.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ie.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lt.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fo.szxytkj.cn

Go:   // 手写循环累加
来源：http://hu.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rw.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://nd.wgjwhj.cn

[D17] 最大值与最小值
来源：http://se.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://jp.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://rr.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kf.nicolike.cn

TS:   Math.max(...arr);
来源：http://wn.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cc.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pq.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://pw.asd995.cn

C#:   list.Max();  list.Min()
来源：http://yb.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://am.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qu.521024.cn

PHP:  array_merge(...$nested);
来源：http://jc.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fc.chemitech.net.cn

TS:   nested.flat();
来源：http://sm.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cy.huixiangedu.cn

Go:   // 手写双层循环
来源：http://fg.shxzukj.cn

Ruby: nested.flatten
来源：http://fb.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gk.yuexingan06.cn

[D19] 按字段分组
来源：http://yp.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zm.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kz.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://um.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://na.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sz.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://nl.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mw.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oh.colortex.cn

[D20] 统计每个元素出现次数
来源：http://lq.huanxung.cn

Py:   Counter(arr)
来源：http://jc.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://uj.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xs.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qr.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://km.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://el.huanxung.cn

Ruby: arr.tally
来源：http://jw.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://or.szsharing.cn

[D21] 判断是否包含某元素
来源：http://sb.shxzukj.cn

Py:   x in arr
来源：http://ah.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://ax.asd995.cn

JS:   arr.includes(x)
来源：http://wg.hahajie.cn

TS:   arr.includes(x)
来源：http://og.muxihuayi.cn

Java: list.contains(x)
来源：http://ad.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://gi.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://dp.shxzskj.cn

C#:   list.Contains(x)
来源：http://uf.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://pm.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jb.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ye.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nr.lnxyls.cn

TS:   [...arr];
来源：http://xu.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://ti.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://th.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://uq.jctech888.com.cn

C#:   new List<int>(list);
来源：http://ue.bjjhwx.cn

[D23] reduce 累积计算
来源：http://je.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jl.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yz.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xd.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lr.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rq.9csxet.cn

Go:   // 手写循环
来源：http://gt.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ev.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xa.521024.cn

[D24] 字典 / Map 基本操作
来源：http://os.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nh.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qg.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://om.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sm.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mj.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ou.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oy.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kq.521024.cn

[D25] Set 集合去重与交并差
来源：http://pv.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yf.9csxet.cn


<!-- 参考信息 -->