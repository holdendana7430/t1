代发 wailian999

================================================================================
来源：http://zw.huixinmuqiang.cn

C. 函数与作用域
来源：http://vs.haigaiapp.cn

================================================================================
来源：http://nl.jianghongdianzi.cn

[C01] 定义函数
来源：http://tj.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://er.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ph.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://iy.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zp.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ed.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tb.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://co.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xx.huixiangedu.cn

[C02] 默认参数
来源：http://mt.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://dv.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lu.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ls.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ps.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ig.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oq.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://ms.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://ky.bookmarksfly.cn

[C03] 可变参数
来源：http://tj.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://ue.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lh.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jd.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bq.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yr.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yz.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aj.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yu.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://ky.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bg.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nw.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://me.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://on.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://rk.521024.cn

Go:   // 无：用配置结构体参数
来源：http://zc.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://tr.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://od.shtwfgs.cn

[C05] 返回多个值
来源：http://sl.newstarts.cn

Py:   return a, b
来源：http://ez.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://sw.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vr.shtwfgs.cn

TS:   return { a, b };
来源：http://ul.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qo.bookmarksfly.cn

Go:   return a, b
来源：http://ys.nszjky.cn

Ruby: return a, b
来源：http://og.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://yr.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://qg.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://cs.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ck.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://sl.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://wo.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tl.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gb.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://qd.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zt.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://ij.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ug.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qe.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xp.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://uu.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pw.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ed.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://dq.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xw.szsharing.cn

[C08] 闭包
来源：http://bj.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ni.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lq.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hx.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cm.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fw.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ht.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eu.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gg.chemitech.net.cn

[C09] 递归
来源：http://od.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://um.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kc.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ro.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cs.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rd.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bg.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qa.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://et.chemitech.net.cn

[C10] 变量作用域
来源：http://fc.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://id.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vk.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lw.muxihuayi.cn

TS:   同 JS
来源：http://ar.szxytkj.cn

Java: 方法内为块级作用域
来源：http://om.panjiajie.cn

Go:   花括号块级作用域
来源：http://ij.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bi.hnjuh.cn

C#:   块级作用域
来源：http://hs.521024.cn

[C11] 模块导入与导出
来源：http://dl.jianghongdianzi.cn

Py:   from module import func
来源：http://bp.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ce.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ba.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cj.haigaiapp.cn

Java: import java.util.List;
来源：http://sl.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ew.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://ur.521024.cn

C#:   using System.Text;
来源：http://nn.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://ka.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://bw.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://tx.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://bz.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://zg.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zd.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ay.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://os.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wg.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://ia.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rt.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vf.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tx.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qy.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ec.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://gv.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qh.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ty.lnxyls.cn

[C14] 泛型函数
来源：http://by.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xz.yuexingan06.cn

PHP:  // 无泛型
来源：http://ft.huixiangedu.cn

JS:   // 无泛型
来源：http://zz.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fe.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wm.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zx.wgjwhj.cn

Ruby: # 无泛型
来源：http://dg.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uy.colortex.cn

[C15] 解构 / 展开参数
来源：http://sl.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oc.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://fz.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hw.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ql.haigaiapp.cn

Java: // 无解构
来源：http://ti.colortex.cn

Go:   // 无解构
来源：http://kh.lnxyls.cn

Ruby: a, b = pair
来源：http://he.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://rv.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://py.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kb.yuntaijiaju.cn

PHP:  // 无重载
来源：http://av.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ns.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://sd.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kp.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://mb.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://pn.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ua.szsharing.cn

================================================================================
来源：http://jp.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://lb.9csxet.cn

================================================================================
来源：http://oy.nicolike.cn

[D01] 创建数组 / 列表
来源：http://pq.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ua.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bo.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qt.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ni.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://el.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://fk.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://zx.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qs.hahajie.cn

[D02] 追加元素到末尾
来源：http://in.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vu.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ut.521024.cn

JS:   arr.push(4);
来源：http://rv.huanxung.cn

TS:   arr.push(4);
来源：http://bx.huanxung.cn

Java: list.add(4);
来源：http://uq.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://pp.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://wx.shtwfgs.cn

C#:   list.Add(4);
来源：http://hd.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://ap.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://ck.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ya.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jx.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://px.szsharing.cn

Java: list.add(0, 0);
来源：http://ma.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zg.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ew.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://um.huixiangedu.cn

[D04] 删除元素
来源：http://zj.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mh.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cw.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://me.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://qt.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zo.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://se.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sx.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eo.hnjuh.cn

[D05] 访问与修改元素
来源：http://qx.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://is.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ck.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dh.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://vw.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://bd.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://ta.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jl.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kk.huixinmuqiang.cn

[D06] 数组长度
来源：http://iq.lnxyls.cn

Py:   len(arr)
来源：http://tg.muxihuayi.cn

PHP:  count($arr);
来源：http://vu.jianghongdianzi.cn

JS:   arr.length
来源：http://gh.shtwfgs.cn

TS:   arr.length
来源：http://gu.jctech888.com.cn

Java: list.size();
来源：http://ax.nicolike.cn

Go:   len(arr)
来源：http://vd.huanxung.cn

Ruby: arr.length; arr.size
来源：http://xo.szsharing.cn

C#:   list.Count;
来源：http://ij.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://jv.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cy.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ls.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://im.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://mm.huanxung.cn

Java: list.subList(1, 4);
来源：http://vm.yuexingan06.cn

Go:   arr[1:4]
来源：http://al.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://os.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://lc.bookmarksfly.cn

[D08] 合并两个数组
来源：http://yl.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://od.colortex.cn

PHP:  array_merge($a, $b);
来源：http://qx.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jm.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://tx.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qg.bjjhwx.cn

Go:   append(a, b...)
来源：http://wv.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://px.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://mo.hnjuh.cn

[D09] 排序（升序）
来源：http://in.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://yl.hahajie.cn

PHP:  sort($arr);
来源：http://om.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://it.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tv.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xb.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cd.jianghongdianzi.cn

Ruby: arr.sort
来源：http://ch.szxytkj.cn

C#:   list.Sort();
来源：http://dk.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uk.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uu.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://us.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ts.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bo.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nj.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uu.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ct.wgjwhj.cn

[D11] 反转数组
来源：http://yi.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wt.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://le.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oi.colortex.cn

TS:   [...arr].reverse();
来源：http://kz.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://nb.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://zy.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://hz.shtwfgs.cn

C#:   list.Reverse();
来源：http://sv.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://iw.521024.cn

Py:   arr.index(x);  x in arr
来源：http://em.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ok.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://as.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ti.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bf.521024.cn

Go:   slices.Index(arr, x)
来源：http://di.haigaiapp.cn

Ruby: arr.index(x)
来源：http://nh.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://gc.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://yv.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ez.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mu.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://cv.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://vn.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lz.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zc.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qg.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qi.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://db.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rh.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mw.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://be.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://eg.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://af.9csxet.cn

Go:   // 手写循环
来源：http://ho.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vn.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qm.muxihuayi.cn

[D15] 去重
来源：http://ht.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bo.9csxet.cn

PHP:  array_unique($arr);
来源：http://fa.nszjky.cn

JS:   [...new Set(arr)]
来源：http://sa.szsharing.cn

TS:   [...new Set(arr)]
来源：http://wi.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://so.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zp.9csxet.cn

Ruby: arr.uniq
来源：http://qa.colortex.cn

C#:   list.Distinct().ToList()
来源：http://vy.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://ma.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lw.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dp.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ec.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nm.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jv.gzmigu.cn

Go:   // 手写循环累加
来源：http://rs.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lz.521024.cn

C#:   list.Sum();  list.Average()
来源：http://sx.shxzskj.cn

[D17] 最大值与最小值
来源：http://ig.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://gm.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://pi.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://he.huanxung.cn

TS:   Math.max(...arr);
来源：http://mo.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qt.newstarts.cn


<!-- 参考信息 -->