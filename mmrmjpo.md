代发 wailian999

[C06] 匿名函数 / lambda
来源：http://vc.szsharing.cn

Py:   square = lambda x: x * x
来源：http://wj.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bi.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://ka.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://tu.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://je.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rp.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://sz.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oh.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://sp.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wx.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jw.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nn.yuexingan06.cn

TS:   arr.map(String)
来源：http://ru.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jz.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zp.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://it.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://so.lnxyls.cn

[C08] 闭包
来源：http://nb.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ep.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wp.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ee.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fg.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gf.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ff.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qo.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yx.shxzukj.cn

[C09] 递归
来源：http://pu.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://av.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tn.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dx.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ka.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yv.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jp.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kf.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mq.muxihuayi.cn

[C10] 变量作用域
来源：http://mm.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gf.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kh.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sg.szxytkj.cn

TS:   同 JS
来源：http://la.gzmigu.cn

Java: 方法内为块级作用域
来源：http://ys.jctech888.com.cn

Go:   花括号块级作用域
来源：http://mo.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rj.muxihuayi.cn

C#:   块级作用域
来源：http://bm.szsharing.cn

[C11] 模块导入与导出
来源：http://bi.nicolike.cn

Py:   from module import func
来源：http://mz.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kp.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dm.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ib.nicolike.cn

Java: import java.util.List;
来源：http://xy.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xt.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://ek.jianghongdianzi.cn

C#:   using System.Text;
来源：http://cf.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://jj.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://bx.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://ko.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://tq.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://vr.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xm.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://nv.521024.cn

Ruby: -> { puts "run" }.call
来源：http://mr.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ps.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://ty.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hw.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sl.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ds.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bs.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oz.colortex.cn

Go:   func add(a, b int) int
来源：http://mi.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ab.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xc.hahajie.cn

[C14] 泛型函数
来源：http://ef.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mj.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://lm.colortex.cn

JS:   // 无泛型
来源：http://kx.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ym.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cz.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xd.muxihuayi.cn

Ruby: # 无泛型
来源：http://tu.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zc.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://rq.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://er.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://lv.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mw.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://in.gzmigu.cn

Java: // 无解构
来源：http://fn.shtwfgs.cn

Go:   // 无解构
来源：http://we.shxzukj.cn

Ruby: a, b = pair
来源：http://qf.colortex.cn

C#:   var (a, b) = pair;
来源：http://cw.nszjky.cn

[C16] 函数 / 方法重载
来源：http://rl.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://te.huixiangedu.cn

PHP:  // 无重载
来源：http://rb.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rq.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://kg.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ts.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://bz.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://vm.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xn.panjiajie.cn

================================================================================
来源：http://uw.colortex.cn

D. 数组 / 列表 / 集合
来源：http://em.asd995.cn

================================================================================
来源：http://di.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://xm.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lw.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aq.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ff.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mo.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qc.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://le.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://ro.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://db.asd995.cn

[D02] 追加元素到末尾
来源：http://kg.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://so.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ut.muxihuayi.cn

JS:   arr.push(4);
来源：http://mn.nicolike.cn

TS:   arr.push(4);
来源：http://uf.shxzukj.cn

Java: list.add(4);
来源：http://ef.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://bk.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://be.asd995.cn

C#:   list.Add(4);
来源：http://zq.newstarts.cn

[D03] 在指定位置插入元素
来源：http://ao.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://of.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://we.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vp.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://yf.newstarts.cn

Java: list.add(0, 0);
来源：http://kt.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pw.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zh.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://cp.nszjky.cn

[D04] 删除元素
来源：http://ll.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wj.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bj.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://do.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://bp.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://do.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ww.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yc.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://si.huanxung.cn

[D05] 访问与修改元素
来源：http://yg.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gl.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uk.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://el.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://pf.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://mi.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://dz.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sh.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qq.bookmarksfly.cn

[D06] 数组长度
来源：http://lr.lnxyls.cn

Py:   len(arr)
来源：http://jm.jianghongdianzi.cn

PHP:  count($arr);
来源：http://zy.szxytkj.cn

JS:   arr.length
来源：http://dc.muxihuayi.cn

TS:   arr.length
来源：http://st.huixiangedu.cn

Java: list.size();
来源：http://gm.chemitech.net.cn

Go:   len(arr)
来源：http://ge.521024.cn

Ruby: arr.length; arr.size
来源：http://eg.haigaiapp.cn

C#:   list.Count;
来源：http://gz.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://wk.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jz.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ve.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://ov.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://so.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://as.jctech888.com.cn

Go:   arr[1:4]
来源：http://na.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://ei.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://dp.wgjwhj.cn

[D08] 合并两个数组
来源：http://xv.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://zy.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://cm.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uw.panjiajie.cn

TS:   [...a, ...b];
来源：http://na.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ux.panjiajie.cn

Go:   append(a, b...)
来源：http://rr.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://yi.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://sf.nicolike.cn

[D09] 排序（升序）
来源：http://ld.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://ym.yuexingan06.cn

PHP:  sort($arr);
来源：http://jz.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rl.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hy.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zc.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dv.bjjhwx.cn

Ruby: arr.sort
来源：http://qq.hnjuh.cn

C#:   list.Sort();
来源：http://jc.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bz.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://br.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ic.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nm.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mg.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fe.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ny.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xd.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cj.wgjwhj.cn

[D11] 反转数组
来源：http://ep.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://te.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://sh.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://su.shxzukj.cn

TS:   [...arr].reverse();
来源：http://mo.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://wu.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://qf.huixiangedu.cn

Ruby: arr.reverse
来源：http://hy.huanxung.cn

C#:   list.Reverse();
来源：http://px.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://ct.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://am.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vk.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ut.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://um.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bn.colortex.cn

Go:   slices.Index(arr, x)
来源：http://wx.bjjhwx.cn

Ruby: arr.index(x)
来源：http://fq.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://yv.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://ca.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cm.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yi.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://vl.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://ch.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zl.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ns.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ah.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tz.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://rr.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://au.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ax.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://ic.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://ko.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qi.jianghongdianzi.cn

Go:   // 手写循环
来源：http://iq.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mj.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tt.muxihuayi.cn

[D15] 去重
来源：http://sl.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oy.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://xi.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://ie.szsharing.cn

TS:   [...new Set(arr)]
来源：http://uj.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vd.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xj.szxytkj.cn

Ruby: arr.uniq
来源：http://jv.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://fb.asd995.cn

[D16] 求和与平均值
来源：http://ah.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wt.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lv.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jv.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://no.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sl.szsharing.cn

Go:   // 手写循环累加
来源：http://qv.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kg.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://th.newstarts.cn

[D17] 最大值与最小值
来源：http://fg.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://af.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://em.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://im.hnjuh.cn

TS:   Math.max(...arr);
来源：http://xl.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ad.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bp.asd995.cn

Ruby: arr.max;  arr.min
来源：http://gs.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://dy.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://cu.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cd.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://tl.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zq.jianghongdianzi.cn

TS:   nested.flat();
来源：http://td.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vz.wgjwhj.cn

Go:   // 手写双层循环
来源：http://ug.shxzukj.cn

Ruby: nested.flatten
来源：http://wr.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xm.521024.cn

[D19] 按字段分组
来源：http://yz.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zp.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jk.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sx.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fm.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://de.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://jt.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fb.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://as.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://ez.wgjwhj.cn

Py:   Counter(arr)
来源：http://ho.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://oq.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sq.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dg.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ba.9csxet.cn

Go:   // 手写 map[T]int
来源：http://on.shxzukj.cn

Ruby: arr.tally
来源：http://lh.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kx.9csxet.cn

[D21] 判断是否包含某元素
来源：http://wx.gzmigu.cn

Py:   x in arr
来源：http://sx.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://cj.huixiangedu.cn

JS:   arr.includes(x)
来源：http://al.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://lu.newstarts.cn

Java: list.contains(x)
来源：http://np.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://nu.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://kl.shxzskj.cn

C#:   list.Contains(x)
来源：http://wt.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://mh.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ux.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://la.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ql.chemitech.net.cn

TS:   [...arr];
来源：http://mx.9csxet.cn

Java: new ArrayList<>(list);
来源：http://cp.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cl.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://oj.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://ja.nszjky.cn


<!-- 参考信息 -->