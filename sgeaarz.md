代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dg.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fv.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cg.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jv.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mt.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bv.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ix.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pn.szxytkj.cn

[C10] 变量作用域
来源：http://ha.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iy.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bv.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pi.yuntaijiaju.cn

TS:   同 JS
来源：http://tj.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://wx.muxihuayi.cn

Go:   花括号块级作用域
来源：http://yq.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cf.jianghongdianzi.cn

C#:   块级作用域
来源：http://vl.szsharing.cn

[C11] 模块导入与导出
来源：http://eg.muxihuayi.cn

Py:   from module import func
来源：http://cl.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ym.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vz.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ms.hnjuh.cn

Java: import java.util.List;
来源：http://tp.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vf.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://jv.newstarts.cn

C#:   using System.Text;
来源：http://tm.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://ef.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://on.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://sz.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://zs.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://sk.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zl.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ig.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://qn.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rd.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://nb.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uy.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ms.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xj.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hw.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ou.asd995.cn

Go:   func add(a, b int) int
来源：http://gd.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hv.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qf.muxihuayi.cn

[C14] 泛型函数
来源：http://te.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tg.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://vd.newstarts.cn

JS:   // 无泛型
来源：http://si.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jq.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dn.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rm.bjjhwx.cn

Ruby: # 无泛型
来源：http://jp.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mf.nicolike.cn

[C15] 解构 / 展开参数
来源：http://yf.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nd.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://sx.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vk.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://da.huixiangedu.cn

Java: // 无解构
来源：http://pd.szsharing.cn

Go:   // 无解构
来源：http://wp.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://lc.521024.cn

C#:   var (a, b) = pair;
来源：http://br.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://ck.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bx.lnxyls.cn

PHP:  // 无重载
来源：http://ow.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://km.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://cl.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ku.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://vc.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://sd.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://af.jianghongdianzi.cn

================================================================================
来源：http://qj.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://em.shxzskj.cn

================================================================================
来源：http://wz.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://ur.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qk.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yu.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tn.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kc.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zr.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://py.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://zu.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oh.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://bm.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gs.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nr.szsharing.cn

JS:   arr.push(4);
来源：http://rl.szxytkj.cn

TS:   arr.push(4);
来源：http://lf.asd995.cn

Java: list.add(4);
来源：http://ze.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://ym.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://dl.bookmarksfly.cn

C#:   list.Add(4);
来源：http://nx.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://hr.asd995.cn

Py:   arr.insert(0, 0)
来源：http://gl.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pz.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ji.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://gf.muxihuayi.cn

Java: list.add(0, 0);
来源：http://aa.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tg.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://az.521024.cn

C#:   list.Insert(0, 0);
来源：http://eu.wgjwhj.cn

[D04] 删除元素
来源：http://cn.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kq.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ii.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fo.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://ef.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://du.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zx.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rh.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tt.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://js.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rl.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wf.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vs.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://km.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://af.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://qx.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gb.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pj.colortex.cn

[D06] 数组长度
来源：http://ap.hnjuh.cn

Py:   len(arr)
来源：http://pp.panjiajie.cn

PHP:  count($arr);
来源：http://ac.shxzukj.cn

JS:   arr.length
来源：http://qh.newstarts.cn

TS:   arr.length
来源：http://ez.chemitech.net.cn

Java: list.size();
来源：http://bq.shxzskj.cn

Go:   len(arr)
来源：http://yy.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://jx.jianghongdianzi.cn

C#:   list.Count;
来源：http://bp.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://dw.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ou.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uk.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://jr.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ck.newstarts.cn

Java: list.subList(1, 4);
来源：http://to.panjiajie.cn

Go:   arr[1:4]
来源：http://xi.521024.cn

Ruby: arr[1, 3]
来源：http://ew.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://cx.hahajie.cn

[D08] 合并两个数组
来源：http://rg.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://oo.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://bc.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jd.chemitech.net.cn

TS:   [...a, ...b];
来源：http://qv.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qc.hnjuh.cn

Go:   append(a, b...)
来源：http://ie.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://gl.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://qr.nszjky.cn

[D09] 排序（升序）
来源：http://zl.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://vg.huixiangedu.cn

PHP:  sort($arr);
来源：http://se.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bx.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ol.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pn.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rs.haigaiapp.cn

Ruby: arr.sort
来源：http://ur.521024.cn

C#:   list.Sort();
来源：http://hs.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wf.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dp.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qy.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rv.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pt.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zx.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pd.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bs.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sv.jctech888.com.cn

[D11] 反转数组
来源：http://nc.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hl.huanxung.cn

PHP:  array_reverse($arr);
来源：http://ix.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vh.newstarts.cn

TS:   [...arr].reverse();
来源：http://sp.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://le.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://fd.asd995.cn

Ruby: arr.reverse
来源：http://is.chemitech.net.cn

C#:   list.Reverse();
来源：http://cg.bjjhwx.cn

[D12] 查找元素下标
来源：http://hm.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://gc.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lj.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://md.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pk.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yx.521024.cn

Go:   slices.Index(arr, x)
来源：http://fo.gzmigu.cn

Ruby: arr.index(x)
来源：http://fn.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://vp.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ur.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bw.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hf.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://kv.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://aw.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zs.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tc.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gz.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yf.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://lq.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ge.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qv.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://ri.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://bq.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cz.bookmarksfly.cn

Go:   // 手写循环
来源：http://ux.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yg.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xs.huixinmuqiang.cn

[D15] 去重
来源：http://sn.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vu.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://gc.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://iq.newstarts.cn

TS:   [...new Set(arr)]
来源：http://mv.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rb.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yp.newstarts.cn

Ruby: arr.uniq
来源：http://ro.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://gx.yuexingan06.cn

[D16] 求和与平均值
来源：http://pq.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nh.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nx.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gz.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ke.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xo.szsharing.cn

Go:   // 手写循环累加
来源：http://ox.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ao.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://gx.asd995.cn

[D17] 最大值与最小值
来源：http://fe.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://ca.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://fn.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ii.asd995.cn

TS:   Math.max(...arr);
来源：http://jt.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qx.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qi.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://be.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://dm.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://vs.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tg.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://jr.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vh.huanxung.cn

TS:   nested.flat();
来源：http://lo.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gl.newstarts.cn

Go:   // 手写双层循环
来源：http://tc.shxzskj.cn

Ruby: nested.flatten
来源：http://ue.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lv.yuexingan06.cn

[D19] 按字段分组
来源：http://va.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iv.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://li.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ov.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://le.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oj.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://wp.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nu.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://es.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://tr.shxzukj.cn

Py:   Counter(arr)
来源：http://lt.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://bj.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ek.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ka.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ki.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://wb.asd995.cn

Ruby: arr.tally
来源：http://ty.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rl.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://ia.szxytkj.cn

Py:   x in arr
来源：http://pg.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://lo.huixiangedu.cn

JS:   arr.includes(x)
来源：http://fa.hahajie.cn

TS:   arr.includes(x)
来源：http://xh.521024.cn

Java: list.contains(x)
来源：http://ou.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://yc.asd995.cn

Ruby: arr.include?(x)
来源：http://eh.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://tm.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://yl.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nk.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ie.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rq.gzmigu.cn

TS:   [...arr];
来源：http://xo.szsharing.cn

Java: new ArrayList<>(list);
来源：http://xr.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tk.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://gk.asd995.cn

C#:   new List<int>(list);
来源：http://po.hnjuh.cn

[D23] reduce 累积计算
来源：http://la.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yy.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sz.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uy.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yg.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wg.yuexingan06.cn

Go:   // 手写循环
来源：http://fn.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sn.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mn.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://yz.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jh.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ym.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ca.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://st.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uf.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lp.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gc.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bw.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ya.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gv.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ut.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fm.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ey.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lt.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nr.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hd.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ce.bookmarksfly.cn

[D26] 数组转字符串
来源：http://zz.huixiangedu.cn


<!-- 参考信息 -->