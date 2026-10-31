代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xx.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ah.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ri.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ha.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://no.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tb.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://al.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://er.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ip.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sw.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ag.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://hk.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://bm.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://pm.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://vd.jianghongdianzi.cn

[C05] 返回多个值
来源：http://fh.bookmarksfly.cn

Py:   return a, b
来源：http://ia.gzmigu.cn

PHP:  return [$a, $b];
来源：http://on.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://io.shxzukj.cn

TS:   return { a, b };
来源：http://js.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hd.nszjky.cn

Go:   return a, b
来源：http://vj.huanxung.cn

Ruby: return a, b
来源：http://hi.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ql.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://od.hahajie.cn

Py:   square = lambda x: x * x
来源：http://cp.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ze.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://ya.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://wb.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ir.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ew.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://ty.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yb.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://ny.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pu.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://su.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gw.521024.cn

TS:   arr.map(String)
来源：http://vq.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sm.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uu.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://sk.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jw.chemitech.net.cn

[C08] 闭包
来源：http://lx.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://he.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xa.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eu.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wl.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ia.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mq.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ns.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://di.asd995.cn

[C09] 递归
来源：http://ee.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tc.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sz.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ww.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mq.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://st.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hp.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fw.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sx.wgjwhj.cn

[C10] 变量作用域
来源：http://dn.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ma.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pf.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bn.bookmarksfly.cn

TS:   同 JS
来源：http://jk.hahajie.cn

Java: 方法内为块级作用域
来源：http://ct.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://di.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cx.jctech888.com.cn

C#:   块级作用域
来源：http://dp.newstarts.cn

[C11] 模块导入与导出
来源：http://zo.chemitech.net.cn

Py:   from module import func
来源：http://bn.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yc.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lw.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ow.lnxyls.cn

Java: import java.util.List;
来源：http://zj.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lq.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://mj.szxytkj.cn

C#:   using System.Text;
来源：http://yv.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://ao.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://mn.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://bk.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://ac.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://al.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qd.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ao.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://ne.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ct.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://do.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aj.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dy.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nk.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sk.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yt.szxytkj.cn

Go:   func add(a, b int) int
来源：http://kj.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rm.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ap.newstarts.cn

[C14] 泛型函数
来源：http://kq.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://io.shxzskj.cn

PHP:  // 无泛型
来源：http://hm.wgjwhj.cn

JS:   // 无泛型
来源：http://tn.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ca.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pt.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cl.gzmigu.cn

Ruby: # 无泛型
来源：http://df.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wq.hahajie.cn

[C15] 解构 / 展开参数
来源：http://nf.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dl.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://fm.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yp.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mz.shxzskj.cn

Java: // 无解构
来源：http://vr.colortex.cn

Go:   // 无解构
来源：http://bf.szsharing.cn

Ruby: a, b = pair
来源：http://sp.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://av.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://sp.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jw.lnxyls.cn

PHP:  // 无重载
来源：http://ky.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ua.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://zf.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uf.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://vm.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://bd.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ar.szxytkj.cn

================================================================================
来源：http://kp.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://tx.szxytkj.cn

================================================================================
来源：http://wl.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://uk.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pt.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tx.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uw.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://og.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vz.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ey.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://il.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gh.gzmigu.cn

[D02] 追加元素到末尾
来源：http://zv.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nv.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tc.muxihuayi.cn

JS:   arr.push(4);
来源：http://vz.huanxung.cn

TS:   arr.push(4);
来源：http://ze.shtwfgs.cn

Java: list.add(4);
来源：http://uz.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://kr.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://kj.521024.cn

C#:   list.Add(4);
来源：http://ts.newstarts.cn

[D03] 在指定位置插入元素
来源：http://pt.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://bf.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xf.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ca.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://ns.newstarts.cn

Java: list.add(0, 0);
来源：http://gh.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pa.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jm.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://oa.wgjwhj.cn

[D04] 删除元素
来源：http://eg.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sc.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fu.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vl.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://is.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yf.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vl.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aw.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lf.nszjky.cn

[D05] 访问与修改元素
来源：http://xd.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cx.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zv.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xt.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://ov.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://kn.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://dz.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://er.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ff.huixiangedu.cn

[D06] 数组长度
来源：http://on.muxihuayi.cn

Py:   len(arr)
来源：http://hn.gzmigu.cn

PHP:  count($arr);
来源：http://rr.hahajie.cn

JS:   arr.length
来源：http://gs.szsharing.cn

TS:   arr.length
来源：http://ct.panjiajie.cn

Java: list.size();
来源：http://um.huanxung.cn

Go:   len(arr)
来源：http://wj.9csxet.cn

Ruby: arr.length; arr.size
来源：http://ys.shxzskj.cn

C#:   list.Count;
来源：http://sk.colortex.cn

[D07] 切片 / 取子数组
来源：http://ix.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vb.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zv.521024.cn

JS:   arr.slice(1, 4);
来源：http://kq.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://jk.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://hy.huanxung.cn

Go:   arr[1:4]
来源：http://qt.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://sn.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://ti.huanxung.cn

[D08] 合并两个数组
来源：http://uc.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://pi.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://dq.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dj.colortex.cn

TS:   [...a, ...b];
来源：http://zm.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pz.bjjhwx.cn

Go:   append(a, b...)
来源：http://xz.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://yk.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://ir.shxzukj.cn

[D09] 排序（升序）
来源：http://ek.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://qp.shxzukj.cn

PHP:  sort($arr);
来源：http://ni.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qu.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ni.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tv.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uh.haigaiapp.cn

Ruby: arr.sort
来源：http://ib.yuntaijiaju.cn

C#:   list.Sort();
来源：http://pv.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qg.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zs.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uf.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vm.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aj.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vj.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wb.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ea.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://md.colortex.cn

[D11] 反转数组
来源：http://ps.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gd.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://it.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uh.nicolike.cn

TS:   [...arr].reverse();
来源：http://pu.hahajie.cn

Java: Collections.reverse(list);
来源：http://db.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://bq.521024.cn

Ruby: arr.reverse
来源：http://ck.yuexingan06.cn

C#:   list.Reverse();
来源：http://kv.newstarts.cn

[D12] 查找元素下标
来源：http://ob.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://so.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yb.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gs.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://db.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eu.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://nn.colortex.cn

Ruby: arr.index(x)
来源：http://lx.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://ce.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://qb.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hx.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tb.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://sn.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://wm.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://du.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nu.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vf.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://es.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://hk.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qt.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kn.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://sl.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://zn.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://td.hnjuh.cn

Go:   // 手写循环
来源：http://xx.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lo.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dv.jctech888.com.cn

[D15] 去重
来源：http://wh.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yv.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ij.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://ke.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://en.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fz.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://il.lnxyls.cn

Ruby: arr.uniq
来源：http://lp.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://fi.huanxung.cn

[D16] 求和与平均值
来源：http://ve.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ip.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://an.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wq.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mg.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yt.asd995.cn

Go:   // 手写循环累加
来源：http://um.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dk.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://xb.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://lm.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://sk.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://mb.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xu.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://ox.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pn.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dq.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://xk.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://jz.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://fs.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://us.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://kx.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hh.521024.cn

TS:   nested.flat();
来源：http://rx.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ql.hahajie.cn

Go:   // 手写双层循环
来源：http://qv.huixiangedu.cn

Ruby: nested.flatten
来源：http://gb.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bk.shxzukj.cn

[D19] 按字段分组
来源：http://ob.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hs.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yq.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eh.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ee.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iz.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://ft.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tm.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kb.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://qo.yuexingan06.cn

Py:   Counter(arr)
来源：http://th.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://zv.gzmigu.cn


<!-- 参考信息 -->