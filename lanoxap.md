代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nk.yuexingan06.cn

Go:   return a, b
来源：http://zx.gzmigu.cn

Ruby: return a, b
来源：http://ls.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://pu.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://db.9csxet.cn

Py:   square = lambda x: x * x
来源：http://qm.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cy.nszjky.cn

JS:   const square = x => x * x;
来源：http://uf.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://mn.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ah.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ke.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://pl.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hp.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://tf.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kt.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vy.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fj.shtwfgs.cn

TS:   arr.map(String)
来源：http://nl.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nh.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dw.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://zq.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ww.huanxung.cn

[C08] 闭包
来源：http://cy.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xh.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hk.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ni.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jm.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vu.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dk.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yr.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qk.yuntaijiaju.cn

[C09] 递归
来源：http://co.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gt.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fj.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gd.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://je.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zz.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sh.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kw.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uu.panjiajie.cn

[C10] 变量作用域
来源：http://zn.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ef.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wh.hahajie.cn

TS:   同 JS
来源：http://iu.hnjuh.cn

Java: 方法内为块级作用域
来源：http://fy.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://fl.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fc.bjjhwx.cn

C#:   块级作用域
来源：http://mn.lnxyls.cn

[C11] 模块导入与导出
来源：http://cv.newstarts.cn

Py:   from module import func
来源：http://ji.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yn.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kz.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yi.newstarts.cn

Java: import java.util.List;
来源：http://po.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yg.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://hy.huixinmuqiang.cn

C#:   using System.Text;
来源：http://xi.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://rt.asd995.cn

Py:   (lambda: print("run"))()
来源：http://bq.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://hn.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://sm.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ri.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lu.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://gp.521024.cn

Ruby: -> { puts "run" }.call
来源：http://xm.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jp.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://ww.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qb.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lp.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hi.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tp.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sq.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://qw.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lf.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fc.huixiangedu.cn

[C14] 泛型函数
来源：http://rn.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oj.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://ea.jianghongdianzi.cn

JS:   // 无泛型
来源：http://hg.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vn.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://la.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://as.szsharing.cn

Ruby: # 无泛型
来源：http://dd.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ap.9csxet.cn

[C15] 解构 / 展开参数
来源：http://ij.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wl.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://dp.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://to.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wk.jctech888.com.cn

Java: // 无解构
来源：http://ow.huixiangedu.cn

Go:   // 无解构
来源：http://qy.nszjky.cn

Ruby: a, b = pair
来源：http://qp.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://tz.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://tl.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nd.huixiangedu.cn

PHP:  // 无重载
来源：http://ib.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ds.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://wh.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ht.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://jy.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://iy.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xi.muxihuayi.cn

================================================================================
来源：http://nt.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ro.lnxyls.cn

================================================================================
来源：http://zf.huanxung.cn

[D01] 创建数组 / 列表
来源：http://an.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lk.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dw.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gi.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dg.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://do.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ye.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://ox.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hp.9csxet.cn

[D02] 追加元素到末尾
来源：http://am.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bg.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ha.hnjuh.cn

JS:   arr.push(4);
来源：http://ax.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://qg.huanxung.cn

Java: list.add(4);
来源：http://hu.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://xl.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://fj.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://eq.nszjky.cn

[D03] 在指定位置插入元素
来源：http://wr.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://vw.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wk.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ul.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://uv.szsharing.cn

Java: list.add(0, 0);
来源：http://mo.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yq.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ja.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://bo.haigaiapp.cn

[D04] 删除元素
来源：http://fo.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qt.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://um.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ei.asd995.cn

TS:   arr.splice(0, 1);
来源：http://jo.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://na.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ab.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kb.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lv.lnxyls.cn

[D05] 访问与修改元素
来源：http://el.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vu.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qp.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sh.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://tc.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://uw.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://xt.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mr.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gm.shtwfgs.cn

[D06] 数组长度
来源：http://he.hnjuh.cn

Py:   len(arr)
来源：http://fs.shxzskj.cn

PHP:  count($arr);
来源：http://at.shtwfgs.cn

JS:   arr.length
来源：http://aw.9csxet.cn

TS:   arr.length
来源：http://ot.asd995.cn

Java: list.size();
来源：http://rk.9csxet.cn

Go:   len(arr)
来源：http://fy.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://al.huanxung.cn

C#:   list.Count;
来源：http://oi.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://fa.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mg.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bm.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://ii.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://ek.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://lp.huixiangedu.cn

Go:   arr[1:4]
来源：http://lk.panjiajie.cn

Ruby: arr[1, 3]
来源：http://oc.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://ms.nszjky.cn

[D08] 合并两个数组
来源：http://mn.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://ng.colortex.cn

PHP:  array_merge($a, $b);
来源：http://dp.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dn.huanxung.cn

TS:   [...a, ...b];
来源：http://ce.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xi.asd995.cn

Go:   append(a, b...)
来源：http://lg.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://ty.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://li.huanxung.cn

[D09] 排序（升序）
来源：http://kq.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://lt.huanxung.cn

PHP:  sort($arr);
来源：http://th.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ck.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jl.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gr.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qq.hnjuh.cn

Ruby: arr.sort
来源：http://gl.shxzukj.cn

C#:   list.Sort();
来源：http://bp.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ey.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vs.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cx.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bk.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yo.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wu.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sm.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ul.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fn.9csxet.cn

[D11] 反转数组
来源：http://iu.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ag.huanxung.cn

PHP:  array_reverse($arr);
来源：http://im.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ru.9csxet.cn

TS:   [...arr].reverse();
来源：http://lo.shxzskj.cn

Java: Collections.reverse(list);
来源：http://ie.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://pm.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://xn.hahajie.cn

C#:   list.Reverse();
来源：http://xq.szsharing.cn

[D12] 查找元素下标
来源：http://ww.521024.cn

Py:   arr.index(x);  x in arr
来源：http://ng.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vq.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sk.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aj.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bh.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://se.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://ns.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://xa.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://yj.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ek.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://co.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://pa.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://ks.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ns.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zk.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mz.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uf.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://wv.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dz.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yz.521024.cn

JS:   arr.map(x => x * 2)
来源：http://cy.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://eb.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ux.colortex.cn

Go:   // 手写循环
来源：http://wz.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hq.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pe.szxytkj.cn

[D15] 去重
来源：http://by.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ui.asd995.cn

PHP:  array_unique($arr);
来源：http://em.newstarts.cn

JS:   [...new Set(arr)]
来源：http://sq.colortex.cn

TS:   [...new Set(arr)]
来源：http://mu.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cl.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qo.9csxet.cn

Ruby: arr.uniq
来源：http://vv.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://no.huixiangedu.cn

[D16] 求和与平均值
来源：http://zq.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ne.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hn.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qz.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qq.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ii.colortex.cn

Go:   // 手写循环累加
来源：http://zv.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mt.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://bz.huanxung.cn

[D17] 最大值与最小值
来源：http://fo.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://jy.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://su.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zq.szsharing.cn

TS:   Math.max(...arr);
来源：http://ot.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nl.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cw.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://ge.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://wy.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://rz.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tz.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://ty.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nv.bjjhwx.cn

TS:   nested.flat();
来源：http://xx.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://it.shxzskj.cn

Go:   // 手写双层循环
来源：http://ry.huanxung.cn

Ruby: nested.flatten
来源：http://dc.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://be.jianghongdianzi.cn

[D19] 按字段分组
来源：http://et.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ss.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eh.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qf.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wf.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hy.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://tt.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aj.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rt.521024.cn

[D20] 统计每个元素出现次数
来源：http://es.muxihuayi.cn

Py:   Counter(arr)
来源：http://kl.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://ei.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://og.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pc.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oq.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://qu.szxytkj.cn

Ruby: arr.tally
来源：http://iy.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bs.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://qc.haigaiapp.cn

Py:   x in arr
来源：http://eg.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://dk.wgjwhj.cn

JS:   arr.includes(x)
来源：http://nn.bjjhwx.cn

TS:   arr.includes(x)
来源：http://qq.yuntaijiaju.cn

Java: list.contains(x)
来源：http://oh.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://fu.9csxet.cn

Ruby: arr.include?(x)
来源：http://mm.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://ox.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://rk.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sh.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ma.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ha.chemitech.net.cn

TS:   [...arr];
来源：http://np.newstarts.cn


<!-- 参考信息 -->