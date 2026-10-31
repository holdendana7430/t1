代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ph.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ai.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kj.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tl.huixinmuqiang.cn

[C10] 变量作用域
来源：http://xt.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pz.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ou.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wa.yuexingan06.cn

TS:   同 JS
来源：http://gc.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://qx.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://et.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ua.shxzukj.cn

C#:   块级作用域
来源：http://pv.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://qq.colortex.cn

Py:   from module import func
来源：http://yw.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dn.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kw.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gx.nicolike.cn

Java: import java.util.List;
来源：http://mj.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://id.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://pz.haigaiapp.cn

C#:   using System.Text;
来源：http://xt.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://tx.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://lk.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://qu.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://qd.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://pz.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ad.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://zi.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ww.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rn.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://ut.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kk.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ir.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ym.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rl.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tm.szxytkj.cn

Go:   func add(a, b int) int
来源：http://ha.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qp.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://or.haigaiapp.cn

[C14] 泛型函数
来源：http://me.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pz.gzmigu.cn

PHP:  // 无泛型
来源：http://ft.jctech888.com.cn

JS:   // 无泛型
来源：http://vx.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qh.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://er.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tr.haigaiapp.cn

Ruby: # 无泛型
来源：http://zz.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wj.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://ug.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sy.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://ud.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vc.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pc.shxzukj.cn

Java: // 无解构
来源：http://vy.jctech888.com.cn

Go:   // 无解构
来源：http://wd.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://wh.szsharing.cn

C#:   var (a, b) = pair;
来源：http://ui.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://sk.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://as.shxzukj.cn

PHP:  // 无重载
来源：http://iu.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uq.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://li.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qz.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://ng.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://dn.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qm.huanxung.cn

================================================================================
来源：http://ut.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://fl.jctech888.com.cn

================================================================================
来源：http://qg.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://jy.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ob.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fq.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qo.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xp.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://po.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://oq.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://tx.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ru.nszjky.cn

[D02] 追加元素到末尾
来源：http://dt.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cd.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mg.yuexingan06.cn

JS:   arr.push(4);
来源：http://pn.szxytkj.cn

TS:   arr.push(4);
来源：http://av.521024.cn

Java: list.add(4);
来源：http://uy.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://eb.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://wc.muxihuayi.cn

C#:   list.Add(4);
来源：http://nd.huanxung.cn

[D03] 在指定位置插入元素
来源：http://kh.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://ac.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xj.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mw.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://hr.hnjuh.cn

Java: list.add(0, 0);
来源：http://re.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dx.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qn.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://uw.9csxet.cn

[D04] 删除元素
来源：http://aa.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tn.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dh.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ow.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://xn.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mx.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lj.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tq.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://no.shxzukj.cn

[D05] 访问与修改元素
来源：http://xg.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://in.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oz.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ih.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ea.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ft.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://zv.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gt.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qp.bookmarksfly.cn

[D06] 数组长度
来源：http://hr.shtwfgs.cn

Py:   len(arr)
来源：http://qy.haigaiapp.cn

PHP:  count($arr);
来源：http://wk.szxytkj.cn

JS:   arr.length
来源：http://nh.nszjky.cn

TS:   arr.length
来源：http://xr.panjiajie.cn

Java: list.size();
来源：http://hw.lnxyls.cn

Go:   len(arr)
来源：http://gq.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://sz.hnjuh.cn

C#:   list.Count;
来源：http://io.9csxet.cn

[D07] 切片 / 取子数组
来源：http://nt.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aj.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eu.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://kz.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://pi.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://cm.szsharing.cn

Go:   arr[1:4]
来源：http://qb.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://yo.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://pq.muxihuayi.cn

[D08] 合并两个数组
来源：http://eh.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://rz.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://rj.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wy.jctech888.com.cn

TS:   [...a, ...b];
来源：http://fk.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lp.521024.cn

Go:   append(a, b...)
来源：http://tl.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://gz.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://se.9csxet.cn

[D09] 排序（升序）
来源：http://pv.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://fn.lnxyls.cn

PHP:  sort($arr);
来源：http://or.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nm.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ks.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://py.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zz.colortex.cn

Ruby: arr.sort
来源：http://sx.huixiangedu.cn

C#:   list.Sort();
来源：http://jf.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ws.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cr.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ir.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bb.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ny.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gz.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cn.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rq.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nw.shxzskj.cn

[D11] 反转数组
来源：http://mm.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yx.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://um.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oo.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://fr.panjiajie.cn

Java: Collections.reverse(list);
来源：http://tg.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://lr.szsharing.cn

Ruby: arr.reverse
来源：http://fg.lnxyls.cn

C#:   list.Reverse();
来源：http://ef.huixiangedu.cn

[D12] 查找元素下标
来源：http://qe.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://lf.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://br.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://us.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mf.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hr.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://ld.jctech888.com.cn

Ruby: arr.index(x)
来源：http://uh.szsharing.cn

C#:   list.IndexOf(x);
来源：http://ed.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://zw.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xl.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dj.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://hs.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://on.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xd.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rq.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jm.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ff.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://fu.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://by.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xx.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://ob.521024.cn

TS:   arr.map(x => x * 2)
来源：http://il.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sr.shxzskj.cn

Go:   // 手写循环
来源：http://gz.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ip.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zr.huixinmuqiang.cn

[D15] 去重
来源：http://xp.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kk.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://ib.newstarts.cn

JS:   [...new Set(arr)]
来源：http://lx.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://su.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kc.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sm.newstarts.cn

Ruby: arr.uniq
来源：http://qr.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://ik.szsharing.cn

[D16] 求和与平均值
来源：http://ka.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ov.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://af.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jp.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qo.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ol.panjiajie.cn

Go:   // 手写循环累加
来源：http://qi.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bg.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://hw.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://ng.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://sb.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://rl.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qc.shxzskj.cn

TS:   Math.max(...arr);
来源：http://ee.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qf.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vd.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://ds.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://yx.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://cw.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://be.521024.cn

PHP:  array_merge(...$nested);
来源：http://gh.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lt.newstarts.cn

TS:   nested.flat();
来源：http://ei.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ji.lnxyls.cn

Go:   // 手写双层循环
来源：http://fv.panjiajie.cn

Ruby: nested.flatten
来源：http://ej.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cs.szxytkj.cn

[D19] 按字段分组
来源：http://zy.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qz.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qd.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xe.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wl.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rs.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://hr.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://en.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bq.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://tz.huanxung.cn

Py:   Counter(arr)
来源：http://yq.asd995.cn

PHP:  array_count_values($arr);
来源：http://sv.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tp.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fa.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cd.nicolike.cn

Go:   // 手写 map[T]int
来源：http://xt.hnjuh.cn

Ruby: arr.tally
来源：http://pc.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zj.huanxung.cn

[D21] 判断是否包含某元素
来源：http://ri.newstarts.cn

Py:   x in arr
来源：http://fe.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://ch.hnjuh.cn

JS:   arr.includes(x)
来源：http://ox.lnxyls.cn

TS:   arr.includes(x)
来源：http://rn.colortex.cn

Java: list.contains(x)
来源：http://ge.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://hy.shxzukj.cn

Ruby: arr.include?(x)
来源：http://dt.panjiajie.cn

C#:   list.Contains(x)
来源：http://df.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://qv.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gu.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ad.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pi.colortex.cn

TS:   [...arr];
来源：http://sn.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://cg.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xx.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://wv.szxytkj.cn

C#:   new List<int>(list);
来源：http://qc.huixiangedu.cn

[D23] reduce 累积计算
来源：http://ss.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bg.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oc.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tk.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://df.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dz.lnxyls.cn

Go:   // 手写循环
来源：http://nk.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fs.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vv.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://fw.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rg.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kq.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kx.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bz.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://df.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mb.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cc.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fo.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://om.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mj.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mc.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pq.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ew.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pu.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://if.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://va.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aa.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://xa.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://tw.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://ok.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://fw.haigaiapp.cn

TS:   arr.join(", ")
来源：http://lm.huixiangedu.cn


<!-- 参考信息 -->