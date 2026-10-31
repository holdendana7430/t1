代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sn.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pv.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kp.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ai.colortex.cn

[C10] 变量作用域
来源：http://hy.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qo.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sq.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://js.hahajie.cn

TS:   同 JS
来源：http://gi.asd995.cn

Java: 方法内为块级作用域
来源：http://pu.huixiangedu.cn

Go:   花括号块级作用域
来源：http://ys.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ty.bookmarksfly.cn

C#:   块级作用域
来源：http://ln.shxzskj.cn

[C11] 模块导入与导出
来源：http://zu.bjjhwx.cn

Py:   from module import func
来源：http://tg.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qn.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ss.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ov.asd995.cn

Java: import java.util.List;
来源：http://wo.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gl.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://br.gzmigu.cn

C#:   using System.Text;
来源：http://yi.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://so.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://hi.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://ik.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://ef.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://np.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ut.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://nh.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://db.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zb.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://ab.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mw.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://at.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bd.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cc.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mc.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://bh.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ch.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jx.bookmarksfly.cn

[C14] 泛型函数
来源：http://bn.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dm.haigaiapp.cn

PHP:  // 无泛型
来源：http://ff.hahajie.cn

JS:   // 无泛型
来源：http://uy.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xo.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yu.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qz.colortex.cn

Ruby: # 无泛型
来源：http://vm.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xo.huanxung.cn

[C15] 解构 / 展开参数
来源：http://fa.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zb.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://kg.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bv.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ng.bookmarksfly.cn

Java: // 无解构
来源：http://ld.szsharing.cn

Go:   // 无解构
来源：http://cp.haigaiapp.cn

Ruby: a, b = pair
来源：http://zd.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://hw.hahajie.cn

[C16] 函数 / 方法重载
来源：http://rn.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vx.shtwfgs.cn

PHP:  // 无重载
来源：http://kk.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rv.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://es.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pp.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://kg.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://lj.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oy.nszjky.cn

================================================================================
来源：http://nt.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://ka.bookmarksfly.cn

================================================================================
来源：http://mb.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://jd.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jg.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://an.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ei.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vk.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ws.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://qf.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://tu.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dn.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://gz.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cj.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yv.haigaiapp.cn

JS:   arr.push(4);
来源：http://mk.huanxung.cn

TS:   arr.push(4);
来源：http://ir.yuexingan06.cn

Java: list.add(4);
来源：http://ll.colortex.cn

Go:   arr = append(arr, 4)
来源：http://cs.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://rg.hahajie.cn

C#:   list.Add(4);
来源：http://ky.newstarts.cn

[D03] 在指定位置插入元素
来源：http://aw.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://mz.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pl.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zx.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://gb.hnjuh.cn

Java: list.add(0, 0);
来源：http://om.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://km.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fz.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://fj.yuexingan06.cn

[D04] 删除元素
来源：http://me.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zo.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hl.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://af.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://yp.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qa.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pt.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sc.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hh.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://ht.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zc.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vt.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oc.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ij.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://sj.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://rm.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ml.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gv.shxzskj.cn

[D06] 数组长度
来源：http://an.521024.cn

Py:   len(arr)
来源：http://wy.jctech888.com.cn

PHP:  count($arr);
来源：http://zw.nicolike.cn

JS:   arr.length
来源：http://fc.521024.cn

TS:   arr.length
来源：http://wb.wgjwhj.cn

Java: list.size();
来源：http://nq.jianghongdianzi.cn

Go:   len(arr)
来源：http://ul.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://am.szsharing.cn

C#:   list.Count;
来源：http://bv.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://nl.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://th.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pe.521024.cn

JS:   arr.slice(1, 4);
来源：http://cu.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://sq.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://nm.jctech888.com.cn

Go:   arr[1:4]
来源：http://as.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://el.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://mx.lnxyls.cn

[D08] 合并两个数组
来源：http://oz.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://ez.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://ie.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yx.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://xl.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ov.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://li.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://bt.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://yt.hnjuh.cn

[D09] 排序（升序）
来源：http://ka.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://cq.shxzskj.cn

PHP:  sort($arr);
来源：http://qk.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jx.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mi.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qc.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ry.newstarts.cn

Ruby: arr.sort
来源：http://fz.hahajie.cn

C#:   list.Sort();
来源：http://pj.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kw.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fd.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oc.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nw.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tz.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ku.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ae.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yy.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ub.huixiangedu.cn

[D11] 反转数组
来源：http://vh.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sw.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://dc.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rh.szxytkj.cn

TS:   [...arr].reverse();
来源：http://hb.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://yd.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://zr.shxzskj.cn

Ruby: arr.reverse
来源：http://in.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://xf.hahajie.cn

[D12] 查找元素下标
来源：http://ue.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://xs.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gr.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rt.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bw.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qx.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://fi.huanxung.cn

Ruby: arr.index(x)
来源：http://bl.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://qz.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://xw.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ki.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iv.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://lk.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://ds.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lc.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://an.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yw.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pd.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://lx.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qm.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kj.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://zq.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://hx.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vs.newstarts.cn

Go:   // 手写循环
来源：http://lc.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qa.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ti.chemitech.net.cn

[D15] 去重
来源：http://mh.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lu.521024.cn

PHP:  array_unique($arr);
来源：http://ck.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://kq.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://ky.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yt.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cb.gzmigu.cn

Ruby: arr.uniq
来源：http://vk.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://bq.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://ad.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ws.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ho.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wl.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zw.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mg.jctech888.com.cn

Go:   // 手写循环累加
来源：http://xm.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mw.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://gy.bjjhwx.cn

[D17] 最大值与最小值
来源：http://my.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://ud.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://zh.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://up.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://hz.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mr.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uy.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://wi.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://ss.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://zr.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hp.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://vr.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xj.huixiangedu.cn

TS:   nested.flat();
来源：http://yl.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cm.shtwfgs.cn

Go:   // 手写双层循环
来源：http://tn.bookmarksfly.cn

Ruby: nested.flatten
来源：http://uy.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vb.shxzskj.cn

[D19] 按字段分组
来源：http://st.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kq.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uy.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lj.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ba.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ye.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://og.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ty.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qm.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://zm.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://dh.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://ex.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hn.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fk.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fb.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://tg.yuntaijiaju.cn

Ruby: arr.tally
来源：http://eq.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yn.9csxet.cn

[D21] 判断是否包含某元素
来源：http://zx.bookmarksfly.cn

Py:   x in arr
来源：http://pb.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://rq.nicolike.cn

JS:   arr.includes(x)
来源：http://vv.shtwfgs.cn

TS:   arr.includes(x)
来源：http://hg.bjjhwx.cn

Java: list.contains(x)
来源：http://zc.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://zy.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://gg.panjiajie.cn

C#:   list.Contains(x)
来源：http://si.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://wr.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xc.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wa.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lx.huixiangedu.cn

TS:   [...arr];
来源：http://kv.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://oh.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tv.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://kc.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://dr.szsharing.cn

[D23] reduce 累积计算
来源：http://ld.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vh.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pn.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nl.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xn.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ei.szxytkj.cn

Go:   // 手写循环
来源：http://qc.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://da.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ml.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://iv.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pj.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yx.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dz.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vs.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ve.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bh.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qq.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vs.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://cm.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tx.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vq.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ol.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ki.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hh.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aq.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://by.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bp.shxzukj.cn

[D26] 数组转字符串
来源：http://bw.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://za.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://gi.haigaiapp.cn

JS:   arr.join(", ")
来源：http://ge.panjiajie.cn

TS:   arr.join(", ")
来源：http://gc.jctech888.com.cn


<!-- 参考信息 -->