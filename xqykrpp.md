代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xk.colortex.cn

Go:   return a, b
来源：http://tt.chemitech.net.cn

Ruby: return a, b
来源：http://lh.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://sw.asd995.cn

[C06] 匿名函数 / lambda
来源：http://tp.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://lf.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rs.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://hn.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://fb.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ma.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wz.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://ro.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cv.colortex.cn

[C07] 把函数作为参数传入
来源：http://mt.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jc.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oi.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hx.nszjky.cn

TS:   arr.map(String)
来源：http://ia.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ab.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://py.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://eg.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rt.colortex.cn

[C08] 闭包
来源：http://df.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wx.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xj.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://al.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lz.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pv.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ky.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fg.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zq.wgjwhj.cn

[C09] 递归
来源：http://zu.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ck.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rc.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pc.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dc.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tq.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cc.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yj.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rr.huixinmuqiang.cn

[C10] 变量作用域
来源：http://cc.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ph.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ko.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kn.9csxet.cn

TS:   同 JS
来源：http://vp.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://kj.newstarts.cn

Go:   花括号块级作用域
来源：http://wp.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://th.shxzskj.cn

C#:   块级作用域
来源：http://dg.huanxung.cn

[C11] 模块导入与导出
来源：http://nb.bookmarksfly.cn

Py:   from module import func
来源：http://qz.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bu.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bt.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jp.hahajie.cn

Java: import java.util.List;
来源：http://fj.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kq.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://uj.bjjhwx.cn

C#:   using System.Text;
来源：http://zf.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://cx.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://lp.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://de.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://ak.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://ym.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mc.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://sj.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://je.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://st.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://mt.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mu.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xk.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ji.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lq.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://md.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://tj.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rq.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cm.chemitech.net.cn

[C14] 泛型函数
来源：http://ce.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ot.huanxung.cn

PHP:  // 无泛型
来源：http://hu.chemitech.net.cn

JS:   // 无泛型
来源：http://td.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ia.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sr.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://di.lnxyls.cn

Ruby: # 无泛型
来源：http://pu.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://er.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://mz.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vj.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://tt.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yy.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rn.shtwfgs.cn

Java: // 无解构
来源：http://wg.wgjwhj.cn

Go:   // 无解构
来源：http://nl.521024.cn

Ruby: a, b = pair
来源：http://os.szsharing.cn

C#:   var (a, b) = pair;
来源：http://kd.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://id.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xw.szsharing.cn

PHP:  // 无重载
来源：http://zd.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vu.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://fe.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kd.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://bb.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://dn.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fh.hnjuh.cn

================================================================================
来源：http://bq.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://gd.lnxyls.cn

================================================================================
来源：http://du.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://rb.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ib.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ig.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fe.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://do.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gd.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://iq.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://uh.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ow.nszjky.cn

[D02] 追加元素到末尾
来源：http://fn.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dk.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uk.gzmigu.cn

JS:   arr.push(4);
来源：http://ul.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://cp.huixiangedu.cn

Java: list.add(4);
来源：http://vo.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://gm.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://ii.szsharing.cn

C#:   list.Add(4);
来源：http://sx.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://lr.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://vi.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ka.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ly.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://bs.shxzukj.cn

Java: list.add(0, 0);
来源：http://tl.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qm.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://if.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://fd.asd995.cn

[D04] 删除元素
来源：http://gq.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jw.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yl.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://el.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://jm.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xl.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fs.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tr.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dg.huanxung.cn

[D05] 访问与修改元素
来源：http://aw.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dn.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tx.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vt.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://vq.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://pj.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ci.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cp.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mw.shxzskj.cn

[D06] 数组长度
来源：http://cn.nicolike.cn

Py:   len(arr)
来源：http://yb.newstarts.cn

PHP:  count($arr);
来源：http://ko.panjiajie.cn

JS:   arr.length
来源：http://vi.jctech888.com.cn

TS:   arr.length
来源：http://ki.shxzskj.cn

Java: list.size();
来源：http://ry.hnjuh.cn

Go:   len(arr)
来源：http://sg.newstarts.cn

Ruby: arr.length; arr.size
来源：http://ye.gzmigu.cn

C#:   list.Count;
来源：http://ot.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://vk.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pq.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kw.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://cb.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://nj.huanxung.cn

Java: list.subList(1, 4);
来源：http://ju.szsharing.cn

Go:   arr[1:4]
来源：http://my.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://xn.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://iv.asd995.cn

[D08] 合并两个数组
来源：http://ay.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://kg.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://pw.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nv.szxytkj.cn

TS:   [...a, ...b];
来源：http://cx.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zl.gzmigu.cn

Go:   append(a, b...)
来源：http://qw.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://ea.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://vh.szsharing.cn

[D09] 排序（升序）
来源：http://ur.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://xj.shxzskj.cn

PHP:  sort($arr);
来源：http://ek.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fj.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yq.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oj.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yt.bookmarksfly.cn

Ruby: arr.sort
来源：http://cm.shtwfgs.cn

C#:   list.Sort();
来源：http://df.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ui.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gc.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hc.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ji.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vj.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ik.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zd.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kl.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fb.jctech888.com.cn

[D11] 反转数组
来源：http://ie.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zy.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://ng.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bj.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://pl.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://gj.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://zp.shxzskj.cn

Ruby: arr.reverse
来源：http://zx.huanxung.cn

C#:   list.Reverse();
来源：http://ev.huanxung.cn

[D12] 查找元素下标
来源：http://cs.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://wu.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pi.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gi.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vm.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xc.colortex.cn

Go:   slices.Index(arr, x)
来源：http://kl.szxytkj.cn

Ruby: arr.index(x)
来源：http://yt.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://uo.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://rw.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ee.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wl.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://yn.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://dr.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ci.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://un.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ce.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ns.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://fc.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wz.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mq.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://xz.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://ra.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hk.muxihuayi.cn

Go:   // 手写循环
来源：http://ip.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xt.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mh.yuntaijiaju.cn

[D15] 去重
来源：http://px.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qg.shxzukj.cn

PHP:  array_unique($arr);
来源：http://om.9csxet.cn

JS:   [...new Set(arr)]
来源：http://br.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://aj.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gt.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ec.shxzukj.cn

Ruby: arr.uniq
来源：http://nl.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://qx.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://pg.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tc.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ji.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xw.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lk.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ez.asd995.cn

Go:   // 手写循环累加
来源：http://rp.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ax.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://qx.shxzskj.cn

[D17] 最大值与最小值
来源：http://dt.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://fw.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://ba.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sr.colortex.cn

TS:   Math.max(...arr);
来源：http://kk.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pj.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bj.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://al.asd995.cn

C#:   list.Max();  list.Min()
来源：http://iz.asd995.cn

[D18] 扁平化嵌套数组
来源：http://al.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fk.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://nh.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xx.szsharing.cn

TS:   nested.flat();
来源：http://pa.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ik.colortex.cn

Go:   // 手写双层循环
来源：http://vn.panjiajie.cn

Ruby: nested.flatten
来源：http://zz.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oy.shxzukj.cn

[D19] 按字段分组
来源：http://qv.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vy.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zj.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rt.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gf.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gl.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://lb.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nz.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tn.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://do.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://xt.huanxung.cn

PHP:  array_count_values($arr);
来源：http://gx.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kk.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kq.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zm.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://is.asd995.cn

Ruby: arr.tally
来源：http://am.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zr.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://fw.yuntaijiaju.cn

Py:   x in arr
来源：http://dp.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://me.chemitech.net.cn

JS:   arr.includes(x)
来源：http://ag.panjiajie.cn

TS:   arr.includes(x)
来源：http://qe.hnjuh.cn

Java: list.contains(x)
来源：http://in.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://yf.lnxyls.cn

Ruby: arr.include?(x)
来源：http://gz.szsharing.cn

C#:   list.Contains(x)
来源：http://vh.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://co.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rc.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bf.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ra.haigaiapp.cn

TS:   [...arr];
来源：http://bl.gzmigu.cn


<!-- 参考信息 -->