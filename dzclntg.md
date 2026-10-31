代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://as.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://oa.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://it.chemitech.net.cn

[C05] 返回多个值
来源：http://eq.521024.cn

Py:   return a, b
来源：http://hd.szsharing.cn

PHP:  return [$a, $b];
来源：http://cz.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://on.muxihuayi.cn

TS:   return { a, b };
来源：http://xf.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ep.shxzukj.cn

Go:   return a, b
来源：http://jh.shxzskj.cn

Ruby: return a, b
来源：http://mi.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://yb.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://zf.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://au.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jv.hnjuh.cn

JS:   const square = x => x * x;
来源：http://ah.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ia.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lv.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ul.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://xm.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yp.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://av.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hu.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ra.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wc.shtwfgs.cn

TS:   arr.map(String)
来源：http://uo.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nm.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bk.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://ci.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sj.szsharing.cn

[C08] 闭包
来源：http://ig.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sx.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pk.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ki.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://em.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yp.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fu.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ym.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ve.szxytkj.cn

[C09] 递归
来源：http://vu.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ts.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hb.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dy.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xk.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gm.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://on.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://il.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ao.newstarts.cn

[C10] 变量作用域
来源：http://ya.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kr.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wf.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jv.wgjwhj.cn

TS:   同 JS
来源：http://uu.shxzskj.cn

Java: 方法内为块级作用域
来源：http://zv.asd995.cn

Go:   花括号块级作用域
来源：http://un.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sy.hahajie.cn

C#:   块级作用域
来源：http://rd.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://fa.9csxet.cn

Py:   from module import func
来源：http://zt.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gl.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cq.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dx.nszjky.cn

Java: import java.util.List;
来源：http://ko.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dw.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://iv.newstarts.cn

C#:   using System.Text;
来源：http://ag.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://my.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://pc.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://kt.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://bs.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://sp.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dw.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://lr.521024.cn

Ruby: -> { puts "run" }.call
来源：http://vj.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ag.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://yi.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jx.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pv.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rx.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jc.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qy.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://bv.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qm.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wc.newstarts.cn

[C14] 泛型函数
来源：http://jk.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fw.yuexingan06.cn

PHP:  // 无泛型
来源：http://oe.huixiangedu.cn

JS:   // 无泛型
来源：http://lr.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ch.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nm.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ds.panjiajie.cn

Ruby: # 无泛型
来源：http://aj.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zu.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://ju.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hw.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://jm.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hk.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oy.shtwfgs.cn

Java: // 无解构
来源：http://hc.shtwfgs.cn

Go:   // 无解构
来源：http://xz.muxihuayi.cn

Ruby: a, b = pair
来源：http://jk.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://aj.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://lq.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ty.9csxet.cn

PHP:  // 无重载
来源：http://zu.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sf.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://rd.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jz.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://my.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://aw.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sx.shtwfgs.cn

================================================================================
来源：http://um.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://ts.szsharing.cn

================================================================================
来源：http://jo.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://nj.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nb.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xu.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://to.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sc.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yw.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://gz.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://qy.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bj.newstarts.cn

[D02] 追加元素到末尾
来源：http://xz.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ch.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ys.huanxung.cn

JS:   arr.push(4);
来源：http://gk.newstarts.cn

TS:   arr.push(4);
来源：http://mk.9csxet.cn

Java: list.add(4);
来源：http://gv.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://yu.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://eb.colortex.cn

C#:   list.Add(4);
来源：http://gm.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://zr.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://yh.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yu.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oz.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ke.muxihuayi.cn

Java: list.add(0, 0);
来源：http://td.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zl.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wi.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://dn.shxzukj.cn

[D04] 删除元素
来源：http://qz.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fu.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://df.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ck.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://pb.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bs.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ln.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pf.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wd.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://dr.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xf.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pn.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hy.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://fv.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://wz.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://cr.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mt.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fo.yuexingan06.cn

[D06] 数组长度
来源：http://fk.huixiangedu.cn

Py:   len(arr)
来源：http://bo.nszjky.cn

PHP:  count($arr);
来源：http://pr.panjiajie.cn

JS:   arr.length
来源：http://hw.521024.cn

TS:   arr.length
来源：http://gq.panjiajie.cn

Java: list.size();
来源：http://tl.szsharing.cn

Go:   len(arr)
来源：http://vm.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://kn.9csxet.cn

C#:   list.Count;
来源：http://vt.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://gz.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yo.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wm.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://ej.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://xi.panjiajie.cn

Java: list.subList(1, 4);
来源：http://mi.szxytkj.cn

Go:   arr[1:4]
来源：http://dc.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://cq.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://vp.lnxyls.cn

[D08] 合并两个数组
来源：http://zl.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://ud.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://ib.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jw.nszjky.cn

TS:   [...a, ...b];
来源：http://cz.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://co.asd995.cn

Go:   append(a, b...)
来源：http://ug.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://as.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://ei.huanxung.cn

[D09] 排序（升序）
来源：http://fg.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ri.yuexingan06.cn

PHP:  sort($arr);
来源：http://hu.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ws.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yh.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xt.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ao.bookmarksfly.cn

Ruby: arr.sort
来源：http://ld.shxzskj.cn

C#:   list.Sort();
来源：http://qu.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gz.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jz.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fu.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gl.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ah.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://da.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pa.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zh.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uq.9csxet.cn

[D11] 反转数组
来源：http://yd.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nb.szsharing.cn

PHP:  array_reverse($arr);
来源：http://pb.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ev.gzmigu.cn

TS:   [...arr].reverse();
来源：http://vv.hnjuh.cn

Java: Collections.reverse(list);
来源：http://cx.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://gh.colortex.cn

Ruby: arr.reverse
来源：http://ug.jctech888.com.cn

C#:   list.Reverse();
来源：http://zt.chemitech.net.cn

[D12] 查找元素下标
来源：http://mk.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://np.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kg.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://el.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fe.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eh.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://ri.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://jm.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://hp.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://yn.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tw.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oq.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://mr.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://bi.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qf.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bq.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ce.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://at.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://gh.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ja.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dm.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://rs.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://zy.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dx.bjjhwx.cn

Go:   // 手写循环
来源：http://jk.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ch.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zs.yuntaijiaju.cn

[D15] 去重
来源：http://jt.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ch.panjiajie.cn

PHP:  array_unique($arr);
来源：http://ec.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://bn.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://hk.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://is.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vt.lnxyls.cn

Ruby: arr.uniq
来源：http://xk.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://ae.lnxyls.cn

[D16] 求和与平均值
来源：http://fd.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zm.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kn.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lv.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zt.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mm.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://cy.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lc.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://hl.hnjuh.cn

[D17] 最大值与最小值
来源：http://sq.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://fc.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://ji.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eo.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://zr.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fo.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tt.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://yk.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://pj.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://aj.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ib.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://et.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bo.bookmarksfly.cn

TS:   nested.flat();
来源：http://as.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bi.huixiangedu.cn

Go:   // 手写双层循环
来源：http://bh.huanxung.cn

Ruby: nested.flatten
来源：http://dz.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sj.shtwfgs.cn

[D19] 按字段分组
来源：http://ki.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://do.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ls.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yw.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pq.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kp.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://kz.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jg.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://il.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://mb.wgjwhj.cn

Py:   Counter(arr)
来源：http://nm.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://ka.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zj.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wl.nicolike.cn

Go:   // 手写 map[T]int
来源：http://ur.szxytkj.cn

Ruby: arr.tally
来源：http://jb.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lx.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://wc.521024.cn

Py:   x in arr
来源：http://cg.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://kc.huixiangedu.cn

JS:   arr.includes(x)
来源：http://kv.lnxyls.cn

TS:   arr.includes(x)
来源：http://tn.shtwfgs.cn

Java: list.contains(x)
来源：http://hx.bookmarksfly.cn


<!-- 参考信息 -->