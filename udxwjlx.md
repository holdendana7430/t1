代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xc.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oi.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oc.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gm.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gl.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cv.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wt.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jf.lnxyls.cn

[C10] 变量作用域
来源：http://rh.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hw.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yf.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mu.nicolike.cn

TS:   同 JS
来源：http://nz.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://hp.colortex.cn

Go:   花括号块级作用域
来源：http://xu.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gd.huanxung.cn

C#:   块级作用域
来源：http://ux.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://fv.shxzukj.cn

Py:   from module import func
来源：http://fo.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qc.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fb.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nm.huanxung.cn

Java: import java.util.List;
来源：http://jj.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yb.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://oe.huixinmuqiang.cn

C#:   using System.Text;
来源：http://gs.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://iu.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://ta.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://qo.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://te.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://bb.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ay.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://wm.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://so.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zw.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://qn.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ks.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ss.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jl.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oh.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zm.shxzukj.cn

Go:   func add(a, b int) int
来源：http://fc.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wx.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bq.szxytkj.cn

[C14] 泛型函数
来源：http://lz.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wf.lnxyls.cn

PHP:  // 无泛型
来源：http://up.nszjky.cn

JS:   // 无泛型
来源：http://vw.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rd.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ts.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xx.yuexingan06.cn

Ruby: # 无泛型
来源：http://ze.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pq.colortex.cn

[C15] 解构 / 展开参数
来源：http://tw.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ny.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://pe.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://le.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ec.asd995.cn

Java: // 无解构
来源：http://qg.jctech888.com.cn

Go:   // 无解构
来源：http://lq.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://ef.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://cb.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://kk.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cu.szxytkj.cn

PHP:  // 无重载
来源：http://ju.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pd.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://vd.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gp.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://sv.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://ex.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ut.9csxet.cn

================================================================================
来源：http://nt.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://lg.shxzskj.cn

================================================================================
来源：http://nz.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://lc.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zz.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uh.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bb.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bf.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vn.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://dk.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://ls.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qy.gzmigu.cn

[D02] 追加元素到末尾
来源：http://ey.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ur.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uu.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://dz.haigaiapp.cn

TS:   arr.push(4);
来源：http://gk.hnjuh.cn

Java: list.add(4);
来源：http://ee.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://ca.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://xe.yuexingan06.cn

C#:   list.Add(4);
来源：http://vy.colortex.cn

[D03] 在指定位置插入元素
来源：http://wv.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://vy.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iq.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ia.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://qe.yuexingan06.cn

Java: list.add(0, 0);
来源：http://ye.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qt.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lm.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://uk.wgjwhj.cn

[D04] 删除元素
来源：http://ap.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ju.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://td.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oq.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://ic.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lu.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ix.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cl.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ur.haigaiapp.cn

[D05] 访问与修改元素
来源：http://sg.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bg.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bw.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zo.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://wm.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://iy.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://oo.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ez.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kf.szsharing.cn

[D06] 数组长度
来源：http://cd.jctech888.com.cn

Py:   len(arr)
来源：http://wx.jianghongdianzi.cn

PHP:  count($arr);
来源：http://fj.wgjwhj.cn

JS:   arr.length
来源：http://sr.szxytkj.cn

TS:   arr.length
来源：http://mp.shxzukj.cn

Java: list.size();
来源：http://fs.lnxyls.cn

Go:   len(arr)
来源：http://zw.nicolike.cn

Ruby: arr.length; arr.size
来源：http://lu.jianghongdianzi.cn

C#:   list.Count;
来源：http://zf.newstarts.cn

[D07] 切片 / 取子数组
来源：http://ll.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://km.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://yx.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://pk.hahajie.cn

Java: list.subList(1, 4);
来源：http://hj.9csxet.cn

Go:   arr[1:4]
来源：http://ou.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://xf.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://sk.shxzukj.cn

[D08] 合并两个数组
来源：http://rn.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://br.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://ma.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rn.nicolike.cn

TS:   [...a, ...b];
来源：http://oy.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://km.haigaiapp.cn

Go:   append(a, b...)
来源：http://uf.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://kn.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://dj.szxytkj.cn

[D09] 排序（升序）
来源：http://zy.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://uq.haigaiapp.cn

PHP:  sort($arr);
来源：http://hj.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cd.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hn.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tc.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://in.9csxet.cn

Ruby: arr.sort
来源：http://al.asd995.cn

C#:   list.Sort();
来源：http://tx.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ks.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ba.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fe.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gs.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://au.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gs.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ld.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://in.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cb.asd995.cn

[D11] 反转数组
来源：http://db.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ee.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://ra.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mr.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://ym.colortex.cn

Java: Collections.reverse(list);
来源：http://pz.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://gf.haigaiapp.cn

Ruby: arr.reverse
来源：http://kt.asd995.cn

C#:   list.Reverse();
来源：http://te.bookmarksfly.cn

[D12] 查找元素下标
来源：http://qy.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://vr.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kw.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://am.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://if.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jt.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://nq.nicolike.cn

Ruby: arr.index(x)
来源：http://ax.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://ov.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://ep.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jw.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rt.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://cf.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://ld.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yv.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tb.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bg.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://em.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://dn.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yi.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ez.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://mi.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://oh.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kl.chemitech.net.cn

Go:   // 手写循环
来源：http://ke.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fy.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ro.shxzukj.cn

[D15] 去重
来源：http://ey.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qr.colortex.cn

PHP:  array_unique($arr);
来源：http://aw.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://wv.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://jz.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pd.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yg.chemitech.net.cn

Ruby: arr.uniq
来源：http://tm.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://sk.nicolike.cn

[D16] 求和与平均值
来源：http://ms.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ha.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xo.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://be.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tx.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wu.chemitech.net.cn

Go:   // 手写循环累加
来源：http://of.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zz.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://ef.nicolike.cn

[D17] 最大值与最小值
来源：http://qq.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://so.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://pf.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gl.huanxung.cn

TS:   Math.max(...arr);
来源：http://nz.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uo.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tj.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://ba.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://re.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://em.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zn.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://fh.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ur.9csxet.cn

TS:   nested.flat();
来源：http://im.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://it.nicolike.cn

Go:   // 手写双层循环
来源：http://xw.szsharing.cn

Ruby: nested.flatten
来源：http://mq.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jc.bjjhwx.cn

[D19] 按字段分组
来源：http://kc.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oh.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ty.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jw.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fs.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ag.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://hu.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fa.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fn.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://vc.muxihuayi.cn

Py:   Counter(arr)
来源：http://na.521024.cn

PHP:  array_count_values($arr);
来源：http://wl.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xn.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ui.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nq.9csxet.cn

Go:   // 手写 map[T]int
来源：http://ji.colortex.cn

Ruby: arr.tally
来源：http://en.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jx.huanxung.cn

[D21] 判断是否包含某元素
来源：http://dh.szxytkj.cn

Py:   x in arr
来源：http://sk.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://bf.lnxyls.cn

JS:   arr.includes(x)
来源：http://gx.yuexingan06.cn

TS:   arr.includes(x)
来源：http://ax.wgjwhj.cn

Java: list.contains(x)
来源：http://il.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://xz.gzmigu.cn

Ruby: arr.include?(x)
来源：http://nq.szsharing.cn

C#:   list.Contains(x)
来源：http://xz.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://bu.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ii.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yl.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ng.yuntaijiaju.cn

TS:   [...arr];
来源：http://rt.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://fw.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fq.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://sc.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://jc.muxihuayi.cn

[D23] reduce 累积计算
来源：http://kk.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kj.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jq.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uf.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qc.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://va.chemitech.net.cn

Go:   // 手写循环
来源：http://bd.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jw.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qm.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://ry.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cz.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ah.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bw.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ii.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rm.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jz.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yp.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uh.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://tf.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tn.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dq.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fm.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uh.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ce.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://az.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vf.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dj.panjiajie.cn

[D26] 数组转字符串
来源：http://qw.haigaiapp.cn


<!-- 参考信息 -->