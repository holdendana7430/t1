代发 wailian999

[C06] 匿名函数 / lambda
来源：http://zo.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://wh.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tr.huanxung.cn

JS:   const square = x => x * x;
来源：http://pf.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://wj.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ju.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fv.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://zo.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cv.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://xe.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rc.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cy.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://go.hahajie.cn

TS:   arr.map(String)
来源：http://ze.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tl.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zw.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://mo.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://je.huixinmuqiang.cn

[C08] 闭包
来源：http://uv.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://de.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zc.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hx.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ik.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zz.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nn.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tg.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dz.huixinmuqiang.cn

[C09] 递归
来源：http://gh.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zz.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ko.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ug.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mo.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://br.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oi.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wp.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fg.bjjhwx.cn

[C10] 变量作用域
来源：http://kh.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qe.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bo.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cf.nicolike.cn

TS:   同 JS
来源：http://mc.hahajie.cn

Java: 方法内为块级作用域
来源：http://es.hahajie.cn

Go:   花括号块级作用域
来源：http://qt.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tw.bjjhwx.cn

C#:   块级作用域
来源：http://yj.shtwfgs.cn

[C11] 模块导入与导出
来源：http://nf.jctech888.com.cn

Py:   from module import func
来源：http://in.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gw.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rx.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zi.yuexingan06.cn

Java: import java.util.List;
来源：http://ee.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oa.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://zp.szxytkj.cn

C#:   using System.Text;
来源：http://qc.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://ge.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://cl.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://xv.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://tu.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ct.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vp.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://wz.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://ls.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lq.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://hp.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://es.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ke.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://he.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ea.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://em.gzmigu.cn

Go:   func add(a, b int) int
来源：http://ns.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xe.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bn.gzmigu.cn

[C14] 泛型函数
来源：http://uj.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hb.hahajie.cn

PHP:  // 无泛型
来源：http://xn.hnjuh.cn

JS:   // 无泛型
来源：http://oa.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zs.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pa.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ol.panjiajie.cn

Ruby: # 无泛型
来源：http://tr.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jr.hahajie.cn

[C15] 解构 / 展开参数
来源：http://cd.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://si.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://jg.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ma.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://da.jctech888.com.cn

Java: // 无解构
来源：http://eb.hahajie.cn

Go:   // 无解构
来源：http://ll.bjjhwx.cn

Ruby: a, b = pair
来源：http://uq.hahajie.cn

C#:   var (a, b) = pair;
来源：http://km.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://dy.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oh.9csxet.cn

PHP:  // 无重载
来源：http://mq.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yr.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://vy.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oz.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://qp.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://kl.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://it.haigaiapp.cn

================================================================================
来源：http://zb.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://qa.colortex.cn

================================================================================
来源：http://ql.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://bd.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zb.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ml.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ex.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ad.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iq.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://rw.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://xe.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dz.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://as.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zx.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mk.newstarts.cn

JS:   arr.push(4);
来源：http://st.shxzskj.cn

TS:   arr.push(4);
来源：http://so.bjjhwx.cn

Java: list.add(4);
来源：http://vl.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://ni.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://hf.shtwfgs.cn

C#:   list.Add(4);
来源：http://si.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://xk.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://ty.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kn.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ry.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://sx.shxzskj.cn

Java: list.add(0, 0);
来源：http://sa.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vn.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eo.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://jz.szxytkj.cn

[D04] 删除元素
来源：http://rq.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bi.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zz.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zh.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://lp.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ew.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tz.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wu.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kn.9csxet.cn

[D05] 访问与修改元素
来源：http://wl.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jt.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wk.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qy.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://xx.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://ua.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://iu.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qe.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ju.shxzskj.cn

[D06] 数组长度
来源：http://su.nszjky.cn

Py:   len(arr)
来源：http://mn.szsharing.cn

PHP:  count($arr);
来源：http://wm.jianghongdianzi.cn

JS:   arr.length
来源：http://vb.yuexingan06.cn

TS:   arr.length
来源：http://hi.9csxet.cn

Java: list.size();
来源：http://ss.jctech888.com.cn

Go:   len(arr)
来源：http://ym.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://ju.huanxung.cn

C#:   list.Count;
来源：http://xa.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://oc.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://he.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zd.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://ln.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://cv.nszjky.cn

Java: list.subList(1, 4);
来源：http://lm.jctech888.com.cn

Go:   arr[1:4]
来源：http://xv.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://dz.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://ck.yuexingan06.cn

[D08] 合并两个数组
来源：http://sn.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://rd.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://oh.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gk.jctech888.com.cn

TS:   [...a, ...b];
来源：http://dv.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xs.shxzskj.cn

Go:   append(a, b...)
来源：http://eo.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://cn.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://uq.hahajie.cn

[D09] 排序（升序）
来源：http://rd.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://va.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://lz.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://io.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ul.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zi.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fx.shxzskj.cn

Ruby: arr.sort
来源：http://nu.9csxet.cn

C#:   list.Sort();
来源：http://wj.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lt.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rl.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eq.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cp.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ej.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://im.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://za.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yv.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.lnxyls.cn

[D11] 反转数组
来源：http://to.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dx.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://wc.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nl.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://ny.521024.cn

Java: Collections.reverse(list);
来源：http://nr.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://rr.nszjky.cn

Ruby: arr.reverse
来源：http://pd.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://la.haigaiapp.cn

[D12] 查找元素下标
来源：http://ye.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://nh.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pp.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gp.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yx.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fv.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://oy.chemitech.net.cn

Ruby: arr.index(x)
来源：http://ky.asd995.cn

C#:   list.IndexOf(x);
来源：http://mr.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://sg.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tk.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pg.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://mf.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://dh.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://np.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bq.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uk.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rm.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://is.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://se.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nl.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://vh.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://ep.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ow.panjiajie.cn

Go:   // 手写循环
来源：http://cq.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ug.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xa.bjjhwx.cn

[D15] 去重
来源：http://qx.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xr.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://nb.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://mr.9csxet.cn

TS:   [...new Set(arr)]
来源：http://hl.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gx.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lm.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://ci.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://xg.bjjhwx.cn

[D16] 求和与平均值
来源：http://wi.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vm.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://na.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qz.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://as.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gn.shxzskj.cn

Go:   // 手写循环累加
来源：http://rq.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ai.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://bg.nicolike.cn

[D17] 最大值与最小值
来源：http://fv.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://at.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://hb.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sy.huanxung.cn

TS:   Math.max(...arr);
来源：http://js.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ch.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yu.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://ux.521024.cn

C#:   list.Max();  list.Min()
来源：http://gt.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://rg.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lz.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://zq.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://us.yuntaijiaju.cn

TS:   nested.flat();
来源：http://zo.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sv.huanxung.cn

Go:   // 手写双层循环
来源：http://um.nicolike.cn

Ruby: nested.flatten
来源：http://me.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ug.chemitech.net.cn

[D19] 按字段分组
来源：http://am.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wn.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uv.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xv.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cd.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cd.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://lt.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wb.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tk.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://te.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://yj.szsharing.cn

PHP:  array_count_values($arr);
来源：http://la.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ff.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sk.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://io.huanxung.cn

Go:   // 手写 map[T]int
来源：http://hg.szsharing.cn

Ruby: arr.tally
来源：http://ht.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ij.9csxet.cn

[D21] 判断是否包含某元素
来源：http://zm.wgjwhj.cn

Py:   x in arr
来源：http://bf.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://rf.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://mo.hahajie.cn

TS:   arr.includes(x)
来源：http://wd.szxytkj.cn

Java: list.contains(x)
来源：http://qe.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://mr.szxytkj.cn

Ruby: arr.include?(x)
来源：http://kh.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://lh.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://bx.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qh.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wn.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pq.hahajie.cn

TS:   [...arr];
来源：http://sw.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://xz.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zj.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://qz.colortex.cn

C#:   new List<int>(list);
来源：http://id.huixiangedu.cn


<!-- 参考信息 -->