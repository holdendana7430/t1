代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://nb.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tr.huixinmuqiang.cn

[C08] 闭包
来源：http://no.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ll.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uf.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wp.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qk.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bm.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nr.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ye.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sv.muxihuayi.cn

[C09] 递归
来源：http://tu.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ip.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oh.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fn.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vl.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mk.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://on.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://id.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yq.newstarts.cn

[C10] 变量作用域
来源：http://cl.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yl.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://px.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ng.szsharing.cn

TS:   同 JS
来源：http://ly.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://jd.huanxung.cn

Go:   花括号块级作用域
来源：http://bn.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ft.9csxet.cn

C#:   块级作用域
来源：http://py.szsharing.cn

[C11] 模块导入与导出
来源：http://ac.colortex.cn

Py:   from module import func
来源：http://of.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sf.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dl.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jh.newstarts.cn

Java: import java.util.List;
来源：http://tf.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iy.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://su.haigaiapp.cn

C#:   using System.Text;
来源：http://le.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://ef.521024.cn

Py:   (lambda: print("run"))()
来源：http://hr.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://pj.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://td.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://og.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pr.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://dk.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://rh.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ne.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://yu.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ih.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ma.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eu.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mo.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ue.shxzukj.cn

Go:   func add(a, b int) int
来源：http://fl.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oe.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ur.chemitech.net.cn

[C14] 泛型函数
来源：http://kh.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yw.szsharing.cn

PHP:  // 无泛型
来源：http://sk.bjjhwx.cn

JS:   // 无泛型
来源：http://sd.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ev.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bz.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nc.shxzukj.cn

Ruby: # 无泛型
来源：http://qd.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ej.huanxung.cn

[C15] 解构 / 展开参数
来源：http://te.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://da.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://of.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mz.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://if.bookmarksfly.cn

Java: // 无解构
来源：http://dz.shtwfgs.cn

Go:   // 无解构
来源：http://ei.panjiajie.cn

Ruby: a, b = pair
来源：http://mg.szsharing.cn

C#:   var (a, b) = pair;
来源：http://kc.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://yh.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nn.shxzskj.cn

PHP:  // 无重载
来源：http://ay.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://am.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://jc.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://il.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://zm.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://ec.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://em.yuexingan06.cn

================================================================================
来源：http://ju.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://as.wgjwhj.cn

================================================================================
来源：http://jp.colortex.cn

[D01] 创建数组 / 列表
来源：http://iq.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kp.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dt.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vg.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hb.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zz.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://xh.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://sh.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yn.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://vw.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hk.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ru.lnxyls.cn

JS:   arr.push(4);
来源：http://ss.shtwfgs.cn

TS:   arr.push(4);
来源：http://ez.nszjky.cn

Java: list.add(4);
来源：http://id.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://gl.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://cb.asd995.cn

C#:   list.Add(4);
来源：http://vv.newstarts.cn

[D03] 在指定位置插入元素
来源：http://ne.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://cg.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cu.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lt.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://ej.shxzukj.cn

Java: list.add(0, 0);
来源：http://hk.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oi.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mr.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://da.hahajie.cn

[D04] 删除元素
来源：http://lb.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://np.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://km.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fh.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://jw.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qp.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rc.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uf.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ks.lnxyls.cn

[D05] 访问与修改元素
来源：http://gs.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ed.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zz.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uz.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://nr.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://oc.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://cu.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ai.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ct.hnjuh.cn

[D06] 数组长度
来源：http://fw.jctech888.com.cn

Py:   len(arr)
来源：http://uy.panjiajie.cn

PHP:  count($arr);
来源：http://cb.shtwfgs.cn

JS:   arr.length
来源：http://il.jctech888.com.cn

TS:   arr.length
来源：http://pk.shxzskj.cn

Java: list.size();
来源：http://bt.szxytkj.cn

Go:   len(arr)
来源：http://hh.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://zo.nszjky.cn

C#:   list.Count;
来源：http://ce.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://ba.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ar.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ol.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://ap.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://jz.hnjuh.cn

Java: list.subList(1, 4);
来源：http://ds.521024.cn

Go:   arr[1:4]
来源：http://vf.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://em.521024.cn

C#:   list.GetRange(1, 3);
来源：http://qr.lnxyls.cn

[D08] 合并两个数组
来源：http://qn.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://qs.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://ko.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vb.hahajie.cn

TS:   [...a, ...b];
来源：http://ys.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lh.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://pj.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://cq.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://xf.asd995.cn

[D09] 排序（升序）
来源：http://um.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://gc.gzmigu.cn

PHP:  sort($arr);
来源：http://ay.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qj.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bf.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nq.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uk.521024.cn

Ruby: arr.sort
来源：http://ac.newstarts.cn

C#:   list.Sort();
来源：http://dy.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ag.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jd.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ki.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qd.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qi.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gy.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pv.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ij.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gf.asd995.cn

[D11] 反转数组
来源：http://oh.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ol.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://gb.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dc.newstarts.cn

TS:   [...arr].reverse();
来源：http://bc.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://aj.colortex.cn

Go:   slices.Reverse(arr)
来源：http://bc.gzmigu.cn

Ruby: arr.reverse
来源：http://cx.shxzskj.cn

C#:   list.Reverse();
来源：http://co.colortex.cn

[D12] 查找元素下标
来源：http://ew.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://mn.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bf.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bp.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xj.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wy.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://rq.yuexingan06.cn

Ruby: arr.index(x)
来源：http://bh.9csxet.cn

C#:   list.IndexOf(x);
来源：http://lh.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://yr.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ju.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jf.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://or.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://du.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://so.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hl.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://it.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ns.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://zr.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rl.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://me.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://at.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://qx.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lh.bjjhwx.cn

Go:   // 手写循环
来源：http://pv.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tk.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ps.hahajie.cn

[D15] 去重
来源：http://by.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tw.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://el.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://kd.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://do.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oo.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ul.huixiangedu.cn

Ruby: arr.uniq
来源：http://tr.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://un.szsharing.cn

[D16] 求和与平均值
来源：http://pf.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gw.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://no.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mn.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ly.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ye.hahajie.cn

Go:   // 手写循环累加
来源：http://kj.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rd.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://gu.huanxung.cn

[D17] 最大值与最小值
来源：http://fa.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://pp.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://os.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lt.asd995.cn

TS:   Math.max(...arr);
来源：http://zr.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ty.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tz.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://ep.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://kr.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://nq.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ve.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://tt.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jb.szxytkj.cn

TS:   nested.flat();
来源：http://ka.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://un.haigaiapp.cn

Go:   // 手写双层循环
来源：http://yk.lnxyls.cn

Ruby: nested.flatten
来源：http://pn.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ic.bookmarksfly.cn

[D19] 按字段分组
来源：http://dw.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wy.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bk.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dj.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uz.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nn.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://vw.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vq.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mn.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://jy.hnjuh.cn

Py:   Counter(arr)
来源：http://zv.huanxung.cn

PHP:  array_count_values($arr);
来源：http://ih.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pr.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tf.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bn.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://nc.shxzskj.cn

Ruby: arr.tally
来源：http://qj.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ha.huanxung.cn

[D21] 判断是否包含某元素
来源：http://ma.gzmigu.cn

Py:   x in arr
来源：http://wk.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://xd.hnjuh.cn

JS:   arr.includes(x)
来源：http://bp.521024.cn

TS:   arr.includes(x)
来源：http://ep.shxzukj.cn

Java: list.contains(x)
来源：http://iw.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://fb.newstarts.cn

Ruby: arr.include?(x)
来源：http://ec.shxzukj.cn

C#:   list.Contains(x)
来源：http://uq.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://um.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pu.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jj.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bq.bjjhwx.cn

TS:   [...arr];
来源：http://ky.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://rd.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://va.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://xm.521024.cn

C#:   new List<int>(list);
来源：http://fg.chemitech.net.cn

[D23] reduce 累积计算
来源：http://pg.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fn.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sk.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://we.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jy.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://at.yuexingan06.cn

Go:   // 手写循环
来源：http://po.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sp.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://av.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://ns.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jk.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cd.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ff.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://or.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yo.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zd.521024.cn


<!-- 参考信息 -->