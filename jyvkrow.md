代发 wailian999

[C06] 匿名函数 / lambda
来源：http://dv.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://rc.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uf.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://ye.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://dl.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cg.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wq.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://oj.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ye.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://yw.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ez.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tx.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yy.gzmigu.cn

TS:   arr.map(String)
来源：http://nj.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://so.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fq.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://jf.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yf.shxzskj.cn

[C08] 闭包
来源：http://gq.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vh.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://at.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vu.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zy.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gk.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ug.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nr.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mo.521024.cn

[C09] 递归
来源：http://tt.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zs.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uy.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fq.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gj.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lm.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ei.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tn.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yw.shxzskj.cn

[C10] 变量作用域
来源：http://vf.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lw.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ah.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lb.jctech888.com.cn

TS:   同 JS
来源：http://xj.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://je.szxytkj.cn

Go:   花括号块级作用域
来源：http://jr.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ap.hnjuh.cn

C#:   块级作用域
来源：http://uh.hahajie.cn

[C11] 模块导入与导出
来源：http://eo.bjjhwx.cn

Py:   from module import func
来源：http://vl.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fg.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gj.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sq.asd995.cn

Java: import java.util.List;
来源：http://gj.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ju.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://jq.nicolike.cn

C#:   using System.Text;
来源：http://md.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://aa.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://qu.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://eo.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://iq.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://oa.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vg.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://fj.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://xy.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nu.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://sq.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ts.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nj.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mp.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uk.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vn.shxzukj.cn

Go:   func add(a, b int) int
来源：http://pe.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://di.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nk.hahajie.cn

[C14] 泛型函数
来源：http://sf.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zf.newstarts.cn

PHP:  // 无泛型
来源：http://rg.nicolike.cn

JS:   // 无泛型
来源：http://ro.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xf.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qs.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ef.bjjhwx.cn

Ruby: # 无泛型
来源：http://bz.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vh.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://cc.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vy.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://op.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xj.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ey.huanxung.cn

Java: // 无解构
来源：http://uf.wgjwhj.cn

Go:   // 无解构
来源：http://ti.haigaiapp.cn

Ruby: a, b = pair
来源：http://dr.nszjky.cn

C#:   var (a, b) = pair;
来源：http://ex.hahajie.cn

[C16] 函数 / 方法重载
来源：http://ml.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ww.nicolike.cn

PHP:  // 无重载
来源：http://yn.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://aj.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://cj.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gy.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://ek.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://an.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ur.huixinmuqiang.cn

================================================================================
来源：http://jl.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://ky.yuntaijiaju.cn

================================================================================
来源：http://ox.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://ue.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bk.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xm.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jb.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bt.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kb.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://ko.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://ad.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://za.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://pe.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sr.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wi.chemitech.net.cn

JS:   arr.push(4);
来源：http://jz.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://ac.gzmigu.cn

Java: list.add(4);
来源：http://ld.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://xv.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://bv.chemitech.net.cn

C#:   list.Add(4);
来源：http://un.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://up.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://nu.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xt.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://na.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://ii.nszjky.cn

Java: list.add(0, 0);
来源：http://un.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ur.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qa.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://tx.colortex.cn

[D04] 删除元素
来源：http://yx.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uk.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mp.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ie.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://kf.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oh.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ju.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ew.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ie.hahajie.cn

[D05] 访问与修改元素
来源：http://zl.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ob.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fx.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dk.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://mo.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://lf.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://op.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dq.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cs.colortex.cn

[D06] 数组长度
来源：http://ng.bookmarksfly.cn

Py:   len(arr)
来源：http://eh.panjiajie.cn

PHP:  count($arr);
来源：http://mc.521024.cn

JS:   arr.length
来源：http://eu.jctech888.com.cn

TS:   arr.length
来源：http://dl.chemitech.net.cn

Java: list.size();
来源：http://hb.huanxung.cn

Go:   len(arr)
来源：http://cg.huanxung.cn

Ruby: arr.length; arr.size
来源：http://uk.lnxyls.cn

C#:   list.Count;
来源：http://gt.nszjky.cn

[D07] 切片 / 取子数组
来源：http://rb.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cs.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hk.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://pt.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://we.szxytkj.cn

Java: list.subList(1, 4);
来源：http://fh.hnjuh.cn

Go:   arr[1:4]
来源：http://fj.newstarts.cn

Ruby: arr[1, 3]
来源：http://vh.521024.cn

C#:   list.GetRange(1, 3);
来源：http://fu.wgjwhj.cn

[D08] 合并两个数组
来源：http://cx.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://po.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://eh.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cf.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ms.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aj.bjjhwx.cn

Go:   append(a, b...)
来源：http://iz.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://za.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://vy.hahajie.cn

[D09] 排序（升序）
来源：http://wz.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ai.hahajie.cn

PHP:  sort($arr);
来源：http://xi.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vr.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rt.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bd.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gi.jianghongdianzi.cn

Ruby: arr.sort
来源：http://gj.hahajie.cn

C#:   list.Sort();
来源：http://ll.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kr.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rt.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gd.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://px.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xe.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rh.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dz.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://by.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jc.hnjuh.cn

[D11] 反转数组
来源：http://jl.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tx.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://fm.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://az.shxzukj.cn

TS:   [...arr].reverse();
来源：http://gr.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://bu.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://dp.shxzskj.cn

Ruby: arr.reverse
来源：http://ik.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://cd.haigaiapp.cn

[D12] 查找元素下标
来源：http://kr.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://mt.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://su.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xu.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kl.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yu.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://hr.yuexingan06.cn

Ruby: arr.index(x)
来源：http://qo.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://vo.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://fy.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zx.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vi.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://wz.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://lf.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tg.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rd.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tc.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://br.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://oy.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vi.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dk.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://qz.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://ur.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cj.huanxung.cn

Go:   // 手写循环
来源：http://il.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iq.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dw.huanxung.cn

[D15] 去重
来源：http://oc.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wi.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://wq.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://zi.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://dc.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ev.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ju.yuexingan06.cn

Ruby: arr.uniq
来源：http://yw.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://my.shtwfgs.cn

[D16] 求和与平均值
来源：http://ny.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ir.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://du.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gn.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tz.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://in.huanxung.cn

Go:   // 手写循环累加
来源：http://qv.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vn.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://wz.huixiangedu.cn

[D17] 最大值与最小值
来源：http://qs.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://na.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://sl.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://el.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://de.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pi.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vt.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://nu.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://na.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://nn.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vy.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://cd.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ub.huixiangedu.cn

TS:   nested.flat();
来源：http://fh.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gt.shtwfgs.cn

Go:   // 手写双层循环
来源：http://ee.chemitech.net.cn

Ruby: nested.flatten
来源：http://lf.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://us.newstarts.cn

[D19] 按字段分组
来源：http://le.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tv.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ts.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qm.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ui.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zr.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://ps.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jp.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fk.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://lb.shxzskj.cn

Py:   Counter(arr)
来源：http://bu.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://kq.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ak.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kj.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qa.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://zh.jctech888.com.cn

Ruby: arr.tally
来源：http://be.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wb.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://cb.szsharing.cn

Py:   x in arr
来源：http://kh.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://gf.newstarts.cn

JS:   arr.includes(x)
来源：http://iv.nszjky.cn

TS:   arr.includes(x)
来源：http://th.huixiangedu.cn

Java: list.contains(x)
来源：http://jt.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://iu.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://fu.chemitech.net.cn

C#:   list.Contains(x)
来源：http://rr.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://ny.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tl.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ez.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mu.bjjhwx.cn

TS:   [...arr];
来源：http://ea.nszjky.cn

Java: new ArrayList<>(list);
来源：http://ky.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ry.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://gp.nicolike.cn

C#:   new List<int>(list);
来源：http://sc.gzmigu.cn


<!-- 参考信息 -->