代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hv.huanxung.cn

Go:   return a, b
来源：http://kw.wgjwhj.cn

Ruby: return a, b
来源：http://yk.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://rv.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://dm.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ji.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ls.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://zs.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://wu.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hp.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://os.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://wo.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fx.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://tx.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lo.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wx.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pm.9csxet.cn

TS:   arr.map(String)
来源：http://zg.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qe.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ii.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://ot.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yh.yuexingan06.cn

[C08] 闭包
来源：http://qa.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wh.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pi.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nz.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tc.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qu.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uq.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zw.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eg.shtwfgs.cn

[C09] 递归
来源：http://lv.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qa.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dg.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ys.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qj.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ty.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hq.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ww.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qg.panjiajie.cn

[C10] 变量作用域
来源：http://bh.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ht.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ig.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ek.huixinmuqiang.cn

TS:   同 JS
来源：http://ue.colortex.cn

Java: 方法内为块级作用域
来源：http://cm.szsharing.cn

Go:   花括号块级作用域
来源：http://au.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://on.lnxyls.cn

C#:   块级作用域
来源：http://ej.panjiajie.cn

[C11] 模块导入与导出
来源：http://cf.colortex.cn

Py:   from module import func
来源：http://ax.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pn.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lo.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ec.szxytkj.cn

Java: import java.util.List;
来源：http://iw.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kh.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://sd.huixinmuqiang.cn

C#:   using System.Text;
来源：http://br.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://gq.colortex.cn

Py:   (lambda: print("run"))()
来源：http://vy.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://xi.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://pr.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://kr.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mv.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://sc.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://mg.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://do.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://hn.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vy.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mp.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vn.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vk.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yh.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://et.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pk.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hd.huanxung.cn

[C14] 泛型函数
来源：http://as.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ph.colortex.cn

PHP:  // 无泛型
来源：http://wi.nszjky.cn

JS:   // 无泛型
来源：http://ft.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yp.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nw.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ma.bjjhwx.cn

Ruby: # 无泛型
来源：http://fe.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yt.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://ne.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wr.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://bl.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ys.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ww.yuexingan06.cn

Java: // 无解构
来源：http://qc.shtwfgs.cn

Go:   // 无解构
来源：http://lx.chemitech.net.cn

Ruby: a, b = pair
来源：http://yp.szsharing.cn

C#:   var (a, b) = pair;
来源：http://pw.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://bg.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fi.szsharing.cn

PHP:  // 无重载
来源：http://hi.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vn.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://fm.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xj.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://zo.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://bx.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hp.haigaiapp.cn

================================================================================
来源：http://jn.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://np.lnxyls.cn

================================================================================
来源：http://tv.colortex.cn

[D01] 创建数组 / 列表
来源：http://ch.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vh.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://na.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kd.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://aq.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dk.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://mt.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://vc.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mf.gzmigu.cn

[D02] 追加元素到末尾
来源：http://yf.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://et.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://un.panjiajie.cn

JS:   arr.push(4);
来源：http://be.chemitech.net.cn

TS:   arr.push(4);
来源：http://vd.haigaiapp.cn

Java: list.add(4);
来源：http://bd.colortex.cn

Go:   arr = append(arr, 4)
来源：http://zf.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ao.newstarts.cn

C#:   list.Add(4);
来源：http://sw.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://of.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://ba.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ed.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ok.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://vz.shtwfgs.cn

Java: list.add(0, 0);
来源：http://jp.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tv.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qo.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://rk.nicolike.cn

[D04] 删除元素
来源：http://aa.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mz.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://em.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zv.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://aj.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ld.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jk.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vu.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vc.wgjwhj.cn

[D05] 访问与修改元素
来源：http://al.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tn.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ag.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wf.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://if.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://qr.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://pt.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kd.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vi.szsharing.cn

[D06] 数组长度
来源：http://vw.bjjhwx.cn

Py:   len(arr)
来源：http://lq.jctech888.com.cn

PHP:  count($arr);
来源：http://ch.yuexingan06.cn

JS:   arr.length
来源：http://rw.nszjky.cn

TS:   arr.length
来源：http://ub.panjiajie.cn

Java: list.size();
来源：http://ue.nszjky.cn

Go:   len(arr)
来源：http://px.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://rh.chemitech.net.cn

C#:   list.Count;
来源：http://tu.newstarts.cn

[D07] 切片 / 取子数组
来源：http://qp.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ti.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nf.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://um.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://my.nszjky.cn

Java: list.subList(1, 4);
来源：http://zw.shtwfgs.cn

Go:   arr[1:4]
来源：http://ow.colortex.cn

Ruby: arr[1, 3]
来源：http://mj.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://fd.huixiangedu.cn

[D08] 合并两个数组
来源：http://fe.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://fw.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://aw.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hf.newstarts.cn

TS:   [...a, ...b];
来源：http://wk.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ng.wgjwhj.cn

Go:   append(a, b...)
来源：http://ls.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://ak.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://qi.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://wr.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://qp.szxytkj.cn

PHP:  sort($arr);
来源：http://zf.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fy.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kb.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fl.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yt.gzmigu.cn

Ruby: arr.sort
来源：http://mi.shxzukj.cn

C#:   list.Sort();
来源：http://wd.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mq.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qw.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sk.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bu.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://an.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xa.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ft.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://us.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qz.asd995.cn

[D11] 反转数组
来源：http://fw.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ve.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://av.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pi.huanxung.cn

TS:   [...arr].reverse();
来源：http://yy.hnjuh.cn

Java: Collections.reverse(list);
来源：http://bv.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://kz.9csxet.cn

Ruby: arr.reverse
来源：http://hw.jctech888.com.cn

C#:   list.Reverse();
来源：http://vu.shxzukj.cn

[D12] 查找元素下标
来源：http://yd.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://dx.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://am.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gc.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ro.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nh.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://qh.huanxung.cn

Ruby: arr.index(x)
来源：http://ea.521024.cn

C#:   list.IndexOf(x);
来源：http://oe.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://ny.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cx.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vj.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://rb.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://bo.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vd.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sg.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ji.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ms.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://lv.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ae.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hj.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://ma.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://ms.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ct.shtwfgs.cn

Go:   // 手写循环
来源：http://lq.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://da.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ep.521024.cn

[D15] 去重
来源：http://gu.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cc.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://hv.colortex.cn

JS:   [...new Set(arr)]
来源：http://po.hahajie.cn

TS:   [...new Set(arr)]
来源：http://he.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xk.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cw.huixiangedu.cn

Ruby: arr.uniq
来源：http://pi.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://ru.panjiajie.cn

[D16] 求和与平均值
来源：http://fo.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://no.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xa.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pe.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lu.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vb.muxihuayi.cn

Go:   // 手写循环累加
来源：http://wv.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ij.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://ve.haigaiapp.cn

[D17] 最大值与最小值
来源：http://lp.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://nz.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://jh.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://am.nicolike.cn

TS:   Math.max(...arr);
来源：http://sx.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tf.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hj.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://rt.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://vq.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://jo.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ho.521024.cn

PHP:  array_merge(...$nested);
来源：http://cd.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://co.521024.cn

TS:   nested.flat();
来源：http://ao.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dp.huixiangedu.cn

Go:   // 手写双层循环
来源：http://lw.hnjuh.cn

Ruby: nested.flatten
来源：http://cr.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ii.chemitech.net.cn

[D19] 按字段分组
来源：http://ht.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ro.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sz.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ft.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ea.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://em.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://yz.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sv.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ym.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://ey.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://dz.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://ce.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gs.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bu.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ei.hahajie.cn

Go:   // 手写 map[T]int
来源：http://ta.panjiajie.cn

Ruby: arr.tally
来源：http://ug.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xv.hahajie.cn

[D21] 判断是否包含某元素
来源：http://cj.colortex.cn

Py:   x in arr
来源：http://di.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://ll.asd995.cn

JS:   arr.includes(x)
来源：http://nu.bjjhwx.cn

TS:   arr.includes(x)
来源：http://ar.chemitech.net.cn

Java: list.contains(x)
来源：http://rw.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://wy.shxzskj.cn

Ruby: arr.include?(x)
来源：http://qq.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://ol.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://xt.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zj.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kv.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jg.huixiangedu.cn

TS:   [...arr];
来源：http://yn.jctech888.com.cn


<!-- 参考信息 -->