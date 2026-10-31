代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://ql.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://av.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://so.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://gx.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fj.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://vl.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hv.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sv.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yv.asd995.cn

TS:   arr.map(String)
来源：http://ws.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cy.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oe.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://xi.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vo.lnxyls.cn

[C08] 闭包
来源：http://ze.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://er.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qj.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ou.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qz.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vk.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vr.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://co.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pc.huixiangedu.cn

[C09] 递归
来源：http://eu.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lc.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fg.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uo.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://os.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yc.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kr.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ar.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yy.huixinmuqiang.cn

[C10] 变量作用域
来源：http://ck.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ll.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hx.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cb.nicolike.cn

TS:   同 JS
来源：http://cj.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://kz.wgjwhj.cn

Go:   花括号块级作用域
来源：http://yb.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vn.asd995.cn

C#:   块级作用域
来源：http://wi.asd995.cn

[C11] 模块导入与导出
来源：http://zs.szxytkj.cn

Py:   from module import func
来源：http://zq.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xo.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sr.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ji.bjjhwx.cn

Java: import java.util.List;
来源：http://fi.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zc.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://ig.jctech888.com.cn

C#:   using System.Text;
来源：http://py.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://vy.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://gf.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://td.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://cq.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://gj.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kb.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://ht.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://xy.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vs.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://ul.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fb.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lm.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pi.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pg.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fj.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://jl.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yi.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ie.wgjwhj.cn

[C14] 泛型函数
来源：http://le.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://um.muxihuayi.cn

PHP:  // 无泛型
来源：http://oj.jianghongdianzi.cn

JS:   // 无泛型
来源：http://hw.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zd.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://co.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gr.yuexingan06.cn

Ruby: # 无泛型
来源：http://je.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gh.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://ei.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bh.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://ug.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vt.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dr.bjjhwx.cn

Java: // 无解构
来源：http://qp.lnxyls.cn

Go:   // 无解构
来源：http://gs.hnjuh.cn

Ruby: a, b = pair
来源：http://tk.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://sp.9csxet.cn

[C16] 函数 / 方法重载
来源：http://wf.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zq.yuexingan06.cn

PHP:  // 无重载
来源：http://tq.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://py.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ox.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oo.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://th.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://ms.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ib.shtwfgs.cn

================================================================================
来源：http://ek.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://fn.gzmigu.cn

================================================================================
来源：http://lf.colortex.cn

[D01] 创建数组 / 列表
来源：http://yp.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ih.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ba.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://az.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hm.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://if.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://fy.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://ro.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ss.hahajie.cn

[D02] 追加元素到末尾
来源：http://vu.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ic.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yi.szxytkj.cn

JS:   arr.push(4);
来源：http://rs.nicolike.cn

TS:   arr.push(4);
来源：http://zf.9csxet.cn

Java: list.add(4);
来源：http://yy.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://kz.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://jw.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://ji.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://vk.521024.cn

Py:   arr.insert(0, 0)
来源：http://ms.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vb.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jd.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://rc.nszjky.cn

Java: list.add(0, 0);
来源：http://qw.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mh.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ol.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://ds.521024.cn

[D04] 删除元素
来源：http://mg.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wx.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zv.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://et.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://cb.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ks.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gs.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ko.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pn.wgjwhj.cn

[D05] 访问与修改元素
来源：http://ti.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://va.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fr.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tf.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://cb.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://pv.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://xo.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dh.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eo.521024.cn

[D06] 数组长度
来源：http://iu.yuntaijiaju.cn

Py:   len(arr)
来源：http://fb.yuexingan06.cn

PHP:  count($arr);
来源：http://vg.huanxung.cn

JS:   arr.length
来源：http://bl.shxzskj.cn

TS:   arr.length
来源：http://ds.521024.cn

Java: list.size();
来源：http://lo.wgjwhj.cn

Go:   len(arr)
来源：http://tp.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://ka.panjiajie.cn

C#:   list.Count;
来源：http://vt.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://yk.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://de.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://as.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://kd.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://lv.szsharing.cn

Java: list.subList(1, 4);
来源：http://we.shxzukj.cn

Go:   arr[1:4]
来源：http://qk.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://hj.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://ze.lnxyls.cn

[D08] 合并两个数组
来源：http://ii.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://uv.521024.cn

PHP:  array_merge($a, $b);
来源：http://dc.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://av.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://ye.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sn.hahajie.cn

Go:   append(a, b...)
来源：http://lc.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://ui.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://mt.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://wb.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://es.lnxyls.cn

PHP:  sort($arr);
来源：http://db.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nm.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mz.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ix.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zw.yuexingan06.cn

Ruby: arr.sort
来源：http://dy.shxzskj.cn

C#:   list.Sort();
来源：http://fg.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qd.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mw.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ud.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://we.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fj.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jy.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vl.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cp.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zu.521024.cn

[D11] 反转数组
来源：http://up.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nv.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://vv.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://or.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://ly.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://zd.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://io.bjjhwx.cn

Ruby: arr.reverse
来源：http://st.hnjuh.cn

C#:   list.Reverse();
来源：http://fk.huanxung.cn

[D12] 查找元素下标
来源：http://mw.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://cz.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kv.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ve.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cw.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nr.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://ex.yuexingan06.cn

Ruby: arr.index(x)
来源：http://mg.9csxet.cn

C#:   list.IndexOf(x);
来源：http://ra.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://fy.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zr.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dc.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://so.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://kx.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://me.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ya.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sx.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eq.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://ux.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cg.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://se.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://du.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://ui.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kg.nszjky.cn

Go:   // 手写循环
来源：http://ri.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mu.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xp.hnjuh.cn

[D15] 去重
来源：http://ir.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wg.huanxung.cn

PHP:  array_unique($arr);
来源：http://il.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://qb.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://fp.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hk.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://en.newstarts.cn

Ruby: arr.uniq
来源：http://rn.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://fu.hnjuh.cn

[D16] 求和与平均值
来源：http://bm.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ls.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nk.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hw.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://da.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gf.newstarts.cn

Go:   // 手写循环累加
来源：http://wy.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://of.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://td.shtwfgs.cn

[D17] 最大值与最小值
来源：http://bu.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://ug.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://ji.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sk.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://oi.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gm.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rr.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://hl.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://hu.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://vj.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sk.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://dw.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bf.gzmigu.cn

TS:   nested.flat();
来源：http://ak.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xw.szsharing.cn

Go:   // 手写双层循环
来源：http://er.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://dw.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://md.yuexingan06.cn

[D19] 按字段分组
来源：http://tj.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://th.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qw.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ok.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xg.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sh.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://mb.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kj.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fq.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://do.newstarts.cn

Py:   Counter(arr)
来源：http://fo.nicolike.cn

PHP:  array_count_values($arr);
来源：http://ac.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ol.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gk.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pj.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://re.newstarts.cn

Ruby: arr.tally
来源：http://jk.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ju.9csxet.cn

[D21] 判断是否包含某元素
来源：http://nu.szsharing.cn

Py:   x in arr
来源：http://rm.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://yt.yuexingan06.cn

JS:   arr.includes(x)
来源：http://zu.521024.cn

TS:   arr.includes(x)
来源：http://hb.muxihuayi.cn

Java: list.contains(x)
来源：http://yh.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://sv.nicolike.cn

Ruby: arr.include?(x)
来源：http://hc.lnxyls.cn

C#:   list.Contains(x)
来源：http://mw.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://xq.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ft.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vp.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bq.huixinmuqiang.cn

TS:   [...arr];
来源：http://ts.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://rp.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cg.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://im.chemitech.net.cn

C#:   new List<int>(list);
来源：http://le.panjiajie.cn

[D23] reduce 累积计算
来源：http://cs.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hc.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nv.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eh.bjjhwx.cn


<!-- 参考信息 -->