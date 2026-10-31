代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ko.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sz.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://th.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ag.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://ry.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://iy.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://jf.jctech888.com.cn

[C05] 返回多个值
来源：http://ni.nszjky.cn

Py:   return a, b
来源：http://tr.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://kf.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fg.jianghongdianzi.cn

TS:   return { a, b };
来源：http://kx.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ei.huanxung.cn

Go:   return a, b
来源：http://ri.9csxet.cn

Ruby: return a, b
来源：http://vf.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://hn.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://im.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://fy.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ht.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://wq.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://ek.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nm.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tk.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://rb.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zm.asd995.cn

[C07] 把函数作为参数传入
来源：http://zp.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gm.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fp.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ce.huanxung.cn

TS:   arr.map(String)
来源：http://vo.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tr.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vm.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://dq.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kg.szsharing.cn

[C08] 闭包
来源：http://es.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zd.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yr.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uw.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://we.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dl.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fx.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hb.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ip.521024.cn

[C09] 递归
来源：http://tv.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lr.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sk.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tk.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ao.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mw.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bm.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://im.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tq.haigaiapp.cn

[C10] 变量作用域
来源：http://qc.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ya.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vy.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fo.haigaiapp.cn

TS:   同 JS
来源：http://ad.hahajie.cn

Java: 方法内为块级作用域
来源：http://ag.shxzukj.cn

Go:   花括号块级作用域
来源：http://ys.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nb.newstarts.cn

C#:   块级作用域
来源：http://fg.shxzukj.cn

[C11] 模块导入与导出
来源：http://vo.wgjwhj.cn

Py:   from module import func
来源：http://rb.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mq.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pe.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bl.szsharing.cn

Java: import java.util.List;
来源：http://mv.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://en.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://zm.hnjuh.cn

C#:   using System.Text;
来源：http://yb.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://yf.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://jo.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://yw.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://kb.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://nm.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tg.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://ut.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://gz.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jx.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://al.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ds.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gv.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dn.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tl.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nt.huanxung.cn

Go:   func add(a, b int) int
来源：http://ze.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yn.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://br.nicolike.cn

[C14] 泛型函数
来源：http://jl.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ve.bookmarksfly.cn

PHP:  // 无泛型
来源：http://pj.muxihuayi.cn

JS:   // 无泛型
来源：http://xv.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wk.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lz.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pv.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://za.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jg.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://fm.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oh.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://bu.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ar.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bl.asd995.cn

Java: // 无解构
来源：http://ng.hahajie.cn

Go:   // 无解构
来源：http://cn.jctech888.com.cn

Ruby: a, b = pair
来源：http://ed.szsharing.cn

C#:   var (a, b) = pair;
来源：http://zj.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://do.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wa.shtwfgs.cn

PHP:  // 无重载
来源：http://cy.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fm.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://aj.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qw.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://yb.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://xy.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jz.shtwfgs.cn

================================================================================
来源：http://ec.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://tq.newstarts.cn

================================================================================
来源：http://ow.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://wh.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lp.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jj.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nz.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ig.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vv.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://dz.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ev.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nk.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://pr.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gq.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qa.hnjuh.cn

JS:   arr.push(4);
来源：http://ls.9csxet.cn

TS:   arr.push(4);
来源：http://dy.yuexingan06.cn

Java: list.add(4);
来源：http://jf.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://sd.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://yy.lnxyls.cn

C#:   list.Add(4);
来源：http://ny.asd995.cn

[D03] 在指定位置插入元素
来源：http://sd.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://py.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ql.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mk.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://if.shxzskj.cn

Java: list.add(0, 0);
来源：http://zs.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vb.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jh.asd995.cn

C#:   list.Insert(0, 0);
来源：http://ma.521024.cn

[D04] 删除元素
来源：http://kj.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xv.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ec.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rz.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://tn.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hi.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ik.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wg.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hl.shxzukj.cn

[D05] 访问与修改元素
来源：http://zr.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://de.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lv.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ts.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://rh.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://xg.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://gg.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uo.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oc.chemitech.net.cn

[D06] 数组长度
来源：http://is.nicolike.cn

Py:   len(arr)
来源：http://bg.jianghongdianzi.cn

PHP:  count($arr);
来源：http://xo.muxihuayi.cn

JS:   arr.length
来源：http://dg.yuexingan06.cn

TS:   arr.length
来源：http://ej.haigaiapp.cn

Java: list.size();
来源：http://ez.hahajie.cn

Go:   len(arr)
来源：http://fr.nicolike.cn

Ruby: arr.length; arr.size
来源：http://xr.bjjhwx.cn

C#:   list.Count;
来源：http://xy.huanxung.cn

[D07] 切片 / 取子数组
来源：http://sm.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jo.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qw.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://tz.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://kz.szsharing.cn

Java: list.subList(1, 4);
来源：http://uk.9csxet.cn

Go:   arr[1:4]
来源：http://yp.shxzskj.cn

Ruby: arr[1, 3]
来源：http://vf.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://fe.wgjwhj.cn

[D08] 合并两个数组
来源：http://gn.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://ow.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://dv.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fb.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ar.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nd.nicolike.cn

Go:   append(a, b...)
来源：http://mn.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://xw.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://db.jctech888.com.cn

[D09] 排序（升序）
来源：http://ox.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://me.muxihuayi.cn

PHP:  sort($arr);
来源：http://jq.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nu.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dn.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ew.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gp.bjjhwx.cn

Ruby: arr.sort
来源：http://fy.hnjuh.cn

C#:   list.Sort();
来源：http://fj.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qw.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jt.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fr.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kq.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tl.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://za.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dc.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ox.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dw.colortex.cn

[D11] 反转数组
来源：http://ma.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://je.521024.cn

PHP:  array_reverse($arr);
来源：http://ra.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qo.shxzukj.cn

TS:   [...arr].reverse();
来源：http://vf.lnxyls.cn

Java: Collections.reverse(list);
来源：http://af.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://us.asd995.cn

Ruby: arr.reverse
来源：http://rz.huanxung.cn

C#:   list.Reverse();
来源：http://wg.yuexingan06.cn

[D12] 查找元素下标
来源：http://ij.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://gb.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wf.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ns.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kj.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xg.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://ma.nicolike.cn

Ruby: arr.index(x)
来源：http://lq.hahajie.cn

C#:   list.IndexOf(x);
来源：http://uc.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://ty.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jq.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yt.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://cn.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://hv.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://su.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aw.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qp.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ld.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://uq.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cy.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xa.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ov.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://vy.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vf.jianghongdianzi.cn

Go:   // 手写循环
来源：http://il.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://za.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ex.muxihuayi.cn

[D15] 去重
来源：http://hu.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://te.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://ic.nszjky.cn

JS:   [...new Set(arr)]
来源：http://fb.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://gq.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rb.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ra.colortex.cn

Ruby: arr.uniq
来源：http://mk.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://rj.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://mc.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fd.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oj.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bo.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yf.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wp.hahajie.cn

Go:   // 手写循环累加
来源：http://ei.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ji.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://hg.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://pu.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://it.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://wi.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jv.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://bl.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zm.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://si.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://ja.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://fd.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://hw.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gb.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://qm.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pa.hnjuh.cn

TS:   nested.flat();
来源：http://yk.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://up.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://sg.asd995.cn

Ruby: nested.flatten
来源：http://rf.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mr.nicolike.cn

[D19] 按字段分组
来源：http://xd.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jl.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pm.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ds.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cv.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xi.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://pc.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://co.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mg.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://ki.haigaiapp.cn

Py:   Counter(arr)
来源：http://nn.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://na.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xt.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dg.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dq.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://dv.521024.cn

Ruby: arr.tally
来源：http://oc.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sl.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://pz.shxzskj.cn

Py:   x in arr
来源：http://eh.nicolike.cn


<!-- 参考信息 -->