代发 wailian999

[C06] 匿名函数 / lambda
来源：http://xe.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://wg.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xo.panjiajie.cn

JS:   const square = x => x * x;
来源：http://ed.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://yt.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eu.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jj.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://dv.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yc.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://gp.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yf.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wa.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mv.hahajie.cn

TS:   arr.map(String)
来源：http://rh.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cc.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vi.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://qf.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://da.huixiangedu.cn

[C08] 闭包
来源：http://oo.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ss.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ob.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iv.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ks.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ij.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ha.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hm.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://js.haigaiapp.cn

[C09] 递归
来源：http://vx.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oq.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rb.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jn.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ua.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ez.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mm.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lm.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gf.yuntaijiaju.cn

[C10] 变量作用域
来源：http://fx.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ec.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ph.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fg.jctech888.com.cn

TS:   同 JS
来源：http://cd.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://mg.chemitech.net.cn

Go:   花括号块级作用域
来源：http://wh.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ul.lnxyls.cn

C#:   块级作用域
来源：http://ap.gzmigu.cn

[C11] 模块导入与导出
来源：http://bi.nszjky.cn

Py:   from module import func
来源：http://nu.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wi.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fb.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cl.yuntaijiaju.cn

Java: import java.util.List;
来源：http://oj.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ui.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://gt.bookmarksfly.cn

C#:   using System.Text;
来源：http://fq.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://vc.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://rm.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://qw.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://ms.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://cd.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ay.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://fv.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://no.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rv.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://iq.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dy.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tz.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ef.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ex.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pu.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://bl.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qi.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://az.huanxung.cn

[C14] 泛型函数
来源：http://yr.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jb.colortex.cn

PHP:  // 无泛型
来源：http://nk.jianghongdianzi.cn

JS:   // 无泛型
来源：http://hq.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nl.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ua.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ek.jctech888.com.cn

Ruby: # 无泛型
来源：http://zp.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pv.szsharing.cn

[C15] 解构 / 展开参数
来源：http://om.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xn.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://ir.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://br.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jh.9csxet.cn

Java: // 无解构
来源：http://vx.panjiajie.cn

Go:   // 无解构
来源：http://sg.szsharing.cn

Ruby: a, b = pair
来源：http://sj.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://hw.521024.cn

[C16] 函数 / 方法重载
来源：http://ff.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ah.nszjky.cn

PHP:  // 无重载
来源：http://ux.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kn.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://pf.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lf.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://tt.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://yl.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ju.hahajie.cn

================================================================================
来源：http://jv.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://ph.huixinmuqiang.cn

================================================================================
来源：http://de.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://ym.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dy.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fj.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bb.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jo.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zo.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://oq.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://yf.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ra.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://xe.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sd.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zx.nicolike.cn

JS:   arr.push(4);
来源：http://ib.bjjhwx.cn

TS:   arr.push(4);
来源：http://uc.szxytkj.cn

Java: list.add(4);
来源：http://wm.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://oh.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://ku.colortex.cn

C#:   list.Add(4);
来源：http://rx.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://hp.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://ix.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://in.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lu.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://ib.nszjky.cn

Java: list.add(0, 0);
来源：http://sy.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vn.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kn.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://tm.huixiangedu.cn

[D04] 删除元素
来源：http://su.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nf.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cx.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nu.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://mk.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kh.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ih.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ig.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fw.shxzukj.cn

[D05] 访问与修改元素
来源：http://ih.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wp.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yo.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tl.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://lx.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://rg.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://va.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sd.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ta.hnjuh.cn

[D06] 数组长度
来源：http://ld.521024.cn

Py:   len(arr)
来源：http://zj.huanxung.cn

PHP:  count($arr);
来源：http://rj.9csxet.cn

JS:   arr.length
来源：http://mc.nszjky.cn

TS:   arr.length
来源：http://bd.yuexingan06.cn

Java: list.size();
来源：http://oq.bookmarksfly.cn

Go:   len(arr)
来源：http://vt.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://jo.nicolike.cn

C#:   list.Count;
来源：http://kp.szsharing.cn

[D07] 切片 / 取子数组
来源：http://da.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ol.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aa.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://fn.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://ra.szsharing.cn

Java: list.subList(1, 4);
来源：http://bt.newstarts.cn

Go:   arr[1:4]
来源：http://ls.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://tu.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://ho.shxzukj.cn

[D08] 合并两个数组
来源：http://iv.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://by.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://mh.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uc.bjjhwx.cn

TS:   [...a, ...b];
来源：http://np.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ti.521024.cn

Go:   append(a, b...)
来源：http://gj.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://ks.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://iw.hnjuh.cn

[D09] 排序（升序）
来源：http://ja.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://rd.wgjwhj.cn

PHP:  sort($arr);
来源：http://qw.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vv.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ib.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://me.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cm.huixiangedu.cn

Ruby: arr.sort
来源：http://fk.nicolike.cn

C#:   list.Sort();
来源：http://ul.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://em.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fd.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mt.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yk.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fa.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dc.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://no.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sz.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pe.colortex.cn

[D11] 反转数组
来源：http://pq.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yb.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://ex.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ui.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://xw.521024.cn

Java: Collections.reverse(list);
来源：http://fo.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://jq.jctech888.com.cn

Ruby: arr.reverse
来源：http://nb.chemitech.net.cn

C#:   list.Reverse();
来源：http://bx.hahajie.cn

[D12] 查找元素下标
来源：http://is.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://sv.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wa.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vx.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://st.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://il.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://pr.newstarts.cn

Ruby: arr.index(x)
来源：http://xy.asd995.cn

C#:   list.IndexOf(x);
来源：http://hm.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://ps.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ig.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dw.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://hi.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://rk.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ab.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://on.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kn.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yp.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://uh.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xn.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hf.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://yy.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://iz.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rm.521024.cn

Go:   // 手写循环
来源：http://zu.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cx.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://af.panjiajie.cn

[D15] 去重
来源：http://yu.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yz.shxzskj.cn

PHP:  array_unique($arr);
来源：http://ec.nszjky.cn

JS:   [...new Set(arr)]
来源：http://cr.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://mb.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xm.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vr.gzmigu.cn

Ruby: arr.uniq
来源：http://ti.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://vg.huixiangedu.cn

[D16] 求和与平均值
来源：http://hm.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gg.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xm.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ux.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pd.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dh.newstarts.cn

Go:   // 手写循环累加
来源：http://my.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vv.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://zx.huanxung.cn

[D17] 最大值与最小值
来源：http://ch.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://wg.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://mo.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sm.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://pn.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yg.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hw.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://uv.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://sg.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://ns.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dp.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://jd.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xz.9csxet.cn

TS:   nested.flat();
来源：http://km.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://to.nszjky.cn

Go:   // 手写双层循环
来源：http://nu.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://ik.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wd.521024.cn

[D19] 按字段分组
来源：http://bf.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xk.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://je.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lt.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nc.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dj.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://sl.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ye.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kk.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://mm.shxzskj.cn

Py:   Counter(arr)
来源：http://hw.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://gd.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://od.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cj.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://og.nszjky.cn

Go:   // 手写 map[T]int
来源：http://ou.szsharing.cn

Ruby: arr.tally
来源：http://qm.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qn.colortex.cn

[D21] 判断是否包含某元素
来源：http://ur.shtwfgs.cn

Py:   x in arr
来源：http://ig.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://tt.colortex.cn

JS:   arr.includes(x)
来源：http://cj.panjiajie.cn

TS:   arr.includes(x)
来源：http://rj.huanxung.cn

Java: list.contains(x)
来源：http://le.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://qh.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://fg.hahajie.cn

C#:   list.Contains(x)
来源：http://nx.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://my.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hn.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://av.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pq.jctech888.com.cn

TS:   [...arr];
来源：http://xi.colortex.cn

Java: new ArrayList<>(list);
来源：http://vc.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://av.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://me.asd995.cn

C#:   new List<int>(list);
来源：http://fw.shxzskj.cn


<!-- 参考信息 -->