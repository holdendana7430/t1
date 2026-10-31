代发 wailian999

Py:   return a, b
来源：http://gp.asd995.cn

PHP:  return [$a, $b];
来源：http://cx.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qk.521024.cn

TS:   return { a, b };
来源：http://uw.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pd.jianghongdianzi.cn

Go:   return a, b
来源：http://xi.bjjhwx.cn

Ruby: return a, b
来源：http://ed.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://zl.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://mk.newstarts.cn

Py:   square = lambda x: x * x
来源：http://dd.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cb.panjiajie.cn

JS:   const square = x => x * x;
来源：http://ef.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://xl.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lz.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ot.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://qu.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dw.colortex.cn

[C07] 把函数作为参数传入
来源：http://qc.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qy.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ro.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bu.chemitech.net.cn

TS:   arr.map(String)
来源：http://gt.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zq.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wq.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://wb.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zw.hnjuh.cn

[C08] 闭包
来源：http://cf.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kc.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dx.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eb.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ol.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sx.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xr.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ae.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nn.gzmigu.cn

[C09] 递归
来源：http://ec.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mt.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wl.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rg.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fj.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pf.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ia.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rx.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mo.panjiajie.cn

[C10] 变量作用域
来源：http://cj.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eq.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wa.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xr.jctech888.com.cn

TS:   同 JS
来源：http://ah.szxytkj.cn

Java: 方法内为块级作用域
来源：http://ok.szsharing.cn

Go:   花括号块级作用域
来源：http://wg.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yz.colortex.cn

C#:   块级作用域
来源：http://ox.gzmigu.cn

[C11] 模块导入与导出
来源：http://pf.szxytkj.cn

Py:   from module import func
来源：http://ld.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zu.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://in.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gq.hahajie.cn

Java: import java.util.List;
来源：http://wk.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nx.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://fe.shxzukj.cn

C#:   using System.Text;
来源：http://pb.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://jj.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://bm.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://tx.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://ey.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://xl.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uk.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ob.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://ao.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jc.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://is.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fm.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eu.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xr.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uw.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gd.szxytkj.cn

Go:   func add(a, b int) int
来源：http://re.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://la.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vu.yuexingan06.cn

[C14] 泛型函数
来源：http://ga.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ju.szsharing.cn

PHP:  // 无泛型
来源：http://gz.huanxung.cn

JS:   // 无泛型
来源：http://ii.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zx.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wf.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ed.lnxyls.cn

Ruby: # 无泛型
来源：http://bd.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xa.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://ki.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ip.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://bt.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yr.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iy.jctech888.com.cn

Java: // 无解构
来源：http://th.lnxyls.cn

Go:   // 无解构
来源：http://dd.nicolike.cn

Ruby: a, b = pair
来源：http://ph.521024.cn

C#:   var (a, b) = pair;
来源：http://ge.asd995.cn

[C16] 函数 / 方法重载
来源：http://fe.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oq.hahajie.cn

PHP:  // 无重载
来源：http://om.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mj.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://gl.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ou.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://eq.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://vg.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sd.haigaiapp.cn

================================================================================
来源：http://fl.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://ru.nszjky.cn

================================================================================
来源：http://jo.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://is.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ee.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bo.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ao.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ci.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hh.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://fj.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://rs.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hx.nszjky.cn

[D02] 追加元素到末尾
来源：http://cf.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hh.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xx.hnjuh.cn

JS:   arr.push(4);
来源：http://ih.yuexingan06.cn

TS:   arr.push(4);
来源：http://xq.szsharing.cn

Java: list.add(4);
来源：http://ri.asd995.cn

Go:   arr = append(arr, 4)
来源：http://wn.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://yf.chemitech.net.cn

C#:   list.Add(4);
来源：http://hk.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://zy.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://yq.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vb.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ox.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://pd.chemitech.net.cn

Java: list.add(0, 0);
来源：http://az.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ae.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ee.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ft.colortex.cn

[D04] 删除元素
来源：http://ah.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dr.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rr.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://if.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://ku.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ff.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ox.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ux.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xv.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://mn.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ro.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tr.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fh.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://fp.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://zu.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://le.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aq.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nn.panjiajie.cn

[D06] 数组长度
来源：http://tj.yuexingan06.cn

Py:   len(arr)
来源：http://qh.shtwfgs.cn

PHP:  count($arr);
来源：http://dy.asd995.cn

JS:   arr.length
来源：http://qw.bookmarksfly.cn

TS:   arr.length
来源：http://vb.chemitech.net.cn

Java: list.size();
来源：http://zw.huixiangedu.cn

Go:   len(arr)
来源：http://lh.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://pe.colortex.cn

C#:   list.Count;
来源：http://al.9csxet.cn

[D07] 切片 / 取子数组
来源：http://tr.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jt.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hw.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://ej.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://qk.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://ab.huanxung.cn

Go:   arr[1:4]
来源：http://wk.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://mz.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://hd.lnxyls.cn

[D08] 合并两个数组
来源：http://rl.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://sk.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://ia.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ou.chemitech.net.cn

TS:   [...a, ...b];
来源：http://nf.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tk.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://zf.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://dy.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://em.bookmarksfly.cn

[D09] 排序（升序）
来源：http://gt.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://tr.haigaiapp.cn

PHP:  sort($arr);
来源：http://ep.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qu.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ww.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lx.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vi.nszjky.cn

Ruby: arr.sort
来源：http://te.bookmarksfly.cn

C#:   list.Sort();
来源：http://jl.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zl.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kv.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mz.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yq.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gv.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yj.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ny.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ob.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://go.szxytkj.cn

[D11] 反转数组
来源：http://kk.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yx.521024.cn

PHP:  array_reverse($arr);
来源：http://ji.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ph.lnxyls.cn

TS:   [...arr].reverse();
来源：http://xq.szxytkj.cn

Java: Collections.reverse(list);
来源：http://fe.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://na.gzmigu.cn

Ruby: arr.reverse
来源：http://hd.shxzukj.cn

C#:   list.Reverse();
来源：http://df.huanxung.cn

[D12] 查找元素下标
来源：http://ry.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://nw.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mt.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eb.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bh.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://to.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://sx.gzmigu.cn

Ruby: arr.index(x)
来源：http://zh.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ff.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://wy.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fu.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tu.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://xg.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://zi.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://st.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://li.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://id.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gb.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://cw.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wr.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qg.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://da.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://qp.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cy.szsharing.cn

Go:   // 手写循环
来源：http://ky.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xy.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zw.hahajie.cn

[D15] 去重
来源：http://ux.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nicolike.cn

PHP:  array_unique($arr);
来源：http://eb.asd995.cn

JS:   [...new Set(arr)]
来源：http://fs.nszjky.cn

TS:   [...new Set(arr)]
来源：http://vg.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ig.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://of.szxytkj.cn

Ruby: arr.uniq
来源：http://xu.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://ri.lnxyls.cn

[D16] 求和与平均值
来源：http://ou.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cr.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tt.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zx.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ge.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://do.gzmigu.cn

Go:   // 手写循环累加
来源：http://aj.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://su.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://fw.gzmigu.cn

[D17] 最大值与最小值
来源：http://vl.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://rn.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://ky.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dv.colortex.cn

TS:   Math.max(...arr);
来源：http://pt.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wr.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vg.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://lt.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://bd.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://vd.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sc.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://nc.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oc.shxzukj.cn

TS:   nested.flat();
来源：http://yd.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yj.huixiangedu.cn

Go:   // 手写双层循环
来源：http://af.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://va.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xr.521024.cn

[D19] 按字段分组
来源：http://qh.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dg.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fg.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bc.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dw.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rl.asd995.cn

Go:   // 手写 map[string][]T
来源：http://bx.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ff.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hb.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://gt.hahajie.cn

Py:   Counter(arr)
来源：http://zq.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://zj.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sy.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mw.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cr.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://ne.chemitech.net.cn

Ruby: arr.tally
来源：http://bi.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hu.nszjky.cn

[D21] 判断是否包含某元素
来源：http://nf.jctech888.com.cn

Py:   x in arr
来源：http://ss.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://za.bjjhwx.cn

JS:   arr.includes(x)
来源：http://zu.jctech888.com.cn

TS:   arr.includes(x)
来源：http://va.lnxyls.cn

Java: list.contains(x)
来源：http://lt.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://ab.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://pg.shxzukj.cn

C#:   list.Contains(x)
来源：http://pj.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://nl.521024.cn


<!-- 参考信息 -->