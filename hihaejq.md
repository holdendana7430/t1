代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qe.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vv.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qp.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ym.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jg.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://le.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zu.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hi.shxzskj.cn

[C10] 变量作用域
来源：http://xm.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ob.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tr.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hr.gzmigu.cn

TS:   同 JS
来源：http://dv.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ox.huanxung.cn

Go:   花括号块级作用域
来源：http://yv.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ck.9csxet.cn

C#:   块级作用域
来源：http://no.shtwfgs.cn

[C11] 模块导入与导出
来源：http://nc.szxytkj.cn

Py:   from module import func
来源：http://sd.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mr.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://on.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://an.shxzukj.cn

Java: import java.util.List;
来源：http://hm.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ni.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://dd.newstarts.cn

C#:   using System.Text;
来源：http://cr.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://nl.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://sx.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://pq.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://zc.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://mn.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sv.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://hp.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://hv.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pk.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://ib.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jv.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ar.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mw.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vz.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bx.nicolike.cn

Go:   func add(a, b int) int
来源：http://ms.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iq.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gm.bookmarksfly.cn

[C14] 泛型函数
来源：http://hk.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xz.muxihuayi.cn

PHP:  // 无泛型
来源：http://av.bjjhwx.cn

JS:   // 无泛型
来源：http://qi.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qz.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kh.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dx.muxihuayi.cn

Ruby: # 无泛型
来源：http://py.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qq.huanxung.cn

[C15] 解构 / 展开参数
来源：http://zu.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zx.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://kn.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xn.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hm.shxzukj.cn

Java: // 无解构
来源：http://sk.huanxung.cn

Go:   // 无解构
来源：http://ka.nicolike.cn

Ruby: a, b = pair
来源：http://eh.newstarts.cn

C#:   var (a, b) = pair;
来源：http://eq.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://hq.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hk.chemitech.net.cn

PHP:  // 无重载
来源：http://fx.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bx.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://yc.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wc.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://rc.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://sj.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qz.jctech888.com.cn

================================================================================
来源：http://it.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://lm.nicolike.cn

================================================================================
来源：http://vk.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://kf.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ah.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ql.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ic.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kg.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://my.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://kk.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://ic.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ef.lnxyls.cn

[D02] 追加元素到末尾
来源：http://ho.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jd.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lf.yuexingan06.cn

JS:   arr.push(4);
来源：http://yd.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://ps.huixiangedu.cn

Java: list.add(4);
来源：http://gu.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://ea.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://hb.newstarts.cn

C#:   list.Add(4);
来源：http://xb.asd995.cn

[D03] 在指定位置插入元素
来源：http://cv.colortex.cn

Py:   arr.insert(0, 0)
来源：http://rj.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://is.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ip.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://fd.jctech888.com.cn

Java: list.add(0, 0);
来源：http://hs.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yv.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fb.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://dv.muxihuayi.cn

[D04] 删除元素
来源：http://pj.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gu.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://py.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://il.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://yj.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nx.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ay.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ly.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oe.9csxet.cn

[D05] 访问与修改元素
来源：http://xz.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lv.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vo.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fb.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://cy.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://bv.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://yr.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ut.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ap.shxzskj.cn

[D06] 数组长度
来源：http://gq.9csxet.cn

Py:   len(arr)
来源：http://fn.bjjhwx.cn

PHP:  count($arr);
来源：http://vj.gzmigu.cn

JS:   arr.length
来源：http://vy.bjjhwx.cn

TS:   arr.length
来源：http://qd.haigaiapp.cn

Java: list.size();
来源：http://fh.yuexingan06.cn

Go:   len(arr)
来源：http://sz.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://uz.jctech888.com.cn

C#:   list.Count;
来源：http://gq.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://kt.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ni.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://km.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://kc.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://xm.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://ic.szxytkj.cn

Go:   arr[1:4]
来源：http://oc.newstarts.cn

Ruby: arr[1, 3]
来源：http://vm.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://wo.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://mt.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://dm.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://ox.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xw.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://tm.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oo.muxihuayi.cn

Go:   append(a, b...)
来源：http://fm.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://fr.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://nz.haigaiapp.cn

[D09] 排序（升序）
来源：http://xf.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://rq.colortex.cn

PHP:  sort($arr);
来源：http://ba.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vs.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xb.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xf.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lz.lnxyls.cn

Ruby: arr.sort
来源：http://rv.haigaiapp.cn

C#:   list.Sort();
来源：http://cb.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aa.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gv.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://op.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pw.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ua.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tk.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gv.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://at.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mx.haigaiapp.cn

[D11] 反转数组
来源：http://zt.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qq.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://dh.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lx.colortex.cn

TS:   [...arr].reverse();
来源：http://sw.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://fw.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://ja.panjiajie.cn

Ruby: arr.reverse
来源：http://ru.nicolike.cn

C#:   list.Reverse();
来源：http://fl.wgjwhj.cn

[D12] 查找元素下标
来源：http://qf.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://ln.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hk.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ul.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uo.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hm.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://rx.huanxung.cn

Ruby: arr.index(x)
来源：http://re.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://je.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://zz.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pp.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bh.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://yb.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://or.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gd.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://we.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bu.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kr.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://nm.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dg.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aq.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://iy.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://fs.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rm.shtwfgs.cn

Go:   // 手写循环
来源：http://sy.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ww.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ou.521024.cn

[D15] 去重
来源：http://aa.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://em.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://xc.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://lx.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://ve.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dj.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ks.szsharing.cn

Ruby: arr.uniq
来源：http://ks.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://gf.nszjky.cn

[D16] 求和与平均值
来源：http://yt.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lb.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ea.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ow.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hf.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tk.shtwfgs.cn

Go:   // 手写循环累加
来源：http://hc.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yv.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://uf.huanxung.cn

[D17] 最大值与最小值
来源：http://wi.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://tf.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://cj.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xn.hnjuh.cn

TS:   Math.max(...arr);
来源：http://xm.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wc.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rd.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://lc.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://gu.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://cg.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xt.colortex.cn

PHP:  array_merge(...$nested);
来源：http://jh.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iy.nicolike.cn

TS:   nested.flat();
来源：http://nl.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dn.panjiajie.cn

Go:   // 手写双层循环
来源：http://ff.szxytkj.cn

Ruby: nested.flatten
来源：http://eo.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vl.nszjky.cn

[D19] 按字段分组
来源：http://ir.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ef.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cy.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ys.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://an.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://au.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://dq.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://va.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fu.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://mg.bookmarksfly.cn

Py:   Counter(arr)
来源：http://vn.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://fy.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cl.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ln.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rp.colortex.cn

Go:   // 手写 map[T]int
来源：http://zo.yuntaijiaju.cn

Ruby: arr.tally
来源：http://rt.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cd.nicolike.cn

[D21] 判断是否包含某元素
来源：http://ac.jctech888.com.cn

Py:   x in arr
来源：http://ev.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://pp.panjiajie.cn

JS:   arr.includes(x)
来源：http://ek.huanxung.cn

TS:   arr.includes(x)
来源：http://pq.huixiangedu.cn

Java: list.contains(x)
来源：http://yw.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://ra.shxzskj.cn

Ruby: arr.include?(x)
来源：http://jo.chemitech.net.cn

C#:   list.Contains(x)
来源：http://th.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://cq.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ob.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cu.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uc.shxzukj.cn

TS:   [...arr];
来源：http://qt.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://db.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://df.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://mv.huixiangedu.cn

C#:   new List<int>(list);
来源：http://oc.shxzskj.cn

[D23] reduce 累积计算
来源：http://zj.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nf.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tc.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dh.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nd.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yf.hahajie.cn

Go:   // 手写循环
来源：http://ju.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fi.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yh.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://tt.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bd.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ci.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ai.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vy.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pu.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://az.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pv.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aw.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://do.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bh.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pu.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zg.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lm.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cs.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://of.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ik.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oy.wgjwhj.cn

[D26] 数组转字符串
来源：http://px.huanxung.cn


<!-- 参考信息 -->