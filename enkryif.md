代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wj.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xj.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jw.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yg.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kf.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lr.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iw.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zm.shxzskj.cn

[C10] 变量作用域
来源：http://zf.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gh.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dw.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tq.yuexingan06.cn

TS:   同 JS
来源：http://kd.lnxyls.cn

Java: 方法内为块级作用域
来源：http://te.shtwfgs.cn

Go:   花括号块级作用域
来源：http://oc.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uq.shxzukj.cn

C#:   块级作用域
来源：http://ek.shxzukj.cn

[C11] 模块导入与导出
来源：http://hb.hnjuh.cn

Py:   from module import func
来源：http://eq.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fu.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fl.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ru.nszjky.cn

Java: import java.util.List;
来源：http://ya.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cu.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ca.panjiajie.cn

C#:   using System.Text;
来源：http://mc.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://yy.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://as.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://bd.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://zb.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://gf.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ln.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://lg.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ky.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jm.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://qo.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wq.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fh.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uf.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ks.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ns.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://vh.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jo.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bb.shxzskj.cn

[C14] 泛型函数
来源：http://lk.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://md.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://fx.lnxyls.cn

JS:   // 无泛型
来源：http://ov.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ub.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ja.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sa.muxihuayi.cn

Ruby: # 无泛型
来源：http://ae.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wo.hahajie.cn

[C15] 解构 / 展开参数
来源：http://bk.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://em.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://cc.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ho.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wf.colortex.cn

Java: // 无解构
来源：http://em.bjjhwx.cn

Go:   // 无解构
来源：http://kq.shxzskj.cn

Ruby: a, b = pair
来源：http://iu.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://oa.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://bd.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ta.lnxyls.cn

PHP:  // 无重载
来源：http://al.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qq.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://gk.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ae.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://lt.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://yh.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yo.bjjhwx.cn

================================================================================
来源：http://lv.asd995.cn

D. 数组 / 列表 / 集合
来源：http://ez.wgjwhj.cn

================================================================================
来源：http://av.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://yh.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fh.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eb.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lx.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eq.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pu.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://su.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ls.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cc.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://aa.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nw.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bt.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://ts.lnxyls.cn

TS:   arr.push(4);
来源：http://vf.hahajie.cn

Java: list.add(4);
来源：http://iy.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://pv.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://zk.hnjuh.cn

C#:   list.Add(4);
来源：http://kj.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ka.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://ij.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://on.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tz.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://xr.9csxet.cn

Java: list.add(0, 0);
来源：http://vk.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lr.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jz.521024.cn

C#:   list.Insert(0, 0);
来源：http://he.yuexingan06.cn

[D04] 删除元素
来源：http://rc.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fa.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://li.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hu.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://xe.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dk.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ss.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xr.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jv.bjjhwx.cn

[D05] 访问与修改元素
来源：http://fl.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wj.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fr.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gw.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://la.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://kz.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://jo.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mq.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aw.muxihuayi.cn

[D06] 数组长度
来源：http://cq.szsharing.cn

Py:   len(arr)
来源：http://qu.jctech888.com.cn

PHP:  count($arr);
来源：http://je.shxzukj.cn

JS:   arr.length
来源：http://lm.newstarts.cn

TS:   arr.length
来源：http://so.huixiangedu.cn

Java: list.size();
来源：http://dx.shxzskj.cn

Go:   len(arr)
来源：http://gs.521024.cn

Ruby: arr.length; arr.size
来源：http://vl.jianghongdianzi.cn

C#:   list.Count;
来源：http://gg.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://rp.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jd.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nx.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://tg.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://ru.9csxet.cn

Java: list.subList(1, 4);
来源：http://se.colortex.cn

Go:   arr[1:4]
来源：http://ia.newstarts.cn

Ruby: arr[1, 3]
来源：http://kl.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://ej.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://pl.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://jl.521024.cn

PHP:  array_merge($a, $b);
来源：http://wo.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vu.newstarts.cn

TS:   [...a, ...b];
来源：http://xr.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yn.newstarts.cn

Go:   append(a, b...)
来源：http://iw.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://kq.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://uw.asd995.cn

[D09] 排序（升序）
来源：http://uz.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://sq.bjjhwx.cn

PHP:  sort($arr);
来源：http://rs.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nw.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pl.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tx.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kh.nszjky.cn

Ruby: arr.sort
来源：http://ss.jianghongdianzi.cn

C#:   list.Sort();
来源：http://aa.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vs.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kk.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://th.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jh.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://br.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pb.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://of.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://se.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cw.bjjhwx.cn

[D11] 反转数组
来源：http://pk.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rw.521024.cn

PHP:  array_reverse($arr);
来源：http://ii.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://te.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://oz.hnjuh.cn

Java: Collections.reverse(list);
来源：http://tg.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://ku.521024.cn

Ruby: arr.reverse
来源：http://ah.nszjky.cn

C#:   list.Reverse();
来源：http://sv.shxzskj.cn

[D12] 查找元素下标
来源：http://gb.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://zh.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mw.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sj.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ol.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wp.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://pi.haigaiapp.cn

Ruby: arr.index(x)
来源：http://td.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://zv.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://lg.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nz.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ra.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://ju.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://qg.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gm.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kd.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oz.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ix.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://jb.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ho.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ru.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://vv.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://qw.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zr.huixiangedu.cn

Go:   // 手写循环
来源：http://tz.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wm.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jv.szsharing.cn

[D15] 去重
来源：http://tb.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ib.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://bx.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://ka.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://oa.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qq.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://um.hahajie.cn

Ruby: arr.uniq
来源：http://ne.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://lp.hahajie.cn

[D16] 求和与平均值
来源：http://tu.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://at.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cq.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kh.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bn.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://us.muxihuayi.cn

Go:   // 手写循环累加
来源：http://iv.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://al.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://nu.9csxet.cn

[D17] 最大值与最小值
来源：http://sk.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://sg.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://ef.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eb.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://qx.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ji.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pj.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://ob.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://hr.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://rb.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ia.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://ly.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wl.hahajie.cn

TS:   nested.flat();
来源：http://oz.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ho.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://hs.nicolike.cn

Ruby: nested.flatten
来源：http://lg.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jn.jianghongdianzi.cn

[D19] 按字段分组
来源：http://vz.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jx.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ac.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jv.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://um.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xx.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://oa.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jq.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nv.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://qd.lnxyls.cn

Py:   Counter(arr)
来源：http://lc.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://ia.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ep.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oy.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fd.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://xo.shtwfgs.cn

Ruby: arr.tally
来源：http://fu.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ft.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://iq.hnjuh.cn

Py:   x in arr
来源：http://ln.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://jc.chemitech.net.cn

JS:   arr.includes(x)
来源：http://oq.panjiajie.cn

TS:   arr.includes(x)
来源：http://zj.huixinmuqiang.cn

Java: list.contains(x)
来源：http://gp.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://fh.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://zi.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://bb.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://wu.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fd.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wd.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mm.yuntaijiaju.cn

TS:   [...arr];
来源：http://dj.asd995.cn

Java: new ArrayList<>(list);
来源：http://nx.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nu.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://wx.521024.cn

C#:   new List<int>(list);
来源：http://aa.wgjwhj.cn

[D23] reduce 累积计算
来源：http://bn.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sv.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qv.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uw.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cd.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tr.asd995.cn

Go:   // 手写循环
来源：http://sb.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://md.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oj.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://fv.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iu.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zo.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gs.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://en.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://as.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tc.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cn.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vq.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://bx.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://la.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ol.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nz.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eu.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cz.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://za.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ue.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cl.huanxung.cn

[D26] 数组转字符串
来源：http://ca.haigaiapp.cn


<!-- 参考信息 -->