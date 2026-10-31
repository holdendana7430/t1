代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://an.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://np.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yy.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yp.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mu.521024.cn

TS:   arr.map(String)
来源：http://bb.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gz.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mh.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://wy.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tk.huanxung.cn

[C08] 闭包
来源：http://tw.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://le.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mi.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lc.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qi.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xv.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vl.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bs.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jx.shxzukj.cn

[C09] 递归
来源：http://rn.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ep.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qm.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xi.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pf.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eh.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ra.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ya.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uf.521024.cn

[C10] 变量作用域
来源：http://pp.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://so.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pr.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sb.lnxyls.cn

TS:   同 JS
来源：http://xt.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://aw.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://op.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vm.bjjhwx.cn

C#:   块级作用域
来源：http://xd.szxytkj.cn

[C11] 模块导入与导出
来源：http://gg.yuntaijiaju.cn

Py:   from module import func
来源：http://ux.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ul.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sg.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bi.lnxyls.cn

Java: import java.util.List;
来源：http://hh.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fx.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://jp.hnjuh.cn

C#:   using System.Text;
来源：http://zo.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://hq.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://sd.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://rj.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://vj.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://rr.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ij.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://gf.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://mh.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ch.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://re.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eq.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kt.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bk.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://up.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ru.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://jl.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://li.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://os.colortex.cn

[C14] 泛型函数
来源：http://bg.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sd.chemitech.net.cn

PHP:  // 无泛型
来源：http://ky.bjjhwx.cn

JS:   // 无泛型
来源：http://ub.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hk.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xy.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xf.shxzskj.cn

Ruby: # 无泛型
来源：http://ao.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fl.hahajie.cn

[C15] 解构 / 展开参数
来源：http://jl.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fu.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://fa.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gn.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ty.lnxyls.cn

Java: // 无解构
来源：http://dy.colortex.cn

Go:   // 无解构
来源：http://yy.chemitech.net.cn

Ruby: a, b = pair
来源：http://tl.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://ue.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://az.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zn.jianghongdianzi.cn

PHP:  // 无重载
来源：http://mm.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://po.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://dw.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qa.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://kk.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://pt.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xl.9csxet.cn

================================================================================
来源：http://qh.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://mi.bjjhwx.cn

================================================================================
来源：http://yo.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://hy.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lz.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ne.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xt.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tb.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ie.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://he.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://fi.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://co.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://dx.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qm.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ng.hnjuh.cn

JS:   arr.push(4);
来源：http://fb.shtwfgs.cn

TS:   arr.push(4);
来源：http://yg.yuexingan06.cn

Java: list.add(4);
来源：http://qc.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://ba.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://cl.szsharing.cn

C#:   list.Add(4);
来源：http://rq.szsharing.cn

[D03] 在指定位置插入元素
来源：http://fc.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://hg.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ho.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jb.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://gh.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://lv.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dt.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xt.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://mv.hahajie.cn

[D04] 删除元素
来源：http://nq.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gb.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kr.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aa.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://pa.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://du.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lo.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gl.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sc.colortex.cn

[D05] 访问与修改元素
来源：http://zj.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rj.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://go.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fx.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://ib.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://vg.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://dw.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lz.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bf.jianghongdianzi.cn

[D06] 数组长度
来源：http://gh.shxzskj.cn

Py:   len(arr)
来源：http://qc.521024.cn

PHP:  count($arr);
来源：http://ro.huanxung.cn

JS:   arr.length
来源：http://ta.nszjky.cn

TS:   arr.length
来源：http://sx.nicolike.cn

Java: list.size();
来源：http://qu.yuexingan06.cn

Go:   len(arr)
来源：http://xk.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://vy.yuntaijiaju.cn

C#:   list.Count;
来源：http://sn.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://lg.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nb.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vi.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://xq.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://tp.shxzukj.cn

Java: list.subList(1, 4);
来源：http://om.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://at.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://rw.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://ee.panjiajie.cn

[D08] 合并两个数组
来源：http://ut.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://we.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://vx.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aw.9csxet.cn

TS:   [...a, ...b];
来源：http://bc.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ou.gzmigu.cn

Go:   append(a, b...)
来源：http://fo.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://fg.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://kb.nicolike.cn

[D09] 排序（升序）
来源：http://aw.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://ks.szxytkj.cn

PHP:  sort($arr);
来源：http://dn.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wj.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ki.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ia.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nu.chemitech.net.cn

Ruby: arr.sort
来源：http://nv.9csxet.cn

C#:   list.Sort();
来源：http://pm.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xv.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uv.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cb.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://la.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hl.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qx.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ok.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mp.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qb.haigaiapp.cn

[D11] 反转数组
来源：http://rx.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xn.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://uw.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gf.shxzukj.cn

TS:   [...arr].reverse();
来源：http://rh.szxytkj.cn

Java: Collections.reverse(list);
来源：http://jw.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://eg.huixiangedu.cn

Ruby: arr.reverse
来源：http://jx.wgjwhj.cn

C#:   list.Reverse();
来源：http://yv.yuexingan06.cn

[D12] 查找元素下标
来源：http://ml.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://mc.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sf.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sn.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ph.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uh.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://qc.chemitech.net.cn

Ruby: arr.index(x)
来源：http://do.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://il.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://vw.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lq.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://es.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://de.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://ty.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fn.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ha.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ig.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mn.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://fk.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ka.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://da.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://ao.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://dv.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ir.yuntaijiaju.cn

Go:   // 手写循环
来源：http://uf.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ps.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ir.szsharing.cn

[D15] 去重
来源：http://gu.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fv.gzmigu.cn

PHP:  array_unique($arr);
来源：http://nn.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://rc.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://sx.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zn.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tg.muxihuayi.cn

Ruby: arr.uniq
来源：http://sj.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://ki.huanxung.cn

[D16] 求和与平均值
来源：http://xe.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wv.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gz.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ns.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iq.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pe.huanxung.cn

Go:   // 手写循环累加
来源：http://jv.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qy.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://vr.gzmigu.cn

[D17] 最大值与最小值
来源：http://wb.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://zc.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://zy.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ci.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://sm.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://am.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mg.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://sd.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://kr.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://ic.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lv.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://nw.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fr.yuntaijiaju.cn

TS:   nested.flat();
来源：http://no.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zc.lnxyls.cn

Go:   // 手写双层循环
来源：http://vx.bjjhwx.cn

Ruby: nested.flatten
来源：http://fa.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ed.nicolike.cn

[D19] 按字段分组
来源：http://hl.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://av.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yf.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://di.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sr.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://al.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://fq.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bc.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://un.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://ys.hahajie.cn

Py:   Counter(arr)
来源：http://wk.szsharing.cn

PHP:  array_count_values($arr);
来源：http://hg.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mh.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oq.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dm.nicolike.cn

Go:   // 手写 map[T]int
来源：http://dw.bjjhwx.cn

Ruby: arr.tally
来源：http://wr.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cj.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://cx.asd995.cn

Py:   x in arr
来源：http://rh.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://os.hnjuh.cn

JS:   arr.includes(x)
来源：http://pf.hahajie.cn

TS:   arr.includes(x)
来源：http://tw.bookmarksfly.cn

Java: list.contains(x)
来源：http://cj.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://ru.huanxung.cn

Ruby: arr.include?(x)
来源：http://tl.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://fu.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://em.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ob.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zc.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rz.shxzukj.cn

TS:   [...arr];
来源：http://ta.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://kf.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ha.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://fp.szsharing.cn

C#:   new List<int>(list);
来源：http://ww.nszjky.cn

[D23] reduce 累积计算
来源：http://ks.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ac.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rf.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nf.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ke.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kx.hahajie.cn

Go:   // 手写循环
来源：http://tr.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xd.hahajie.cn


<!-- 参考信息 -->