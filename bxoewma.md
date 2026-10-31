代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gk.nicolike.cn

Go:   return a, b
来源：http://rh.panjiajie.cn

Ruby: return a, b
来源：http://ix.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://yz.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://cx.nszjky.cn

Py:   square = lambda x: x * x
来源：http://wd.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fi.521024.cn

JS:   const square = x => x * x;
来源：http://qr.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://vl.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vc.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sx.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://ub.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://un.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://qe.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ja.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bw.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sk.asd995.cn

TS:   arr.map(String)
来源：http://zt.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pa.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ln.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://wa.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cu.hnjuh.cn

[C08] 闭包
来源：http://bd.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vl.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rq.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sd.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tn.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kz.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dv.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xs.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mh.yuntaijiaju.cn

[C09] 递归
来源：http://ui.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rw.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kh.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ep.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hh.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://su.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lx.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eq.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nn.muxihuayi.cn

[C10] 变量作用域
来源：http://eh.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ue.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ko.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hj.hahajie.cn

TS:   同 JS
来源：http://mf.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://sz.wgjwhj.cn

Go:   花括号块级作用域
来源：http://tl.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wb.nicolike.cn

C#:   块级作用域
来源：http://bp.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://wv.muxihuayi.cn

Py:   from module import func
来源：http://zi.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wb.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fv.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zb.shxzskj.cn

Java: import java.util.List;
来源：http://fn.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kb.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://ak.shxzskj.cn

C#:   using System.Text;
来源：http://dx.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://ux.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://js.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://hk.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://uj.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://gg.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yr.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://ta.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://kg.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hb.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://ln.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dw.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xy.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qo.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hy.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fx.szxytkj.cn

Go:   func add(a, b int) int
来源：http://fz.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qa.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gi.lnxyls.cn

[C14] 泛型函数
来源：http://vs.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dt.chemitech.net.cn

PHP:  // 无泛型
来源：http://er.chemitech.net.cn

JS:   // 无泛型
来源：http://zz.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fy.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ii.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://um.shtwfgs.cn

Ruby: # 无泛型
来源：http://ft.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gu.huanxung.cn

[C15] 解构 / 展开参数
来源：http://bx.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gj.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://se.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tp.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lx.gzmigu.cn

Java: // 无解构
来源：http://bw.nicolike.cn

Go:   // 无解构
来源：http://qs.nicolike.cn

Ruby: a, b = pair
来源：http://jq.nicolike.cn

C#:   var (a, b) = pair;
来源：http://je.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://ka.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tq.bookmarksfly.cn

PHP:  // 无重载
来源：http://lb.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nu.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ld.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kh.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://iu.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://pl.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ym.nszjky.cn

================================================================================
来源：http://ec.asd995.cn

D. 数组 / 列表 / 集合
来源：http://zl.wgjwhj.cn

================================================================================
来源：http://nf.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://qe.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jt.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xp.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ok.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xb.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ml.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://qf.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://in.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fo.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://qf.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hy.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://of.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://ax.huixiangedu.cn

TS:   arr.push(4);
来源：http://lu.lnxyls.cn

Java: list.add(4);
来源：http://yx.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://vi.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://bb.shtwfgs.cn

C#:   list.Add(4);
来源：http://sw.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://vz.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://gl.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://co.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nd.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://bl.shxzskj.cn

Java: list.add(0, 0);
来源：http://tl.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gy.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mx.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://pg.newstarts.cn

[D04] 删除元素
来源：http://vk.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ai.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mp.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jy.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://cw.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ze.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zn.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dn.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ch.hnjuh.cn

[D05] 访问与修改元素
来源：http://la.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mv.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jb.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gm.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://fe.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://qo.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://sg.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vo.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hl.newstarts.cn

[D06] 数组长度
来源：http://mp.szsharing.cn

Py:   len(arr)
来源：http://ni.szsharing.cn

PHP:  count($arr);
来源：http://ug.panjiajie.cn

JS:   arr.length
来源：http://ct.lnxyls.cn

TS:   arr.length
来源：http://oq.shxzskj.cn

Java: list.size();
来源：http://es.szsharing.cn

Go:   len(arr)
来源：http://pg.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://jt.szxytkj.cn

C#:   list.Count;
来源：http://qo.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://mt.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mo.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ma.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://aw.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://uz.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://nd.521024.cn

Go:   arr[1:4]
来源：http://lv.gzmigu.cn

Ruby: arr[1, 3]
来源：http://bz.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://kq.huixiangedu.cn

[D08] 合并两个数组
来源：http://ek.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://xs.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://au.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pl.muxihuayi.cn

TS:   [...a, ...b];
来源：http://mp.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ae.wgjwhj.cn

Go:   append(a, b...)
来源：http://kc.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://es.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://rf.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://vn.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://li.huixiangedu.cn

PHP:  sort($arr);
来源：http://kt.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mk.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cr.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ek.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://od.nicolike.cn

Ruby: arr.sort
来源：http://nm.yuntaijiaju.cn

C#:   list.Sort();
来源：http://es.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dx.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ry.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qc.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ze.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yu.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rm.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kq.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cx.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://if.szsharing.cn

[D11] 反转数组
来源：http://yj.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jv.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://yw.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://by.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://gp.asd995.cn

Java: Collections.reverse(list);
来源：http://ej.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://nt.nicolike.cn

Ruby: arr.reverse
来源：http://jm.haigaiapp.cn

C#:   list.Reverse();
来源：http://kc.jctech888.com.cn

[D12] 查找元素下标
来源：http://du.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://op.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bs.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ub.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://du.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kn.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://ej.gzmigu.cn

Ruby: arr.index(x)
来源：http://nx.9csxet.cn

C#:   list.IndexOf(x);
来源：http://ld.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://da.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://on.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ch.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://df.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://tg.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ig.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ye.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ok.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ai.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://nk.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://va.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vf.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://uz.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://uw.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vj.yuntaijiaju.cn

Go:   // 手写循环
来源：http://yt.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sp.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zp.jctech888.com.cn

[D15] 去重
来源：http://ky.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eq.9csxet.cn

PHP:  array_unique($arr);
来源：http://qb.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://sh.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://gy.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bj.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vb.jctech888.com.cn

Ruby: arr.uniq
来源：http://br.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://wp.shxzukj.cn

[D16] 求和与平均值
来源：http://yg.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://md.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nc.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://le.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ar.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fe.panjiajie.cn

Go:   // 手写循环累加
来源：http://rt.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ku.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://ro.huixiangedu.cn

[D17] 最大值与最小值
来源：http://eb.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://bb.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://ak.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ev.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://sq.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://th.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yo.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://ly.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://hw.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://qt.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qd.521024.cn

PHP:  array_merge(...$nested);
来源：http://yn.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fe.jctech888.com.cn

TS:   nested.flat();
来源：http://yk.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wf.yuexingan06.cn

Go:   // 手写双层循环
来源：http://hp.szxytkj.cn

Ruby: nested.flatten
来源：http://up.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ra.szsharing.cn

[D19] 按字段分组
来源：http://ci.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cn.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kf.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rk.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ra.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pr.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://fj.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fq.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bw.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://fg.gzmigu.cn

Py:   Counter(arr)
来源：http://vp.521024.cn

PHP:  array_count_values($arr);
来源：http://uh.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ip.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sx.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rm.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://jq.asd995.cn

Ruby: arr.tally
来源：http://vp.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bu.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://zk.nicolike.cn

Py:   x in arr
来源：http://en.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://kt.szxytkj.cn

JS:   arr.includes(x)
来源：http://ev.nszjky.cn

TS:   arr.includes(x)
来源：http://vg.shxzukj.cn

Java: list.contains(x)
来源：http://zn.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://kd.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://lm.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://js.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://zf.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vb.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yi.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qd.yuntaijiaju.cn

TS:   [...arr];
来源：http://bp.chemitech.net.cn


<!-- 参考信息 -->