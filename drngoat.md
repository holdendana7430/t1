代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://im.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://db.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iu.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ni.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jo.nicolike.cn

TS:   arr.map(String)
来源：http://fj.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mk.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://io.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://zp.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ev.bookmarksfly.cn

[C08] 闭包
来源：http://ry.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kk.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gk.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mz.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://th.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jj.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ca.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hb.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qx.szxytkj.cn

[C09] 递归
来源：http://ym.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zm.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cb.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ja.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mm.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://us.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://se.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://es.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://km.shxzskj.cn

[C10] 变量作用域
来源：http://in.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ns.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bt.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://da.bjjhwx.cn

TS:   同 JS
来源：http://eo.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://ew.bjjhwx.cn

Go:   花括号块级作用域
来源：http://gr.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eh.haigaiapp.cn

C#:   块级作用域
来源：http://ny.huanxung.cn

[C11] 模块导入与导出
来源：http://ji.bjjhwx.cn

Py:   from module import func
来源：http://vw.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tk.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pp.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lo.lnxyls.cn

Java: import java.util.List;
来源：http://rj.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lb.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ba.huixinmuqiang.cn

C#:   using System.Text;
来源：http://tm.521024.cn

[C12] 立即执行函数 IIFE
来源：http://nl.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://ey.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://cn.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ri.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://su.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bn.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://hp.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://ur.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://in.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://ii.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xw.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lr.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ge.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jo.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tm.asd995.cn

Go:   func add(a, b int) int
来源：http://rf.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mz.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sf.shtwfgs.cn

[C14] 泛型函数
来源：http://cf.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fn.huanxung.cn

PHP:  // 无泛型
来源：http://ja.asd995.cn

JS:   // 无泛型
来源：http://ra.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ni.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vx.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://is.newstarts.cn

Ruby: # 无泛型
来源：http://bo.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nc.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://lx.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qv.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://we.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nv.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jl.hnjuh.cn

Java: // 无解构
来源：http://ek.szsharing.cn

Go:   // 无解构
来源：http://fp.haigaiapp.cn

Ruby: a, b = pair
来源：http://mn.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://fc.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://bk.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xp.bjjhwx.cn

PHP:  // 无重载
来源：http://xx.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ue.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://id.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://an.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://ho.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://kz.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jf.yuntaijiaju.cn

================================================================================
来源：http://fw.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://yn.gzmigu.cn

================================================================================
来源：http://xa.nicolike.cn

[D01] 创建数组 / 列表
来源：http://pz.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rv.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lu.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fz.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qw.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xw.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://hj.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://wj.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pg.szsharing.cn

[D02] 追加元素到末尾
来源：http://vo.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rg.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sv.haigaiapp.cn

JS:   arr.push(4);
来源：http://no.wgjwhj.cn

TS:   arr.push(4);
来源：http://de.bjjhwx.cn

Java: list.add(4);
来源：http://bm.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://zx.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://fs.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://ag.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://mw.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://zs.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ox.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://al.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://vw.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://zt.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rm.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ug.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://kx.shxzskj.cn

[D04] 删除元素
来源：http://zl.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hc.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dr.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ew.asd995.cn

TS:   arr.splice(0, 1);
来源：http://vc.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://in.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ov.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zr.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bs.asd995.cn

[D05] 访问与修改元素
来源：http://pb.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ru.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xu.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ze.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://zg.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://vy.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ro.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mb.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://an.jianghongdianzi.cn

[D06] 数组长度
来源：http://ar.wgjwhj.cn

Py:   len(arr)
来源：http://af.hahajie.cn

PHP:  count($arr);
来源：http://ye.huixinmuqiang.cn

JS:   arr.length
来源：http://hv.jctech888.com.cn

TS:   arr.length
来源：http://lt.shxzukj.cn

Java: list.size();
来源：http://vl.hahajie.cn

Go:   len(arr)
来源：http://nl.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://ov.shxzukj.cn

C#:   list.Count;
来源：http://dt.521024.cn

[D07] 切片 / 取子数组
来源：http://yp.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gb.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dn.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://gp.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://oj.9csxet.cn

Java: list.subList(1, 4);
来源：http://yr.chemitech.net.cn

Go:   arr[1:4]
来源：http://wr.asd995.cn

Ruby: arr[1, 3]
来源：http://cj.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://wp.szsharing.cn

[D08] 合并两个数组
来源：http://ir.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://ud.colortex.cn

PHP:  array_merge($a, $b);
来源：http://vx.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://el.panjiajie.cn

TS:   [...a, ...b];
来源：http://qn.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sg.nicolike.cn

Go:   append(a, b...)
来源：http://gs.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://ql.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://wu.panjiajie.cn

[D09] 排序（升序）
来源：http://ok.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://lj.bjjhwx.cn

PHP:  sort($arr);
来源：http://rj.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ii.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fg.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pc.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dw.hahajie.cn

Ruby: arr.sort
来源：http://uj.9csxet.cn

C#:   list.Sort();
来源：http://us.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yv.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qf.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bt.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uj.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yg.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vd.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://df.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ye.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yg.huanxung.cn

[D11] 反转数组
来源：http://po.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://og.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://bf.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://id.9csxet.cn

TS:   [...arr].reverse();
来源：http://es.9csxet.cn

Java: Collections.reverse(list);
来源：http://so.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://pk.muxihuayi.cn

Ruby: arr.reverse
来源：http://ai.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://aa.haigaiapp.cn

[D12] 查找元素下标
来源：http://rh.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://qk.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pn.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nd.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wa.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pz.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://ov.gzmigu.cn

Ruby: arr.index(x)
来源：http://lr.huanxung.cn

C#:   list.IndexOf(x);
来源：http://rt.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://pe.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qq.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bu.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://ch.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://dg.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ad.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sd.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kn.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hb.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://dq.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cs.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vv.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://wa.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://bc.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bs.lnxyls.cn

Go:   // 手写循环
来源：http://qo.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nw.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xp.muxihuayi.cn

[D15] 去重
来源：http://jn.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eh.shxzukj.cn

PHP:  array_unique($arr);
来源：http://yi.nicolike.cn

JS:   [...new Set(arr)]
来源：http://ux.hahajie.cn

TS:   [...new Set(arr)]
来源：http://ua.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nv.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ig.yuexingan06.cn

Ruby: arr.uniq
来源：http://rd.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://gr.hnjuh.cn

[D16] 求和与平均值
来源：http://hv.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nr.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mm.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wu.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jr.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ns.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://yq.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xw.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://fj.jctech888.com.cn

[D17] 最大值与最小值
来源：http://ef.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://au.521024.cn

PHP:  max($arr);  min($arr);
来源：http://ca.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hr.hnjuh.cn

TS:   Math.max(...arr);
来源：http://sb.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lq.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bj.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://si.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://pf.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://ie.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xw.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://nj.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vv.haigaiapp.cn

TS:   nested.flat();
来源：http://js.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mw.haigaiapp.cn

Go:   // 手写双层循环
来源：http://ew.shxzskj.cn

Ruby: nested.flatten
来源：http://ua.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dw.9csxet.cn

[D19] 按字段分组
来源：http://qr.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xf.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://um.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jt.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ws.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cy.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://kl.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cw.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lw.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://tq.muxihuayi.cn

Py:   Counter(arr)
来源：http://yj.newstarts.cn

PHP:  array_count_values($arr);
来源：http://tu.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ds.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ji.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xe.nicolike.cn

Go:   // 手写 map[T]int
来源：http://qp.muxihuayi.cn

Ruby: arr.tally
来源：http://yy.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bl.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://ik.colortex.cn

Py:   x in arr
来源：http://le.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://nu.9csxet.cn

JS:   arr.includes(x)
来源：http://tr.szsharing.cn

TS:   arr.includes(x)
来源：http://hi.huanxung.cn

Java: list.contains(x)
来源：http://oe.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://mc.nicolike.cn

Ruby: arr.include?(x)
来源：http://vo.hnjuh.cn

C#:   list.Contains(x)
来源：http://xf.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://ed.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cl.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qw.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jy.shtwfgs.cn

TS:   [...arr];
来源：http://fn.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://wm.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://eq.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://ol.haigaiapp.cn

C#:   new List<int>(list);
来源：http://ls.nszjky.cn

[D23] reduce 累积计算
来源：http://mb.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qf.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hd.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iu.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gy.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hg.yuntaijiaju.cn

Go:   // 手写循环
来源：http://re.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fl.szsharing.cn


<!-- 参考信息 -->