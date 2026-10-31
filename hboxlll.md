代发 wailian999

[C06] 匿名函数 / lambda
来源：http://ch.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://mr.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kk.hahajie.cn

JS:   const square = x => x * x;
来源：http://ur.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://ce.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yp.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nu.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://dh.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yt.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://kq.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tj.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pd.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jw.jctech888.com.cn

TS:   arr.map(String)
来源：http://qm.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bj.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ih.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://nn.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jz.9csxet.cn

[C08] 闭包
来源：http://yf.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ht.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uf.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fy.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ct.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uh.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sy.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qu.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://so.huixiangedu.cn

[C09] 递归
来源：http://dq.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jr.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://je.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xw.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uv.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://be.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ym.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zc.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mw.gzmigu.cn

[C10] 变量作用域
来源：http://po.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zu.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://un.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://do.haigaiapp.cn

TS:   同 JS
来源：http://kd.asd995.cn

Java: 方法内为块级作用域
来源：http://zd.newstarts.cn

Go:   花括号块级作用域
来源：http://xn.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xe.haigaiapp.cn

C#:   块级作用域
来源：http://kj.nszjky.cn

[C11] 模块导入与导出
来源：http://ft.szsharing.cn

Py:   from module import func
来源：http://rx.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nx.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ln.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wb.9csxet.cn

Java: import java.util.List;
来源：http://op.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jf.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://ga.shtwfgs.cn

C#:   using System.Text;
来源：http://to.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://yt.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://ic.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://zd.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://wg.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://of.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ln.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://xl.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://cc.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zu.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://xt.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lq.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mg.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://go.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kw.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sl.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://yz.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ns.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mh.gzmigu.cn

[C14] 泛型函数
来源：http://jy.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wi.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://ft.panjiajie.cn

JS:   // 无泛型
来源：http://eh.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://it.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qi.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ub.wgjwhj.cn

Ruby: # 无泛型
来源：http://st.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jf.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://dx.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vn.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://xh.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lr.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gr.huixiangedu.cn

Java: // 无解构
来源：http://cv.yuntaijiaju.cn

Go:   // 无解构
来源：http://ym.yuexingan06.cn

Ruby: a, b = pair
来源：http://yy.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://bj.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://dg.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vz.huanxung.cn

PHP:  // 无重载
来源：http://nx.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vr.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://ph.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ok.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://ze.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://eh.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qs.newstarts.cn

================================================================================
来源：http://kc.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://sm.huixiangedu.cn

================================================================================
来源：http://et.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://cn.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gm.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://df.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://av.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lt.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zq.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://pd.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://uz.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jz.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://xe.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ct.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nc.huixiangedu.cn

JS:   arr.push(4);
来源：http://pa.huanxung.cn

TS:   arr.push(4);
来源：http://xo.asd995.cn

Java: list.add(4);
来源：http://ox.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://ek.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://de.newstarts.cn

C#:   list.Add(4);
来源：http://po.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://ie.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://yo.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sg.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nx.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://hx.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://fp.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dm.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nb.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://br.jianghongdianzi.cn

[D04] 删除元素
来源：http://gy.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uu.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ze.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jy.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://ux.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nw.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gi.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://on.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fu.panjiajie.cn

[D05] 访问与修改元素
来源：http://mh.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bt.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://el.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ua.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://bf.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://pi.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://cm.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jt.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eb.colortex.cn

[D06] 数组长度
来源：http://tv.chemitech.net.cn

Py:   len(arr)
来源：http://rv.nicolike.cn

PHP:  count($arr);
来源：http://bp.shxzskj.cn

JS:   arr.length
来源：http://kf.huixiangedu.cn

TS:   arr.length
来源：http://zn.huixinmuqiang.cn

Java: list.size();
来源：http://hr.huanxung.cn

Go:   len(arr)
来源：http://kx.colortex.cn

Ruby: arr.length; arr.size
来源：http://ti.bjjhwx.cn

C#:   list.Count;
来源：http://fo.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://ya.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hg.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://se.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://wr.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://iz.huanxung.cn

Java: list.subList(1, 4);
来源：http://jl.521024.cn

Go:   arr[1:4]
来源：http://it.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://gq.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://er.szsharing.cn

[D08] 合并两个数组
来源：http://ch.521024.cn

Py:   a + b;  a.extend(b)
来源：http://em.asd995.cn

PHP:  array_merge($a, $b);
来源：http://og.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nl.colortex.cn

TS:   [...a, ...b];
来源：http://et.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://av.huanxung.cn

Go:   append(a, b...)
来源：http://hr.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://jm.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://jz.newstarts.cn

[D09] 排序（升序）
来源：http://ni.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://hi.szxytkj.cn

PHP:  sort($arr);
来源：http://cg.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pc.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bw.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rh.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xg.colortex.cn

Ruby: arr.sort
来源：http://pl.yuntaijiaju.cn

C#:   list.Sort();
来源：http://le.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rk.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yz.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://be.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ea.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qi.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jo.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gx.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zn.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rl.lnxyls.cn

[D11] 反转数组
来源：http://pt.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ut.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://qz.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nf.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://lo.hahajie.cn

Java: Collections.reverse(list);
来源：http://my.colortex.cn

Go:   slices.Reverse(arr)
来源：http://fo.szsharing.cn

Ruby: arr.reverse
来源：http://rc.jctech888.com.cn

C#:   list.Reverse();
来源：http://fi.huanxung.cn

[D12] 查找元素下标
来源：http://nu.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://gc.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ug.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cr.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ru.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mo.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://jn.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://ua.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://fv.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://mi.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bj.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ky.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://dr.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://yq.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rl.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qk.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://es.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zj.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://lu.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vp.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://or.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://st.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://lp.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oy.jianghongdianzi.cn

Go:   // 手写循环
来源：http://tl.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gf.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ad.bookmarksfly.cn

[D15] 去重
来源：http://bb.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kr.huanxung.cn

PHP:  array_unique($arr);
来源：http://um.newstarts.cn

JS:   [...new Set(arr)]
来源：http://vl.nicolike.cn

TS:   [...new Set(arr)]
来源：http://ee.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mk.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hw.shxzukj.cn

Ruby: arr.uniq
来源：http://dq.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://qr.jctech888.com.cn

[D16] 求和与平均值
来源：http://ry.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yu.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://if.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ef.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ey.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lv.bjjhwx.cn

Go:   // 手写循环累加
来源：http://ll.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pv.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://we.muxihuayi.cn

[D17] 最大值与最小值
来源：http://uc.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://yc.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://rm.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nb.szxytkj.cn

TS:   Math.max(...arr);
来源：http://be.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://to.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://km.asd995.cn

Ruby: arr.max;  arr.min
来源：http://nx.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://cm.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://iy.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cl.521024.cn

PHP:  array_merge(...$nested);
来源：http://of.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dz.panjiajie.cn

TS:   nested.flat();
来源：http://jq.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://du.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://hx.bjjhwx.cn

Ruby: nested.flatten
来源：http://ia.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hy.bjjhwx.cn

[D19] 按字段分组
来源：http://je.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ne.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ui.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://do.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://te.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rk.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://dv.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fp.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hd.521024.cn

[D20] 统计每个元素出现次数
来源：http://sf.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://qk.szsharing.cn

PHP:  array_count_values($arr);
来源：http://os.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gk.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vp.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yc.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://dr.bjjhwx.cn

Ruby: arr.tally
来源：http://sp.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ye.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://ro.gzmigu.cn

Py:   x in arr
来源：http://gk.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://va.panjiajie.cn

JS:   arr.includes(x)
来源：http://of.szsharing.cn

TS:   arr.includes(x)
来源：http://et.shtwfgs.cn

Java: list.contains(x)
来源：http://wn.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://oj.lnxyls.cn

Ruby: arr.include?(x)
来源：http://nw.huanxung.cn

C#:   list.Contains(x)
来源：http://ef.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://tn.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qw.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nu.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lm.panjiajie.cn

TS:   [...arr];
来源：http://zy.szsharing.cn

Java: new ArrayList<>(list);
来源：http://jt.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yz.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://lp.lnxyls.cn

C#:   new List<int>(list);
来源：http://mh.shxzskj.cn


<!-- 参考信息 -->