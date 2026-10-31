代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vl.huixinmuqiang.cn

Go:   return a, b
来源：http://ql.haigaiapp.cn

Ruby: return a, b
来源：http://mx.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://pg.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://ig.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://tb.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jt.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://fi.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://dy.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hc.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gq.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://si.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dq.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://jk.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cb.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hs.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ff.muxihuayi.cn

TS:   arr.map(String)
来源：http://tm.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ck.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ra.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://st.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ku.shxzskj.cn

[C08] 闭包
来源：http://tr.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://io.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qd.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qs.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pv.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sz.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mb.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ba.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oy.colortex.cn

[C09] 递归
来源：http://uq.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ho.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hh.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ng.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wx.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vg.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jk.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ir.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bc.9csxet.cn

[C10] 变量作用域
来源：http://us.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vt.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ta.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://je.jctech888.com.cn

TS:   同 JS
来源：http://zi.panjiajie.cn

Java: 方法内为块级作用域
来源：http://cc.panjiajie.cn

Go:   花括号块级作用域
来源：http://lc.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xz.jctech888.com.cn

C#:   块级作用域
来源：http://ee.521024.cn

[C11] 模块导入与导出
来源：http://fz.hnjuh.cn

Py:   from module import func
来源：http://mh.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oj.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qp.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tz.newstarts.cn

Java: import java.util.List;
来源：http://vy.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ve.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://nq.nszjky.cn

C#:   using System.Text;
来源：http://oa.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://ni.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://zp.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://ir.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://ws.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://eu.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hg.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://gn.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://kw.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lp.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://sy.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rs.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eg.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gu.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cr.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://js.newstarts.cn

Go:   func add(a, b int) int
来源：http://rz.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jx.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uv.lnxyls.cn

[C14] 泛型函数
来源：http://va.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hr.nicolike.cn

PHP:  // 无泛型
来源：http://iz.shtwfgs.cn

JS:   // 无泛型
来源：http://pe.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xa.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ug.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yk.panjiajie.cn

Ruby: # 无泛型
来源：http://bp.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sd.nicolike.cn

[C15] 解构 / 展开参数
来源：http://mb.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ab.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://sl.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qp.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tc.panjiajie.cn

Java: // 无解构
来源：http://ki.bjjhwx.cn

Go:   // 无解构
来源：http://ci.shxzukj.cn

Ruby: a, b = pair
来源：http://mr.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://ja.nicolike.cn

[C16] 函数 / 方法重载
来源：http://ig.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tv.shxzukj.cn

PHP:  // 无重载
来源：http://qf.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yl.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://dj.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://un.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://zu.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://uq.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ka.huixiangedu.cn

================================================================================
来源：http://nj.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://ww.bookmarksfly.cn

================================================================================
来源：http://nn.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://da.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kb.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sd.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hh.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ek.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gu.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ne.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://pw.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pm.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://vw.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fg.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eu.colortex.cn

JS:   arr.push(4);
来源：http://fb.szxytkj.cn

TS:   arr.push(4);
来源：http://ke.wgjwhj.cn

Java: list.add(4);
来源：http://yq.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://ac.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://hl.szxytkj.cn

C#:   list.Add(4);
来源：http://dg.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://rk.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://fh.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://il.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ov.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://zs.colortex.cn

Java: list.add(0, 0);
来源：http://mp.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gk.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://or.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://pz.nszjky.cn

[D04] 删除元素
来源：http://qi.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rk.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pj.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jf.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://fw.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wy.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://do.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vx.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ji.haigaiapp.cn

[D05] 访问与修改元素
来源：http://uv.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dd.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://em.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fp.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://gh.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ri.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://ps.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qh.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yf.newstarts.cn

[D06] 数组长度
来源：http://pn.shxzukj.cn

Py:   len(arr)
来源：http://fv.nicolike.cn

PHP:  count($arr);
来源：http://rk.jctech888.com.cn

JS:   arr.length
来源：http://le.gzmigu.cn

TS:   arr.length
来源：http://ic.yuntaijiaju.cn

Java: list.size();
来源：http://wf.yuntaijiaju.cn

Go:   len(arr)
来源：http://sl.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://rk.jctech888.com.cn

C#:   list.Count;
来源：http://fm.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://sh.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lz.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uu.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://qb.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://pk.521024.cn

Java: list.subList(1, 4);
来源：http://qf.huixiangedu.cn

Go:   arr[1:4]
来源：http://al.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://ot.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://ke.jctech888.com.cn

[D08] 合并两个数组
来源：http://sj.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://vv.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://jb.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kx.bjjhwx.cn

TS:   [...a, ...b];
来源：http://ax.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ez.huanxung.cn

Go:   append(a, b...)
来源：http://rv.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://xp.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://af.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://cn.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://qi.bookmarksfly.cn

PHP:  sort($arr);
来源：http://hg.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zk.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pe.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zy.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xm.szsharing.cn

Ruby: arr.sort
来源：http://op.huixiangedu.cn

C#:   list.Sort();
来源：http://ls.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dg.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ql.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yo.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rx.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wb.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ie.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yv.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jo.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cx.huixinmuqiang.cn

[D11] 反转数组
来源：http://gc.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://no.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://ux.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ex.asd995.cn

TS:   [...arr].reverse();
来源：http://zs.nszjky.cn

Java: Collections.reverse(list);
来源：http://jh.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://ir.haigaiapp.cn

Ruby: arr.reverse
来源：http://uz.shtwfgs.cn

C#:   list.Reverse();
来源：http://xn.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://dy.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://tn.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jm.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ky.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qu.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iv.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://xo.yuexingan06.cn

Ruby: arr.index(x)
来源：http://ug.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://ut.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://qe.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vg.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tk.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://zn.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://xr.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rp.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://le.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ua.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://go.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://ss.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cy.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oh.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://nf.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://dc.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ts.gzmigu.cn

Go:   // 手写循环
来源：http://st.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kr.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://te.chemitech.net.cn

[D15] 去重
来源：http://co.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pz.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://cw.hahajie.cn

JS:   [...new Set(arr)]
来源：http://bt.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://hb.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wu.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ii.shtwfgs.cn

Ruby: arr.uniq
来源：http://yj.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://ud.haigaiapp.cn

[D16] 求和与平均值
来源：http://pv.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ij.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ej.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pe.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yy.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vg.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://iq.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vt.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://at.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://rf.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://ig.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://cw.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fh.hahajie.cn

TS:   Math.max(...arr);
来源：http://ov.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jg.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uk.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://gg.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://pz.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://it.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ot.colortex.cn

PHP:  array_merge(...$nested);
来源：http://ii.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mv.haigaiapp.cn

TS:   nested.flat();
来源：http://jb.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://io.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://xr.521024.cn

Ruby: nested.flatten
来源：http://ia.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qe.gzmigu.cn

[D19] 按字段分组
来源：http://xa.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iq.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yd.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pa.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fw.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mr.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://zz.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gj.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ga.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://fx.bjjhwx.cn

Py:   Counter(arr)
来源：http://sj.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://mg.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://za.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://it.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ng.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://bt.jctech888.com.cn

Ruby: arr.tally
来源：http://ir.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mi.colortex.cn

[D21] 判断是否包含某元素
来源：http://by.panjiajie.cn

Py:   x in arr
来源：http://bt.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://zf.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://em.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://cr.yuexingan06.cn

Java: list.contains(x)
来源：http://tz.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://yy.521024.cn

Ruby: arr.include?(x)
来源：http://wc.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://qt.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://zj.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jy.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sc.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iy.gzmigu.cn

TS:   [...arr];
来源：http://jm.huanxung.cn


<!-- 参考信息 -->