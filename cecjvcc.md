代发 wailian999

C#:   块级作用域
来源：http://we.huanxung.cn

[C11] 模块导入与导出
来源：http://br.huixinmuqiang.cn

Py:   from module import func
来源：http://ol.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yh.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mk.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ya.jctech888.com.cn

Java: import java.util.List;
来源：http://jo.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://br.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://qr.colortex.cn

C#:   using System.Text;
来源：http://od.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://up.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://fs.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://yx.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://ft.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://iw.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://co.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://gb.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://fr.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ui.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://kh.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ax.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kl.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fh.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fz.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rt.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://pq.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ts.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kp.521024.cn

[C14] 泛型函数
来源：http://ix.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kk.lnxyls.cn

PHP:  // 无泛型
来源：http://zi.wgjwhj.cn

JS:   // 无泛型
来源：http://qy.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ej.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tf.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qm.gzmigu.cn

Ruby: # 无泛型
来源：http://mg.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yf.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://dv.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ie.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://lh.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ng.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ew.9csxet.cn

Java: // 无解构
来源：http://nd.huixinmuqiang.cn

Go:   // 无解构
来源：http://zp.huixiangedu.cn

Ruby: a, b = pair
来源：http://ot.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://wf.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://bm.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bi.wgjwhj.cn

PHP:  // 无重载
来源：http://vj.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mx.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ov.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://eg.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://lm.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://nw.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lp.lnxyls.cn

================================================================================
来源：http://bk.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://db.newstarts.cn

================================================================================
来源：http://dc.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://ou.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rb.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rl.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cx.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rg.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gj.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://xp.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://no.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wx.asd995.cn

[D02] 追加元素到末尾
来源：http://zc.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hv.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kv.chemitech.net.cn

JS:   arr.push(4);
来源：http://ow.bjjhwx.cn

TS:   arr.push(4);
来源：http://od.wgjwhj.cn

Java: list.add(4);
来源：http://og.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://lc.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://uj.chemitech.net.cn

C#:   list.Add(4);
来源：http://te.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://rp.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://dg.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zf.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yl.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://wa.hnjuh.cn

Java: list.add(0, 0);
来源：http://ll.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://la.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://au.colortex.cn

C#:   list.Insert(0, 0);
来源：http://bo.asd995.cn

[D04] 删除元素
来源：http://ak.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vm.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mo.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ah.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://yb.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kb.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jv.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rx.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://og.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://xb.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oe.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gp.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rg.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://rg.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://tk.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://jn.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://br.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xf.521024.cn

[D06] 数组长度
来源：http://tu.nicolike.cn

Py:   len(arr)
来源：http://vl.jctech888.com.cn

PHP:  count($arr);
来源：http://ou.hnjuh.cn

JS:   arr.length
来源：http://ot.chemitech.net.cn

TS:   arr.length
来源：http://dt.haigaiapp.cn

Java: list.size();
来源：http://ny.huixiangedu.cn

Go:   len(arr)
来源：http://fh.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://lj.521024.cn

C#:   list.Count;
来源：http://cv.szsharing.cn

[D07] 切片 / 取子数组
来源：http://qk.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jq.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jv.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://pl.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ju.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://gy.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://nr.huanxung.cn

Ruby: arr[1, 3]
来源：http://eg.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://sa.wgjwhj.cn

[D08] 合并两个数组
来源：http://fm.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://iu.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://jh.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mb.shxzskj.cn

TS:   [...a, ...b];
来源：http://xn.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yu.lnxyls.cn

Go:   append(a, b...)
来源：http://rv.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://nv.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://oz.nicolike.cn

[D09] 排序（升序）
来源：http://vb.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://sb.lnxyls.cn

PHP:  sort($arr);
来源：http://xc.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gf.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lo.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eu.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pc.shxzukj.cn

Ruby: arr.sort
来源：http://gy.nszjky.cn

C#:   list.Sort();
来源：http://bq.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mh.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sp.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jj.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ah.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zl.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lo.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://my.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gu.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mn.hnjuh.cn

[D11] 反转数组
来源：http://bt.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cg.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://fy.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nf.521024.cn

TS:   [...arr].reverse();
来源：http://ja.panjiajie.cn

Java: Collections.reverse(list);
来源：http://yk.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://kw.nicolike.cn

Ruby: arr.reverse
来源：http://oc.lnxyls.cn

C#:   list.Reverse();
来源：http://ny.huixiangedu.cn

[D12] 查找元素下标
来源：http://xt.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://eo.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gf.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://es.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lc.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://su.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://xd.nszjky.cn

Ruby: arr.index(x)
来源：http://qi.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://qu.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://wp.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ft.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ap.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://rn.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://qo.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bc.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rz.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ig.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hh.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://fg.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qg.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ef.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://hz.521024.cn

TS:   arr.map(x => x * 2)
来源：http://de.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ch.panjiajie.cn

Go:   // 手写循环
来源：http://dn.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dt.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pz.hnjuh.cn

[D15] 去重
来源：http://fn.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jm.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://kv.521024.cn

JS:   [...new Set(arr)]
来源：http://au.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://gz.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uk.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ey.hahajie.cn

Ruby: arr.uniq
来源：http://nw.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://ly.jctech888.com.cn

[D16] 求和与平均值
来源：http://fp.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mt.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eb.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://no.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pc.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bl.panjiajie.cn

Go:   // 手写循环累加
来源：http://al.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vx.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://tk.shxzskj.cn

[D17] 最大值与最小值
来源：http://cr.asd995.cn

Py:   max(arr);  min(arr)
来源：http://df.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://ny.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://po.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://de.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jb.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jt.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://cg.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://yz.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://lu.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://di.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://hs.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fe.muxihuayi.cn

TS:   nested.flat();
来源：http://ht.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wo.chemitech.net.cn

Go:   // 手写双层循环
来源：http://uy.hnjuh.cn

Ruby: nested.flatten
来源：http://yk.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://os.szxytkj.cn

[D19] 按字段分组
来源：http://je.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cp.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tl.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rm.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ye.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ax.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://ke.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ah.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cq.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://st.nszjky.cn

Py:   Counter(arr)
来源：http://go.nszjky.cn

PHP:  array_count_values($arr);
来源：http://bm.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hw.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jk.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xo.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://ox.hahajie.cn

Ruby: arr.tally
来源：http://iq.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ez.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://xb.521024.cn

Py:   x in arr
来源：http://mt.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://kq.shxzskj.cn

JS:   arr.includes(x)
来源：http://kx.haigaiapp.cn

TS:   arr.includes(x)
来源：http://wk.asd995.cn

Java: list.contains(x)
来源：http://el.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://lh.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://nj.wgjwhj.cn

C#:   list.Contains(x)
来源：http://kz.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://ca.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ls.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ex.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pb.yuntaijiaju.cn

TS:   [...arr];
来源：http://sz.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://we.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ek.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://za.asd995.cn

C#:   new List<int>(list);
来源：http://mf.panjiajie.cn

[D23] reduce 累积计算
来源：http://kd.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lg.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ol.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dn.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nk.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://le.asd995.cn

Go:   // 手写循环
来源：http://ka.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ko.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yp.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://qy.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pq.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mf.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nb.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ou.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lu.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dd.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://es.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vr.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://jk.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fs.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://db.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://md.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wo.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ud.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nl.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tz.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fo.bookmarksfly.cn

[D26] 数组转字符串
来源：http://fu.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://hc.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://kn.shtwfgs.cn

JS:   arr.join(", ")
来源：http://kz.gzmigu.cn

TS:   arr.join(", ")
来源：http://si.nicolike.cn

Java: String.join(", ", list)
来源：http://gp.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://cd.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://lg.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://cw.huixiangedu.cn

================================================================================
来源：http://lg.muxihuayi.cn

E. 字符串处理
来源：http://uk.colortex.cn

================================================================================
来源：http://hn.shxzskj.cn

[E01] 拼接字符串
来源：http://ll.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bd.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tl.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://id.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vh.9csxet.cn


<!-- 参考信息 -->