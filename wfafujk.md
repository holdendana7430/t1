代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://jw.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://sj.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://ht.panjiajie.cn

[C05] 返回多个值
来源：http://iu.huixinmuqiang.cn

Py:   return a, b
来源：http://pt.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://vw.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ub.jctech888.com.cn

TS:   return { a, b };
来源：http://us.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://za.huanxung.cn

Go:   return a, b
来源：http://jr.colortex.cn

Ruby: return a, b
来源：http://fm.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://cz.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://ul.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://bb.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vv.521024.cn

JS:   const square = x => x * x;
来源：http://pv.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://jk.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ec.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ce.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://vq.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gg.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://ah.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://me.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cq.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zn.lnxyls.cn

TS:   arr.map(String)
来源：http://ar.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ry.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fx.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://rz.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mg.muxihuayi.cn

[C08] 闭包
来源：http://uo.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://br.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ks.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gl.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uo.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xg.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jo.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bd.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mb.hnjuh.cn

[C09] 递归
来源：http://wf.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jf.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pr.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ul.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ya.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yb.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lj.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ni.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ev.wgjwhj.cn

[C10] 变量作用域
来源：http://ch.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zx.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aa.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hi.szsharing.cn

TS:   同 JS
来源：http://bo.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://cx.colortex.cn

Go:   花括号块级作用域
来源：http://og.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rk.jctech888.com.cn

C#:   块级作用域
来源：http://hv.hnjuh.cn

[C11] 模块导入与导出
来源：http://ay.nszjky.cn

Py:   from module import func
来源：http://km.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://as.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ib.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mm.newstarts.cn

Java: import java.util.List;
来源：http://gx.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ht.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://nf.shxzskj.cn

C#:   using System.Text;
来源：http://uz.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://uq.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://js.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://hs.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://qk.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://af.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://on.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://mv.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://dd.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ac.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://yv.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dq.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ki.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qt.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ym.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nw.shxzskj.cn

Go:   func add(a, b int) int
来源：http://nv.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xg.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ie.szxytkj.cn

[C14] 泛型函数
来源：http://qz.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ji.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://hv.shxzskj.cn

JS:   // 无泛型
来源：http://qb.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vc.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cv.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dm.huixiangedu.cn

Ruby: # 无泛型
来源：http://xz.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tr.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://fx.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xm.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://hh.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gz.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oz.haigaiapp.cn

Java: // 无解构
来源：http://dh.shtwfgs.cn

Go:   // 无解构
来源：http://ze.szsharing.cn

Ruby: a, b = pair
来源：http://jg.nicolike.cn

C#:   var (a, b) = pair;
来源：http://cd.9csxet.cn

[C16] 函数 / 方法重载
来源：http://lv.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oe.szsharing.cn

PHP:  // 无重载
来源：http://sf.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://un.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://hj.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ry.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://ug.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ld.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hd.shtwfgs.cn

================================================================================
来源：http://qc.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://gr.huanxung.cn

================================================================================
来源：http://fu.huanxung.cn

[D01] 创建数组 / 列表
来源：http://lo.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hv.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xh.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lg.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vr.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wl.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ue.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://kc.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qm.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://bw.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jp.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sg.huanxung.cn

JS:   arr.push(4);
来源：http://nh.newstarts.cn

TS:   arr.push(4);
来源：http://qz.szxytkj.cn

Java: list.add(4);
来源：http://wl.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://lg.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://da.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://eg.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://ka.521024.cn

Py:   arr.insert(0, 0)
来源：http://tn.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lj.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xh.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://eh.shxzskj.cn

Java: list.add(0, 0);
来源：http://qf.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://il.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ev.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://ms.huanxung.cn

[D04] 删除元素
来源：http://lr.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uh.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ea.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mt.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://nv.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://be.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ul.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cm.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bl.shtwfgs.cn

[D05] 访问与修改元素
来源：http://di.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lc.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://em.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kc.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://np.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://wn.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://qm.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vb.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gz.bookmarksfly.cn

[D06] 数组长度
来源：http://pq.jctech888.com.cn

Py:   len(arr)
来源：http://pj.shxzskj.cn

PHP:  count($arr);
来源：http://mv.bookmarksfly.cn

JS:   arr.length
来源：http://ms.lnxyls.cn

TS:   arr.length
来源：http://rv.bookmarksfly.cn

Java: list.size();
来源：http://du.huixinmuqiang.cn

Go:   len(arr)
来源：http://ud.huanxung.cn

Ruby: arr.length; arr.size
来源：http://cz.jianghongdianzi.cn

C#:   list.Count;
来源：http://ot.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://hm.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rz.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qn.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://oz.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://wg.colortex.cn

Java: list.subList(1, 4);
来源：http://zc.shtwfgs.cn

Go:   arr[1:4]
来源：http://ts.nszjky.cn

Ruby: arr[1, 3]
来源：http://dt.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://ne.colortex.cn

[D08] 合并两个数组
来源：http://zd.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://ux.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://wp.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ju.newstarts.cn

TS:   [...a, ...b];
来源：http://ff.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gi.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://dk.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://wz.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://zw.521024.cn

[D09] 排序（升序）
来源：http://xy.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://xn.panjiajie.cn

PHP:  sort($arr);
来源：http://vn.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eu.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zl.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xc.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lw.wgjwhj.cn

Ruby: arr.sort
来源：http://ic.colortex.cn

C#:   list.Sort();
来源：http://ss.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hl.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pw.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dd.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oe.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ir.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iw.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kw.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rt.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ww.huixinmuqiang.cn

[D11] 反转数组
来源：http://ck.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zj.521024.cn

PHP:  array_reverse($arr);
来源：http://qc.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vq.colortex.cn

TS:   [...arr].reverse();
来源：http://bl.szxytkj.cn

Java: Collections.reverse(list);
来源：http://rb.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://hg.shxzukj.cn

Ruby: arr.reverse
来源：http://im.nszjky.cn

C#:   list.Reverse();
来源：http://ti.newstarts.cn

[D12] 查找元素下标
来源：http://xt.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://bc.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://el.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bt.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tr.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qh.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://vl.nszjky.cn

Ruby: arr.index(x)
来源：http://of.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://ef.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://ro.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ry.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tc.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://hc.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://zu.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ox.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zf.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pq.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://el.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ha.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ur.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xb.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://tr.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://bm.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ze.hahajie.cn

Go:   // 手写循环
来源：http://wm.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uz.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bh.huixiangedu.cn

[D15] 去重
来源：http://sd.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ig.panjiajie.cn

PHP:  array_unique($arr);
来源：http://qt.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://gw.szsharing.cn

TS:   [...new Set(arr)]
来源：http://gm.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://id.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dj.bookmarksfly.cn

Ruby: arr.uniq
来源：http://qf.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://zp.szxytkj.cn

[D16] 求和与平均值
来源：http://px.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://se.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tv.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sk.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fk.huixiangedu.cn

Go:   // 手写循环累加
来源：http://bh.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ko.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://em.szsharing.cn

[D17] 最大值与最小值
来源：http://qa.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://ee.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://ke.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://er.hnjuh.cn

TS:   Math.max(...arr);
来源：http://lk.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xt.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iu.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://uh.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://es.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://ks.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mk.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://pa.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lb.chemitech.net.cn

TS:   nested.flat();
来源：http://ho.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xb.lnxyls.cn

Go:   // 手写双层循环
来源：http://ke.haigaiapp.cn

Ruby: nested.flatten
来源：http://cv.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ve.yuntaijiaju.cn

[D19] 按字段分组
来源：http://fj.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wi.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://na.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rt.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nx.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://el.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://eu.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xv.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jc.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://nj.nicolike.cn

Py:   Counter(arr)
来源：http://gs.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://dz.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oo.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wy.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bw.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://wa.hnjuh.cn

Ruby: arr.tally
来源：http://ys.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ek.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://td.shxzskj.cn

Py:   x in arr
来源：http://gw.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://un.gzmigu.cn

JS:   arr.includes(x)
来源：http://hq.hnjuh.cn

TS:   arr.includes(x)
来源：http://pb.panjiajie.cn

Java: list.contains(x)
来源：http://ul.9csxet.cn


<!-- 参考信息 -->