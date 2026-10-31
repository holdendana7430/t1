代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nf.nicolike.cn

TS:   arr.map(String)
来源：http://px.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rn.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kw.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://az.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ow.nszjky.cn

[C08] 闭包
来源：http://fx.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hb.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qo.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zv.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jr.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hf.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pm.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zs.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cj.jctech888.com.cn

[C09] 递归
来源：http://ra.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://so.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vy.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cg.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://de.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yw.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ur.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dv.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ho.newstarts.cn

[C10] 变量作用域
来源：http://ne.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pf.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kb.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zw.shxzskj.cn

TS:   同 JS
来源：http://tu.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://te.shxzskj.cn

Go:   花括号块级作用域
来源：http://gp.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ab.huixinmuqiang.cn

C#:   块级作用域
来源：http://eh.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://vk.huanxung.cn

Py:   from module import func
来源：http://sl.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mn.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jz.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ew.huixiangedu.cn

Java: import java.util.List;
来源：http://ys.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cz.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://xk.nicolike.cn

C#:   using System.Text;
来源：http://qs.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://wr.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://bl.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://mm.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://fp.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://rl.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zf.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://cc.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://vz.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fq.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://xm.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ml.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rm.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jn.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bz.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eq.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://ri.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://um.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sn.huixiangedu.cn

[C14] 泛型函数
来源：http://qk.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ir.asd995.cn

PHP:  // 无泛型
来源：http://zg.chemitech.net.cn

JS:   // 无泛型
来源：http://gn.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pl.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://se.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fq.shxzskj.cn

Ruby: # 无泛型
来源：http://pl.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qg.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://xl.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yk.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://ln.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mn.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vw.shtwfgs.cn

Java: // 无解构
来源：http://sp.shtwfgs.cn

Go:   // 无解构
来源：http://vx.colortex.cn

Ruby: a, b = pair
来源：http://yh.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://gm.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://za.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ew.huixiangedu.cn

PHP:  // 无重载
来源：http://ie.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yt.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://rd.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yc.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ne.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://am.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gd.panjiajie.cn

================================================================================
来源：http://mz.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://mp.szxytkj.cn

================================================================================
来源：http://ro.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://va.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mp.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xo.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vg.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://co.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ss.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://cd.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://ly.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bo.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://ve.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yn.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ia.521024.cn

JS:   arr.push(4);
来源：http://wt.shxzskj.cn

TS:   arr.push(4);
来源：http://ee.bookmarksfly.cn

Java: list.add(4);
来源：http://oy.asd995.cn

Go:   arr = append(arr, 4)
来源：http://lj.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://as.newstarts.cn

C#:   list.Add(4);
来源：http://ll.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://fm.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://xo.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ff.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://dp.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://he.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uj.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yi.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://ri.nszjky.cn

[D04] 删除元素
来源：http://im.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pe.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cb.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xz.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://vc.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ua.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://br.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rq.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cx.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://iu.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ng.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mn.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qc.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://gk.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://om.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://wc.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://za.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bt.9csxet.cn

[D06] 数组长度
来源：http://xc.huixiangedu.cn

Py:   len(arr)
来源：http://va.521024.cn

PHP:  count($arr);
来源：http://ta.9csxet.cn

JS:   arr.length
来源：http://gw.nszjky.cn

TS:   arr.length
来源：http://yy.wgjwhj.cn

Java: list.size();
来源：http://ua.chemitech.net.cn

Go:   len(arr)
来源：http://gz.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://zk.nszjky.cn

C#:   list.Count;
来源：http://de.9csxet.cn

[D07] 切片 / 取子数组
来源：http://gv.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sk.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vl.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://qk.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://oj.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://lj.nicolike.cn

Go:   arr[1:4]
来源：http://yj.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://fy.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://og.newstarts.cn

[D08] 合并两个数组
来源：http://uo.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://ia.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://yw.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tw.wgjwhj.cn

TS:   [...a, ...b];
来源：http://bv.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bt.nszjky.cn

Go:   append(a, b...)
来源：http://jr.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://qa.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://vh.bjjhwx.cn

[D09] 排序（升序）
来源：http://sy.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://yh.huixiangedu.cn

PHP:  sort($arr);
来源：http://bb.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tn.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ni.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gm.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bm.521024.cn

Ruby: arr.sort
来源：http://kw.chemitech.net.cn

C#:   list.Sort();
来源：http://ly.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mw.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mx.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lz.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kk.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xy.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ip.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pi.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tw.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iy.haigaiapp.cn

[D11] 反转数组
来源：http://qo.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ic.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://kg.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uk.hahajie.cn

TS:   [...arr].reverse();
来源：http://vy.huanxung.cn

Java: Collections.reverse(list);
来源：http://an.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://hq.haigaiapp.cn

Ruby: arr.reverse
来源：http://zr.lnxyls.cn

C#:   list.Reverse();
来源：http://xf.nicolike.cn

[D12] 查找元素下标
来源：http://en.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://cp.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xf.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jy.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bh.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ti.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://ds.shtwfgs.cn

Ruby: arr.index(x)
来源：http://dw.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://ly.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://gq.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wi.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sf.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://nk.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://tc.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ip.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cy.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uy.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wn.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://hm.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zw.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://om.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://jh.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://re.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xl.colortex.cn

Go:   // 手写循环
来源：http://ar.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rj.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bc.jctech888.com.cn

[D15] 去重
来源：http://bs.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qx.colortex.cn

PHP:  array_unique($arr);
来源：http://ah.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://lc.nicolike.cn

TS:   [...new Set(arr)]
来源：http://pm.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xu.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cr.lnxyls.cn

Ruby: arr.uniq
来源：http://za.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://oi.wgjwhj.cn

[D16] 求和与平均值
来源：http://nv.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cw.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ff.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hk.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bk.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qm.szxytkj.cn

Go:   // 手写循环累加
来源：http://wi.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wz.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://qy.wgjwhj.cn

[D17] 最大值与最小值
来源：http://yy.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://jk.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://kz.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hd.shxzskj.cn

TS:   Math.max(...arr);
来源：http://co.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nw.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://te.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://ne.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://xf.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://lx.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hf.521024.cn

PHP:  array_merge(...$nested);
来源：http://sr.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gp.gzmigu.cn

TS:   nested.flat();
来源：http://sr.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mu.colortex.cn

Go:   // 手写双层循环
来源：http://ym.9csxet.cn

Ruby: nested.flatten
来源：http://ow.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://us.jianghongdianzi.cn

[D19] 按字段分组
来源：http://se.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://db.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ab.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hq.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zm.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wu.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://tl.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fs.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lx.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://kn.szxytkj.cn

Py:   Counter(arr)
来源：http://th.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://ul.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://du.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://re.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cb.colortex.cn

Go:   // 手写 map[T]int
来源：http://ci.521024.cn

Ruby: arr.tally
来源：http://uc.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cd.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://dq.521024.cn

Py:   x in arr
来源：http://yd.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://id.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://ar.nicolike.cn

TS:   arr.includes(x)
来源：http://wv.huixiangedu.cn

Java: list.contains(x)
来源：http://gx.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://la.szsharing.cn

Ruby: arr.include?(x)
来源：http://ut.wgjwhj.cn

C#:   list.Contains(x)
来源：http://pm.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://xr.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://za.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bp.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ef.shtwfgs.cn

TS:   [...arr];
来源：http://vl.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ea.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://in.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://ss.shxzskj.cn

C#:   new List<int>(list);
来源：http://zb.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://gb.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cz.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rs.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://to.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ig.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gx.huixiangedu.cn

Go:   // 手写循环
来源：http://dz.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ch.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nz.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://vl.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oh.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yi.jctech888.com.cn


<!-- 参考信息 -->