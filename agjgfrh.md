代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kk.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pg.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wm.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yf.hahajie.cn

[C10] 变量作用域
来源：http://ba.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pe.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://md.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zw.hnjuh.cn

TS:   同 JS
来源：http://xb.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://bf.bjjhwx.cn

Go:   花括号块级作用域
来源：http://tu.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fk.jianghongdianzi.cn

C#:   块级作用域
来源：http://go.nicolike.cn

[C11] 模块导入与导出
来源：http://bp.shxzskj.cn

Py:   from module import func
来源：http://gc.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ll.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jc.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ef.yuexingan06.cn

Java: import java.util.List;
来源：http://ak.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bn.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://xx.newstarts.cn

C#:   using System.Text;
来源：http://oa.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://xu.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://is.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://no.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://zl.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://oy.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aj.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://se.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://zy.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ol.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://tj.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pb.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xw.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zq.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://km.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cx.asd995.cn

Go:   func add(a, b int) int
来源：http://aa.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kz.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hd.hahajie.cn

[C14] 泛型函数
来源：http://bc.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kq.jctech888.com.cn

PHP:  // 无泛型
来源：http://jh.9csxet.cn

JS:   // 无泛型
来源：http://le.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jp.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jh.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ie.lnxyls.cn

Ruby: # 无泛型
来源：http://zb.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://br.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://xg.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bo.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://qh.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uu.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cm.wgjwhj.cn

Java: // 无解构
来源：http://ev.huixinmuqiang.cn

Go:   // 无解构
来源：http://xu.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://lu.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://mn.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://tm.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gj.yuexingan06.cn

PHP:  // 无重载
来源：http://ya.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yv.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://oy.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gh.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://dl.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://wo.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jn.huanxung.cn

================================================================================
来源：http://um.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://mq.yuexingan06.cn

================================================================================
来源：http://rg.nicolike.cn

[D01] 创建数组 / 列表
来源：http://lu.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ma.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ja.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mo.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fd.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://za.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://uo.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://it.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yj.panjiajie.cn

[D02] 追加元素到末尾
来源：http://jp.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sj.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xd.gzmigu.cn

JS:   arr.push(4);
来源：http://fj.colortex.cn

TS:   arr.push(4);
来源：http://qt.szsharing.cn

Java: list.add(4);
来源：http://hd.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://nv.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://az.haigaiapp.cn

C#:   list.Add(4);
来源：http://jq.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://ah.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://rn.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sl.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aq.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://eb.bjjhwx.cn

Java: list.add(0, 0);
来源：http://bt.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lf.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qj.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://uu.szxytkj.cn

[D04] 删除元素
来源：http://qf.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mb.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yj.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oc.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://eg.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zf.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sl.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mv.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ua.szsharing.cn

[D05] 访问与修改元素
来源：http://wh.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wj.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dg.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sj.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://bz.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://gt.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://yf.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://in.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pg.huanxung.cn

[D06] 数组长度
来源：http://nq.chemitech.net.cn

Py:   len(arr)
来源：http://gy.hahajie.cn

PHP:  count($arr);
来源：http://iw.9csxet.cn

JS:   arr.length
来源：http://tp.huanxung.cn

TS:   arr.length
来源：http://ci.huanxung.cn

Java: list.size();
来源：http://ku.muxihuayi.cn

Go:   len(arr)
来源：http://yk.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://xz.lnxyls.cn

C#:   list.Count;
来源：http://jx.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://zr.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://km.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vg.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://gc.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://gl.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://ta.nicolike.cn

Go:   arr[1:4]
来源：http://fx.szsharing.cn

Ruby: arr[1, 3]
来源：http://gs.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://ab.newstarts.cn

[D08] 合并两个数组
来源：http://bt.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://wr.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://bv.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kz.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://fl.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wi.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://rq.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://wt.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://bn.colortex.cn

[D09] 排序（升序）
来源：http://ps.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://kv.szsharing.cn

PHP:  sort($arr);
来源：http://et.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qd.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ye.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rv.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nw.yuexingan06.cn

Ruby: arr.sort
来源：http://tl.panjiajie.cn

C#:   list.Sort();
来源：http://rs.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pq.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jo.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vx.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yd.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pq.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zo.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pq.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bz.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aq.colortex.cn

[D11] 反转数组
来源：http://nu.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fx.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://dd.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qk.shxzskj.cn

TS:   [...arr].reverse();
来源：http://ye.nicolike.cn

Java: Collections.reverse(list);
来源：http://yi.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://bt.asd995.cn

Ruby: arr.reverse
来源：http://gh.wgjwhj.cn

C#:   list.Reverse();
来源：http://yj.panjiajie.cn

[D12] 查找元素下标
来源：http://hh.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://cm.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gc.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vp.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lv.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://se.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://sm.haigaiapp.cn

Ruby: arr.index(x)
来源：http://ca.9csxet.cn

C#:   list.IndexOf(x);
来源：http://sm.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://ec.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mt.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://db.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://ks.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://ra.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tc.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://or.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hn.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dj.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://by.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yl.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yq.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://fy.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://og.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bp.huixiangedu.cn

Go:   // 手写循环
来源：http://wf.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bz.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kf.hahajie.cn

[D15] 去重
来源：http://yu.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sv.shxzskj.cn

PHP:  array_unique($arr);
来源：http://sy.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://tv.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://nz.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lg.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pe.lnxyls.cn

Ruby: arr.uniq
来源：http://bo.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://yz.szsharing.cn

[D16] 求和与平均值
来源：http://or.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ac.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ff.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tt.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xp.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nw.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://jp.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ss.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://lp.wgjwhj.cn

[D17] 最大值与最小值
来源：http://it.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://nj.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://bc.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://py.shxzskj.cn

TS:   Math.max(...arr);
来源：http://nm.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rg.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tq.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://ba.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://yu.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://we.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://li.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://oo.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sw.521024.cn

TS:   nested.flat();
来源：http://dl.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kg.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://ut.muxihuayi.cn

Ruby: nested.flatten
来源：http://rb.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jk.jctech888.com.cn

[D19] 按字段分组
来源：http://cs.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kf.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bz.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://la.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fu.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dh.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://qo.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rm.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yo.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://pp.szxytkj.cn

Py:   Counter(arr)
来源：http://od.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://ug.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xe.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gv.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jg.szsharing.cn

Go:   // 手写 map[T]int
来源：http://tb.wgjwhj.cn

Ruby: arr.tally
来源：http://da.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hi.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://ot.yuexingan06.cn

Py:   x in arr
来源：http://jc.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://rt.yuexingan06.cn

JS:   arr.includes(x)
来源：http://tb.szxytkj.cn

TS:   arr.includes(x)
来源：http://mi.muxihuayi.cn

Java: list.contains(x)
来源：http://tx.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://zp.newstarts.cn

Ruby: arr.include?(x)
来源：http://qd.chemitech.net.cn

C#:   list.Contains(x)
来源：http://ra.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://qt.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uu.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fk.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lw.szxytkj.cn

TS:   [...arr];
来源：http://rt.nicolike.cn

Java: new ArrayList<>(list);
来源：http://yc.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sa.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://xg.wgjwhj.cn

C#:   new List<int>(list);
来源：http://bj.asd995.cn

[D23] reduce 累积计算
来源：http://gh.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oi.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vn.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wj.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ym.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qv.yuntaijiaju.cn

Go:   // 手写循环
来源：http://up.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hv.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ov.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://fk.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mk.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ch.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bn.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ng.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zx.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yd.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yb.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://io.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://hf.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ln.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nk.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vb.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://em.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lc.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hw.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://km.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ju.shxzskj.cn

[D26] 数组转字符串
来源：http://mp.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://lb.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://ha.haigaiapp.cn

JS:   arr.join(", ")
来源：http://td.jctech888.com.cn

TS:   arr.join(", ")
来源：http://cr.yuntaijiaju.cn


<!-- 参考信息 -->