代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://hz.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://su.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://ve.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fz.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://my.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dp.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vy.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://fy.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://qb.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://cu.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://gk.bookmarksfly.cn

[C05] 返回多个值
来源：http://ar.panjiajie.cn

Py:   return a, b
来源：http://bu.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://ch.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mo.gzmigu.cn

TS:   return { a, b };
来源：http://kf.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sk.shxzskj.cn

Go:   return a, b
来源：http://sk.huanxung.cn

Ruby: return a, b
来源：http://yv.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://ym.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://sm.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://uf.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xc.colortex.cn

JS:   const square = x => x * x;
来源：http://wn.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://no.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zl.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cz.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://yb.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ur.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://ga.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jm.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cz.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ia.nszjky.cn

TS:   arr.map(String)
来源：http://cz.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yi.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ca.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://bd.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sc.hnjuh.cn

[C08] 闭包
来源：http://xq.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cm.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://al.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://go.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qy.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bq.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fg.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ub.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dc.bjjhwx.cn

[C09] 递归
来源：http://ch.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ko.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jp.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pu.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wg.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uo.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ut.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gb.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jp.newstarts.cn

[C10] 变量作用域
来源：http://vb.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xb.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bz.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yl.nszjky.cn

TS:   同 JS
来源：http://lf.newstarts.cn

Java: 方法内为块级作用域
来源：http://vr.haigaiapp.cn

Go:   花括号块级作用域
来源：http://cd.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ud.nszjky.cn

C#:   块级作用域
来源：http://hj.nicolike.cn

[C11] 模块导入与导出
来源：http://cj.bookmarksfly.cn

Py:   from module import func
来源：http://qz.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iv.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ma.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mg.szsharing.cn

Java: import java.util.List;
来源：http://ra.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xg.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://kj.wgjwhj.cn

C#:   using System.Text;
来源：http://gi.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://kd.colortex.cn

Py:   (lambda: print("run"))()
来源：http://zn.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://kj.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://ic.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://ov.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ti.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ii.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://ez.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ks.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://ok.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pg.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cy.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vc.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cv.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yj.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://sq.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fz.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lm.panjiajie.cn

[C14] 泛型函数
来源：http://oj.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uc.jctech888.com.cn

PHP:  // 无泛型
来源：http://hy.shxzukj.cn

JS:   // 无泛型
来源：http://vs.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cn.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://di.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lq.bjjhwx.cn

Ruby: # 无泛型
来源：http://je.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bj.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://fr.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cf.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://ui.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fs.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cn.shtwfgs.cn

Java: // 无解构
来源：http://nl.shtwfgs.cn

Go:   // 无解构
来源：http://um.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://ek.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://me.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://gd.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uf.panjiajie.cn

PHP:  // 无重载
来源：http://md.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fq.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://zz.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mk.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://na.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://ag.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dr.panjiajie.cn

================================================================================
来源：http://hm.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://yy.bookmarksfly.cn

================================================================================
来源：http://ue.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://ol.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ly.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tr.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ja.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ej.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dn.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://hu.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://jr.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wd.szsharing.cn

[D02] 追加元素到末尾
来源：http://wo.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gn.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ze.shxzukj.cn

JS:   arr.push(4);
来源：http://su.nicolike.cn

TS:   arr.push(4);
来源：http://hw.jctech888.com.cn

Java: list.add(4);
来源：http://al.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://wm.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://wr.hahajie.cn

C#:   list.Add(4);
来源：http://gf.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://ms.colortex.cn

Py:   arr.insert(0, 0)
来源：http://uc.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bq.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bu.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://ei.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://vf.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ur.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ma.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://zi.shtwfgs.cn

[D04] 删除元素
来源：http://sh.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fy.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://px.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fw.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://kc.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tr.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cz.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bf.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qd.shxzukj.cn

[D05] 访问与修改元素
来源：http://co.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://md.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hr.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://we.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://bi.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://bd.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ri.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eu.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ry.shtwfgs.cn

[D06] 数组长度
来源：http://fw.jianghongdianzi.cn

Py:   len(arr)
来源：http://ie.huanxung.cn

PHP:  count($arr);
来源：http://ph.wgjwhj.cn

JS:   arr.length
来源：http://de.szxytkj.cn

TS:   arr.length
来源：http://up.colortex.cn

Java: list.size();
来源：http://fe.huanxung.cn

Go:   len(arr)
来源：http://bg.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://hq.yuntaijiaju.cn

C#:   list.Count;
来源：http://ec.szsharing.cn

[D07] 切片 / 取子数组
来源：http://kc.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nh.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ir.colortex.cn

JS:   arr.slice(1, 4);
来源：http://vk.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://lj.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://dz.jctech888.com.cn

Go:   arr[1:4]
来源：http://ak.newstarts.cn

Ruby: arr[1, 3]
来源：http://cx.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://da.colortex.cn

[D08] 合并两个数组
来源：http://cl.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://hq.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://sa.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bq.lnxyls.cn

TS:   [...a, ...b];
来源：http://bh.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://po.nszjky.cn

Go:   append(a, b...)
来源：http://ie.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://em.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://rd.nszjky.cn

[D09] 排序（升序）
来源：http://ak.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ux.szsharing.cn

PHP:  sort($arr);
来源：http://dq.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nw.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gz.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qv.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ko.wgjwhj.cn

Ruby: arr.sort
来源：http://sv.huixiangedu.cn

C#:   list.Sort();
来源：http://km.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fc.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fn.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fe.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ft.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mt.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qo.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pv.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jk.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uw.9csxet.cn

[D11] 反转数组
来源：http://sf.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cf.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://oo.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ad.521024.cn

TS:   [...arr].reverse();
来源：http://ja.nicolike.cn

Java: Collections.reverse(list);
来源：http://uo.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://pq.huanxung.cn

Ruby: arr.reverse
来源：http://jk.shxzskj.cn

C#:   list.Reverse();
来源：http://cw.asd995.cn

[D12] 查找元素下标
来源：http://mc.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://dg.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oz.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zv.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://km.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pc.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://ay.shxzukj.cn

Ruby: arr.index(x)
来源：http://yv.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://zj.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://jg.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://he.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yx.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://cb.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://qi.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mf.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mp.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ut.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://le.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://yw.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hc.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zl.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://pt.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://ds.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zk.bookmarksfly.cn

Go:   // 手写循环
来源：http://jl.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dz.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sy.yuntaijiaju.cn

[D15] 去重
来源：http://xo.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ca.9csxet.cn

PHP:  array_unique($arr);
来源：http://zr.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://ta.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://se.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sc.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mi.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://wx.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://wl.hnjuh.cn

[D16] 求和与平均值
来源：http://ed.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qv.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iw.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ax.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ve.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qz.521024.cn

Go:   // 手写循环累加
来源：http://pp.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cl.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://hx.521024.cn

[D17] 最大值与最小值
来源：http://xa.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://bc.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://tx.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rd.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://zg.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ic.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wi.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://hv.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://no.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://fg.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zd.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://nz.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nx.huixiangedu.cn

TS:   nested.flat();
来源：http://hl.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zf.521024.cn

Go:   // 手写双层循环
来源：http://ts.shxzskj.cn

Ruby: nested.flatten
来源：http://po.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iu.bjjhwx.cn

[D19] 按字段分组
来源：http://fd.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ya.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rf.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://km.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ll.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oi.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://ey.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xw.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gk.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://jh.yuexingan06.cn

Py:   Counter(arr)
来源：http://bf.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://yk.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oc.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yi.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qi.nicolike.cn

Go:   // 手写 map[T]int
来源：http://os.bookmarksfly.cn


<!-- 参考信息 -->