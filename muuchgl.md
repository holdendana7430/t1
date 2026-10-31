代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://wd.yuntaijiaju.cn

[C03] 可变参数
来源：http://kq.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://hv.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rf.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tc.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gz.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dj.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yq.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ds.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://px.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://la.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tz.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://he.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ek.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mk.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://bm.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://ic.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://an.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://cg.hahajie.cn

[C05] 返回多个值
来源：http://nh.muxihuayi.cn

Py:   return a, b
来源：http://ke.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://gg.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pz.9csxet.cn

TS:   return { a, b };
来源：http://of.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xq.shxzskj.cn

Go:   return a, b
来源：http://uq.bookmarksfly.cn

Ruby: return a, b
来源：http://qb.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://jm.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://kz.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://wy.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wx.shxzukj.cn

JS:   const square = x => x * x;
来源：http://em.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://lw.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ni.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mf.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://uw.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yo.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://nd.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bd.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jp.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bl.hnjuh.cn

TS:   arr.map(String)
来源：http://uc.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://in.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ha.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://xg.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xl.nszjky.cn

[C08] 闭包
来源：http://zq.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mi.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ei.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ks.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://va.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cf.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qy.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mj.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bn.szsharing.cn

[C09] 递归
来源：http://ei.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://di.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ah.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sk.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tj.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yz.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ie.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bw.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ok.bjjhwx.cn

[C10] 变量作用域
来源：http://gq.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sr.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ec.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zg.wgjwhj.cn

TS:   同 JS
来源：http://ex.szsharing.cn

Java: 方法内为块级作用域
来源：http://mh.shxzskj.cn

Go:   花括号块级作用域
来源：http://pp.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gq.hnjuh.cn

C#:   块级作用域
来源：http://yp.szsharing.cn

[C11] 模块导入与导出
来源：http://cw.nicolike.cn

Py:   from module import func
来源：http://li.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://el.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kg.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://op.haigaiapp.cn

Java: import java.util.List;
来源：http://fi.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ma.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ge.lnxyls.cn

C#:   using System.Text;
来源：http://vd.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://eh.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://vy.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://dz.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://ij.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://zo.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qc.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://ke.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://cd.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kd.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://my.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hi.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zs.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rj.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ca.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ge.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://ve.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://po.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cl.nicolike.cn

[C14] 泛型函数
来源：http://pq.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tw.nszjky.cn

PHP:  // 无泛型
来源：http://si.huixinmuqiang.cn

JS:   // 无泛型
来源：http://tr.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lm.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yt.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jb.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://ug.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mf.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://hh.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aa.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://zh.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://di.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bc.nicolike.cn

Java: // 无解构
来源：http://vs.panjiajie.cn

Go:   // 无解构
来源：http://sf.huixiangedu.cn

Ruby: a, b = pair
来源：http://cw.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://ga.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://ve.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xl.wgjwhj.cn

PHP:  // 无重载
来源：http://zi.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ng.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ua.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gj.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://oq.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://mj.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://if.jctech888.com.cn

================================================================================
来源：http://dm.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://vp.nszjky.cn

================================================================================
来源：http://mi.asd995.cn

[D01] 创建数组 / 列表
来源：http://bj.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sd.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nc.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yi.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wb.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xv.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://dc.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://ld.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://db.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://uv.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dm.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fd.colortex.cn

JS:   arr.push(4);
来源：http://kg.nicolike.cn

TS:   arr.push(4);
来源：http://uz.nicolike.cn

Java: list.add(4);
来源：http://xm.asd995.cn

Go:   arr = append(arr, 4)
来源：http://xh.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://ee.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://qr.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://ar.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://gc.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ms.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pd.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://iw.colortex.cn

Java: list.add(0, 0);
来源：http://yb.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vg.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tr.521024.cn

C#:   list.Insert(0, 0);
来源：http://yy.szxytkj.cn

[D04] 删除元素
来源：http://hq.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://go.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cq.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yw.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://km.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vw.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fm.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fn.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://em.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://xt.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yg.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gx.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gm.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://tz.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://zt.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xl.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lk.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ba.shxzskj.cn

[D06] 数组长度
来源：http://dx.yuexingan06.cn

Py:   len(arr)
来源：http://cn.wgjwhj.cn

PHP:  count($arr);
来源：http://ku.shxzukj.cn

JS:   arr.length
来源：http://ni.chemitech.net.cn

TS:   arr.length
来源：http://hl.shtwfgs.cn

Java: list.size();
来源：http://qw.bookmarksfly.cn

Go:   len(arr)
来源：http://oa.newstarts.cn

Ruby: arr.length; arr.size
来源：http://mg.bjjhwx.cn

C#:   list.Count;
来源：http://he.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://me.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jl.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yo.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://qm.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://ml.9csxet.cn

Java: list.subList(1, 4);
来源：http://za.jctech888.com.cn

Go:   arr[1:4]
来源：http://pr.shxzukj.cn

Ruby: arr[1, 3]
来源：http://yx.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://yo.szxytkj.cn

[D08] 合并两个数组
来源：http://tg.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://yr.colortex.cn

PHP:  array_merge($a, $b);
来源：http://vy.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ep.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ph.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xb.yuexingan06.cn

Go:   append(a, b...)
来源：http://ak.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ft.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://um.shtwfgs.cn

[D09] 排序（升序）
来源：http://du.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://aq.huanxung.cn

PHP:  sort($arr);
来源：http://un.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://he.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ad.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hs.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wo.colortex.cn

Ruby: arr.sort
来源：http://vd.gzmigu.cn

C#:   list.Sort();
来源：http://pj.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ur.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://is.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jv.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zk.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ng.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dy.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ob.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vl.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mr.shxzukj.cn

[D11] 反转数组
来源：http://xo.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oe.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://wv.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dd.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://ym.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://yw.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://iq.nszjky.cn

Ruby: arr.reverse
来源：http://qe.gzmigu.cn

C#:   list.Reverse();
来源：http://zh.nszjky.cn

[D12] 查找元素下标
来源：http://za.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://qp.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cm.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://va.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ff.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xq.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://er.asd995.cn

Ruby: arr.index(x)
来源：http://ka.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://fi.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://ys.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qh.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pv.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://zq.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://cs.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dp.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uz.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ps.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rg.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://xo.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fl.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uz.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://ht.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://jc.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ql.521024.cn

Go:   // 手写循环
来源：http://hr.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pl.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xm.wgjwhj.cn

[D15] 去重
来源：http://nk.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zg.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://ma.huanxung.cn

JS:   [...new Set(arr)]
来源：http://ls.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://lm.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://is.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zi.asd995.cn

Ruby: arr.uniq
来源：http://oj.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://kc.nicolike.cn

[D16] 求和与平均值
来源：http://wz.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xg.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qq.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ex.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mh.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vr.haigaiapp.cn

Go:   // 手写循环累加
来源：http://mo.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nu.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://hg.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://ud.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://gv.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://mo.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jz.9csxet.cn

TS:   Math.max(...arr);
来源：http://qo.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bt.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sx.521024.cn

Ruby: arr.max;  arr.min
来源：http://oe.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://xa.521024.cn

[D18] 扁平化嵌套数组
来源：http://ct.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://og.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://db.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://me.asd995.cn

TS:   nested.flat();
来源：http://ir.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zv.haigaiapp.cn

Go:   // 手写双层循环
来源：http://qk.nicolike.cn

Ruby: nested.flatten
来源：http://bj.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ln.521024.cn

[D19] 按字段分组
来源：http://jm.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://le.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xe.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kh.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qy.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iy.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://kv.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yz.9csxet.cn


<!-- 参考信息 -->