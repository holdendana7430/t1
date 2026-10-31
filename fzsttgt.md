代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ga.szxytkj.cn

Go:   return a, b
来源：http://yu.nicolike.cn

Ruby: return a, b
来源：http://bo.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://qo.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://fr.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://rr.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kt.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://fc.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://of.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ra.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yl.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://wh.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fc.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://nq.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ay.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qd.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pu.asd995.cn

TS:   arr.map(String)
来源：http://th.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mg.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uk.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://jv.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://br.gzmigu.cn

[C08] 闭包
来源：http://ir.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kj.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rd.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xc.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lm.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qc.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://er.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rj.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ev.muxihuayi.cn

[C09] 递归
来源：http://vd.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vb.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ft.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zs.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ss.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://as.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pm.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://um.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ir.hnjuh.cn

[C10] 变量作用域
来源：http://na.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zq.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hh.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zo.panjiajie.cn

TS:   同 JS
来源：http://tq.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://ik.bjjhwx.cn

Go:   花括号块级作用域
来源：http://lf.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kp.shtwfgs.cn

C#:   块级作用域
来源：http://xx.wgjwhj.cn

[C11] 模块导入与导出
来源：http://nn.nicolike.cn

Py:   from module import func
来源：http://eb.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zp.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ty.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qm.lnxyls.cn

Java: import java.util.List;
来源：http://iw.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gd.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://qu.521024.cn

C#:   using System.Text;
来源：http://ma.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://ge.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://ex.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://rz.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://it.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://rd.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fx.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://uf.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://lg.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qp.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://ff.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zf.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xh.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://on.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hk.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kw.nszjky.cn

Go:   func add(a, b int) int
来源：http://tq.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xs.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ti.colortex.cn

[C14] 泛型函数
来源：http://ef.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nn.shxzukj.cn

PHP:  // 无泛型
来源：http://eh.bjjhwx.cn

JS:   // 无泛型
来源：http://qp.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oh.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sv.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qg.hahajie.cn

Ruby: # 无泛型
来源：http://xe.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://my.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://np.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pz.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://de.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fm.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fj.521024.cn

Java: // 无解构
来源：http://dx.haigaiapp.cn

Go:   // 无解构
来源：http://bq.muxihuayi.cn

Ruby: a, b = pair
来源：http://nb.asd995.cn

C#:   var (a, b) = pair;
来源：http://jh.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://me.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xh.szsharing.cn

PHP:  // 无重载
来源：http://of.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ul.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ko.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zz.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://mm.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://ui.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iz.nszjky.cn

================================================================================
来源：http://sa.asd995.cn

D. 数组 / 列表 / 集合
来源：http://gl.haigaiapp.cn

================================================================================
来源：http://rn.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://qk.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lk.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://je.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zu.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://th.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ri.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://te.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://hj.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wj.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://fg.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hb.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iw.newstarts.cn

JS:   arr.push(4);
来源：http://wz.chemitech.net.cn

TS:   arr.push(4);
来源：http://rw.colortex.cn

Java: list.add(4);
来源：http://dd.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://ck.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://xj.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://kr.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://kf.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://oa.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cq.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zj.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://qb.szsharing.cn

Java: list.add(0, 0);
来源：http://pz.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lc.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pg.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://jk.yuexingan06.cn

[D04] 删除元素
来源：http://pv.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gn.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aa.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mu.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://ei.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ge.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ny.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jp.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ms.panjiajie.cn

[D05] 访问与修改元素
来源：http://pz.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eo.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xh.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hy.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://id.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://kw.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://yb.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zm.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qe.haigaiapp.cn

[D06] 数组长度
来源：http://vc.muxihuayi.cn

Py:   len(arr)
来源：http://tv.huixinmuqiang.cn

PHP:  count($arr);
来源：http://gq.jctech888.com.cn

JS:   arr.length
来源：http://pv.nszjky.cn

TS:   arr.length
来源：http://mu.szxytkj.cn

Java: list.size();
来源：http://hl.hnjuh.cn

Go:   len(arr)
来源：http://sm.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://dr.szsharing.cn

C#:   list.Count;
来源：http://ox.521024.cn

[D07] 切片 / 取子数组
来源：http://bf.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mf.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xo.colortex.cn

JS:   arr.slice(1, 4);
来源：http://uq.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://qv.shxzskj.cn

Java: list.subList(1, 4);
来源：http://ea.nszjky.cn

Go:   arr[1:4]
来源：http://mh.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://ir.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://zb.asd995.cn

[D08] 合并两个数组
来源：http://cv.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://ga.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://gw.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yj.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://uh.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uu.bookmarksfly.cn

Go:   append(a, b...)
来源：http://bv.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://pj.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://kn.hahajie.cn

[D09] 排序（升序）
来源：http://us.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://oj.hnjuh.cn

PHP:  sort($arr);
来源：http://jd.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sw.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qj.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xo.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ui.jianghongdianzi.cn

Ruby: arr.sort
来源：http://fp.shtwfgs.cn

C#:   list.Sort();
来源：http://au.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mq.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vo.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sd.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nl.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ce.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xj.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ui.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://er.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qk.huanxung.cn

[D11] 反转数组
来源：http://gk.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://is.szsharing.cn

PHP:  array_reverse($arr);
来源：http://sc.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qa.asd995.cn

TS:   [...arr].reverse();
来源：http://hk.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://wq.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://wm.panjiajie.cn

Ruby: arr.reverse
来源：http://wy.yuexingan06.cn

C#:   list.Reverse();
来源：http://fo.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://ou.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://td.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zp.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ej.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ub.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ln.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://ml.huixiangedu.cn

Ruby: arr.index(x)
来源：http://qj.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://lg.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://ls.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xc.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oe.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://tr.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://hf.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gy.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qj.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://id.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cu.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://ri.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xd.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://di.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://fg.521024.cn

TS:   arr.map(x => x * 2)
来源：http://lh.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ie.huixinmuqiang.cn

Go:   // 手写循环
来源：http://qq.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ll.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sz.shxzukj.cn

[D15] 去重
来源：http://ii.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ir.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://te.asd995.cn

JS:   [...new Set(arr)]
来源：http://zv.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://tq.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tq.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ko.shtwfgs.cn

Ruby: arr.uniq
来源：http://km.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://lz.szsharing.cn

[D16] 求和与平均值
来源：http://na.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://he.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ph.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cg.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ch.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wz.haigaiapp.cn

Go:   // 手写循环累加
来源：http://xr.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tn.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://at.szsharing.cn

[D17] 最大值与最小值
来源：http://um.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://rn.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://ol.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sp.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://sg.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ns.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yb.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://dr.colortex.cn

C#:   list.Max();  list.Min()
来源：http://kq.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://eu.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ws.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://rp.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jd.9csxet.cn

TS:   nested.flat();
来源：http://ut.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ih.hnjuh.cn

Go:   // 手写双层循环
来源：http://qn.lnxyls.cn

Ruby: nested.flatten
来源：http://jq.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yh.nicolike.cn

[D19] 按字段分组
来源：http://ig.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ou.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wl.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xm.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zs.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yd.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://oe.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ya.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vr.asd995.cn

[D20] 统计每个元素出现次数
来源：http://rf.szsharing.cn

Py:   Counter(arr)
来源：http://rb.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://ed.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://up.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yj.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sb.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://zl.bookmarksfly.cn

Ruby: arr.tally
来源：http://mp.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xk.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://rk.colortex.cn

Py:   x in arr
来源：http://hc.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://mm.hahajie.cn

JS:   arr.includes(x)
来源：http://nt.newstarts.cn

TS:   arr.includes(x)
来源：http://bq.szsharing.cn

Java: list.contains(x)
来源：http://si.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://rv.szsharing.cn

Ruby: arr.include?(x)
来源：http://fj.hnjuh.cn

C#:   list.Contains(x)
来源：http://im.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://jd.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tj.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yc.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://km.szxytkj.cn

TS:   [...arr];
来源：http://cu.huixinmuqiang.cn


<!-- 参考信息 -->