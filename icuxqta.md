代发 wailian999

TS:   同 JS
来源：http://qd.shxzukj.cn

Java: 方法内为块级作用域
来源：http://gt.chemitech.net.cn

Go:   花括号块级作用域
来源：http://uh.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cn.muxihuayi.cn

C#:   块级作用域
来源：http://ki.nicolike.cn

[C11] 模块导入与导出
来源：http://gg.chemitech.net.cn

Py:   from module import func
来源：http://dy.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tl.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uc.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hb.szxytkj.cn

Java: import java.util.List;
来源：http://me.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sd.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://rp.newstarts.cn

C#:   using System.Text;
来源：http://gf.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://nd.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://ab.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://va.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://oq.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://to.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cv.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://wa.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://tv.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tl.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://mz.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sm.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://io.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dl.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qz.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cz.lnxyls.cn

Go:   func add(a, b int) int
来源：http://ma.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ta.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://na.newstarts.cn

[C14] 泛型函数
来源：http://bl.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gr.asd995.cn

PHP:  // 无泛型
来源：http://vy.chemitech.net.cn

JS:   // 无泛型
来源：http://vr.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dt.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rw.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://so.shxzukj.cn

Ruby: # 无泛型
来源：http://on.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ux.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://vg.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://us.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://ki.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fh.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yk.haigaiapp.cn

Java: // 无解构
来源：http://eh.gzmigu.cn

Go:   // 无解构
来源：http://vg.asd995.cn

Ruby: a, b = pair
来源：http://ae.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://zn.asd995.cn

[C16] 函数 / 方法重载
来源：http://gt.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ny.haigaiapp.cn

PHP:  // 无重载
来源：http://ys.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fe.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://fy.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://om.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://rx.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://uc.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nm.yuexingan06.cn

================================================================================
来源：http://xy.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://mn.panjiajie.cn

================================================================================
来源：http://ea.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://aw.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kk.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ry.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yu.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nc.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ht.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://yi.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://kx.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://px.hahajie.cn

[D02] 追加元素到末尾
来源：http://ri.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vi.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://go.shtwfgs.cn

JS:   arr.push(4);
来源：http://gn.hnjuh.cn

TS:   arr.push(4);
来源：http://qr.hahajie.cn

Java: list.add(4);
来源：http://bd.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://yf.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://fc.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://vg.9csxet.cn

[D03] 在指定位置插入元素
来源：http://mi.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://co.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uh.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dc.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://op.shtwfgs.cn

Java: list.add(0, 0);
来源：http://xi.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cp.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hh.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://wk.lnxyls.cn

[D04] 删除元素
来源：http://cb.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wj.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pm.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vu.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://cn.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ub.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wr.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ap.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://np.wgjwhj.cn

[D05] 访问与修改元素
来源：http://ia.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qr.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yu.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bf.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://cq.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://dn.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://ny.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wu.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://df.hnjuh.cn

[D06] 数组长度
来源：http://sg.colortex.cn

Py:   len(arr)
来源：http://wn.yuexingan06.cn

PHP:  count($arr);
来源：http://gi.wgjwhj.cn

JS:   arr.length
来源：http://uv.panjiajie.cn

TS:   arr.length
来源：http://om.huanxung.cn

Java: list.size();
来源：http://ef.lnxyls.cn

Go:   len(arr)
来源：http://ph.9csxet.cn

Ruby: arr.length; arr.size
来源：http://tu.haigaiapp.cn

C#:   list.Count;
来源：http://gk.asd995.cn

[D07] 切片 / 取子数组
来源：http://vr.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ir.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tv.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://sc.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://mt.asd995.cn

Java: list.subList(1, 4);
来源：http://ex.bookmarksfly.cn

Go:   arr[1:4]
来源：http://rk.newstarts.cn

Ruby: arr[1, 3]
来源：http://la.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://em.huixiangedu.cn

[D08] 合并两个数组
来源：http://fz.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://uz.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://nq.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ub.newstarts.cn

TS:   [...a, ...b];
来源：http://bl.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dm.nszjky.cn

Go:   append(a, b...)
来源：http://ky.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://jh.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://og.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://tb.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://yp.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://ae.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ak.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cs.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ci.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xo.muxihuayi.cn

Ruby: arr.sort
来源：http://bg.shtwfgs.cn

C#:   list.Sort();
来源：http://yp.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wk.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fy.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tg.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zn.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cf.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dw.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rh.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qo.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ls.haigaiapp.cn

[D11] 反转数组
来源：http://cg.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pt.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://bc.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wy.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://gy.huanxung.cn

Java: Collections.reverse(list);
来源：http://jh.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://ik.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://wr.panjiajie.cn

C#:   list.Reverse();
来源：http://uf.bjjhwx.cn

[D12] 查找元素下标
来源：http://ft.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://zo.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://df.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eb.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fx.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iz.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://hb.nicolike.cn

Ruby: arr.index(x)
来源：http://xr.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://sr.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://pd.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ej.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rn.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://rj.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://ox.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ri.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nr.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xc.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qv.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://vy.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ic.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kn.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://wr.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://qz.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sx.lnxyls.cn

Go:   // 手写循环
来源：http://lc.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pn.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oj.bjjhwx.cn

[D15] 去重
来源：http://jr.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vn.asd995.cn

PHP:  array_unique($arr);
来源：http://pr.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://xf.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://ii.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yp.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ja.szsharing.cn

Ruby: arr.uniq
来源：http://jp.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://oz.hahajie.cn

[D16] 求和与平均值
来源：http://me.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bg.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ui.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nm.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://te.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sa.nszjky.cn

Go:   // 手写循环累加
来源：http://vd.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tb.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://lx.hahajie.cn

[D17] 最大值与最小值
来源：http://jd.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://ew.521024.cn

PHP:  max($arr);  min($arr);
来源：http://pb.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gc.hnjuh.cn

TS:   Math.max(...arr);
来源：http://gi.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gp.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qs.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://sx.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://ay.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://fb.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ft.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://sq.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ol.huixiangedu.cn

TS:   nested.flat();
来源：http://nk.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qr.shxzskj.cn

Go:   // 手写双层循环
来源：http://cb.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://rv.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gz.panjiajie.cn

[D19] 按字段分组
来源：http://zx.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pp.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yi.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ws.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nc.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ve.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://hp.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zv.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ju.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://rp.wgjwhj.cn

Py:   Counter(arr)
来源：http://yy.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://ty.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tg.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oq.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://di.colortex.cn

Go:   // 手写 map[T]int
来源：http://gy.gzmigu.cn

Ruby: arr.tally
来源：http://al.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zg.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://re.bookmarksfly.cn

Py:   x in arr
来源：http://bn.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://ph.huixiangedu.cn

JS:   arr.includes(x)
来源：http://nh.colortex.cn

TS:   arr.includes(x)
来源：http://ta.wgjwhj.cn

Java: list.contains(x)
来源：http://zv.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://jr.asd995.cn

Ruby: arr.include?(x)
来源：http://mi.lnxyls.cn

C#:   list.Contains(x)
来源：http://ai.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://pv.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gd.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jq.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hr.jianghongdianzi.cn

TS:   [...arr];
来源：http://ua.hahajie.cn

Java: new ArrayList<>(list);
来源：http://lx.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cm.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://ul.nicolike.cn

C#:   new List<int>(list);
来源：http://ki.shxzskj.cn

[D23] reduce 累积计算
来源：http://gt.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pe.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mz.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tw.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bs.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vx.colortex.cn

Go:   // 手写循环
来源：http://ln.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://le.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://su.521024.cn

[D24] 字典 / Map 基本操作
来源：http://bp.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uy.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oi.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ub.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hq.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gx.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iz.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nk.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bk.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://pl.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kb.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gu.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nx.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dc.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tg.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xx.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cu.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dw.shxzskj.cn

[D26] 数组转字符串
来源：http://yc.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://mq.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://mx.nicolike.cn

JS:   arr.join(", ")
来源：http://av.nszjky.cn

TS:   arr.join(", ")
来源：http://cu.asd995.cn

Java: String.join(", ", list)
来源：http://xr.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://kw.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://ei.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://kf.9csxet.cn

================================================================================
来源：http://ic.bookmarksfly.cn

E. 字符串处理
来源：http://uj.newstarts.cn

================================================================================
来源：http://kp.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://uc.gzmigu.cn


<!-- 参考信息 -->