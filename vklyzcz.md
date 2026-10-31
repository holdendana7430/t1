代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://jd.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://gp.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kv.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sj.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sq.nszjky.cn

TS:   arr.map(String)
来源：http://xi.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yo.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cq.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://wa.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xy.newstarts.cn

[C08] 闭包
来源：http://ip.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cg.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dn.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ey.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wi.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ev.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jh.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ad.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yv.wgjwhj.cn

[C09] 递归
来源：http://bv.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gi.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xi.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yq.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sw.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zw.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cm.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hc.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cu.yuexingan06.cn

[C10] 变量作用域
来源：http://ak.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zs.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hc.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uc.muxihuayi.cn

TS:   同 JS
来源：http://yr.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://oh.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://gx.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://du.jianghongdianzi.cn

C#:   块级作用域
来源：http://vl.shtwfgs.cn

[C11] 模块导入与导出
来源：http://ob.shxzukj.cn

Py:   from module import func
来源：http://tc.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vf.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vu.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ym.jctech888.com.cn

Java: import java.util.List;
来源：http://pp.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dd.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://gb.wgjwhj.cn

C#:   using System.Text;
来源：http://qa.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://xy.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://jb.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://ko.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://uk.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://al.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ym.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://dk.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://xn.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yj.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://wt.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ze.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wa.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nj.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jy.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kw.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://zh.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xc.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mk.muxihuayi.cn

[C14] 泛型函数
来源：http://zj.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hh.shxzukj.cn

PHP:  // 无泛型
来源：http://uk.521024.cn

JS:   // 无泛型
来源：http://zh.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gb.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://br.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eu.newstarts.cn

Ruby: # 无泛型
来源：http://gy.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ib.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://pp.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gf.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://ok.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rt.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nd.haigaiapp.cn

Java: // 无解构
来源：http://zn.muxihuayi.cn

Go:   // 无解构
来源：http://jx.hahajie.cn

Ruby: a, b = pair
来源：http://xs.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://an.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://pl.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gu.nicolike.cn

PHP:  // 无重载
来源：http://fn.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sl.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://tl.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ve.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://us.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://yv.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ff.jianghongdianzi.cn

================================================================================
来源：http://jr.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://sb.nszjky.cn

================================================================================
来源：http://hy.nszjky.cn

[D01] 创建数组 / 列表
来源：http://uy.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nc.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://td.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jc.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://na.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ow.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://gz.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://ys.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zy.newstarts.cn

[D02] 追加元素到末尾
来源：http://hp.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fd.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dj.bookmarksfly.cn

JS:   arr.push(4);
来源：http://eg.panjiajie.cn

TS:   arr.push(4);
来源：http://ay.jianghongdianzi.cn

Java: list.add(4);
来源：http://qi.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://yw.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://yw.colortex.cn

C#:   list.Add(4);
来源：http://so.newstarts.cn

[D03] 在指定位置插入元素
来源：http://hj.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://cy.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oa.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rc.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://yc.lnxyls.cn

Java: list.add(0, 0);
来源：http://pr.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yu.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ao.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://ap.shxzukj.cn

[D04] 删除元素
来源：http://ri.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://or.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lt.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ww.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://bt.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wo.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mm.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://op.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cc.yuexingan06.cn

[D05] 访问与修改元素
来源：http://zj.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kl.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cm.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://il.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://ib.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://if.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://er.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://id.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ai.shtwfgs.cn

[D06] 数组长度
来源：http://mi.hahajie.cn

Py:   len(arr)
来源：http://wj.9csxet.cn

PHP:  count($arr);
来源：http://zz.jianghongdianzi.cn

JS:   arr.length
来源：http://wr.gzmigu.cn

TS:   arr.length
来源：http://my.shxzskj.cn

Java: list.size();
来源：http://zx.9csxet.cn

Go:   len(arr)
来源：http://ak.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://bq.panjiajie.cn

C#:   list.Count;
来源：http://qd.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://yi.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nx.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dd.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://dj.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://ez.shxzukj.cn

Java: list.subList(1, 4);
来源：http://am.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://jz.szsharing.cn

Ruby: arr[1, 3]
来源：http://ej.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://ch.muxihuayi.cn

[D08] 合并两个数组
来源：http://kq.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://ej.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://qh.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wj.haigaiapp.cn

TS:   [...a, ...b];
来源：http://vr.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vg.szsharing.cn

Go:   append(a, b...)
来源：http://fk.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://si.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://jn.haigaiapp.cn

[D09] 排序（升序）
来源：http://gy.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://bv.shtwfgs.cn

PHP:  sort($arr);
来源：http://bs.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oy.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lk.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://to.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uo.yuexingan06.cn

Ruby: arr.sort
来源：http://ny.muxihuayi.cn

C#:   list.Sort();
来源：http://ph.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fv.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rr.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gd.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ew.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://la.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xj.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aw.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ll.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fb.lnxyls.cn

[D11] 反转数组
来源：http://fc.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lv.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://xe.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gq.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://ac.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://eo.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://zz.nicolike.cn

Ruby: arr.reverse
来源：http://es.szxytkj.cn

C#:   list.Reverse();
来源：http://ew.huixiangedu.cn

[D12] 查找元素下标
来源：http://bd.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://uf.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wa.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dr.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://za.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sv.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://uq.colortex.cn

Ruby: arr.index(x)
来源：http://zb.newstarts.cn

C#:   list.IndexOf(x);
来源：http://ym.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://pr.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zr.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sj.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://as.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://lq.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bn.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ln.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://be.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ru.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://oa.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ix.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jr.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://eo.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://wt.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sj.hahajie.cn

Go:   // 手写循环
来源：http://cf.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ub.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gq.shxzukj.cn

[D15] 去重
来源：http://xa.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wp.9csxet.cn

PHP:  array_unique($arr);
来源：http://vu.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://oe.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://lk.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ek.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dn.shxzskj.cn

Ruby: arr.uniq
来源：http://nz.colortex.cn

C#:   list.Distinct().ToList()
来源：http://br.huanxung.cn

[D16] 求和与平均值
来源：http://wa.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://de.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zw.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vv.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cq.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zg.newstarts.cn

Go:   // 手写循环累加
来源：http://do.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lg.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://rk.huanxung.cn

[D17] 最大值与最小值
来源：http://yy.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://dq.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://bn.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://be.panjiajie.cn

TS:   Math.max(...arr);
来源：http://py.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zg.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oq.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://os.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ab.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://qb.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gq.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://xu.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wk.nicolike.cn

TS:   nested.flat();
来源：http://aq.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uo.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://jh.jctech888.com.cn

Ruby: nested.flatten
来源：http://wu.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gm.yuexingan06.cn

[D19] 按字段分组
来源：http://ja.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bp.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qi.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sy.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ut.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ql.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://bd.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tn.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hp.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://pt.colortex.cn

Py:   Counter(arr)
来源：http://xx.nicolike.cn

PHP:  array_count_values($arr);
来源：http://in.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://av.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lm.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ex.nszjky.cn

Go:   // 手写 map[T]int
来源：http://nx.lnxyls.cn

Ruby: arr.tally
来源：http://vx.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gd.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://fm.9csxet.cn

Py:   x in arr
来源：http://ys.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://xl.asd995.cn

JS:   arr.includes(x)
来源：http://jk.asd995.cn

TS:   arr.includes(x)
来源：http://eu.nicolike.cn

Java: list.contains(x)
来源：http://sd.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://db.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://re.shxzukj.cn

C#:   list.Contains(x)
来源：http://uj.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://ch.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jg.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://df.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://we.shxzukj.cn

TS:   [...arr];
来源：http://jz.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://yz.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://si.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://ra.shtwfgs.cn

C#:   new List<int>(list);
来源：http://os.shtwfgs.cn

[D23] reduce 累积计算
来源：http://um.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ns.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qj.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yw.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bl.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ld.yuexingan06.cn

Go:   // 手写循环
来源：http://zj.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ig.huanxung.cn


<!-- 参考信息 -->