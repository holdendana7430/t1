代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://am.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wp.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://is.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://js.gzmigu.cn

[C02] 默认参数
来源：http://gx.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://qr.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://do.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://rh.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sj.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tu.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wa.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://yf.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://af.asd995.cn

[C03] 可变参数
来源：http://co.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://pi.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ng.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ll.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dg.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ct.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uv.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pz.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://zo.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wl.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hp.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://el.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://si.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://iq.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://hd.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://gw.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://ga.jctech888.com.cn

[C05] 返回多个值
来源：http://bl.panjiajie.cn

Py:   return a, b
来源：http://zn.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://qf.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lg.jianghongdianzi.cn

TS:   return { a, b };
来源：http://ai.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kh.panjiajie.cn

Go:   return a, b
来源：http://ha.nszjky.cn

Ruby: return a, b
来源：http://qw.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://rd.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://th.asd995.cn

Py:   square = lambda x: x * x
来源：http://ym.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wc.nicolike.cn

JS:   const square = x => x * x;
来源：http://cc.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://dy.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tj.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gk.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://jr.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xt.hahajie.cn

[C07] 把函数作为参数传入
来源：http://bw.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wy.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bm.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tm.jctech888.com.cn

TS:   arr.map(String)
来源：http://sb.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pm.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rr.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://hv.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cy.asd995.cn

[C08] 闭包
来源：http://ad.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pq.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sz.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sl.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mx.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ci.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dm.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://do.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sn.9csxet.cn

[C09] 递归
来源：http://bo.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://of.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pj.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wd.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sr.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oc.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nt.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ja.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nj.gzmigu.cn

[C10] 变量作用域
来源：http://jh.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hp.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jk.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xr.nicolike.cn

TS:   同 JS
来源：http://aw.nicolike.cn

Java: 方法内为块级作用域
来源：http://sc.jctech888.com.cn

Go:   花括号块级作用域
来源：http://ez.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bi.huixinmuqiang.cn

C#:   块级作用域
来源：http://cb.nicolike.cn

[C11] 模块导入与导出
来源：http://ih.panjiajie.cn

Py:   from module import func
来源：http://ns.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ex.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mi.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ff.gzmigu.cn

Java: import java.util.List;
来源：http://uq.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lk.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://la.lnxyls.cn

C#:   using System.Text;
来源：http://kr.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://vn.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://kd.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://bi.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://lt.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://om.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gs.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://uw.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://pe.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gw.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://nb.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uw.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bt.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oe.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lr.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://au.szxytkj.cn

Go:   func add(a, b int) int
来源：http://rt.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ld.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hc.521024.cn

[C14] 泛型函数
来源：http://za.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://em.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://yg.muxihuayi.cn

JS:   // 无泛型
来源：http://aw.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wm.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zj.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ni.szsharing.cn

Ruby: # 无泛型
来源：http://ue.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qt.hahajie.cn

[C15] 解构 / 展开参数
来源：http://kn.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hq.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://at.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ms.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dv.gzmigu.cn

Java: // 无解构
来源：http://bd.colortex.cn

Go:   // 无解构
来源：http://nr.9csxet.cn

Ruby: a, b = pair
来源：http://hz.hahajie.cn

C#:   var (a, b) = pair;
来源：http://yt.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://ty.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://go.gzmigu.cn

PHP:  // 无重载
来源：http://rd.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://in.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://gc.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gv.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://jl.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://ag.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tw.chemitech.net.cn

================================================================================
来源：http://sk.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://dw.panjiajie.cn

================================================================================
来源：http://uy.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://eo.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aw.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gb.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://am.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ve.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ma.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://rn.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://bx.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zx.huanxung.cn

[D02] 追加元素到末尾
来源：http://zd.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zt.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uy.colortex.cn

JS:   arr.push(4);
来源：http://bl.newstarts.cn

TS:   arr.push(4);
来源：http://ih.9csxet.cn

Java: list.add(4);
来源：http://fp.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://fv.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://kk.szxytkj.cn

C#:   list.Add(4);
来源：http://dv.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://gm.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://vs.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yo.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lv.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://pi.haigaiapp.cn

Java: list.add(0, 0);
来源：http://bs.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ys.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ai.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://at.shtwfgs.cn

[D04] 删除元素
来源：http://ey.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qd.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mn.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://in.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://ia.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zw.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jq.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dj.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aq.nszjky.cn

[D05] 访问与修改元素
来源：http://tv.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vq.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mo.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://za.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://xx.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://cq.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://dp.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mg.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mn.shtwfgs.cn

[D06] 数组长度
来源：http://av.jctech888.com.cn

Py:   len(arr)
来源：http://fx.newstarts.cn

PHP:  count($arr);
来源：http://hg.shxzukj.cn

JS:   arr.length
来源：http://lt.bjjhwx.cn

TS:   arr.length
来源：http://rx.yuexingan06.cn

Java: list.size();
来源：http://hm.yuntaijiaju.cn

Go:   len(arr)
来源：http://kc.nszjky.cn

Ruby: arr.length; arr.size
来源：http://gf.shxzskj.cn

C#:   list.Count;
来源：http://sb.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://ye.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zq.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uc.colortex.cn

JS:   arr.slice(1, 4);
来源：http://ch.asd995.cn

TS:   arr.slice(1, 4);
来源：http://uc.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://ib.wgjwhj.cn

Go:   arr[1:4]
来源：http://wq.newstarts.cn

Ruby: arr[1, 3]
来源：http://rj.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://gw.huixiangedu.cn

[D08] 合并两个数组
来源：http://fs.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://vb.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://lv.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hr.hnjuh.cn

TS:   [...a, ...b];
来源：http://qq.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lw.shxzukj.cn

Go:   append(a, b...)
来源：http://nv.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://ei.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://vh.hnjuh.cn

[D09] 排序（升序）
来源：http://in.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://gp.shtwfgs.cn

PHP:  sort($arr);
来源：http://ex.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qt.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wl.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ls.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nk.newstarts.cn

Ruby: arr.sort
来源：http://qx.haigaiapp.cn

C#:   list.Sort();
来源：http://by.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tt.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zt.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ud.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rf.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ml.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lh.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vw.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ii.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://us.szxytkj.cn

[D11] 反转数组
来源：http://qv.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://al.newstarts.cn

PHP:  array_reverse($arr);
来源：http://pq.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ds.lnxyls.cn

TS:   [...arr].reverse();
来源：http://vs.nicolike.cn

Java: Collections.reverse(list);
来源：http://zq.521024.cn

Go:   slices.Reverse(arr)
来源：http://or.muxihuayi.cn

Ruby: arr.reverse
来源：http://my.shtwfgs.cn

C#:   list.Reverse();
来源：http://xn.nszjky.cn

[D12] 查找元素下标
来源：http://fh.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://sg.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ib.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tm.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qp.colortex.cn

Go:   slices.Index(arr, x)
来源：http://db.shxzskj.cn

Ruby: arr.index(x)
来源：http://bk.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://xk.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://eo.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nc.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gv.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://xp.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://fx.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zb.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ks.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sr.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bl.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://wp.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gq.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sq.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://ni.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://iu.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://do.bookmarksfly.cn

Go:   // 手写循环
来源：http://so.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ni.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qv.yuexingan06.cn

[D15] 去重
来源：http://vh.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qg.nszjky.cn

PHP:  array_unique($arr);
来源：http://ea.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://xp.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://jn.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tn.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zr.bookmarksfly.cn

Ruby: arr.uniq
来源：http://yz.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://zx.huixiangedu.cn

[D16] 求和与平均值
来源：http://gn.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nh.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ks.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sc.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fv.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://na.shxzskj.cn

Go:   // 手写循环累加
来源：http://ts.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nj.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://lq.colortex.cn

[D17] 最大值与最小值
来源：http://mp.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://sn.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://lu.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mz.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://eu.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qz.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gx.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://ft.colortex.cn

C#:   list.Max();  list.Min()
来源：http://wn.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://ul.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ry.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://go.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mu.muxihuayi.cn

TS:   nested.flat();
来源：http://gn.newstarts.cn


<!-- 参考信息 -->