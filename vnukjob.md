代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ol.szsharing.cn

Go:   return a, b
来源：http://vc.szxytkj.cn

Ruby: return a, b
来源：http://ex.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://ds.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://bg.asd995.cn

Py:   square = lambda x: x * x
来源：http://fz.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://od.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://jo.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://xm.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://na.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oi.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://cu.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ki.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://yz.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yv.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://of.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gp.9csxet.cn

TS:   arr.map(String)
来源：http://tc.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ee.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kc.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://ju.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nl.huixinmuqiang.cn

[C08] 闭包
来源：http://qd.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ks.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wm.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bb.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hf.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dn.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ms.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bx.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wa.hahajie.cn

[C09] 递归
来源：http://iu.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vr.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sw.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hl.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jq.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qp.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hm.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yn.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jy.9csxet.cn

[C10] 变量作用域
来源：http://hy.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ay.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pk.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ji.colortex.cn

TS:   同 JS
来源：http://td.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://po.asd995.cn

Go:   花括号块级作用域
来源：http://vs.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ui.jianghongdianzi.cn

C#:   块级作用域
来源：http://ot.jctech888.com.cn

[C11] 模块导入与导出
来源：http://ql.asd995.cn

Py:   from module import func
来源：http://mx.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mz.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ps.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://do.shtwfgs.cn

Java: import java.util.List;
来源：http://lh.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iv.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://bh.yuntaijiaju.cn

C#:   using System.Text;
来源：http://ds.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://sp.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://ko.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://jr.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://uj.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://lf.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zn.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://re.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://dv.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xc.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://bu.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yk.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dp.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kv.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://da.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ur.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://vq.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lw.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qz.shxzskj.cn

[C14] 泛型函数
来源：http://tr.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://km.newstarts.cn

PHP:  // 无泛型
来源：http://ew.gzmigu.cn

JS:   // 无泛型
来源：http://ja.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jl.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dw.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ma.hnjuh.cn

Ruby: # 无泛型
来源：http://ye.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sz.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://dh.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rm.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://mo.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fu.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rp.yuntaijiaju.cn

Java: // 无解构
来源：http://da.shxzskj.cn

Go:   // 无解构
来源：http://mz.colortex.cn

Ruby: a, b = pair
来源：http://be.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://rn.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://xd.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ot.szsharing.cn

PHP:  // 无重载
来源：http://yb.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://et.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://wm.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jx.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://qa.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://es.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ue.bookmarksfly.cn

================================================================================
来源：http://bj.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://gj.szxytkj.cn

================================================================================
来源：http://xi.szsharing.cn

[D01] 创建数组 / 列表
来源：http://kw.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pa.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bc.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oh.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hq.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://um.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://dt.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://ik.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yq.lnxyls.cn

[D02] 追加元素到末尾
来源：http://dx.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uz.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lk.shxzskj.cn

JS:   arr.push(4);
来源：http://gt.bjjhwx.cn

TS:   arr.push(4);
来源：http://jq.huixiangedu.cn

Java: list.add(4);
来源：http://rx.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://rr.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://mq.panjiajie.cn

C#:   list.Add(4);
来源：http://qw.hahajie.cn

[D03] 在指定位置插入元素
来源：http://ny.asd995.cn

Py:   arr.insert(0, 0)
来源：http://kt.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sv.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xq.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://rg.9csxet.cn

Java: list.add(0, 0);
来源：http://na.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yi.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vv.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://tm.yuntaijiaju.cn

[D04] 删除元素
来源：http://dc.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cp.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tx.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dm.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://nc.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://os.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nc.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bd.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yr.nicolike.cn

[D05] 访问与修改元素
来源：http://wc.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kd.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eq.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jx.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://ns.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://gb.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://hj.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bs.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://df.lnxyls.cn

[D06] 数组长度
来源：http://jv.huixinmuqiang.cn

Py:   len(arr)
来源：http://jw.nszjky.cn

PHP:  count($arr);
来源：http://ah.wgjwhj.cn

JS:   arr.length
来源：http://ku.panjiajie.cn

TS:   arr.length
来源：http://ha.szsharing.cn

Java: list.size();
来源：http://yc.panjiajie.cn

Go:   len(arr)
来源：http://ta.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://sp.shxzskj.cn

C#:   list.Count;
来源：http://yg.nicolike.cn

[D07] 切片 / 取子数组
来源：http://el.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ju.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xi.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://mi.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://ud.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://ny.nicolike.cn

Go:   arr[1:4]
来源：http://vj.gzmigu.cn

Ruby: arr[1, 3]
来源：http://wx.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://cs.nicolike.cn

[D08] 合并两个数组
来源：http://jz.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://qk.colortex.cn

PHP:  array_merge($a, $b);
来源：http://zs.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://he.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://hy.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pm.wgjwhj.cn

Go:   append(a, b...)
来源：http://rw.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://sp.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://gw.shtwfgs.cn

[D09] 排序（升序）
来源：http://ox.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://os.szxytkj.cn

PHP:  sort($arr);
来源：http://vf.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://es.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bb.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vp.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yl.nszjky.cn

Ruby: arr.sort
来源：http://rh.yuntaijiaju.cn

C#:   list.Sort();
来源：http://vn.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zm.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ui.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ut.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mu.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ar.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://re.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sx.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yq.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ym.haigaiapp.cn

[D11] 反转数组
来源：http://xb.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gg.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://sh.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ms.panjiajie.cn

TS:   [...arr].reverse();
来源：http://ct.nszjky.cn

Java: Collections.reverse(list);
来源：http://pu.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://pr.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://uc.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://hh.hnjuh.cn

[D12] 查找元素下标
来源：http://ap.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://fn.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vd.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wm.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sj.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ql.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://eo.haigaiapp.cn

Ruby: arr.index(x)
来源：http://zw.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://oo.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://uc.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xi.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oj.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://qk.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://pd.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ga.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://no.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vx.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ju.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://qq.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nz.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fa.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://yw.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://pl.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ij.nicolike.cn

Go:   // 手写循环
来源：http://vf.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ca.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ld.panjiajie.cn

[D15] 去重
来源：http://os.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jb.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://jm.colortex.cn

JS:   [...new Set(arr)]
来源：http://uf.9csxet.cn

TS:   [...new Set(arr)]
来源：http://bl.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qh.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cq.huixiangedu.cn

Ruby: arr.uniq
来源：http://um.asd995.cn

C#:   list.Distinct().ToList()
来源：http://jh.lnxyls.cn

[D16] 求和与平均值
来源：http://oz.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sf.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ib.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rs.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vr.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tm.chemitech.net.cn

Go:   // 手写循环累加
来源：http://bb.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tw.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://wj.szsharing.cn

[D17] 最大值与最小值
来源：http://ly.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://va.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://zi.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fk.huanxung.cn

TS:   Math.max(...arr);
来源：http://jz.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zo.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bg.colortex.cn

Ruby: arr.max;  arr.min
来源：http://ba.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://zo.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://lv.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xl.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://xc.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vh.szsharing.cn

TS:   nested.flat();
来源：http://jk.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tv.colortex.cn

Go:   // 手写双层循环
来源：http://ba.bookmarksfly.cn

Ruby: nested.flatten
来源：http://lg.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://di.gzmigu.cn

[D19] 按字段分组
来源：http://cv.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uk.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zm.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://on.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://eq.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fy.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://fk.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pb.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zy.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://jh.shxzskj.cn

Py:   Counter(arr)
来源：http://ot.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://av.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ag.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ig.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jm.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://ph.shxzukj.cn

Ruby: arr.tally
来源：http://rf.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iu.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://bi.yuntaijiaju.cn

Py:   x in arr
来源：http://fl.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://cu.jctech888.com.cn

JS:   arr.includes(x)
来源：http://vq.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://zx.bookmarksfly.cn

Java: list.contains(x)
来源：http://nh.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://us.panjiajie.cn

Ruby: arr.include?(x)
来源：http://xa.shxzukj.cn

C#:   list.Contains(x)
来源：http://zj.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://wx.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://es.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vx.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tq.muxihuayi.cn

TS:   [...arr];
来源：http://ia.huixiangedu.cn


<!-- 参考信息 -->