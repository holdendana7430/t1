代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sx.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://un.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xr.bjjhwx.cn

[C09] 递归
来源：http://hx.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mw.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ba.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ci.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vu.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ly.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kw.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://st.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jp.yuexingan06.cn

[C10] 变量作用域
来源：http://jw.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dy.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xx.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ek.hahajie.cn

TS:   同 JS
来源：http://cb.colortex.cn

Java: 方法内为块级作用域
来源：http://ue.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://zw.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sn.colortex.cn

C#:   块级作用域
来源：http://ep.szxytkj.cn

[C11] 模块导入与导出
来源：http://gg.colortex.cn

Py:   from module import func
来源：http://zj.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ws.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xr.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://no.chemitech.net.cn

Java: import java.util.List;
来源：http://gb.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xm.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ck.hahajie.cn

C#:   using System.Text;
来源：http://sy.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://jx.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://ks.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://sk.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://ba.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://un.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lr.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://lc.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://fv.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oj.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://jm.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cx.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hl.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ie.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dc.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xh.panjiajie.cn

Go:   func add(a, b int) int
来源：http://aq.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vy.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://je.shtwfgs.cn

[C14] 泛型函数
来源：http://jk.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bc.bjjhwx.cn

PHP:  // 无泛型
来源：http://un.panjiajie.cn

JS:   // 无泛型
来源：http://gr.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ip.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://js.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ad.gzmigu.cn

Ruby: # 无泛型
来源：http://qm.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ni.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://er.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pz.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://bg.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://af.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gr.huanxung.cn

Java: // 无解构
来源：http://wu.huanxung.cn

Go:   // 无解构
来源：http://tw.hahajie.cn

Ruby: a, b = pair
来源：http://uj.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://if.9csxet.cn

[C16] 函数 / 方法重载
来源：http://wv.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rc.chemitech.net.cn

PHP:  // 无重载
来源：http://os.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ku.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://ku.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iz.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://ku.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://vb.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lx.asd995.cn

================================================================================
来源：http://tr.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://fl.asd995.cn

================================================================================
来源：http://xa.colortex.cn

[D01] 创建数组 / 列表
来源：http://ra.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bm.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://td.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vb.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jh.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mw.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://gv.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://te.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dy.colortex.cn

[D02] 追加元素到末尾
来源：http://wm.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://un.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sf.nszjky.cn

JS:   arr.push(4);
来源：http://tf.huanxung.cn

TS:   arr.push(4);
来源：http://rk.gzmigu.cn

Java: list.add(4);
来源：http://yc.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://yp.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://kl.muxihuayi.cn

C#:   list.Add(4);
来源：http://ry.nszjky.cn

[D03] 在指定位置插入元素
来源：http://ab.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://wk.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sr.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mq.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://pb.lnxyls.cn

Java: list.add(0, 0);
来源：http://ow.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://es.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tr.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://gb.chemitech.net.cn

[D04] 删除元素
来源：http://tl.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tr.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tk.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hh.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://lo.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://al.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qz.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wr.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ic.shxzukj.cn

[D05] 访问与修改元素
来源：http://vi.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zh.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zg.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ad.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://yc.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://bu.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://ta.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sp.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ic.newstarts.cn

[D06] 数组长度
来源：http://pj.huixiangedu.cn

Py:   len(arr)
来源：http://uu.huixiangedu.cn

PHP:  count($arr);
来源：http://hq.521024.cn

JS:   arr.length
来源：http://mj.bjjhwx.cn

TS:   arr.length
来源：http://ko.bjjhwx.cn

Java: list.size();
来源：http://bn.hahajie.cn

Go:   len(arr)
来源：http://qp.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://ks.hnjuh.cn

C#:   list.Count;
来源：http://hy.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://yw.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tb.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ap.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://fp.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://bh.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://oa.hahajie.cn

Go:   arr[1:4]
来源：http://pw.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://rg.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://vm.nicolike.cn

[D08] 合并两个数组
来源：http://xl.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://zb.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://tb.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zk.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://qk.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chemitech.net.cn

Go:   append(a, b...)
来源：http://yn.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://kw.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://bw.huanxung.cn

[D09] 排序（升序）
来源：http://oq.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ei.chemitech.net.cn

PHP:  sort($arr);
来源：http://lk.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://if.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yi.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gb.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://im.szsharing.cn

Ruby: arr.sort
来源：http://lp.yuntaijiaju.cn

C#:   list.Sort();
来源：http://cg.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ok.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yj.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://in.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://as.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qj.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jn.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ly.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qc.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kl.huixinmuqiang.cn

[D11] 反转数组
来源：http://pe.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kf.9csxet.cn

PHP:  array_reverse($arr);
来源：http://fh.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ub.521024.cn

TS:   [...arr].reverse();
来源：http://yo.nszjky.cn

Java: Collections.reverse(list);
来源：http://mj.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://tz.panjiajie.cn

Ruby: arr.reverse
来源：http://ue.huanxung.cn

C#:   list.Reverse();
来源：http://zc.9csxet.cn

[D12] 查找元素下标
来源：http://ie.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://qp.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://op.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cl.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ir.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mp.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://tt.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://ko.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://pt.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://lg.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fb.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iu.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://lx.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://em.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ka.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ej.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vp.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cq.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://xu.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tq.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kg.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://cw.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://ns.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ii.newstarts.cn

Go:   // 手写循环
来源：http://wd.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bt.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tw.colortex.cn

[D15] 去重
来源：http://nr.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sl.asd995.cn

PHP:  array_unique($arr);
来源：http://ic.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://cz.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://vm.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://su.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mi.szsharing.cn

Ruby: arr.uniq
来源：http://ra.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://hz.nicolike.cn

[D16] 求和与平均值
来源：http://nm.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://on.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ee.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qp.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oa.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sw.newstarts.cn

Go:   // 手写循环累加
来源：http://td.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ng.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://wy.muxihuayi.cn

[D17] 最大值与最小值
来源：http://do.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://uu.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://yv.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dn.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://dt.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mt.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zv.asd995.cn

Ruby: arr.max;  arr.min
来源：http://up.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://ma.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://bl.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zj.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://gx.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vn.gzmigu.cn

TS:   nested.flat();
来源：http://ot.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kc.nszjky.cn

Go:   // 手写双层循环
来源：http://ze.bjjhwx.cn

Ruby: nested.flatten
来源：http://fc.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mw.nszjky.cn

[D19] 按字段分组
来源：http://oq.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zr.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://as.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://az.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ac.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ig.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://qf.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ij.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rt.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://gy.hnjuh.cn

Py:   Counter(arr)
来源：http://xw.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://un.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cd.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fc.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gr.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://ad.panjiajie.cn

Ruby: arr.tally
来源：http://mk.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hr.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://uc.bjjhwx.cn

Py:   x in arr
来源：http://ab.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://xg.gzmigu.cn

JS:   arr.includes(x)
来源：http://ux.hahajie.cn

TS:   arr.includes(x)
来源：http://kc.bookmarksfly.cn

Java: list.contains(x)
来源：http://zy.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://wj.newstarts.cn

Ruby: arr.include?(x)
来源：http://lt.asd995.cn

C#:   list.Contains(x)
来源：http://is.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://jx.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ei.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pv.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wt.newstarts.cn

TS:   [...arr];
来源：http://st.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://wc.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://np.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://mw.wgjwhj.cn

C#:   new List<int>(list);
来源：http://tf.wgjwhj.cn

[D23] reduce 累积计算
来源：http://uj.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zj.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ml.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://my.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zt.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ti.521024.cn

Go:   // 手写循环
来源：http://yy.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ds.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tn.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://kg.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://em.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dd.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://le.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yt.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ll.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ca.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mp.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mr.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://fw.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yk.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ts.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qb.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bi.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zo.shxzukj.cn


<!-- 参考信息 -->