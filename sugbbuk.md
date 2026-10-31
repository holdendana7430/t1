代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://li.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gd.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ls.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://do.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hv.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://op.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jg.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pl.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pc.szsharing.cn

TS:   arr.map(String)
来源：http://qo.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rg.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fo.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://np.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ba.huanxung.cn

[C08] 闭包
来源：http://yv.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lw.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fp.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wk.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gw.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kr.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zv.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wm.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ei.szsharing.cn

[C09] 递归
来源：http://op.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bu.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://md.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fz.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wo.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ig.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wc.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://er.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ad.shtwfgs.cn

[C10] 变量作用域
来源：http://ez.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lt.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://az.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kh.szxytkj.cn

TS:   同 JS
来源：http://la.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://hs.chemitech.net.cn

Go:   花括号块级作用域
来源：http://td.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://js.nszjky.cn

C#:   块级作用域
来源：http://jg.hnjuh.cn

[C11] 模块导入与导出
来源：http://ss.shtwfgs.cn

Py:   from module import func
来源：http://zy.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gr.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xv.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fa.bookmarksfly.cn

Java: import java.util.List;
来源：http://yo.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cj.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://ji.panjiajie.cn

C#:   using System.Text;
来源：http://my.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://vh.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://gj.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://qj.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://cm.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://bm.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hx.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://tz.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://oj.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jj.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://fw.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oa.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xp.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://az.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wl.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cg.hnjuh.cn

Go:   func add(a, b int) int
来源：http://aq.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gd.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qa.bjjhwx.cn

[C14] 泛型函数
来源：http://me.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zd.colortex.cn

PHP:  // 无泛型
来源：http://bd.wgjwhj.cn

JS:   // 无泛型
来源：http://eh.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yu.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pa.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nf.bookmarksfly.cn

Ruby: # 无泛型
来源：http://rv.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bd.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://iu.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zr.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://as.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vi.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zm.hnjuh.cn

Java: // 无解构
来源：http://bl.newstarts.cn

Go:   // 无解构
来源：http://em.hnjuh.cn

Ruby: a, b = pair
来源：http://tv.huanxung.cn

C#:   var (a, b) = pair;
来源：http://ed.newstarts.cn

[C16] 函数 / 方法重载
来源：http://tr.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zz.521024.cn

PHP:  // 无重载
来源：http://oh.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mb.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://ho.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nd.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://tq.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://yk.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ex.shxzukj.cn

================================================================================
来源：http://oq.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://fv.shxzukj.cn

================================================================================
来源：http://iy.newstarts.cn

[D01] 创建数组 / 列表
来源：http://rg.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vz.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cw.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gt.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nf.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ti.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://mg.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://bc.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://un.szsharing.cn

[D02] 追加元素到末尾
来源：http://mi.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gm.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://po.chemitech.net.cn

JS:   arr.push(4);
来源：http://sw.szsharing.cn

TS:   arr.push(4);
来源：http://xx.szsharing.cn

Java: list.add(4);
来源：http://zs.colortex.cn

Go:   arr = append(arr, 4)
来源：http://ye.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://ao.muxihuayi.cn

C#:   list.Add(4);
来源：http://yg.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://dl.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://fx.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pc.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lj.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://zo.9csxet.cn

Java: list.add(0, 0);
来源：http://ve.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ny.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ty.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://ug.shxzukj.cn

[D04] 删除元素
来源：http://vs.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tj.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bc.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fg.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://qj.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hg.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nm.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nw.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ka.huixiangedu.cn

[D05] 访问与修改元素
来源：http://xe.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ao.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uw.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zz.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://rw.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://ns.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://ek.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wp.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://li.szsharing.cn

[D06] 数组长度
来源：http://fc.huixinmuqiang.cn

Py:   len(arr)
来源：http://md.nicolike.cn

PHP:  count($arr);
来源：http://wz.newstarts.cn

JS:   arr.length
来源：http://qn.nszjky.cn

TS:   arr.length
来源：http://bg.jctech888.com.cn

Java: list.size();
来源：http://ks.asd995.cn

Go:   len(arr)
来源：http://wh.9csxet.cn

Ruby: arr.length; arr.size
来源：http://zl.asd995.cn

C#:   list.Count;
来源：http://nl.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://hp.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nh.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zt.colortex.cn

JS:   arr.slice(1, 4);
来源：http://xh.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://ei.lnxyls.cn

Java: list.subList(1, 4);
来源：http://cr.huanxung.cn

Go:   arr[1:4]
来源：http://kz.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://kj.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://jk.muxihuayi.cn

[D08] 合并两个数组
来源：http://jv.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://kf.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://uz.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nv.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://mt.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iv.asd995.cn

Go:   append(a, b...)
来源：http://ph.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://eh.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://ok.bjjhwx.cn

[D09] 排序（升序）
来源：http://nw.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://fv.huixiangedu.cn

PHP:  sort($arr);
来源：http://lq.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iw.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bd.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yo.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ye.shxzskj.cn

Ruby: arr.sort
来源：http://nt.nicolike.cn

C#:   list.Sort();
来源：http://sl.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xa.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rz.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cr.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vv.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xj.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mn.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yn.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ib.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ul.bjjhwx.cn

[D11] 反转数组
来源：http://qq.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vi.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://dv.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tp.gzmigu.cn

TS:   [...arr].reverse();
来源：http://fr.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://ff.asd995.cn

Go:   slices.Reverse(arr)
来源：http://fm.huanxung.cn

Ruby: arr.reverse
来源：http://iy.szxytkj.cn

C#:   list.Reverse();
来源：http://xd.shxzukj.cn

[D12] 查找元素下标
来源：http://zu.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://bt.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gv.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mu.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qd.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://er.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://xu.huanxung.cn

Ruby: arr.index(x)
来源：http://zl.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://mx.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://ed.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wo.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dw.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://gx.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://fd.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jt.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jq.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ha.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://by.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://wm.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iv.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gc.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://le.521024.cn

TS:   arr.map(x => x * 2)
来源：http://zz.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dl.jianghongdianzi.cn

Go:   // 手写循环
来源：http://sh.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ob.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yn.szsharing.cn

[D15] 去重
来源：http://bb.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rf.shxzukj.cn

PHP:  array_unique($arr);
来源：http://re.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://ce.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://ea.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://js.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xr.gzmigu.cn

Ruby: arr.uniq
来源：http://sl.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://ji.colortex.cn

[D16] 求和与平均值
来源：http://in.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qu.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://va.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jk.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tg.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cu.panjiajie.cn

Go:   // 手写循环累加
来源：http://bk.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vd.521024.cn

C#:   list.Sum();  list.Average()
来源：http://iw.panjiajie.cn

[D17] 最大值与最小值
来源：http://tc.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://wb.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://rc.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ko.shxzukj.cn

TS:   Math.max(...arr);
来源：http://fp.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lw.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wu.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://gq.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://xq.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://yf.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cv.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://th.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kn.shxzukj.cn

TS:   nested.flat();
来源：http://sa.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pa.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://gs.521024.cn

Ruby: nested.flatten
来源：http://yg.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lr.huixiangedu.cn

[D19] 按字段分组
来源：http://po.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gy.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://no.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xz.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://af.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cb.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://ut.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pk.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hs.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://ey.yuexingan06.cn

Py:   Counter(arr)
来源：http://zj.521024.cn

PHP:  array_count_values($arr);
来源：http://ru.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pi.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gm.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dw.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://bg.wgjwhj.cn

Ruby: arr.tally
来源：http://yw.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aa.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://aq.jianghongdianzi.cn

Py:   x in arr
来源：http://hv.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://mj.jctech888.com.cn

JS:   arr.includes(x)
来源：http://bz.asd995.cn

TS:   arr.includes(x)
来源：http://sk.huixiangedu.cn

Java: list.contains(x)
来源：http://zt.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://tw.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://bv.huanxung.cn

C#:   list.Contains(x)
来源：http://kb.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://qc.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pp.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ln.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://us.hahajie.cn

TS:   [...arr];
来源：http://py.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://nd.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qh.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://yf.hahajie.cn

C#:   new List<int>(list);
来源：http://bi.shtwfgs.cn

[D23] reduce 累积计算
来源：http://vc.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://se.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://es.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://us.jctech888.com.cn


<!-- 参考信息 -->