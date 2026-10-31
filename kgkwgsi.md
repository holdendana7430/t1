代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xl.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lf.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mf.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eq.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xx.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mv.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yh.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lo.bookmarksfly.cn

[C10] 变量作用域
来源：http://lf.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ut.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cn.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hl.yuexingan06.cn

TS:   同 JS
来源：http://ud.hahajie.cn

Java: 方法内为块级作用域
来源：http://uw.haigaiapp.cn

Go:   花括号块级作用域
来源：http://lg.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tx.hahajie.cn

C#:   块级作用域
来源：http://im.shxzukj.cn

[C11] 模块导入与导出
来源：http://lu.shtwfgs.cn

Py:   from module import func
来源：http://wn.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lj.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qm.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pj.nszjky.cn

Java: import java.util.List;
来源：http://wp.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rt.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://iq.lnxyls.cn

C#:   using System.Text;
来源：http://wd.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://hn.521024.cn

Py:   (lambda: print("run"))()
来源：http://bx.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://yq.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://px.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://wf.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cq.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://vw.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://wp.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://el.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://td.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://li.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ld.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oa.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ug.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sl.hnjuh.cn

Go:   func add(a, b int) int
来源：http://gr.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fo.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bm.shxzskj.cn

[C14] 泛型函数
来源：http://mt.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wb.bjjhwx.cn

PHP:  // 无泛型
来源：http://xl.huixinmuqiang.cn

JS:   // 无泛型
来源：http://ky.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pe.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vr.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hg.huixiangedu.cn

Ruby: # 无泛型
来源：http://rs.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jr.szsharing.cn

[C15] 解构 / 展开参数
来源：http://wo.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://au.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://hy.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pz.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wh.yuexingan06.cn

Java: // 无解构
来源：http://li.huixiangedu.cn

Go:   // 无解构
来源：http://hq.shxzskj.cn

Ruby: a, b = pair
来源：http://jj.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://jq.newstarts.cn

[C16] 函数 / 方法重载
来源：http://wp.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ty.shtwfgs.cn

PHP:  // 无重载
来源：http://cd.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ql.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://pu.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pc.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://we.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://ke.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ky.yuexingan06.cn

================================================================================
来源：http://ld.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://bj.yuexingan06.cn

================================================================================
来源：http://fe.nicolike.cn

[D01] 创建数组 / 列表
来源：http://kt.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wb.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zn.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ai.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ge.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ps.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://cm.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://bz.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ja.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://kw.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tm.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://om.bjjhwx.cn

JS:   arr.push(4);
来源：http://dc.lnxyls.cn

TS:   arr.push(4);
来源：http://yn.jctech888.com.cn

Java: list.add(4);
来源：http://lf.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://cu.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://nu.shxzukj.cn

C#:   list.Add(4);
来源：http://zp.nicolike.cn

[D03] 在指定位置插入元素
来源：http://mg.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://no.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jp.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vn.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://dy.gzmigu.cn

Java: list.add(0, 0);
来源：http://fm.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hw.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dd.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://ly.jianghongdianzi.cn

[D04] 删除元素
来源：http://zo.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bq.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://al.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gw.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://dh.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jb.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lc.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pv.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wb.yuexingan06.cn

[D05] 访问与修改元素
来源：http://cm.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lo.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ul.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fu.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ej.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://oy.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://un.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kj.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ua.jctech888.com.cn

[D06] 数组长度
来源：http://ov.huixiangedu.cn

Py:   len(arr)
来源：http://ik.nszjky.cn

PHP:  count($arr);
来源：http://xf.521024.cn

JS:   arr.length
来源：http://tt.hnjuh.cn

TS:   arr.length
来源：http://hs.huanxung.cn

Java: list.size();
来源：http://jt.shxzskj.cn

Go:   len(arr)
来源：http://dz.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://uk.shxzukj.cn

C#:   list.Count;
来源：http://vd.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://xs.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sc.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xt.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://iz.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://fm.newstarts.cn

Java: list.subList(1, 4);
来源：http://uh.huanxung.cn

Go:   arr[1:4]
来源：http://pm.521024.cn

Ruby: arr[1, 3]
来源：http://xz.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://hu.bookmarksfly.cn

[D08] 合并两个数组
来源：http://xl.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://pr.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://xy.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rt.gzmigu.cn

TS:   [...a, ...b];
来源：http://xv.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://op.colortex.cn

Go:   append(a, b...)
来源：http://zm.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://mp.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://si.nszjky.cn

[D09] 排序（升序）
来源：http://ie.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://bm.shxzukj.cn

PHP:  sort($arr);
来源：http://nb.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jq.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rd.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://so.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vz.bookmarksfly.cn

Ruby: arr.sort
来源：http://sk.wgjwhj.cn

C#:   list.Sort();
来源：http://vt.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nd.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xt.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aj.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hp.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dd.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ag.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yc.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fp.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sg.nszjky.cn

[D11] 反转数组
来源：http://de.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gc.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://sn.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hk.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://hy.colortex.cn

Java: Collections.reverse(list);
来源：http://fq.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://jx.huixiangedu.cn

Ruby: arr.reverse
来源：http://qc.9csxet.cn

C#:   list.Reverse();
来源：http://zk.shxzskj.cn

[D12] 查找元素下标
来源：http://ok.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://zd.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ic.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ak.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mx.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rl.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://hk.colortex.cn

Ruby: arr.index(x)
来源：http://wu.szsharing.cn

C#:   list.IndexOf(x);
来源：http://wo.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://be.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ed.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tt.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://xs.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://rs.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qf.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eb.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zr.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vz.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://cn.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://it.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://td.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://yr.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://jf.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ex.asd995.cn

Go:   // 手写循环
来源：http://it.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vq.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nd.jianghongdianzi.cn

[D15] 去重
来源：http://vl.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eg.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://eu.asd995.cn

JS:   [...new Set(arr)]
来源：http://vk.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://la.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cl.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nc.shxzukj.cn

Ruby: arr.uniq
来源：http://no.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://tg.jctech888.com.cn

[D16] 求和与平均值
来源：http://gl.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qo.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xg.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ol.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bd.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bg.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://jm.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wz.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://yz.panjiajie.cn

[D17] 最大值与最小值
来源：http://uy.521024.cn

Py:   max(arr);  min(arr)
来源：http://pm.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ri.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kv.nszjky.cn

TS:   Math.max(...arr);
来源：http://gh.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ok.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://by.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://cn.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://gx.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://ab.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fn.colortex.cn

PHP:  array_merge(...$nested);
来源：http://sm.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mo.haigaiapp.cn

TS:   nested.flat();
来源：http://em.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vg.szxytkj.cn

Go:   // 手写双层循环
来源：http://gi.9csxet.cn

Ruby: nested.flatten
来源：http://by.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ye.yuexingan06.cn

[D19] 按字段分组
来源：http://za.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iw.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yi.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eh.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kb.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rv.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://fx.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fy.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ws.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://od.9csxet.cn

Py:   Counter(arr)
来源：http://vd.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://hw.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ak.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lq.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://se.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://ek.shtwfgs.cn

Ruby: arr.tally
来源：http://ut.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uk.521024.cn

[D21] 判断是否包含某元素
来源：http://im.huanxung.cn

Py:   x in arr
来源：http://tl.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://gf.muxihuayi.cn

JS:   arr.includes(x)
来源：http://am.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://ms.wgjwhj.cn

Java: list.contains(x)
来源：http://bp.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://za.nicolike.cn

Ruby: arr.include?(x)
来源：http://os.chemitech.net.cn

C#:   list.Contains(x)
来源：http://gn.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://ge.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wf.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dp.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xc.jctech888.com.cn

TS:   [...arr];
来源：http://uh.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ea.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ss.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://qd.hahajie.cn

C#:   new List<int>(list);
来源：http://zg.bjjhwx.cn

[D23] reduce 累积计算
来源：http://rm.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jf.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cq.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jf.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dn.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mc.gzmigu.cn

Go:   // 手写循环
来源：http://ck.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gl.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yw.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://ua.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cv.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bt.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ib.shxzukj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://li.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fx.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eq.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://du.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wj.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://in.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ur.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jt.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nu.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sp.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hs.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pk.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://if.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jn.haigaiapp.cn

[D26] 数组转字符串
来源：http://bi.panjiajie.cn


<!-- 参考信息 -->