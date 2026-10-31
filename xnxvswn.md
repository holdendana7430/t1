代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sm.hnjuh.cn

TS:   arr.map(String)
来源：http://ih.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://js.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nr.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://bu.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yb.szsharing.cn

[C08] 闭包
来源：http://yv.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ei.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qp.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aj.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qv.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yh.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sc.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lc.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pw.lnxyls.cn

[C09] 递归
来源：http://wk.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ok.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ii.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ns.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bb.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xx.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oh.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xi.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jp.jianghongdianzi.cn

[C10] 变量作用域
来源：http://yx.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pg.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nx.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zw.asd995.cn

TS:   同 JS
来源：http://pb.shxzukj.cn

Java: 方法内为块级作用域
来源：http://zm.wgjwhj.cn

Go:   花括号块级作用域
来源：http://fn.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fi.shxzskj.cn

C#:   块级作用域
来源：http://fr.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://kj.wgjwhj.cn

Py:   from module import func
来源：http://xa.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xa.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kr.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pm.lnxyls.cn

Java: import java.util.List;
来源：http://rb.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ve.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://sy.jctech888.com.cn

C#:   using System.Text;
来源：http://ze.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://po.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://dg.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://ms.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://qg.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://ru.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ej.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://bp.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://wp.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rp.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://jf.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hu.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eq.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ox.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ng.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://js.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://sb.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pi.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zr.asd995.cn

[C14] 泛型函数
来源：http://sq.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sd.asd995.cn

PHP:  // 无泛型
来源：http://re.wgjwhj.cn

JS:   // 无泛型
来源：http://wq.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zn.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nx.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yl.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://cy.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nl.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://oq.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aq.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://ku.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dx.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ny.yuntaijiaju.cn

Java: // 无解构
来源：http://xl.bookmarksfly.cn

Go:   // 无解构
来源：http://xb.nicolike.cn

Ruby: a, b = pair
来源：http://ot.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://wb.nszjky.cn

[C16] 函数 / 方法重载
来源：http://ts.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ym.yuntaijiaju.cn

PHP:  // 无重载
来源：http://ap.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qw.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ll.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hd.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://qs.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ar.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zx.huixiangedu.cn

================================================================================
来源：http://ia.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://pc.bjjhwx.cn

================================================================================
来源：http://ew.huanxung.cn

[D01] 创建数组 / 列表
来源：http://sa.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://op.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tn.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wc.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wg.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cx.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://df.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://wy.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eo.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://er.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dk.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ld.newstarts.cn

JS:   arr.push(4);
来源：http://fk.9csxet.cn

TS:   arr.push(4);
来源：http://ge.muxihuayi.cn

Java: list.add(4);
来源：http://lb.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://or.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://tp.shtwfgs.cn

C#:   list.Add(4);
来源：http://ee.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ui.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://gm.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lu.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://of.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://ek.huanxung.cn

Java: list.add(0, 0);
来源：http://tx.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bf.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zc.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://dt.asd995.cn

[D04] 删除元素
来源：http://dh.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ec.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://px.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://or.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://ap.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ug.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xm.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://if.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ln.nszjky.cn

[D05] 访问与修改元素
来源：http://ny.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bn.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gp.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jr.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://cl.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://rs.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://el.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lq.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gq.bjjhwx.cn

[D06] 数组长度
来源：http://md.asd995.cn

Py:   len(arr)
来源：http://kv.szxytkj.cn

PHP:  count($arr);
来源：http://kt.colortex.cn

JS:   arr.length
来源：http://fw.jianghongdianzi.cn

TS:   arr.length
来源：http://nh.jianghongdianzi.cn

Java: list.size();
来源：http://bo.hahajie.cn

Go:   len(arr)
来源：http://wl.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://on.muxihuayi.cn

C#:   list.Count;
来源：http://fa.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://ql.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pt.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://md.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://qd.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://ku.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://zv.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://jt.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://ij.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://dr.lnxyls.cn

[D08] 合并两个数组
来源：http://qb.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://ly.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://xo.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gi.shxzukj.cn

TS:   [...a, ...b];
来源：http://uy.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oo.colortex.cn

Go:   append(a, b...)
来源：http://ja.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://ny.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://jp.huixiangedu.cn

[D09] 排序（升序）
来源：http://hh.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://no.lnxyls.cn

PHP:  sort($arr);
来源：http://jb.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ms.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://el.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ei.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://io.hahajie.cn

Ruby: arr.sort
来源：http://kc.asd995.cn

C#:   list.Sort();
来源：http://ft.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ow.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://as.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gh.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://un.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kh.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ij.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dy.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mv.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oe.hahajie.cn

[D11] 反转数组
来源：http://dc.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gd.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://tg.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ol.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://dt.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://xe.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://tv.nszjky.cn

Ruby: arr.reverse
来源：http://ic.wgjwhj.cn

C#:   list.Reverse();
来源：http://ea.newstarts.cn

[D12] 查找元素下标
来源：http://sv.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://wg.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://en.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fd.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://up.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fx.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://lo.bjjhwx.cn

Ruby: arr.index(x)
来源：http://el.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://aq.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://sa.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ak.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xf.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://gd.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://qf.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dy.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uz.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bs.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tj.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://ng.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jn.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yw.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://xi.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://ke.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mx.huanxung.cn

Go:   // 手写循环
来源：http://cv.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yc.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dq.shxzskj.cn

[D15] 去重
来源：http://nx.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fk.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://fs.huanxung.cn

JS:   [...new Set(arr)]
来源：http://bq.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://ci.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vk.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ar.shtwfgs.cn

Ruby: arr.uniq
来源：http://vx.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://ws.szxytkj.cn

[D16] 求和与平均值
来源：http://zi.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://md.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zk.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bk.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cc.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kb.szsharing.cn

Go:   // 手写循环累加
来源：http://kt.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zn.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://jc.panjiajie.cn

[D17] 最大值与最小值
来源：http://lt.521024.cn

Py:   max(arr);  min(arr)
来源：http://oo.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://vv.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://id.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://rl.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jc.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vg.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://do.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://fj.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://jh.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nw.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://js.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ad.bjjhwx.cn

TS:   nested.flat();
来源：http://qw.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ct.521024.cn

Go:   // 手写双层循环
来源：http://dr.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://ru.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zw.chemitech.net.cn

[D19] 按字段分组
来源：http://qo.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kc.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://br.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tw.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tn.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ku.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://bs.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ew.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ca.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://hu.gzmigu.cn

Py:   Counter(arr)
来源：http://yo.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://fr.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nm.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ko.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ri.colortex.cn

Go:   // 手写 map[T]int
来源：http://fl.nszjky.cn

Ruby: arr.tally
来源：http://mz.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://az.colortex.cn

[D21] 判断是否包含某元素
来源：http://bm.szsharing.cn

Py:   x in arr
来源：http://xg.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://qb.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://rd.lnxyls.cn

TS:   arr.includes(x)
来源：http://sh.nszjky.cn

Java: list.contains(x)
来源：http://yb.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://le.asd995.cn

Ruby: arr.include?(x)
来源：http://hj.jctech888.com.cn

C#:   list.Contains(x)
来源：http://la.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://xg.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qz.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ma.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://be.huanxung.cn

TS:   [...arr];
来源：http://xt.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://fb.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dp.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://zl.jctech888.com.cn

C#:   new List<int>(list);
来源：http://nk.521024.cn

[D23] reduce 累积计算
来源：http://rt.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qk.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cl.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yj.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zm.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vb.nszjky.cn

Go:   // 手写循环
来源：http://rq.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lf.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bn.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://wn.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bt.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ku.yuexingan06.cn


<!-- 参考信息 -->