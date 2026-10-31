代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://fl.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://mq.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nu.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hg.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sr.chemitech.net.cn

TS:   arr.map(String)
来源：http://do.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hr.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hp.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://dg.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ty.nicolike.cn

[C08] 闭包
来源：http://bb.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sw.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aw.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hv.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fu.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tt.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yh.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qq.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ll.newstarts.cn

[C09] 递归
来源：http://yo.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mu.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vp.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://of.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vx.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yf.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pp.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sb.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lv.hnjuh.cn

[C10] 变量作用域
来源：http://om.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fm.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gv.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xy.muxihuayi.cn

TS:   同 JS
来源：http://mr.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://wd.gzmigu.cn

Go:   花括号块级作用域
来源：http://mk.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dn.chemitech.net.cn

C#:   块级作用域
来源：http://cn.9csxet.cn

[C11] 模块导入与导出
来源：http://hu.bookmarksfly.cn

Py:   from module import func
来源：http://ht.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vx.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lc.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xx.asd995.cn

Java: import java.util.List;
来源：http://hg.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://an.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://ry.jctech888.com.cn

C#:   using System.Text;
来源：http://nt.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://tr.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://ed.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://fa.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ks.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://dg.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wu.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://em.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://zp.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wl.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://ex.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ny.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bq.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rj.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://td.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oe.nicolike.cn

Go:   func add(a, b int) int
来源：http://ia.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fh.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sf.bookmarksfly.cn

[C14] 泛型函数
来源：http://rs.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qj.521024.cn

PHP:  // 无泛型
来源：http://tm.shxzskj.cn

JS:   // 无泛型
来源：http://zc.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gy.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hc.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ua.bookmarksfly.cn

Ruby: # 无泛型
来源：http://pt.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pg.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://lu.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fo.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://no.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kq.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://of.bookmarksfly.cn

Java: // 无解构
来源：http://pl.chemitech.net.cn

Go:   // 无解构
来源：http://ra.jctech888.com.cn

Ruby: a, b = pair
来源：http://be.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://sg.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://xn.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jj.yuexingan06.cn

PHP:  // 无重载
来源：http://kg.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mf.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://it.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://aa.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://ua.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://bt.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rl.jianghongdianzi.cn

================================================================================
来源：http://ts.521024.cn

D. 数组 / 列表 / 集合
来源：http://cl.huanxung.cn

================================================================================
来源：http://iw.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://mv.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tx.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ll.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wt.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eb.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zq.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://dn.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://qj.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dc.colortex.cn

[D02] 追加元素到末尾
来源：http://sk.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ot.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fq.bookmarksfly.cn

JS:   arr.push(4);
来源：http://yv.hnjuh.cn

TS:   arr.push(4);
来源：http://kx.nicolike.cn

Java: list.add(4);
来源：http://dt.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://af.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://ny.shxzukj.cn

C#:   list.Add(4);
来源：http://os.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://ep.colortex.cn

Py:   arr.insert(0, 0)
来源：http://uz.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dz.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dp.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://es.nszjky.cn

Java: list.add(0, 0);
来源：http://cd.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rr.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lh.521024.cn

C#:   list.Insert(0, 0);
来源：http://bm.jctech888.com.cn

[D04] 删除元素
来源：http://hv.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fe.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ee.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jf.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://ar.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://at.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fn.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wm.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cn.shxzukj.cn

[D05] 访问与修改元素
来源：http://vj.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iy.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hd.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uv.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://vj.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://gm.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://uo.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hv.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ac.yuexingan06.cn

[D06] 数组长度
来源：http://id.jianghongdianzi.cn

Py:   len(arr)
来源：http://wd.szxytkj.cn

PHP:  count($arr);
来源：http://bt.yuntaijiaju.cn

JS:   arr.length
来源：http://oo.bjjhwx.cn

TS:   arr.length
来源：http://eo.hnjuh.cn

Java: list.size();
来源：http://gr.huixiangedu.cn

Go:   len(arr)
来源：http://pb.9csxet.cn

Ruby: arr.length; arr.size
来源：http://es.yuexingan06.cn

C#:   list.Count;
来源：http://ya.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://zj.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kd.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tt.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://nf.colortex.cn

TS:   arr.slice(1, 4);
来源：http://vi.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://tk.shxzukj.cn

Go:   arr[1:4]
来源：http://zv.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://vs.521024.cn

C#:   list.GetRange(1, 3);
来源：http://hh.szxytkj.cn

[D08] 合并两个数组
来源：http://mn.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://jv.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://aa.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mt.haigaiapp.cn

TS:   [...a, ...b];
来源：http://su.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bw.shxzskj.cn

Go:   append(a, b...)
来源：http://yk.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://sb.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://tj.shxzukj.cn

[D09] 排序（升序）
来源：http://jf.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://sl.bjjhwx.cn

PHP:  sort($arr);
来源：http://ob.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dl.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wk.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lz.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qc.bookmarksfly.cn

Ruby: arr.sort
来源：http://up.521024.cn

C#:   list.Sort();
来源：http://of.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lv.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nv.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yn.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://en.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bf.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fk.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bp.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ag.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://es.nszjky.cn

[D11] 反转数组
来源：http://fm.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wg.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://tu.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yt.szxytkj.cn

TS:   [...arr].reverse();
来源：http://ky.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://yz.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://uy.bjjhwx.cn

Ruby: arr.reverse
来源：http://wr.muxihuayi.cn

C#:   list.Reverse();
来源：http://uq.asd995.cn

[D12] 查找元素下标
来源：http://jy.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://af.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://to.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ww.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vu.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xt.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://ha.haigaiapp.cn

Ruby: arr.index(x)
来源：http://xf.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://fy.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://rj.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ce.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vv.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://wg.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://hc.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ec.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iz.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uv.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nk.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://yf.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yh.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uk.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://oo.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://zj.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ag.hahajie.cn

Go:   // 手写循环
来源：http://ib.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ej.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ak.chemitech.net.cn

[D15] 去重
来源：http://iw.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eb.szxytkj.cn

PHP:  array_unique($arr);
来源：http://db.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://lc.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://jr.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vl.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://un.bookmarksfly.cn

Ruby: arr.uniq
来源：http://fd.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://fh.newstarts.cn

[D16] 求和与平均值
来源：http://nu.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ne.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qv.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wd.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vb.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rh.yuexingan06.cn

Go:   // 手写循环累加
来源：http://bj.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tr.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://mg.asd995.cn

[D17] 最大值与最小值
来源：http://jo.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://hn.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://mn.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zm.521024.cn

TS:   Math.max(...arr);
来源：http://hm.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tr.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dw.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://hn.asd995.cn

C#:   list.Max();  list.Min()
来源：http://qe.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://th.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ys.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://by.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jn.szsharing.cn

TS:   nested.flat();
来源：http://fq.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qw.bjjhwx.cn

Go:   // 手写双层循环
来源：http://fw.lnxyls.cn

Ruby: nested.flatten
来源：http://yr.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yi.huixinmuqiang.cn

[D19] 按字段分组
来源：http://ye.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oi.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iy.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ar.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://am.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zl.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://lz.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://in.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sj.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://vd.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://rw.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://vr.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iq.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uq.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://od.colortex.cn

Go:   // 手写 map[T]int
来源：http://wk.asd995.cn

Ruby: arr.tally
来源：http://ms.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qj.nicolike.cn

[D21] 判断是否包含某元素
来源：http://lp.yuntaijiaju.cn

Py:   x in arr
来源：http://fz.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://tc.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://de.szsharing.cn

TS:   arr.includes(x)
来源：http://lp.wgjwhj.cn

Java: list.contains(x)
来源：http://ax.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://bw.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://oq.huanxung.cn

C#:   list.Contains(x)
来源：http://wt.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://uk.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mi.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lt.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lm.newstarts.cn

TS:   [...arr];
来源：http://fl.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://xb.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://of.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://it.shxzskj.cn

C#:   new List<int>(list);
来源：http://ou.muxihuayi.cn

[D23] reduce 累积计算
来源：http://gl.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qq.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ll.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xp.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ef.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zo.wgjwhj.cn

Go:   // 手写循环
来源：http://qt.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sg.newstarts.cn


<!-- 参考信息 -->