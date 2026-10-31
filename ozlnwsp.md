代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mv.shxzskj.cn

Go:   return a, b
来源：http://bh.huanxung.cn

Ruby: return a, b
来源：http://xf.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://bt.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://ge.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://pz.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xs.szsharing.cn

JS:   const square = x => x * x;
来源：http://oz.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://cz.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xq.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://px.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://kn.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://fz.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://al.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bx.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wh.shtwfgs.cn

TS:   arr.map(String)
来源：http://fc.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xu.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gi.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://rr.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xg.bjjhwx.cn

[C08] 闭包
来源：http://hk.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zx.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rc.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://te.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bv.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kz.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ce.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ht.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bl.gzmigu.cn

[C09] 递归
来源：http://gm.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qw.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://us.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ca.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tp.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zv.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://me.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bn.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fy.muxihuayi.cn

[C10] 变量作用域
来源：http://yj.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jt.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dc.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tn.bjjhwx.cn

TS:   同 JS
来源：http://va.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://tq.haigaiapp.cn

Go:   花括号块级作用域
来源：http://fv.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sa.wgjwhj.cn

C#:   块级作用域
来源：http://wr.521024.cn

[C11] 模块导入与导出
来源：http://xs.hahajie.cn

Py:   from module import func
来源：http://ah.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hc.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ll.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ji.asd995.cn

Java: import java.util.List;
来源：http://jc.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://px.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://ta.huixinmuqiang.cn

C#:   using System.Text;
来源：http://ks.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://io.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://wm.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://yp.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://ga.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://ko.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mg.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://dy.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://mp.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mp.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://rg.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ec.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dt.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qo.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://os.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sj.lnxyls.cn

Go:   func add(a, b int) int
来源：http://ah.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tw.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ti.jianghongdianzi.cn

[C14] 泛型函数
来源：http://nu.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fd.haigaiapp.cn

PHP:  // 无泛型
来源：http://tc.jianghongdianzi.cn

JS:   // 无泛型
来源：http://vt.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ex.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fb.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ty.newstarts.cn

Ruby: # 无泛型
来源：http://po.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xy.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://jy.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ly.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://nh.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yr.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lu.jctech888.com.cn

Java: // 无解构
来源：http://ye.nicolike.cn

Go:   // 无解构
来源：http://yi.panjiajie.cn

Ruby: a, b = pair
来源：http://dh.huanxung.cn

C#:   var (a, b) = pair;
来源：http://lb.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://ih.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bq.huixiangedu.cn

PHP:  // 无重载
来源：http://zm.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fo.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ud.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://aj.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://xa.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://gv.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oe.bjjhwx.cn

================================================================================
来源：http://jh.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://rq.asd995.cn

================================================================================
来源：http://lt.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://bx.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rg.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pt.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yt.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hr.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zg.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://ay.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://nx.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sd.lnxyls.cn

[D02] 追加元素到末尾
来源：http://iw.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jv.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zt.hnjuh.cn

JS:   arr.push(4);
来源：http://sw.haigaiapp.cn

TS:   arr.push(4);
来源：http://pg.jctech888.com.cn

Java: list.add(4);
来源：http://gt.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://tm.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://cx.gzmigu.cn

C#:   list.Add(4);
来源：http://td.asd995.cn

[D03] 在指定位置插入元素
来源：http://dv.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://sz.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vb.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ae.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://fo.haigaiapp.cn

Java: list.add(0, 0);
来源：http://yc.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iq.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yj.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://bz.newstarts.cn

[D04] 删除元素
来源：http://mw.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://il.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hl.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sr.colortex.cn

TS:   arr.splice(0, 1);
来源：http://am.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kf.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bv.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mf.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ig.hnjuh.cn

[D05] 访问与修改元素
来源：http://hv.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rl.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qd.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hg.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://ga.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://xu.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://xj.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wx.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rn.shxzskj.cn

[D06] 数组长度
来源：http://xa.521024.cn

Py:   len(arr)
来源：http://na.hnjuh.cn

PHP:  count($arr);
来源：http://qa.jctech888.com.cn

JS:   arr.length
来源：http://jw.yuntaijiaju.cn

TS:   arr.length
来源：http://vt.szxytkj.cn

Java: list.size();
来源：http://hn.colortex.cn

Go:   len(arr)
来源：http://qm.521024.cn

Ruby: arr.length; arr.size
来源：http://ns.shtwfgs.cn

C#:   list.Count;
来源：http://yi.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://av.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://to.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wh.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://xi.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://sh.9csxet.cn

Java: list.subList(1, 4);
来源：http://gq.szsharing.cn

Go:   arr[1:4]
来源：http://qc.hnjuh.cn

Ruby: arr[1, 3]
来源：http://pj.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://as.521024.cn

[D08] 合并两个数组
来源：http://zw.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://nd.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://uc.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vn.colortex.cn

TS:   [...a, ...b];
来源：http://yu.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bn.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://pv.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://ts.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://it.shtwfgs.cn

[D09] 排序（升序）
来源：http://jz.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://ga.shxzukj.cn

PHP:  sort($arr);
来源：http://on.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://re.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rg.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kh.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bw.newstarts.cn

Ruby: arr.sort
来源：http://gc.chemitech.net.cn

C#:   list.Sort();
来源：http://mo.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bt.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ir.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ct.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xa.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rx.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pa.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ic.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ew.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bb.huixiangedu.cn

[D11] 反转数组
来源：http://gs.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://df.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://am.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ks.szsharing.cn

TS:   [...arr].reverse();
来源：http://xy.newstarts.cn

Java: Collections.reverse(list);
来源：http://gj.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://sh.shtwfgs.cn

Ruby: arr.reverse
来源：http://sf.9csxet.cn

C#:   list.Reverse();
来源：http://zw.bjjhwx.cn

[D12] 查找元素下标
来源：http://ki.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://bu.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ps.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tw.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bh.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hq.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://mf.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://hd.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://vz.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://iu.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wk.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bw.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://uq.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://gi.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zo.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://of.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fo.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pg.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://rc.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xj.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ss.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://ls.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://cf.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yi.bjjhwx.cn

Go:   // 手写循环
来源：http://lx.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://to.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sq.huixinmuqiang.cn

[D15] 去重
来源：http://zb.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ma.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://jg.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://wy.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://qx.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uq.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vm.muxihuayi.cn

Ruby: arr.uniq
来源：http://ff.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://am.nicolike.cn

[D16] 求和与平均值
来源：http://sk.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dv.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ks.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mf.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cd.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hm.9csxet.cn

Go:   // 手写循环累加
来源：http://fy.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ew.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://bj.wgjwhj.cn

[D17] 最大值与最小值
来源：http://sh.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://ia.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://nm.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dj.szsharing.cn

TS:   Math.max(...arr);
来源：http://ui.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mc.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ux.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://qp.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://zr.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://tu.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yl.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://ed.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kq.newstarts.cn

TS:   nested.flat();
来源：http://cr.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kd.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://iq.nszjky.cn

Ruby: nested.flatten
来源：http://vn.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://du.bjjhwx.cn

[D19] 按字段分组
来源：http://lx.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bd.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://py.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zn.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vf.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xa.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://ww.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gb.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rq.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://qk.asd995.cn

Py:   Counter(arr)
来源：http://te.szsharing.cn

PHP:  array_count_values($arr);
来源：http://fc.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ds.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gp.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dm.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://dz.nszjky.cn

Ruby: arr.tally
来源：http://sc.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lk.nicolike.cn

[D21] 判断是否包含某元素
来源：http://pu.nicolike.cn

Py:   x in arr
来源：http://xi.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://zd.muxihuayi.cn

JS:   arr.includes(x)
来源：http://fs.gzmigu.cn

TS:   arr.includes(x)
来源：http://ks.huixiangedu.cn

Java: list.contains(x)
来源：http://kq.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://sr.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://vs.muxihuayi.cn

C#:   list.Contains(x)
来源：http://rq.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://oh.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ny.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xp.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pk.521024.cn

TS:   [...arr];
来源：http://wi.huanxung.cn


<!-- 参考信息 -->