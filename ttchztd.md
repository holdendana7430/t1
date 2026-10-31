代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://br.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hy.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lj.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kz.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zl.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ii.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://gy.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xl.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nl.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sn.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ps.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://hv.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://yg.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://vb.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://va.hnjuh.cn

[C05] 返回多个值
来源：http://vl.shxzskj.cn

Py:   return a, b
来源：http://ve.lnxyls.cn

PHP:  return [$a, $b];
来源：http://iz.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://em.haigaiapp.cn

TS:   return { a, b };
来源：http://hc.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kd.asd995.cn

Go:   return a, b
来源：http://dt.nicolike.cn

Ruby: return a, b
来源：http://ml.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://aa.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://au.szsharing.cn

Py:   square = lambda x: x * x
来源：http://kr.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ok.nszjky.cn

JS:   const square = x => x * x;
来源：http://el.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://fn.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jh.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rc.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://zh.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sa.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://az.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ad.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ho.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ks.colortex.cn

TS:   arr.map(String)
来源：http://cz.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wt.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ky.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://aj.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hq.hahajie.cn

[C08] 闭包
来源：http://af.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gm.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wr.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://if.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bz.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rx.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oh.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gm.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://av.haigaiapp.cn

[C09] 递归
来源：http://tt.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ve.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qp.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ij.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pr.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ca.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nb.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yd.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ss.asd995.cn

[C10] 变量作用域
来源：http://co.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qr.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ck.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://id.jctech888.com.cn

TS:   同 JS
来源：http://iz.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://um.szxytkj.cn

Go:   花括号块级作用域
来源：http://ac.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gg.nicolike.cn

C#:   块级作用域
来源：http://sr.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://uz.hahajie.cn

Py:   from module import func
来源：http://zw.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dz.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ae.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wg.colortex.cn

Java: import java.util.List;
来源：http://dh.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ap.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://bm.yuntaijiaju.cn

C#:   using System.Text;
来源：http://yf.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://aa.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://is.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://nz.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://rg.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://xc.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ve.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://xn.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://ey.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yh.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://pr.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://om.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hu.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sj.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bk.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://md.szxytkj.cn

Go:   func add(a, b int) int
来源：http://eg.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vf.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dq.muxihuayi.cn

[C14] 泛型函数
来源：http://ph.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pt.chemitech.net.cn

PHP:  // 无泛型
来源：http://bw.shxzukj.cn

JS:   // 无泛型
来源：http://ny.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xe.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ab.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wj.shtwfgs.cn

Ruby: # 无泛型
来源：http://lg.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uc.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://lu.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ss.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://dd.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ql.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nt.haigaiapp.cn

Java: // 无解构
来源：http://qp.yuntaijiaju.cn

Go:   // 无解构
来源：http://eu.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://hz.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://ob.hahajie.cn

[C16] 函数 / 方法重载
来源：http://oo.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dp.szxytkj.cn

PHP:  // 无重载
来源：http://dd.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tp.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://mm.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ix.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ee.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ul.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://us.chemitech.net.cn

================================================================================
来源：http://vv.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://at.lnxyls.cn

================================================================================
来源：http://fq.521024.cn

[D01] 创建数组 / 列表
来源：http://fr.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wx.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pr.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vh.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://re.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wd.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://wp.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://fq.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ou.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://ua.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vn.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ca.nicolike.cn

JS:   arr.push(4);
来源：http://de.yuexingan06.cn

TS:   arr.push(4);
来源：http://rw.shtwfgs.cn

Java: list.add(4);
来源：http://qy.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://hs.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://xy.jctech888.com.cn

C#:   list.Add(4);
来源：http://tp.colortex.cn

[D03] 在指定位置插入元素
来源：http://mo.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://kx.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cu.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oc.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://vl.shxzukj.cn

Java: list.add(0, 0);
来源：http://yy.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ct.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hh.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://uy.bookmarksfly.cn

[D04] 删除元素
来源：http://mt.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jt.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rk.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vr.colortex.cn

TS:   arr.splice(0, 1);
来源：http://yq.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fc.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qs.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bi.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://io.hnjuh.cn

[D05] 访问与修改元素
来源：http://ev.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://us.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vl.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tg.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://mz.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://xw.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://tw.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://du.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ck.wgjwhj.cn

[D06] 数组长度
来源：http://ba.gzmigu.cn

Py:   len(arr)
来源：http://bk.nszjky.cn

PHP:  count($arr);
来源：http://dc.newstarts.cn

JS:   arr.length
来源：http://vz.jianghongdianzi.cn

TS:   arr.length
来源：http://sm.shtwfgs.cn

Java: list.size();
来源：http://gi.bookmarksfly.cn

Go:   len(arr)
来源：http://jk.newstarts.cn

Ruby: arr.length; arr.size
来源：http://rl.shtwfgs.cn

C#:   list.Count;
来源：http://nn.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://wd.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gr.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vy.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://me.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://ty.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://qf.lnxyls.cn

Go:   arr[1:4]
来源：http://rb.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://ke.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://ws.muxihuayi.cn

[D08] 合并两个数组
来源：http://fn.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://vv.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://od.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iw.panjiajie.cn

TS:   [...a, ...b];
来源：http://us.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sj.haigaiapp.cn

Go:   append(a, b...)
来源：http://nb.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://jc.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://rm.haigaiapp.cn

[D09] 排序（升序）
来源：http://pe.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://dn.shtwfgs.cn

PHP:  sort($arr);
来源：http://jd.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lr.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zt.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tx.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qw.hnjuh.cn

Ruby: arr.sort
来源：http://sx.wgjwhj.cn

C#:   list.Sort();
来源：http://go.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wh.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xu.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://if.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://df.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sd.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tx.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ia.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zy.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gi.panjiajie.cn

[D11] 反转数组
来源：http://ua.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rv.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://xg.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://az.gzmigu.cn

TS:   [...arr].reverse();
来源：http://dz.nicolike.cn

Java: Collections.reverse(list);
来源：http://mo.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://ap.bookmarksfly.cn

Ruby: arr.reverse
来源：http://so.nicolike.cn

C#:   list.Reverse();
来源：http://eu.nicolike.cn

[D12] 查找元素下标
来源：http://vu.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://dg.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://no.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hu.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yw.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cb.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://ys.panjiajie.cn

Ruby: arr.index(x)
来源：http://tv.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://ld.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://gq.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lt.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ma.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://kn.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://ly.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yw.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ft.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wa.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bl.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://it.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rk.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ed.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://qm.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://ja.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oy.lnxyls.cn

Go:   // 手写循环
来源：http://ub.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mm.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cc.muxihuayi.cn

[D15] 去重
来源：http://ck.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eh.nszjky.cn

PHP:  array_unique($arr);
来源：http://kl.asd995.cn

JS:   [...new Set(arr)]
来源：http://li.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://nx.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://na.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xw.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://yr.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://fw.panjiajie.cn

[D16] 求和与平均值
来源：http://lf.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hp.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ad.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bh.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ya.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cl.panjiajie.cn

Go:   // 手写循环累加
来源：http://uv.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://my.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://qi.hnjuh.cn

[D17] 最大值与最小值
来源：http://qj.asd995.cn

Py:   max(arr);  min(arr)
来源：http://an.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://jp.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://si.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://nt.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gu.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nr.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://bz.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://yu.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://uc.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mr.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://yg.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tu.hnjuh.cn

TS:   nested.flat();
来源：http://ah.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://en.asd995.cn

Go:   // 手写双层循环
来源：http://uf.hahajie.cn

Ruby: nested.flatten
来源：http://cn.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jo.huixiangedu.cn

[D19] 按字段分组
来源：http://pb.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lj.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jl.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kt.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hu.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nv.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://kr.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aa.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zk.521024.cn

[D20] 统计每个元素出现次数
来源：http://be.nszjky.cn

Py:   Counter(arr)
来源：http://tb.9csxet.cn

PHP:  array_count_values($arr);
来源：http://fz.lnxyls.cn


<!-- 参考信息 -->