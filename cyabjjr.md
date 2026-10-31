代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://oe.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://yi.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://ef.9csxet.cn

[C05] 返回多个值
来源：http://td.huixiangedu.cn

Py:   return a, b
来源：http://cs.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://gh.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://up.jctech888.com.cn

TS:   return { a, b };
来源：http://kw.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mc.nicolike.cn

Go:   return a, b
来源：http://yd.haigaiapp.cn

Ruby: return a, b
来源：http://fv.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ff.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://ct.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://np.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xp.nszjky.cn

JS:   const square = x => x * x;
来源：http://op.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://le.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kf.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://af.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://rx.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cd.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://vp.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lv.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tb.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lq.hahajie.cn

TS:   arr.map(String)
来源：http://hl.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jn.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xi.521024.cn

Ruby: arr.map(&:upcase)
来源：http://va.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nl.huixiangedu.cn

[C08] 闭包
来源：http://ic.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ts.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ag.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qz.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yg.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://go.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gm.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ex.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ru.9csxet.cn

[C09] 递归
来源：http://oz.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fp.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tu.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pm.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://un.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wn.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://af.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rt.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kz.shxzskj.cn

[C10] 变量作用域
来源：http://qz.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fv.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fp.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iy.jianghongdianzi.cn

TS:   同 JS
来源：http://hh.lnxyls.cn

Java: 方法内为块级作用域
来源：http://jq.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://ki.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mf.wgjwhj.cn

C#:   块级作用域
来源：http://bj.gzmigu.cn

[C11] 模块导入与导出
来源：http://ad.hnjuh.cn

Py:   from module import func
来源：http://yl.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ih.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rq.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jw.yuexingan06.cn

Java: import java.util.List;
来源：http://nb.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yj.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://jq.huanxung.cn

C#:   using System.Text;
来源：http://kr.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://po.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://mq.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://vz.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://yt.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://za.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gd.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://yt.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://ir.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yi.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://ze.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bt.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xf.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nf.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vr.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cq.521024.cn

Go:   func add(a, b int) int
来源：http://ij.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yn.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bi.muxihuayi.cn

[C14] 泛型函数
来源：http://bj.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jg.colortex.cn

PHP:  // 无泛型
来源：http://yi.nicolike.cn

JS:   // 无泛型
来源：http://ts.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jt.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vt.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dq.chemitech.net.cn

Ruby: # 无泛型
来源：http://fn.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ye.huanxung.cn

[C15] 解构 / 展开参数
来源：http://lc.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jp.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://is.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ww.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tl.bookmarksfly.cn

Java: // 无解构
来源：http://sd.wgjwhj.cn

Go:   // 无解构
来源：http://jb.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://np.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://ae.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://vr.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rs.hahajie.cn

PHP:  // 无重载
来源：http://fi.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yk.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://jq.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ih.521024.cn

Go:   // 无重载：用不同函数名
来源：http://ty.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://du.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ci.huanxung.cn

================================================================================
来源：http://qm.521024.cn

D. 数组 / 列表 / 集合
来源：http://dg.haigaiapp.cn

================================================================================
来源：http://rj.szsharing.cn

[D01] 创建数组 / 列表
来源：http://tv.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cn.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jv.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rp.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vu.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tv.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://do.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://vj.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qo.hnjuh.cn

[D02] 追加元素到末尾
来源：http://rn.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://so.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cu.nszjky.cn

JS:   arr.push(4);
来源：http://ug.szxytkj.cn

TS:   arr.push(4);
来源：http://wj.huanxung.cn

Java: list.add(4);
来源：http://qv.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://sn.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://qc.jctech888.com.cn

C#:   list.Add(4);
来源：http://xy.nicolike.cn

[D03] 在指定位置插入元素
来源：http://lx.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://wc.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mi.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ba.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ij.521024.cn

Java: list.add(0, 0);
来源：http://pj.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pi.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ch.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://nq.szxytkj.cn

[D04] 删除元素
来源：http://jk.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jw.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xl.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xk.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://tn.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ct.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://va.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zr.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iq.wgjwhj.cn

[D05] 访问与修改元素
来源：http://mu.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qk.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xk.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fc.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://uj.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://cr.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://lf.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ta.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ro.muxihuayi.cn

[D06] 数组长度
来源：http://uc.shxzskj.cn

Py:   len(arr)
来源：http://yv.shxzskj.cn

PHP:  count($arr);
来源：http://ew.yuexingan06.cn

JS:   arr.length
来源：http://gx.chemitech.net.cn

TS:   arr.length
来源：http://lm.shxzukj.cn

Java: list.size();
来源：http://fd.szsharing.cn

Go:   len(arr)
来源：http://us.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://dx.yuntaijiaju.cn

C#:   list.Count;
来源：http://ky.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://an.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hr.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://de.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://fj.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://sb.panjiajie.cn

Java: list.subList(1, 4);
来源：http://hq.wgjwhj.cn

Go:   arr[1:4]
来源：http://vq.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://uw.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://bf.9csxet.cn

[D08] 合并两个数组
来源：http://al.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://io.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://sr.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ei.panjiajie.cn

TS:   [...a, ...b];
来源：http://uw.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sr.shtwfgs.cn

Go:   append(a, b...)
来源：http://mo.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://yd.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://wi.gzmigu.cn

[D09] 排序（升序）
来源：http://kv.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://zw.shxzukj.cn

PHP:  sort($arr);
来源：http://fz.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fn.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tm.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://je.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zp.bookmarksfly.cn

Ruby: arr.sort
来源：http://pi.bookmarksfly.cn

C#:   list.Sort();
来源：http://iw.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qv.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ae.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wi.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gt.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mf.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xe.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iv.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jj.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ua.muxihuayi.cn

[D11] 反转数组
来源：http://ga.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://no.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://oh.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qe.9csxet.cn

TS:   [...arr].reverse();
来源：http://th.gzmigu.cn

Java: Collections.reverse(list);
来源：http://qc.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://za.colortex.cn

Ruby: arr.reverse
来源：http://ov.bookmarksfly.cn

C#:   list.Reverse();
来源：http://rf.newstarts.cn

[D12] 查找元素下标
来源：http://ls.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://jw.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gn.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ot.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pl.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qf.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://mf.szsharing.cn

Ruby: arr.index(x)
来源：http://ld.huanxung.cn

C#:   list.IndexOf(x);
来源：http://yj.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ht.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://od.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vd.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://tb.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://az.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qk.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pm.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xj.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fl.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://tg.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mb.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ye.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://wi.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://fr.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rm.wgjwhj.cn

Go:   // 手写循环
来源：http://of.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ba.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zs.lnxyls.cn

[D15] 去重
来源：http://nk.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wf.lnxyls.cn

PHP:  array_unique($arr);
来源：http://ha.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://bk.nicolike.cn

TS:   [...new Set(arr)]
来源：http://pi.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hm.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ph.9csxet.cn

Ruby: arr.uniq
来源：http://of.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://ml.hahajie.cn

[D16] 求和与平均值
来源：http://rq.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yw.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ly.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sz.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wv.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pv.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://bz.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pe.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://sw.colortex.cn

[D17] 最大值与最小值
来源：http://tb.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://cr.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://ll.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rb.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://fo.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oq.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ca.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://kn.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://jq.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://vv.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oo.asd995.cn

PHP:  array_merge(...$nested);
来源：http://vp.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jt.lnxyls.cn

TS:   nested.flat();
来源：http://or.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zx.hnjuh.cn

Go:   // 手写双层循环
来源：http://am.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://db.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ul.szxytkj.cn

[D19] 按字段分组
来源：http://ps.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nn.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ad.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://or.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hi.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cu.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://ax.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rk.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zw.asd995.cn

[D20] 统计每个元素出现次数
来源：http://mz.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://eg.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://zr.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nv.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tb.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vz.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://re.bjjhwx.cn

Ruby: arr.tally
来源：http://ff.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cx.newstarts.cn

[D21] 判断是否包含某元素
来源：http://ac.bookmarksfly.cn

Py:   x in arr
来源：http://bz.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://gh.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://dl.chemitech.net.cn

TS:   arr.includes(x)
来源：http://aa.yuntaijiaju.cn

Java: list.contains(x)
来源：http://kv.jianghongdianzi.cn


<!-- 参考信息 -->