代发 wailian999

[C02] 默认参数
来源：http://tm.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://pl.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iv.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://ro.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dy.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oo.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zg.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://qk.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://vb.huixiangedu.cn

[C03] 可变参数
来源：http://qj.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://ju.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lk.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zm.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tl.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://su.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hg.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nv.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://av.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://og.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xw.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mj.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ip.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wc.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://dk.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://fm.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://up.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://jo.haigaiapp.cn

[C05] 返回多个值
来源：http://qp.shxzskj.cn

Py:   return a, b
来源：http://vw.gzmigu.cn

PHP:  return [$a, $b];
来源：http://sq.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vk.huixinmuqiang.cn

TS:   return { a, b };
来源：http://mp.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tb.nszjky.cn

Go:   return a, b
来源：http://oj.nszjky.cn

Ruby: return a, b
来源：http://zs.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://km.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://id.9csxet.cn

Py:   square = lambda x: x * x
来源：http://zn.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qz.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://bd.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://eg.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sj.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lu.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://pi.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://is.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://bx.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lo.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fd.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jn.huanxung.cn

TS:   arr.map(String)
来源：http://by.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qu.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bc.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://ah.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pm.521024.cn

[C08] 闭包
来源：http://zo.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://of.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rt.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xs.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lq.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yo.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ow.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rk.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yb.hahajie.cn

[C09] 递归
来源：http://ro.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ei.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vq.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eh.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ca.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hu.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kx.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wa.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yt.haigaiapp.cn

[C10] 变量作用域
来源：http://qa.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yf.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://br.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hg.hnjuh.cn

TS:   同 JS
来源：http://rh.hnjuh.cn

Java: 方法内为块级作用域
来源：http://lp.shxzukj.cn

Go:   花括号块级作用域
来源：http://rz.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gw.colortex.cn

C#:   块级作用域
来源：http://av.bjjhwx.cn

[C11] 模块导入与导出
来源：http://ex.jianghongdianzi.cn

Py:   from module import func
来源：http://mw.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ai.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gy.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cd.szxytkj.cn

Java: import java.util.List;
来源：http://on.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ws.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://ow.jianghongdianzi.cn

C#:   using System.Text;
来源：http://li.521024.cn

[C12] 立即执行函数 IIFE
来源：http://nk.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://wl.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://fg.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://hp.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://gn.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bg.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://qh.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://fe.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vx.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://ho.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kf.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ed.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jj.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ws.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vi.shxzskj.cn

Go:   func add(a, b int) int
来源：http://ce.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gh.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nb.jctech888.com.cn

[C14] 泛型函数
来源：http://yd.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cc.wgjwhj.cn

PHP:  // 无泛型
来源：http://bh.jctech888.com.cn

JS:   // 无泛型
来源：http://pd.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oe.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bh.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ki.haigaiapp.cn

Ruby: # 无泛型
来源：http://gu.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zu.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://nl.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ju.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://pq.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uk.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vq.yuexingan06.cn

Java: // 无解构
来源：http://an.asd995.cn

Go:   // 无解构
来源：http://wm.bookmarksfly.cn

Ruby: a, b = pair
来源：http://qv.hahajie.cn

C#:   var (a, b) = pair;
来源：http://xy.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://rf.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gw.panjiajie.cn

PHP:  // 无重载
来源：http://ax.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lw.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://pp.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jx.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://mi.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://sr.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://le.chemitech.net.cn

================================================================================
来源：http://bx.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://wk.szsharing.cn

================================================================================
来源：http://eh.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://ou.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hw.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ow.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fy.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bl.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ih.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://id.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://rz.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yc.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://ze.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mi.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sm.lnxyls.cn

JS:   arr.push(4);
来源：http://tm.lnxyls.cn

TS:   arr.push(4);
来源：http://xi.asd995.cn

Java: list.add(4);
来源：http://tx.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://sk.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://pg.wgjwhj.cn

C#:   list.Add(4);
来源：http://vk.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://ou.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://yf.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yj.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zo.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://jv.lnxyls.cn

Java: list.add(0, 0);
来源：http://oi.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ly.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vp.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://tf.hnjuh.cn

[D04] 删除元素
来源：http://hv.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nz.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mc.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ld.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://ga.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://js.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ry.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oc.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ip.huanxung.cn

[D05] 访问与修改元素
来源：http://ne.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fv.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://md.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qa.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://af.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://nv.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://lb.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vg.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rx.nicolike.cn

[D06] 数组长度
来源：http://hy.nicolike.cn

Py:   len(arr)
来源：http://ov.hnjuh.cn

PHP:  count($arr);
来源：http://ih.hnjuh.cn

JS:   arr.length
来源：http://zy.yuexingan06.cn

TS:   arr.length
来源：http://rx.wgjwhj.cn

Java: list.size();
来源：http://lk.huixinmuqiang.cn

Go:   len(arr)
来源：http://fu.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://hx.haigaiapp.cn

C#:   list.Count;
来源：http://qn.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://ig.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dm.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dn.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://cg.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://lb.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://cx.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://su.asd995.cn

Ruby: arr[1, 3]
来源：http://hz.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://ix.muxihuayi.cn

[D08] 合并两个数组
来源：http://ya.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://vc.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://tl.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kc.newstarts.cn

TS:   [...a, ...b];
来源：http://to.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rj.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://tz.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://kt.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://ic.wgjwhj.cn

[D09] 排序（升序）
来源：http://yu.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://qm.nicolike.cn

PHP:  sort($arr);
来源：http://lm.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tb.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gw.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ci.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gi.panjiajie.cn

Ruby: arr.sort
来源：http://uu.nszjky.cn

C#:   list.Sort();
来源：http://gj.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zg.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gg.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pt.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ds.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ou.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dg.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ii.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pm.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mt.shxzukj.cn

[D11] 反转数组
来源：http://wv.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://no.nszjky.cn

PHP:  array_reverse($arr);
来源：http://rv.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://px.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://xv.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://en.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://cv.jctech888.com.cn

Ruby: arr.reverse
来源：http://kd.hahajie.cn

C#:   list.Reverse();
来源：http://tg.jctech888.com.cn

[D12] 查找元素下标
来源：http://lx.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://tp.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ze.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://er.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fy.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gg.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://rn.asd995.cn

Ruby: arr.index(x)
来源：http://io.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://ra.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://dp.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xe.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fw.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://tk.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://cw.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yn.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qk.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://km.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cb.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://mc.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pt.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ly.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://zn.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://db.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yo.yuexingan06.cn

Go:   // 手写循环
来源：http://fb.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hl.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cr.colortex.cn

[D15] 去重
来源：http://oq.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tz.nicolike.cn

PHP:  array_unique($arr);
来源：http://iz.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://gw.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://xs.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rn.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ee.muxihuayi.cn

Ruby: arr.uniq
来源：http://nf.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://in.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://rs.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yq.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ww.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wc.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dz.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lm.asd995.cn

Go:   // 手写循环累加
来源：http://jc.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zm.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://ss.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ij.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://sf.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ly.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bo.hahajie.cn

TS:   Math.max(...arr);
来源：http://kx.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rq.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wd.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://nz.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://mz.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://kl.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yw.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://nh.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uv.panjiajie.cn

TS:   nested.flat();
来源：http://lg.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pq.nicolike.cn

Go:   // 手写双层循环
来源：http://sc.muxihuayi.cn

Ruby: nested.flatten
来源：http://vw.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mj.huanxung.cn


<!-- 参考信息 -->