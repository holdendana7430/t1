代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sl.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oy.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hg.huixinmuqiang.cn

[C09] 递归
来源：http://zk.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://av.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ij.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ap.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ex.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qt.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ag.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hu.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wq.panjiajie.cn

[C10] 变量作用域
来源：http://ug.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xo.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://js.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tz.muxihuayi.cn

TS:   同 JS
来源：http://fe.newstarts.cn

Java: 方法内为块级作用域
来源：http://ci.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://nn.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://we.yuexingan06.cn

C#:   块级作用域
来源：http://ou.haigaiapp.cn

[C11] 模块导入与导出
来源：http://gm.jctech888.com.cn

Py:   from module import func
来源：http://sm.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rd.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xv.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ho.haigaiapp.cn

Java: import java.util.List;
来源：http://sj.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dq.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://ba.gzmigu.cn

C#:   using System.Text;
来源：http://yt.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://ru.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://bp.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://dl.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://tr.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://tt.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sk.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://uw.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://xk.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vr.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://gx.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://no.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xd.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://na.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wm.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xt.hnjuh.cn

Go:   func add(a, b int) int
来源：http://mo.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hw.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jn.huixiangedu.cn

[C14] 泛型函数
来源：http://fo.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ls.colortex.cn

PHP:  // 无泛型
来源：http://cu.szsharing.cn

JS:   // 无泛型
来源：http://up.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://og.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jw.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jx.haigaiapp.cn

Ruby: # 无泛型
来源：http://gy.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lp.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://sa.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sn.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://yb.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://io.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rz.nszjky.cn

Java: // 无解构
来源：http://id.shxzskj.cn

Go:   // 无解构
来源：http://mg.szsharing.cn

Ruby: a, b = pair
来源：http://fo.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://za.hahajie.cn

[C16] 函数 / 方法重载
来源：http://qg.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sj.shxzukj.cn

PHP:  // 无重载
来源：http://oe.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cw.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://bt.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tv.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://fz.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://sl.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rn.yuexingan06.cn

================================================================================
来源：http://yl.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://na.521024.cn

================================================================================
来源：http://zn.szsharing.cn

[D01] 创建数组 / 列表
来源：http://vn.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vy.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zt.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rt.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lb.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bn.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://ak.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://dq.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ol.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://uo.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hp.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mo.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://vi.nszjky.cn

TS:   arr.push(4);
来源：http://rm.huixiangedu.cn

Java: list.add(4);
来源：http://rt.521024.cn

Go:   arr = append(arr, 4)
来源：http://qu.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://km.colortex.cn

C#:   list.Add(4);
来源：http://oj.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://ei.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://kk.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yl.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://so.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://tv.muxihuayi.cn

Java: list.add(0, 0);
来源：http://yd.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gk.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mx.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://xp.szsharing.cn

[D04] 删除元素
来源：http://jp.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jk.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rl.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ek.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://le.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vc.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ou.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hb.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cc.shtwfgs.cn

[D05] 访问与修改元素
来源：http://un.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://am.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jz.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://la.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://fe.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://zi.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://yj.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cs.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://es.hahajie.cn

[D06] 数组长度
来源：http://du.huixiangedu.cn

Py:   len(arr)
来源：http://mp.shxzskj.cn

PHP:  count($arr);
来源：http://od.wgjwhj.cn

JS:   arr.length
来源：http://rr.nszjky.cn

TS:   arr.length
来源：http://vj.muxihuayi.cn

Java: list.size();
来源：http://th.shtwfgs.cn

Go:   len(arr)
来源：http://kf.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://dt.wgjwhj.cn

C#:   list.Count;
来源：http://ss.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://fm.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ev.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jj.colortex.cn

JS:   arr.slice(1, 4);
来源：http://ou.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://xo.shxzskj.cn

Java: list.subList(1, 4);
来源：http://ru.shxzukj.cn

Go:   arr[1:4]
来源：http://lt.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://kv.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://ke.panjiajie.cn

[D08] 合并两个数组
来源：http://xu.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://io.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://vi.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ks.yuexingan06.cn

TS:   [...a, ...b];
来源：http://fc.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bh.haigaiapp.cn

Go:   append(a, b...)
来源：http://ge.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://wv.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://yv.hnjuh.cn

[D09] 排序（升序）
来源：http://pp.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://sl.szsharing.cn

PHP:  sort($arr);
来源：http://mv.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://de.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ax.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ng.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lx.shxzskj.cn

Ruby: arr.sort
来源：http://fs.shtwfgs.cn

C#:   list.Sort();
来源：http://mn.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xw.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pr.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dr.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jl.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ue.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zu.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ku.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oj.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ji.jianghongdianzi.cn

[D11] 反转数组
来源：http://fs.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xf.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://ba.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yl.panjiajie.cn

TS:   [...arr].reverse();
来源：http://tq.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://ho.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://wt.bookmarksfly.cn

Ruby: arr.reverse
来源：http://hf.szxytkj.cn

C#:   list.Reverse();
来源：http://yj.asd995.cn

[D12] 查找元素下标
来源：http://kj.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://qp.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lu.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pw.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lk.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jd.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://yh.lnxyls.cn

Ruby: arr.index(x)
来源：http://gi.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://oh.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://lh.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vq.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mx.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://hw.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://op.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://in.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zl.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://br.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ly.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://mq.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ty.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ig.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://ah.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://ds.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ii.colortex.cn

Go:   // 手写循环
来源：http://pm.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://js.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://of.jianghongdianzi.cn

[D15] 去重
来源：http://hh.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qz.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://zs.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://ea.colortex.cn

TS:   [...new Set(arr)]
来源：http://im.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nl.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rl.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://ui.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://ih.huanxung.cn

[D16] 求和与平均值
来源：http://lg.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://og.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lq.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cl.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zc.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://up.shtwfgs.cn

Go:   // 手写循环累加
来源：http://la.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ou.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://tj.nszjky.cn

[D17] 最大值与最小值
来源：http://wp.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://pe.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://zb.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cv.gzmigu.cn

TS:   Math.max(...arr);
来源：http://dh.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ha.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cg.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://br.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://zz.asd995.cn

[D18] 扁平化嵌套数组
来源：http://mt.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ec.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://ja.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ur.shxzskj.cn

TS:   nested.flat();
来源：http://zu.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lc.9csxet.cn

Go:   // 手写双层循环
来源：http://tc.shxzukj.cn

Ruby: nested.flatten
来源：http://hm.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pb.huanxung.cn

[D19] 按字段分组
来源：http://vk.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mh.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cf.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nq.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hd.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hj.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://zv.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ly.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://na.521024.cn

[D20] 统计每个元素出现次数
来源：http://pk.bjjhwx.cn

Py:   Counter(arr)
来源：http://sy.hahajie.cn

PHP:  array_count_values($arr);
来源：http://iq.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ky.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vm.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ka.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://cp.yuexingan06.cn

Ruby: arr.tally
来源：http://ev.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dx.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://yr.muxihuayi.cn

Py:   x in arr
来源：http://xq.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://jg.shxzukj.cn

JS:   arr.includes(x)
来源：http://og.nszjky.cn

TS:   arr.includes(x)
来源：http://bw.hnjuh.cn

Java: list.contains(x)
来源：http://la.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://mq.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://vc.asd995.cn

C#:   list.Contains(x)
来源：http://gt.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://ve.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qg.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qy.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gu.shxzskj.cn

TS:   [...arr];
来源：http://xa.szsharing.cn

Java: new ArrayList<>(list);
来源：http://wc.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cy.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://vc.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://ee.colortex.cn

[D23] reduce 累积计算
来源：http://kh.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gl.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nv.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zo.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zz.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xj.panjiajie.cn

Go:   // 手写循环
来源：http://li.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://po.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fq.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://bc.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oy.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ge.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yj.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ot.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ir.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://by.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cs.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jc.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://po.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tg.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cs.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sa.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ph.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ez.chemitech.net.cn


<!-- 参考信息 -->