代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hk.hnjuh.cn

TS:   arr.map(String)
来源：http://ah.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://em.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jw.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://qe.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rn.szsharing.cn

[C08] 闭包
来源：http://hi.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ds.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ba.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ja.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bi.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yg.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jj.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hr.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kf.hahajie.cn

[C09] 递归
来源：http://kb.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oa.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lt.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cr.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xp.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fy.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kz.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mi.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ms.hnjuh.cn

[C10] 变量作用域
来源：http://bx.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vz.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hd.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jg.szxytkj.cn

TS:   同 JS
来源：http://tf.521024.cn

Java: 方法内为块级作用域
来源：http://fs.shxzukj.cn

Go:   花括号块级作用域
来源：http://qo.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://id.chemitech.net.cn

C#:   块级作用域
来源：http://lw.huanxung.cn

[C11] 模块导入与导出
来源：http://gr.shxzskj.cn

Py:   from module import func
来源：http://vq.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://na.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oe.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pn.huixiangedu.cn

Java: import java.util.List;
来源：http://uv.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lj.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://ir.huanxung.cn

C#:   using System.Text;
来源：http://rz.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://qb.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://he.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://hg.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://ne.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://mk.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eb.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://dz.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://hy.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xb.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://zd.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ag.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kr.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yt.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gz.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sv.shxzskj.cn

Go:   func add(a, b int) int
来源：http://rx.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xj.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eu.hnjuh.cn

[C14] 泛型函数
来源：http://ao.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cy.colortex.cn

PHP:  // 无泛型
来源：http://qc.lnxyls.cn

JS:   // 无泛型
来源：http://yf.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pi.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tr.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hb.521024.cn

Ruby: # 无泛型
来源：http://ht.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iy.9csxet.cn

[C15] 解构 / 展开参数
来源：http://td.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qn.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://nn.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://un.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ei.bookmarksfly.cn

Java: // 无解构
来源：http://ei.huixiangedu.cn

Go:   // 无解构
来源：http://sq.hahajie.cn

Ruby: a, b = pair
来源：http://cj.asd995.cn

C#:   var (a, b) = pair;
来源：http://ek.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://ac.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qk.szsharing.cn

PHP:  // 无重载
来源：http://bf.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sy.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://xv.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pp.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://dc.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ab.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rc.bjjhwx.cn

================================================================================
来源：http://gt.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://qi.gzmigu.cn

================================================================================
来源：http://pt.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://hs.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://su.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qa.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://le.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qs.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ms.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://ag.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://zl.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bb.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://mp.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fp.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mb.szsharing.cn

JS:   arr.push(4);
来源：http://ra.521024.cn

TS:   arr.push(4);
来源：http://uj.muxihuayi.cn

Java: list.add(4);
来源：http://ho.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://mn.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://ck.panjiajie.cn

C#:   list.Add(4);
来源：http://kc.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://xq.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://pe.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cs.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pr.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://ks.wgjwhj.cn

Java: list.add(0, 0);
来源：http://mx.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yo.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dk.colortex.cn

C#:   list.Insert(0, 0);
来源：http://rx.jctech888.com.cn

[D04] 删除元素
来源：http://ig.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ee.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fo.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nx.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://rr.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ju.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eq.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ub.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ww.muxihuayi.cn

[D05] 访问与修改元素
来源：http://bd.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ya.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ls.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yz.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://lz.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://fw.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://lz.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://no.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gz.9csxet.cn

[D06] 数组长度
来源：http://pe.asd995.cn

Py:   len(arr)
来源：http://xt.yuntaijiaju.cn

PHP:  count($arr);
来源：http://wi.huixiangedu.cn

JS:   arr.length
来源：http://ja.asd995.cn

TS:   arr.length
来源：http://ix.jctech888.com.cn

Java: list.size();
来源：http://qa.huanxung.cn

Go:   len(arr)
来源：http://ey.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://dz.panjiajie.cn

C#:   list.Count;
来源：http://bj.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://wz.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qe.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jg.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://fj.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://ha.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://xv.muxihuayi.cn

Go:   arr[1:4]
来源：http://fn.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://yh.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://ky.muxihuayi.cn

[D08] 合并两个数组
来源：http://ix.521024.cn

Py:   a + b;  a.extend(b)
来源：http://nm.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://kg.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yj.lnxyls.cn

TS:   [...a, ...b];
来源：http://ze.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ub.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://qv.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://vi.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://gs.chemitech.net.cn

[D09] 排序（升序）
来源：http://ez.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wv.colortex.cn

PHP:  sort($arr);
来源：http://oe.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rv.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xw.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mu.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kq.shxzukj.cn

Ruby: arr.sort
来源：http://dq.chemitech.net.cn

C#:   list.Sort();
来源：http://nv.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eh.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sj.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lp.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ih.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ag.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qc.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zx.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gy.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mx.shxzskj.cn

[D11] 反转数组
来源：http://xt.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sz.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://xm.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wi.colortex.cn

TS:   [...arr].reverse();
来源：http://qs.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://vu.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://xm.lnxyls.cn

Ruby: arr.reverse
来源：http://nj.shxzukj.cn

C#:   list.Reverse();
来源：http://ay.szsharing.cn

[D12] 查找元素下标
来源：http://pc.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://ic.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://le.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cf.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fk.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zb.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://di.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://pa.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://yr.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://di.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vn.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rn.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://zi.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://ny.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jk.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://he.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yh.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pw.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ax.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ao.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pi.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://pm.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://yu.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://il.huanxung.cn

Go:   // 手写循环
来源：http://en.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rn.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://su.haigaiapp.cn

[D15] 去重
来源：http://gx.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uz.szxytkj.cn

PHP:  array_unique($arr);
来源：http://zu.nszjky.cn

JS:   [...new Set(arr)]
来源：http://bm.szsharing.cn

TS:   [...new Set(arr)]
来源：http://ub.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jo.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cy.lnxyls.cn

Ruby: arr.uniq
来源：http://gh.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://bc.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://pd.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yq.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://da.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dr.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tx.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zx.shxzukj.cn

Go:   // 手写循环累加
来源：http://ou.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cb.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://ix.gzmigu.cn

[D17] 最大值与最小值
来源：http://dq.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://dc.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://zw.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pe.lnxyls.cn

TS:   Math.max(...arr);
来源：http://qa.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ho.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ua.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://li.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://kp.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://vg.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nj.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://ty.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://po.huixinmuqiang.cn

TS:   nested.flat();
来源：http://hd.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tn.huanxung.cn

Go:   // 手写双层循环
来源：http://oc.hnjuh.cn

Ruby: nested.flatten
来源：http://hw.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rd.szxytkj.cn

[D19] 按字段分组
来源：http://lx.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yb.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ro.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bh.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dr.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xo.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://zp.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dk.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wg.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://kz.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://xr.hahajie.cn

PHP:  array_count_values($arr);
来源：http://wy.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zn.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lq.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rb.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://mk.panjiajie.cn

Ruby: arr.tally
来源：http://pc.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pm.hahajie.cn

[D21] 判断是否包含某元素
来源：http://bn.jctech888.com.cn

Py:   x in arr
来源：http://er.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://my.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://oa.gzmigu.cn

TS:   arr.includes(x)
来源：http://qw.gzmigu.cn

Java: list.contains(x)
来源：http://su.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://yy.szxytkj.cn

Ruby: arr.include?(x)
来源：http://wh.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://nc.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://wn.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://om.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bg.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nz.shxzukj.cn

TS:   [...arr];
来源：http://vb.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://kw.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yd.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://yv.bjjhwx.cn

C#:   new List<int>(list);
来源：http://tk.asd995.cn

[D23] reduce 累积计算
来源：http://ck.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eh.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hv.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ac.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ek.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bs.haigaiapp.cn

Go:   // 手写循环
来源：http://kv.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://el.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hy.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://wl.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yb.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vm.521024.cn


<!-- 参考信息 -->