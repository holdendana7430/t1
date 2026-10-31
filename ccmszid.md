代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://of.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sb.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fz.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://ip.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://om.nszjky.cn

[C07] 把函数作为参数传入
来源：http://wg.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mc.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zm.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ww.hahajie.cn

TS:   arr.map(String)
来源：http://jn.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tm.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hr.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://rx.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ku.shtwfgs.cn

[C08] 闭包
来源：http://sx.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://co.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jg.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zj.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hu.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qe.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ag.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wu.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xw.gzmigu.cn

[C09] 递归
来源：http://hv.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zd.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vl.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wv.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mi.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oy.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rf.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lv.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wl.gzmigu.cn

[C10] 变量作用域
来源：http://rv.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zm.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kz.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ob.shtwfgs.cn

TS:   同 JS
来源：http://bu.lnxyls.cn

Java: 方法内为块级作用域
来源：http://pk.huanxung.cn

Go:   花括号块级作用域
来源：http://hn.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eq.wgjwhj.cn

C#:   块级作用域
来源：http://df.shtwfgs.cn

[C11] 模块导入与导出
来源：http://gd.jctech888.com.cn

Py:   from module import func
来源：http://qp.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oc.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gh.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qf.newstarts.cn

Java: import java.util.List;
来源：http://yb.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pn.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://pi.9csxet.cn

C#:   using System.Text;
来源：http://xh.521024.cn

[C12] 立即执行函数 IIFE
来源：http://ul.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://ga.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://pj.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://at.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://hp.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ko.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://ef.521024.cn

Ruby: -> { puts "run" }.call
来源：http://db.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ud.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://wm.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bz.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fq.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ok.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dz.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wv.asd995.cn

Go:   func add(a, b int) int
来源：http://gj.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wy.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nu.huanxung.cn

[C14] 泛型函数
来源：http://bd.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qb.yuexingan06.cn

PHP:  // 无泛型
来源：http://fh.hahajie.cn

JS:   // 无泛型
来源：http://ga.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ig.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://je.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ao.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://bz.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zd.huanxung.cn

[C15] 解构 / 展开参数
来源：http://ac.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ij.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://kf.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ig.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dd.yuexingan06.cn

Java: // 无解构
来源：http://gr.chemitech.net.cn

Go:   // 无解构
来源：http://kk.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://em.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://qp.hahajie.cn

[C16] 函数 / 方法重载
来源：http://ch.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://si.szxytkj.cn

PHP:  // 无重载
来源：http://th.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lt.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://kb.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wh.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://la.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://bl.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oz.chemitech.net.cn

================================================================================
来源：http://jx.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://fs.shtwfgs.cn

================================================================================
来源：http://qo.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://cp.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zr.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jj.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qn.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://av.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pt.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://vt.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://fl.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://er.szsharing.cn

[D02] 追加元素到末尾
来源：http://vz.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ak.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vg.muxihuayi.cn

JS:   arr.push(4);
来源：http://hk.shtwfgs.cn

TS:   arr.push(4);
来源：http://tn.lnxyls.cn

Java: list.add(4);
来源：http://hi.colortex.cn

Go:   arr = append(arr, 4)
来源：http://at.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://xk.newstarts.cn

C#:   list.Add(4);
来源：http://ix.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://jd.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://er.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mf.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kw.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://bt.huanxung.cn

Java: list.add(0, 0);
来源：http://ow.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yr.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qk.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://xp.521024.cn

[D04] 删除元素
来源：http://ks.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sd.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vs.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ky.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://xv.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ae.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ym.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wh.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qp.lnxyls.cn

[D05] 访问与修改元素
来源：http://od.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pb.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lb.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mt.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://rz.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://kt.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ne.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bz.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fw.gzmigu.cn

[D06] 数组长度
来源：http://pt.colortex.cn

Py:   len(arr)
来源：http://to.bookmarksfly.cn

PHP:  count($arr);
来源：http://gr.huixinmuqiang.cn

JS:   arr.length
来源：http://cm.huanxung.cn

TS:   arr.length
来源：http://mr.wgjwhj.cn

Java: list.size();
来源：http://zb.chemitech.net.cn

Go:   len(arr)
来源：http://jq.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://zh.bookmarksfly.cn

C#:   list.Count;
来源：http://cv.521024.cn

[D07] 切片 / 取子数组
来源：http://pj.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mh.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ss.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://yr.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://hw.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://gw.haigaiapp.cn

Go:   arr[1:4]
来源：http://vi.9csxet.cn

Ruby: arr[1, 3]
来源：http://hb.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://kp.9csxet.cn

[D08] 合并两个数组
来源：http://rs.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://mt.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://gj.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gzmigu.cn

TS:   [...a, ...b];
来源：http://bp.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ty.jctech888.com.cn

Go:   append(a, b...)
来源：http://en.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://er.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://wq.chemitech.net.cn

[D09] 排序（升序）
来源：http://vx.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://tx.bookmarksfly.cn

PHP:  sort($arr);
来源：http://kz.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vp.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ug.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ac.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cz.newstarts.cn

Ruby: arr.sort
来源：http://mw.shxzukj.cn

C#:   list.Sort();
来源：http://ui.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ql.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pz.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ax.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wx.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oe.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xg.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ne.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nd.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jo.huixinmuqiang.cn

[D11] 反转数组
来源：http://qu.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ip.colortex.cn

PHP:  array_reverse($arr);
来源：http://mj.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xo.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://vo.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://eu.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://cv.nszjky.cn

Ruby: arr.reverse
来源：http://xi.shtwfgs.cn

C#:   list.Reverse();
来源：http://ix.panjiajie.cn

[D12] 查找元素下标
来源：http://oi.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://iq.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ez.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://di.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ah.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mh.colortex.cn

Go:   slices.Index(arr, x)
来源：http://wo.hahajie.cn

Ruby: arr.index(x)
来源：http://ve.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://au.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://mu.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tw.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://en.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://cz.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://bd.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bv.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dg.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ra.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vx.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://gp.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://as.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xp.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ko.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://dy.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rc.nicolike.cn

Go:   // 手写循环
来源：http://fr.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zl.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mm.wgjwhj.cn

[D15] 去重
来源：http://rl.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ha.nicolike.cn

PHP:  array_unique($arr);
来源：http://lw.hahajie.cn

JS:   [...new Set(arr)]
来源：http://ac.newstarts.cn

TS:   [...new Set(arr)]
来源：http://az.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zf.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uo.chemitech.net.cn

Ruby: arr.uniq
来源：http://yw.colortex.cn

C#:   list.Distinct().ToList()
来源：http://rl.lnxyls.cn

[D16] 求和与平均值
来源：http://ck.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://so.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bu.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://te.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sh.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zr.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://ps.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zx.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://kr.haigaiapp.cn

[D17] 最大值与最小值
来源：http://nv.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://jv.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://vw.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jf.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://cc.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yb.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ft.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://lf.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://xw.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://pn.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://um.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://uk.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fj.huixinmuqiang.cn

TS:   nested.flat();
来源：http://xe.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://po.yuexingan06.cn

Go:   // 手写双层循环
来源：http://cm.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://ev.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ax.szxytkj.cn

[D19] 按字段分组
来源：http://cm.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zk.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qt.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ti.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xp.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tr.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://rg.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sa.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mn.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://cx.shxzukj.cn

Py:   Counter(arr)
来源：http://et.asd995.cn

PHP:  array_count_values($arr);
来源：http://mi.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ja.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tr.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://au.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://jf.panjiajie.cn

Ruby: arr.tally
来源：http://xd.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cb.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://ny.521024.cn

Py:   x in arr
来源：http://wt.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://km.wgjwhj.cn

JS:   arr.includes(x)
来源：http://wq.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://qq.bookmarksfly.cn

Java: list.contains(x)
来源：http://yj.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://cs.huanxung.cn

Ruby: arr.include?(x)
来源：http://sf.wgjwhj.cn

C#:   list.Contains(x)
来源：http://fb.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://dr.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bq.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tx.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eu.bjjhwx.cn

TS:   [...arr];
来源：http://mo.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://ra.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xh.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://yb.9csxet.cn

C#:   new List<int>(list);
来源：http://ef.wgjwhj.cn

[D23] reduce 累积计算
来源：http://ka.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kc.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ju.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vi.shtwfgs.cn


<!-- 参考信息 -->