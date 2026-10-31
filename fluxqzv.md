代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mq.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ru.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eb.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cq.shxzskj.cn

[C10] 变量作用域
来源：http://us.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yv.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ae.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ec.yuexingan06.cn

TS:   同 JS
来源：http://jo.nicolike.cn

Java: 方法内为块级作用域
来源：http://es.szsharing.cn

Go:   花括号块级作用域
来源：http://vu.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cw.shxzskj.cn

C#:   块级作用域
来源：http://bq.jctech888.com.cn

[C11] 模块导入与导出
来源：http://rw.9csxet.cn

Py:   from module import func
来源：http://so.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aw.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://po.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://du.newstarts.cn

Java: import java.util.List;
来源：http://yh.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sb.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://wa.bookmarksfly.cn

C#:   using System.Text;
来源：http://np.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://jc.521024.cn

Py:   (lambda: print("run"))()
来源：http://jt.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://fd.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://ny.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://in.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xn.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://gm.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://hw.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xv.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://ze.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sr.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ek.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://to.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://md.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vw.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://ji.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xd.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qx.shxzukj.cn

[C14] 泛型函数
来源：http://gc.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://et.muxihuayi.cn

PHP:  // 无泛型
来源：http://vo.9csxet.cn

JS:   // 无泛型
来源：http://lk.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fa.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://er.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dt.huanxung.cn

Ruby: # 无泛型
来源：http://va.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yg.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://tv.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nm.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://ve.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bg.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dj.muxihuayi.cn

Java: // 无解构
来源：http://nw.wgjwhj.cn

Go:   // 无解构
来源：http://vz.lnxyls.cn

Ruby: a, b = pair
来源：http://vx.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://oc.521024.cn

[C16] 函数 / 方法重载
来源：http://ww.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fu.wgjwhj.cn

PHP:  // 无重载
来源：http://bz.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jx.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ws.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gk.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ta.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://aq.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ya.huixiangedu.cn

================================================================================
来源：http://ce.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://uf.panjiajie.cn

================================================================================
来源：http://gm.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://qt.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ix.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qv.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wy.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://as.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ap.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://th.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://cd.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fz.szsharing.cn

[D02] 追加元素到末尾
来源：http://xh.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ed.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tc.newstarts.cn

JS:   arr.push(4);
来源：http://pj.9csxet.cn

TS:   arr.push(4);
来源：http://na.lnxyls.cn

Java: list.add(4);
来源：http://di.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://qa.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://lc.nicolike.cn

C#:   list.Add(4);
来源：http://dw.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://fc.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://vc.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hq.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wz.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://rd.jctech888.com.cn

Java: list.add(0, 0);
来源：http://nd.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cm.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jr.asd995.cn

C#:   list.Insert(0, 0);
来源：http://uz.newstarts.cn

[D04] 删除元素
来源：http://jp.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ri.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mf.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oi.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://bt.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jg.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pc.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zl.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ob.521024.cn

[D05] 访问与修改元素
来源：http://ry.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kq.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cz.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pd.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://rp.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://xt.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://vn.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ji.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vg.nszjky.cn

[D06] 数组长度
来源：http://jm.muxihuayi.cn

Py:   len(arr)
来源：http://uj.huanxung.cn

PHP:  count($arr);
来源：http://yb.haigaiapp.cn

JS:   arr.length
来源：http://xh.shxzskj.cn

TS:   arr.length
来源：http://tt.huixinmuqiang.cn

Java: list.size();
来源：http://hm.bjjhwx.cn

Go:   len(arr)
来源：http://fw.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://te.hnjuh.cn

C#:   list.Count;
来源：http://vj.hahajie.cn

[D07] 切片 / 取子数组
来源：http://vm.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zw.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sw.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://ti.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://cf.nicolike.cn

Java: list.subList(1, 4);
来源：http://sx.szsharing.cn

Go:   arr[1:4]
来源：http://rk.lnxyls.cn

Ruby: arr[1, 3]
来源：http://xb.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://vm.huixiangedu.cn

[D08] 合并两个数组
来源：http://va.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://sy.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://pb.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://va.chemitech.net.cn

TS:   [...a, ...b];
来源：http://kq.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zt.haigaiapp.cn

Go:   append(a, b...)
来源：http://ko.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://ai.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://zt.yuexingan06.cn

[D09] 排序（升序）
来源：http://um.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://nn.9csxet.cn

PHP:  sort($arr);
来源：http://vo.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iz.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yr.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uv.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zl.lnxyls.cn

Ruby: arr.sort
来源：http://se.huanxung.cn

C#:   list.Sort();
来源：http://ps.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bx.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ol.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ch.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kf.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sr.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xb.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ne.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rq.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zu.521024.cn

[D11] 反转数组
来源：http://tg.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bb.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://cs.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rr.hahajie.cn

TS:   [...arr].reverse();
来源：http://iq.shxzukj.cn

Java: Collections.reverse(list);
来源：http://ub.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://mq.jctech888.com.cn

Ruby: arr.reverse
来源：http://gn.panjiajie.cn

C#:   list.Reverse();
来源：http://en.panjiajie.cn

[D12] 查找元素下标
来源：http://yb.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://ve.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ot.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://so.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gd.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jh.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://aq.nicolike.cn

Ruby: arr.index(x)
来源：http://rd.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://yu.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://dt.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ma.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ie.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ir.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://fr.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fz.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dh.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nw.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vg.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://xr.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qm.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ko.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://km.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://fu.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gp.colortex.cn

Go:   // 手写循环
来源：http://oc.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ht.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fg.shtwfgs.cn

[D15] 去重
来源：http://nl.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sd.shxzskj.cn

PHP:  array_unique($arr);
来源：http://mo.asd995.cn

JS:   [...new Set(arr)]
来源：http://pz.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://fg.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pc.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://te.bjjhwx.cn

Ruby: arr.uniq
来源：http://nt.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://sk.shxzskj.cn

[D16] 求和与平均值
来源：http://jn.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hb.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qr.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xt.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://if.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yv.lnxyls.cn

Go:   // 手写循环累加
来源：http://ur.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sx.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://xi.nicolike.cn

[D17] 最大值与最小值
来源：http://ey.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://jj.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://sh.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://du.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://bu.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dv.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bs.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://ez.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://ci.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://fx.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://di.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://uf.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bc.chemitech.net.cn

TS:   nested.flat();
来源：http://dc.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://al.9csxet.cn

Go:   // 手写双层循环
来源：http://kd.bjjhwx.cn

Ruby: nested.flatten
来源：http://vq.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ii.jianghongdianzi.cn

[D19] 按字段分组
来源：http://ry.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pb.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qb.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vm.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bx.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lo.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://zs.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uw.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://up.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://ij.szsharing.cn

Py:   Counter(arr)
来源：http://oi.asd995.cn

PHP:  array_count_values($arr);
来源：http://bk.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zb.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ky.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yn.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://or.szsharing.cn

Ruby: arr.tally
来源：http://ec.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vi.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://fp.bjjhwx.cn

Py:   x in arr
来源：http://pb.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://ii.nszjky.cn

JS:   arr.includes(x)
来源：http://sd.panjiajie.cn

TS:   arr.includes(x)
来源：http://br.521024.cn

Java: list.contains(x)
来源：http://qv.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://it.gzmigu.cn

Ruby: arr.include?(x)
来源：http://vj.huanxung.cn

C#:   list.Contains(x)
来源：http://ld.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://ob.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vs.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mw.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yt.jianghongdianzi.cn

TS:   [...arr];
来源：http://rb.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://ep.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://st.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://cg.huixiangedu.cn

C#:   new List<int>(list);
来源：http://xv.hahajie.cn

[D23] reduce 累积计算
来源：http://gd.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://be.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tp.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pj.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mt.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xa.hahajie.cn

Go:   // 手写循环
来源：http://mg.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ci.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tl.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://or.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://up.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://em.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://in.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fp.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bj.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dd.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kb.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hx.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://fs.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cd.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zf.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hc.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hw.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://al.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://og.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jd.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qu.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://gl.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://bo.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://ur.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://hd.shxzskj.cn

TS:   arr.join(", ")
来源：http://vq.shtwfgs.cn


<!-- 参考信息 -->