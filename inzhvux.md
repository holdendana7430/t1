代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://nz.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gz.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hd.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://mw.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://cd.jctech888.com.cn

[C03] 可变参数
来源：http://vm.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://eq.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mu.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lh.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jx.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wq.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hx.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vi.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dy.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://cr.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gk.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://di.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://av.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lj.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://hi.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://ks.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://cf.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://xk.chemitech.net.cn

[C05] 返回多个值
来源：http://kg.huixinmuqiang.cn

Py:   return a, b
来源：http://sm.szxytkj.cn

PHP:  return [$a, $b];
来源：http://vn.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cs.newstarts.cn

TS:   return { a, b };
来源：http://rq.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hw.gzmigu.cn

Go:   return a, b
来源：http://ba.asd995.cn

Ruby: return a, b
来源：http://fl.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://kx.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://mz.colortex.cn

Py:   square = lambda x: x * x
来源：http://nc.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ye.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://rc.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://fb.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tm.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cn.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://ib.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lu.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://lx.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kf.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nq.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wy.panjiajie.cn

TS:   arr.map(String)
来源：http://py.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hh.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pt.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://nr.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nx.chemitech.net.cn

[C08] 闭包
来源：http://nc.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ox.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ii.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tv.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ns.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pq.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ai.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lb.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://px.521024.cn

[C09] 递归
来源：http://mw.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rs.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lc.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hd.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nd.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ag.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vn.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://am.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zp.shtwfgs.cn

[C10] 变量作用域
来源：http://ta.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rt.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vg.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ic.bjjhwx.cn

TS:   同 JS
来源：http://eb.lnxyls.cn

Java: 方法内为块级作用域
来源：http://em.bjjhwx.cn

Go:   花括号块级作用域
来源：http://cs.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ji.hnjuh.cn

C#:   块级作用域
来源：http://bh.lnxyls.cn

[C11] 模块导入与导出
来源：http://hb.szxytkj.cn

Py:   from module import func
来源：http://vz.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wg.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://op.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ec.szxytkj.cn

Java: import java.util.List;
来源：http://qy.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wy.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://ls.newstarts.cn

C#:   using System.Text;
来源：http://fi.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://vt.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://ir.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://ys.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://yn.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://ts.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eg.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://rr.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://wj.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://en.521024.cn

[C13] 类型声明 / 类型注解
来源：http://ah.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ff.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gj.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kk.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qy.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ii.huanxung.cn

Go:   func add(a, b int) int
来源：http://bd.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bu.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ok.lnxyls.cn

[C14] 泛型函数
来源：http://nk.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uv.9csxet.cn

PHP:  // 无泛型
来源：http://mu.521024.cn

JS:   // 无泛型
来源：http://pk.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qv.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oj.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kq.wgjwhj.cn

Ruby: # 无泛型
来源：http://om.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qv.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://cc.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ut.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://zs.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lt.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mr.jctech888.com.cn

Java: // 无解构
来源：http://wq.bookmarksfly.cn

Go:   // 无解构
来源：http://cs.newstarts.cn

Ruby: a, b = pair
来源：http://ec.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://ku.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://gd.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pj.yuexingan06.cn

PHP:  // 无重载
来源：http://cj.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zc.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://iq.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://co.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://ae.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://ci.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iy.huanxung.cn

================================================================================
来源：http://up.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://bg.gzmigu.cn

================================================================================
来源：http://bb.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://vw.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kp.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qo.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://du.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bi.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mj.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://jn.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://lp.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xq.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://wn.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aj.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rj.yuexingan06.cn

JS:   arr.push(4);
来源：http://dz.nicolike.cn

TS:   arr.push(4);
来源：http://uz.yuntaijiaju.cn

Java: list.add(4);
来源：http://dx.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://pg.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://js.hnjuh.cn

C#:   list.Add(4);
来源：http://vr.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://mh.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://fo.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ka.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ca.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://ow.shxzskj.cn

Java: list.add(0, 0);
来源：http://nr.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yn.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sd.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://fn.hahajie.cn

[D04] 删除元素
来源：http://ur.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nw.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jc.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ku.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://yp.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eu.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xs.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fp.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vb.szsharing.cn

[D05] 访问与修改元素
来源：http://ar.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ob.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://my.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ky.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://dy.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://wl.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://hc.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bn.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qk.yuntaijiaju.cn

[D06] 数组长度
来源：http://am.shxzskj.cn

Py:   len(arr)
来源：http://xs.haigaiapp.cn

PHP:  count($arr);
来源：http://uw.panjiajie.cn

JS:   arr.length
来源：http://yy.nicolike.cn

TS:   arr.length
来源：http://rh.chemitech.net.cn

Java: list.size();
来源：http://ua.asd995.cn

Go:   len(arr)
来源：http://kt.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://lq.panjiajie.cn

C#:   list.Count;
来源：http://hv.szsharing.cn

[D07] 切片 / 取子数组
来源：http://lg.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tr.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jz.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://ze.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://jv.colortex.cn

Java: list.subList(1, 4);
来源：http://sq.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://iq.nszjky.cn

Ruby: arr[1, 3]
来源：http://bc.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://hn.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://jg.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://pp.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://il.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fw.szsharing.cn

TS:   [...a, ...b];
来源：http://yu.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gk.asd995.cn

Go:   append(a, b...)
来源：http://kr.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://cr.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://ag.shtwfgs.cn

[D09] 排序（升序）
来源：http://rb.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://lr.shxzskj.cn

PHP:  sort($arr);
来源：http://um.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ru.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kb.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ep.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zm.shxzskj.cn

Ruby: arr.sort
来源：http://kg.huixiangedu.cn

C#:   list.Sort();
来源：http://oq.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hg.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sx.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xo.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qw.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://br.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nd.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://re.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://on.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kp.nicolike.cn

[D11] 反转数组
来源：http://fw.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lq.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://yv.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sn.nicolike.cn

TS:   [...arr].reverse();
来源：http://qk.szxytkj.cn

Java: Collections.reverse(list);
来源：http://yt.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://fj.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://gb.newstarts.cn

C#:   list.Reverse();
来源：http://cj.huixiangedu.cn

[D12] 查找元素下标
来源：http://av.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://ay.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://by.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qz.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://og.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xb.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://jn.shtwfgs.cn

Ruby: arr.index(x)
来源：http://vm.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://wv.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://zo.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://im.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fw.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://qx.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://js.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ib.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://af.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pt.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hb.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://vf.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mj.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lm.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://gr.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://im.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gn.colortex.cn

Go:   // 手写循环
来源：http://jl.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gq.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xu.yuntaijiaju.cn

[D15] 去重
来源：http://bk.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://em.szxytkj.cn

PHP:  array_unique($arr);
来源：http://up.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://ul.9csxet.cn

TS:   [...new Set(arr)]
来源：http://ia.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qy.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yv.panjiajie.cn

Ruby: arr.uniq
来源：http://bj.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://dg.muxihuayi.cn

[D16] 求和与平均值
来源：http://hv.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yk.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qf.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ni.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ir.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xj.lnxyls.cn

Go:   // 手写循环累加
来源：http://bu.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ol.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://wu.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ij.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://wp.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ie.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ao.newstarts.cn

TS:   Math.max(...arr);
来源：http://va.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eq.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ca.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://iy.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://hu.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://ss.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qa.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://ji.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ow.wgjwhj.cn

TS:   nested.flat();
来源：http://wi.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xj.chemitech.net.cn

Go:   // 手写双层循环
来源：http://mp.wgjwhj.cn

Ruby: nested.flatten
来源：http://cd.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zd.lnxyls.cn

[D19] 按字段分组
来源：http://sd.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ms.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xv.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mg.shxzskj.cn


<!-- 参考信息 -->