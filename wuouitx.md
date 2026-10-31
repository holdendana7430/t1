代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vo.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wk.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iy.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://ms.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://gl.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://xf.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://ic.yuexingan06.cn

[C05] 返回多个值
来源：http://aw.521024.cn

Py:   return a, b
来源：http://yq.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://sb.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lm.hahajie.cn

TS:   return { a, b };
来源：http://wg.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ib.jianghongdianzi.cn

Go:   return a, b
来源：http://zs.huixinmuqiang.cn

Ruby: return a, b
来源：http://aw.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://ae.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://jv.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://sn.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bd.hnjuh.cn

JS:   const square = x => x * x;
来源：http://hg.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ay.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ky.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dv.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://vr.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gn.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://oe.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ya.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aq.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hm.asd995.cn

TS:   arr.map(String)
来源：http://ua.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://av.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fx.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://tl.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zh.shxzukj.cn

[C08] 闭包
来源：http://ux.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tl.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bt.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ce.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rx.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pt.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ro.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://po.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dz.jianghongdianzi.cn

[C09] 递归
来源：http://tt.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tz.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dy.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cr.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tf.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nz.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://my.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xc.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ta.bjjhwx.cn

[C10] 变量作用域
来源：http://zk.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hi.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dt.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bm.shtwfgs.cn

TS:   同 JS
来源：http://nb.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://jj.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://gn.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://co.huixinmuqiang.cn

C#:   块级作用域
来源：http://oq.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://nm.nszjky.cn

Py:   from module import func
来源：http://fv.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gg.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oa.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://he.szsharing.cn

Java: import java.util.List;
来源：http://yk.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cw.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://oq.colortex.cn

C#:   using System.Text;
来源：http://xk.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://nq.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://mb.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://oq.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://do.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://ov.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vp.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://xd.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://jo.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ci.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://ck.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kn.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sk.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bd.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bk.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cb.szsharing.cn

Go:   func add(a, b int) int
来源：http://ue.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yl.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tq.521024.cn

[C14] 泛型函数
来源：http://iy.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://at.521024.cn

PHP:  // 无泛型
来源：http://xu.nicolike.cn

JS:   // 无泛型
来源：http://bl.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yp.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jw.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rm.521024.cn

Ruby: # 无泛型
来源：http://yh.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ai.asd995.cn

[C15] 解构 / 展开参数
来源：http://vk.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qg.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://yv.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lj.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uw.nicolike.cn

Java: // 无解构
来源：http://va.newstarts.cn

Go:   // 无解构
来源：http://dj.bjjhwx.cn

Ruby: a, b = pair
来源：http://ty.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://hn.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://dc.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tm.yuntaijiaju.cn

PHP:  // 无重载
来源：http://pj.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ud.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://it.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xt.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://xg.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://bb.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ll.jctech888.com.cn

================================================================================
来源：http://zy.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://uq.hahajie.cn

================================================================================
来源：http://qr.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://vh.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aw.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ys.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ll.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ud.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ed.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://da.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://ks.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cc.hahajie.cn

[D02] 追加元素到末尾
来源：http://da.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iv.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yt.nszjky.cn

JS:   arr.push(4);
来源：http://ca.hnjuh.cn

TS:   arr.push(4);
来源：http://qz.panjiajie.cn

Java: list.add(4);
来源：http://dv.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://kj.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://tv.gzmigu.cn

C#:   list.Add(4);
来源：http://lq.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://nf.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://ip.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bn.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ba.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ir.chemitech.net.cn

Java: list.add(0, 0);
来源：http://ig.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yt.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nj.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://mv.wgjwhj.cn

[D04] 删除元素
来源：http://tb.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sw.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cv.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://go.colortex.cn

TS:   arr.splice(0, 1);
来源：http://ef.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pa.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vh.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hn.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lz.muxihuayi.cn

[D05] 访问与修改元素
来源：http://qn.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pw.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://io.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ko.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://ox.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://en.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://yn.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fl.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wp.hnjuh.cn

[D06] 数组长度
来源：http://nx.hahajie.cn

Py:   len(arr)
来源：http://ih.panjiajie.cn

PHP:  count($arr);
来源：http://zh.hahajie.cn

JS:   arr.length
来源：http://bu.wgjwhj.cn

TS:   arr.length
来源：http://ae.yuexingan06.cn

Java: list.size();
来源：http://yp.asd995.cn

Go:   len(arr)
来源：http://ec.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://dk.gzmigu.cn

C#:   list.Count;
来源：http://fx.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://mx.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qn.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wj.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://ki.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://fz.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://xk.newstarts.cn

Go:   arr[1:4]
来源：http://ng.hnjuh.cn

Ruby: arr[1, 3]
来源：http://vd.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://xe.wgjwhj.cn

[D08] 合并两个数组
来源：http://kf.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://pi.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://zm.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sq.nicolike.cn

TS:   [...a, ...b];
来源：http://us.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pg.hnjuh.cn

Go:   append(a, b...)
来源：http://ps.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://jt.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://ql.panjiajie.cn

[D09] 排序（升序）
来源：http://lj.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://lm.hahajie.cn

PHP:  sort($arr);
来源：http://qd.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wt.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ys.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xh.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dt.szxytkj.cn

Ruby: arr.sort
来源：http://po.bjjhwx.cn

C#:   list.Sort();
来源：http://xr.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://va.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uq.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ec.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qx.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ss.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hs.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://by.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://co.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oy.wgjwhj.cn

[D11] 反转数组
来源：http://wf.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jr.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://cj.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yw.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://wk.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://mz.521024.cn

Go:   slices.Reverse(arr)
来源：http://or.newstarts.cn

Ruby: arr.reverse
来源：http://gj.9csxet.cn

C#:   list.Reverse();
来源：http://me.yuexingan06.cn

[D12] 查找元素下标
来源：http://uj.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://ut.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://to.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eo.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mk.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fz.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://fd.szxytkj.cn

Ruby: arr.index(x)
来源：http://on.521024.cn

C#:   list.IndexOf(x);
来源：http://dw.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://eb.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nz.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://po.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://ae.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://fe.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://su.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wj.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wg.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ed.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://rx.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oi.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://od.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://it.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://lp.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://le.hnjuh.cn

Go:   // 手写循环
来源：http://fz.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vr.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rm.newstarts.cn

[D15] 去重
来源：http://wt.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sx.gzmigu.cn

PHP:  array_unique($arr);
来源：http://np.nszjky.cn

JS:   [...new Set(arr)]
来源：http://cr.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://lm.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wv.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ul.521024.cn

Ruby: arr.uniq
来源：http://ae.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://ia.yuexingan06.cn

[D16] 求和与平均值
来源：http://sr.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ls.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://de.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wq.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qz.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ik.szsharing.cn

Go:   // 手写循环累加
来源：http://eh.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ln.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://bz.521024.cn

[D17] 最大值与最小值
来源：http://iq.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://zj.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://jm.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jk.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://ww.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://au.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ms.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://fe.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://yz.asd995.cn

[D18] 扁平化嵌套数组
来源：http://zu.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vi.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://lk.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pm.bjjhwx.cn

TS:   nested.flat();
来源：http://fa.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zt.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://aa.nszjky.cn

Ruby: nested.flatten
来源：http://ea.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://au.panjiajie.cn

[D19] 按字段分组
来源：http://qj.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ai.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zi.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ih.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ps.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wy.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://zf.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ia.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cb.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://fm.gzmigu.cn

Py:   Counter(arr)
来源：http://mm.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://bx.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uu.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ow.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ls.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://yx.jctech888.com.cn

Ruby: arr.tally
来源：http://ld.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xo.9csxet.cn

[D21] 判断是否包含某元素
来源：http://ht.shxzukj.cn

Py:   x in arr
来源：http://kh.newstarts.cn


<!-- 参考信息 -->