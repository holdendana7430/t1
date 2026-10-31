代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uv.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://im.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uk.yuntaijiaju.cn

[C09] 递归
来源：http://ux.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jp.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gg.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iz.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ha.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://my.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nx.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iu.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zs.huixiangedu.cn

[C10] 变量作用域
来源：http://zw.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qo.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tl.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kx.hnjuh.cn

TS:   同 JS
来源：http://nu.hnjuh.cn

Java: 方法内为块级作用域
来源：http://wy.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://lv.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://be.wgjwhj.cn

C#:   块级作用域
来源：http://ah.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://ww.chemitech.net.cn

Py:   from module import func
来源：http://xy.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wa.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ra.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vd.jctech888.com.cn

Java: import java.util.List;
来源：http://pl.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yo.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://rg.huixinmuqiang.cn

C#:   using System.Text;
来源：http://gr.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://ss.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://zo.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://hc.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://uu.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ks.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tr.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://hb.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://rf.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ow.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://dh.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jr.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ii.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mh.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ts.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://od.nszjky.cn

Go:   func add(a, b int) int
来源：http://xh.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qn.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://us.bookmarksfly.cn

[C14] 泛型函数
来源：http://ok.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pc.bjjhwx.cn

PHP:  // 无泛型
来源：http://do.yuntaijiaju.cn

JS:   // 无泛型
来源：http://jz.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cb.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sl.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ka.bookmarksfly.cn

Ruby: # 无泛型
来源：http://bi.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nl.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://pw.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sj.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://in.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gg.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yx.colortex.cn

Java: // 无解构
来源：http://zm.huixiangedu.cn

Go:   // 无解构
来源：http://ab.nszjky.cn

Ruby: a, b = pair
来源：http://dx.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://gh.newstarts.cn

[C16] 函数 / 方法重载
来源：http://gv.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pc.yuntaijiaju.cn

PHP:  // 无重载
来源：http://gf.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ne.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://fc.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gv.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://en.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://jv.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ku.chemitech.net.cn

================================================================================
来源：http://ff.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://aw.huanxung.cn

================================================================================
来源：http://fw.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://rk.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://go.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fg.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cp.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://di.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tf.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://ku.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://pk.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mu.szsharing.cn

[D02] 追加元素到末尾
来源：http://jt.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://az.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uu.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://nc.hnjuh.cn

TS:   arr.push(4);
来源：http://sz.chemitech.net.cn

Java: list.add(4);
来源：http://lr.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://wc.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://gs.yuexingan06.cn

C#:   list.Add(4);
来源：http://kc.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://qn.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://nh.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://at.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bq.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://nx.newstarts.cn

Java: list.add(0, 0);
来源：http://nw.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wh.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ci.colortex.cn

C#:   list.Insert(0, 0);
来源：http://nj.haigaiapp.cn

[D04] 删除元素
来源：http://cg.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mo.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mb.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ai.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://ox.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fz.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://em.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://au.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qy.huanxung.cn

[D05] 访问与修改元素
来源：http://pg.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://um.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gj.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bh.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://la.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://vw.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://my.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nd.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://st.gzmigu.cn

[D06] 数组长度
来源：http://no.nszjky.cn

Py:   len(arr)
来源：http://rv.jctech888.com.cn

PHP:  count($arr);
来源：http://zf.hahajie.cn

JS:   arr.length
来源：http://sf.yuexingan06.cn

TS:   arr.length
来源：http://qe.wgjwhj.cn

Java: list.size();
来源：http://fx.panjiajie.cn

Go:   len(arr)
来源：http://lk.szsharing.cn

Ruby: arr.length; arr.size
来源：http://pc.hnjuh.cn

C#:   list.Count;
来源：http://ym.nicolike.cn

[D07] 切片 / 取子数组
来源：http://or.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yn.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ut.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://wz.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://yw.lnxyls.cn

Java: list.subList(1, 4);
来源：http://lk.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://rz.szxytkj.cn

Ruby: arr[1, 3]
来源：http://em.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://vb.bjjhwx.cn

[D08] 合并两个数组
来源：http://ks.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://ia.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://tl.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eu.hahajie.cn

TS:   [...a, ...b];
来源：http://aw.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fl.nszjky.cn

Go:   append(a, b...)
来源：http://nd.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://by.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://au.wgjwhj.cn

[D09] 排序（升序）
来源：http://pm.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://et.szxytkj.cn

PHP:  sort($arr);
来源：http://tz.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sw.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sd.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xb.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://th.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ix.huixinmuqiang.cn

C#:   list.Sort();
来源：http://nb.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rn.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jk.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dy.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mx.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ui.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ji.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dd.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ei.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kx.haigaiapp.cn

[D11] 反转数组
来源：http://pa.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qo.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://no.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lo.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://tz.szsharing.cn

Java: Collections.reverse(list);
来源：http://hv.asd995.cn

Go:   slices.Reverse(arr)
来源：http://xb.hahajie.cn

Ruby: arr.reverse
来源：http://fg.shtwfgs.cn

C#:   list.Reverse();
来源：http://pd.521024.cn

[D12] 查找元素下标
来源：http://bl.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://ni.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zk.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nt.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cy.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sq.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://ok.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://sc.huanxung.cn

C#:   list.IndexOf(x);
来源：http://zu.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://bv.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ed.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jo.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://mj.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://qm.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gd.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gz.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wg.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nc.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://wr.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ii.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fk.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://nb.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://ba.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nd.newstarts.cn

Go:   // 手写循环
来源：http://oo.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wu.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fk.huixinmuqiang.cn

[D15] 去重
来源：http://en.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jr.nszjky.cn

PHP:  array_unique($arr);
来源：http://vz.huanxung.cn

JS:   [...new Set(arr)]
来源：http://cl.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://aw.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ko.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ad.hahajie.cn

Ruby: arr.uniq
来源：http://ht.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://ed.huanxung.cn

[D16] 求和与平均值
来源：http://ix.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://na.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oo.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://in.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yy.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jk.wgjwhj.cn

Go:   // 手写循环累加
来源：http://rp.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qf.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://qq.shxzukj.cn

[D17] 最大值与最小值
来源：http://ao.asd995.cn

Py:   max(arr);  min(arr)
来源：http://wo.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://mj.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gb.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://dy.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pk.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zb.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://za.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://bl.asd995.cn

[D18] 扁平化嵌套数组
来源：http://ni.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hd.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://hu.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fp.nszjky.cn

TS:   nested.flat();
来源：http://qw.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nx.colortex.cn

Go:   // 手写双层循环
来源：http://qb.shtwfgs.cn

Ruby: nested.flatten
来源：http://yu.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ki.haigaiapp.cn

[D19] 按字段分组
来源：http://yx.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gi.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ll.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sl.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ot.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ge.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://hj.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ic.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://me.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://ez.wgjwhj.cn

Py:   Counter(arr)
来源：http://qo.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://gq.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ln.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sh.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pv.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://oc.huanxung.cn

Ruby: arr.tally
来源：http://ts.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bn.9csxet.cn

[D21] 判断是否包含某元素
来源：http://bl.nicolike.cn

Py:   x in arr
来源：http://dv.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://zn.hahajie.cn

JS:   arr.includes(x)
来源：http://ob.521024.cn

TS:   arr.includes(x)
来源：http://pp.wgjwhj.cn

Java: list.contains(x)
来源：http://vu.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://tc.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://wq.9csxet.cn

C#:   list.Contains(x)
来源：http://zj.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://bs.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ei.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wn.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qz.hnjuh.cn

TS:   [...arr];
来源：http://ba.nicolike.cn

Java: new ArrayList<>(list);
来源：http://pd.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kl.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://qr.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://dr.shxzskj.cn

[D23] reduce 累积计算
来源：http://wq.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gr.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hk.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ta.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dz.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ab.bookmarksfly.cn

Go:   // 手写循环
来源：http://dz.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tj.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vl.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://vv.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zb.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dw.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cy.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://un.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://og.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://db.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nw.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wu.colortex.cn

[D25] Set 集合去重与交并差
来源：http://vm.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bv.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jr.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cm.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zt.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ve.panjiajie.cn


<!-- 参考信息 -->