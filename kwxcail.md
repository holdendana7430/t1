代发 wailian999

[C02] 默认参数
来源：http://pl.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://po.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yg.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ss.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zz.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lp.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://il.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ja.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://wa.szsharing.cn

[C03] 可变参数
来源：http://se.521024.cn

Py:   def total(*args): return sum(args)
来源：http://vv.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zl.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://md.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yl.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pa.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bd.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jq.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bx.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://kf.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ry.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bl.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cg.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uy.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ot.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://kj.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://bo.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://gl.wgjwhj.cn

[C05] 返回多个值
来源：http://py.huixiangedu.cn

Py:   return a, b
来源：http://se.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://uf.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://db.9csxet.cn

TS:   return { a, b };
来源：http://dm.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kb.newstarts.cn

Go:   return a, b
来源：http://ln.hnjuh.cn

Ruby: return a, b
来源：http://wc.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://uj.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://bw.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://ae.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tv.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://ci.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://eo.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jl.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dr.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://mm.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fx.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://pe.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mk.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ad.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vg.chemitech.net.cn

TS:   arr.map(String)
来源：http://hl.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hj.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ha.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://ec.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bm.shxzukj.cn

[C08] 闭包
来源：http://dq.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bl.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oe.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dd.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vi.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xs.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wi.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kp.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://da.bjjhwx.cn

[C09] 递归
来源：http://hs.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uq.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kk.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sa.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://va.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pv.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hv.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gm.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fu.nszjky.cn

[C10] 变量作用域
来源：http://vv.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rz.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gc.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sc.szsharing.cn

TS:   同 JS
来源：http://jn.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://sl.haigaiapp.cn

Go:   花括号块级作用域
来源：http://ak.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pf.jctech888.com.cn

C#:   块级作用域
来源：http://lz.bjjhwx.cn

[C11] 模块导入与导出
来源：http://xi.lnxyls.cn

Py:   from module import func
来源：http://rd.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://az.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vl.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uk.shxzskj.cn

Java: import java.util.List;
来源：http://nf.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rx.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ng.shxzskj.cn

C#:   using System.Text;
来源：http://eh.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://xi.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://ke.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://or.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://dh.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://pi.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pg.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ho.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://pm.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jz.521024.cn

[C13] 类型声明 / 类型注解
来源：http://id.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kq.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tw.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zf.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ue.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nu.9csxet.cn

Go:   func add(a, b int) int
来源：http://wx.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kq.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yz.wgjwhj.cn

[C14] 泛型函数
来源：http://jw.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kk.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://bg.chemitech.net.cn

JS:   // 无泛型
来源：http://wi.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bs.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iq.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gl.shxzukj.cn

Ruby: # 无泛型
来源：http://zy.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wa.nicolike.cn

[C15] 解构 / 展开参数
来源：http://mf.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kb.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://ys.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eu.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wa.hahajie.cn

Java: // 无解构
来源：http://vh.yuntaijiaju.cn

Go:   // 无解构
来源：http://jh.hnjuh.cn

Ruby: a, b = pair
来源：http://ox.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://ia.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://rp.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oy.yuexingan06.cn

PHP:  // 无重载
来源：http://kg.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rg.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://de.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nz.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://qp.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://tk.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ut.jianghongdianzi.cn

================================================================================
来源：http://tn.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ex.wgjwhj.cn

================================================================================
来源：http://ym.asd995.cn

[D01] 创建数组 / 列表
来源：http://sv.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sn.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://du.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wg.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fe.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tt.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://ow.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://ft.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bq.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://es.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mz.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ot.huanxung.cn

JS:   arr.push(4);
来源：http://xi.huixiangedu.cn

TS:   arr.push(4);
来源：http://lk.panjiajie.cn

Java: list.add(4);
来源：http://no.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://az.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://nd.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://ox.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://iv.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://or.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hn.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ji.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://rd.wgjwhj.cn

Java: list.add(0, 0);
来源：http://xo.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qt.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kl.asd995.cn

C#:   list.Insert(0, 0);
来源：http://rb.nicolike.cn

[D04] 删除元素
来源：http://ru.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yj.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pi.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vy.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://ur.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rc.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mi.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sw.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cm.panjiajie.cn

[D05] 访问与修改元素
来源：http://yx.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lu.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hc.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ia.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://xg.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://xe.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://dr.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wz.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kf.gzmigu.cn

[D06] 数组长度
来源：http://vx.521024.cn

Py:   len(arr)
来源：http://lh.9csxet.cn

PHP:  count($arr);
来源：http://cl.huixiangedu.cn

JS:   arr.length
来源：http://ii.szsharing.cn

TS:   arr.length
来源：http://oa.bjjhwx.cn

Java: list.size();
来源：http://wu.haigaiapp.cn

Go:   len(arr)
来源：http://tw.asd995.cn

Ruby: arr.length; arr.size
来源：http://az.chemitech.net.cn

C#:   list.Count;
来源：http://ei.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://nj.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aj.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fl.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://yc.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://md.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://zq.huixiangedu.cn

Go:   arr[1:4]
来源：http://gh.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://mw.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://fp.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://md.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://xx.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://rj.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ip.haigaiapp.cn

TS:   [...a, ...b];
来源：http://fr.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nt.shxzukj.cn

Go:   append(a, b...)
来源：http://yo.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://sz.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://bk.bookmarksfly.cn

[D09] 排序（升序）
来源：http://ue.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://yn.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://vn.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mk.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kj.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ja.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wi.yuexingan06.cn

Ruby: arr.sort
来源：http://pn.shxzskj.cn

C#:   list.Sort();
来源：http://zb.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fb.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cv.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wa.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qj.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ba.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rs.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wk.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://de.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tp.colortex.cn

[D11] 反转数组
来源：http://og.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pl.asd995.cn

PHP:  array_reverse($arr);
来源：http://si.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hc.asd995.cn

TS:   [...arr].reverse();
来源：http://mo.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://zd.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://ym.asd995.cn

Ruby: arr.reverse
来源：http://si.huixiangedu.cn

C#:   list.Reverse();
来源：http://vd.hahajie.cn

[D12] 查找元素下标
来源：http://rh.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://ct.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://af.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hj.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uo.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wr.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://ey.muxihuayi.cn

Ruby: arr.index(x)
来源：http://fw.nicolike.cn

C#:   list.IndexOf(x);
来源：http://rh.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ai.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dg.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ra.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://oc.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://ig.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://le.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sa.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gp.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pm.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://yj.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pq.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ih.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://qm.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://gf.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qi.shxzskj.cn

Go:   // 手写循环
来源：http://cq.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ts.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://py.wgjwhj.cn

[D15] 去重
来源：http://fh.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zr.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://jp.colortex.cn

JS:   [...new Set(arr)]
来源：http://gk.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://ck.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sw.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wy.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://nv.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://kp.yuexingan06.cn

[D16] 求和与平均值
来源：http://bq.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jq.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mb.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ai.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bq.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rj.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://xw.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mm.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://jo.shtwfgs.cn

[D17] 最大值与最小值
来源：http://la.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://ih.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://sw.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wf.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://zx.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ag.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xh.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://sl.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://oy.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://hy.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dk.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://sr.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ht.colortex.cn

TS:   nested.flat();
来源：http://fr.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gf.huanxung.cn

Go:   // 手写双层循环
来源：http://qm.szxytkj.cn

Ruby: nested.flatten
来源：http://gj.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qm.muxihuayi.cn


<!-- 参考信息 -->