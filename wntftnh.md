代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ze.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://an.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ds.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rv.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://en.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sn.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zn.521024.cn

[C09] 递归
来源：http://md.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hf.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ih.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yd.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cx.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cx.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bn.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fs.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mp.jianghongdianzi.cn

[C10] 变量作用域
来源：http://dl.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zo.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ez.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lm.gzmigu.cn

TS:   同 JS
来源：http://nb.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://ax.asd995.cn

Go:   花括号块级作用域
来源：http://ei.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rq.shxzukj.cn

C#:   块级作用域
来源：http://yb.asd995.cn

[C11] 模块导入与导出
来源：http://iq.huixinmuqiang.cn

Py:   from module import func
来源：http://un.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://er.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nj.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://je.nicolike.cn

Java: import java.util.List;
来源：http://rg.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ea.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://ki.newstarts.cn

C#:   using System.Text;
来源：http://zq.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://yb.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://ws.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://ok.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://pt.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://bx.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hp.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://pa.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://bq.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jn.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://dt.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://do.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ik.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://us.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hf.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ae.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://fn.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wa.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://as.colortex.cn

[C14] 泛型函数
来源：http://fv.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://an.nszjky.cn

PHP:  // 无泛型
来源：http://kf.chemitech.net.cn

JS:   // 无泛型
来源：http://hd.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sw.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dw.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cg.shtwfgs.cn

Ruby: # 无泛型
来源：http://sz.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jc.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://dy.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iq.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://fg.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dp.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ns.haigaiapp.cn

Java: // 无解构
来源：http://lg.9csxet.cn

Go:   // 无解构
来源：http://ty.szxytkj.cn

Ruby: a, b = pair
来源：http://ka.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://zs.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://xp.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fv.chemitech.net.cn

PHP:  // 无重载
来源：http://ij.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ag.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://cr.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://di.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://ma.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://ct.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cn.gzmigu.cn

================================================================================
来源：http://ef.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://vp.haigaiapp.cn

================================================================================
来源：http://va.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://wb.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lx.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://on.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ub.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vg.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vh.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://uo.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://mh.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cs.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://se.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pt.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rx.chemitech.net.cn

JS:   arr.push(4);
来源：http://tp.shxzukj.cn

TS:   arr.push(4);
来源：http://yo.wgjwhj.cn

Java: list.add(4);
来源：http://ky.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://ee.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://ph.haigaiapp.cn

C#:   list.Add(4);
来源：http://rv.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://ar.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://zt.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gz.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rl.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://li.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://fm.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gb.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tq.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://yd.szsharing.cn

[D04] 删除元素
来源：http://oq.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zl.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://de.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bt.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://lr.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vq.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ji.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yg.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qi.szxytkj.cn

[D05] 访问与修改元素
来源：http://ey.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zf.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fb.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://by.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ag.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://yd.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://jp.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xy.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bn.szsharing.cn

[D06] 数组长度
来源：http://pw.hahajie.cn

Py:   len(arr)
来源：http://ee.jianghongdianzi.cn

PHP:  count($arr);
来源：http://cq.huixinmuqiang.cn

JS:   arr.length
来源：http://zr.newstarts.cn

TS:   arr.length
来源：http://kk.chemitech.net.cn

Java: list.size();
来源：http://tv.bjjhwx.cn

Go:   len(arr)
来源：http://zx.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://tx.521024.cn

C#:   list.Count;
来源：http://uc.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://vi.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cm.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://it.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://va.colortex.cn

TS:   arr.slice(1, 4);
来源：http://mg.gzmigu.cn

Java: list.subList(1, 4);
来源：http://yx.bookmarksfly.cn

Go:   arr[1:4]
来源：http://pl.nicolike.cn

Ruby: arr[1, 3]
来源：http://ty.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://cy.hahajie.cn

[D08] 合并两个数组
来源：http://rw.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://me.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://rd.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tc.jctech888.com.cn

TS:   [...a, ...b];
来源：http://gb.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://we.bookmarksfly.cn

Go:   append(a, b...)
来源：http://oc.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://mw.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://xx.lnxyls.cn

[D09] 排序（升序）
来源：http://ip.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://mv.jctech888.com.cn

PHP:  sort($arr);
来源：http://gr.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qy.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nl.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fl.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gz.bjjhwx.cn

Ruby: arr.sort
来源：http://hr.asd995.cn

C#:   list.Sort();
来源：http://tv.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nl.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yo.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ov.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ml.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uh.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hf.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qd.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nr.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nn.hahajie.cn

[D11] 反转数组
来源：http://go.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tr.newstarts.cn

PHP:  array_reverse($arr);
来源：http://xy.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://db.huanxung.cn

TS:   [...arr].reverse();
来源：http://fc.huanxung.cn

Java: Collections.reverse(list);
来源：http://zd.colortex.cn

Go:   slices.Reverse(arr)
来源：http://gu.asd995.cn

Ruby: arr.reverse
来源：http://mz.shxzskj.cn

C#:   list.Reverse();
来源：http://rn.wgjwhj.cn

[D12] 查找元素下标
来源：http://hy.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://yq.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jv.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kf.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mj.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hp.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://bu.shxzskj.cn

Ruby: arr.index(x)
来源：http://jq.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://eo.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://hc.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tm.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lw.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://oj.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://hf.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wp.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cs.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qw.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uk.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://vp.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iv.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pw.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://rb.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://xt.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bw.yuntaijiaju.cn

Go:   // 手写循环
来源：http://og.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oh.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cf.wgjwhj.cn

[D15] 去重
来源：http://gu.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cx.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://cj.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://uf.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://rr.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cr.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://es.huanxung.cn

Ruby: arr.uniq
来源：http://mx.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://cz.huanxung.cn

[D16] 求和与平均值
来源：http://qq.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yf.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jc.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kp.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bd.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cj.521024.cn

Go:   // 手写循环累加
来源：http://ph.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mw.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://bg.newstarts.cn

[D17] 最大值与最小值
来源：http://hm.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://ve.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://ej.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qw.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://ch.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jc.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://if.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://he.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://dl.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://ok.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ua.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://fl.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yh.colortex.cn

TS:   nested.flat();
来源：http://jm.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ed.panjiajie.cn

Go:   // 手写双层循环
来源：http://sy.hahajie.cn

Ruby: nested.flatten
来源：http://mt.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nb.szsharing.cn

[D19] 按字段分组
来源：http://fo.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hx.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://li.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pl.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qi.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gr.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://tw.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xb.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ap.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://yk.lnxyls.cn

Py:   Counter(arr)
来源：http://kj.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://qr.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zp.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yv.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wq.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://vz.jctech888.com.cn

Ruby: arr.tally
来源：http://ob.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oj.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://ln.asd995.cn

Py:   x in arr
来源：http://yg.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://vq.yuexingan06.cn

JS:   arr.includes(x)
来源：http://dq.yuexingan06.cn

TS:   arr.includes(x)
来源：http://fp.colortex.cn

Java: list.contains(x)
来源：http://oi.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://xc.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://wi.shxzskj.cn

C#:   list.Contains(x)
来源：http://pv.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://bj.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eg.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vo.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uc.huixiangedu.cn

TS:   [...arr];
来源：http://rv.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://jk.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mo.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://dj.hnjuh.cn

C#:   new List<int>(list);
来源：http://zy.szsharing.cn

[D23] reduce 累积计算
来源：http://gu.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://us.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mb.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nu.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pz.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://an.haigaiapp.cn

Go:   // 手写循环
来源：http://fr.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zv.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kq.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://un.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vx.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://az.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zh.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tj.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kg.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ce.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ay.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vc.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://se.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qw.bookmarksfly.cn


<!-- 参考信息 -->