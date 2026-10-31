代发 wailian999

Py:   if not data: return
来源：http://qy.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://zs.haigaiapp.cn

JS:   if (!data) return;
来源：http://le.jctech888.com.cn

TS:   if (!data) return;
来源：http://oh.bjjhwx.cn

Java: if (data == null) return;
来源：http://hw.muxihuayi.cn

Go:   if data == nil { return }
来源：http://ya.shxzukj.cn

Ruby: return if data.nil?
来源：http://lo.gzmigu.cn

C#:   if (data == null) return;
来源：http://kf.yuexingan06.cn

================================================================================
来源：http://dz.huanxung.cn

C. 函数与作用域
来源：http://cl.colortex.cn

================================================================================
来源：http://ns.haigaiapp.cn

[C01] 定义函数
来源：http://ad.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://ff.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eq.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://sl.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pn.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://us.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cz.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://vk.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wq.hnjuh.cn

[C02] 默认参数
来源：http://bp.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://wr.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://al.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://kl.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ce.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uk.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://at.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://nw.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://oo.shxzukj.cn

[C03] 可变参数
来源：http://gw.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://sl.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ey.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qk.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eb.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vc.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bd.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oo.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yj.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://vq.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fm.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fj.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rr.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bq.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://pg.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://zp.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://iu.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://ve.jianghongdianzi.cn

[C05] 返回多个值
来源：http://tg.gzmigu.cn

Py:   return a, b
来源：http://lw.panjiajie.cn

PHP:  return [$a, $b];
来源：http://pm.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ol.shxzukj.cn

TS:   return { a, b };
来源：http://kn.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hi.bookmarksfly.cn

Go:   return a, b
来源：http://qz.shxzukj.cn

Ruby: return a, b
来源：http://nn.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://xc.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://xv.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://qh.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bn.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://dh.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://rx.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rn.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nx.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://rb.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fv.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://el.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qw.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://md.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ja.bookmarksfly.cn

TS:   arr.map(String)
来源：http://vk.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://of.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sy.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://il.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xq.nszjky.cn

[C08] 闭包
来源：http://do.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zd.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xc.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ym.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fy.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oc.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lm.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ly.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xt.jctech888.com.cn

[C09] 递归
来源：http://ot.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sb.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aw.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ps.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bh.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pi.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mj.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ao.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lz.bookmarksfly.cn

[C10] 变量作用域
来源：http://jw.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ve.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ub.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qi.bookmarksfly.cn

TS:   同 JS
来源：http://ec.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://it.huixiangedu.cn

Go:   花括号块级作用域
来源：http://nu.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gj.muxihuayi.cn

C#:   块级作用域
来源：http://us.wgjwhj.cn

[C11] 模块导入与导出
来源：http://ul.shxzskj.cn

Py:   from module import func
来源：http://wc.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cy.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sv.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wp.chemitech.net.cn

Java: import java.util.List;
来源：http://qm.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ed.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://qe.colortex.cn

C#:   using System.Text;
来源：http://gx.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://wk.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://hb.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://ck.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://id.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ul.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hm.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://jt.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://rt.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lh.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://lr.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ut.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vh.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vx.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ri.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xy.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://fe.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ur.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lg.chemitech.net.cn

[C14] 泛型函数
来源：http://an.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ut.huixiangedu.cn

PHP:  // 无泛型
来源：http://cv.szsharing.cn

JS:   // 无泛型
来源：http://tt.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ia.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://li.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xm.szsharing.cn

Ruby: # 无泛型
来源：http://ac.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hd.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://rr.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ti.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://bt.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nf.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tm.haigaiapp.cn

Java: // 无解构
来源：http://cl.yuntaijiaju.cn

Go:   // 无解构
来源：http://bx.panjiajie.cn

Ruby: a, b = pair
来源：http://dh.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://sq.nicolike.cn

[C16] 函数 / 方法重载
来源：http://bh.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aj.jianghongdianzi.cn

PHP:  // 无重载
来源：http://mr.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jp.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://bl.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ek.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://kb.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://ty.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ds.szsharing.cn

================================================================================
来源：http://ex.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://jg.asd995.cn

================================================================================
来源：http://ws.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://qp.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://al.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dk.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aj.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ds.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mr.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://qi.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://zy.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sc.nszjky.cn

[D02] 追加元素到末尾
来源：http://vi.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rb.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rf.gzmigu.cn

JS:   arr.push(4);
来源：http://ie.lnxyls.cn

TS:   arr.push(4);
来源：http://xk.huixinmuqiang.cn

Java: list.add(4);
来源：http://hq.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://wq.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://oy.colortex.cn

C#:   list.Add(4);
来源：http://cx.asd995.cn

[D03] 在指定位置插入元素
来源：http://pf.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://oo.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vt.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mo.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://vx.gzmigu.cn

Java: list.add(0, 0);
来源：http://nk.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ve.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fn.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://ib.9csxet.cn

[D04] 删除元素
来源：http://cb.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fb.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://of.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fg.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://hy.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qr.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zh.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xb.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qt.yuexingan06.cn

[D05] 访问与修改元素
来源：http://de.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oe.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ml.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://to.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://jz.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://ru.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ai.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vy.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pk.bjjhwx.cn

[D06] 数组长度
来源：http://ki.shxzskj.cn

Py:   len(arr)
来源：http://mv.shtwfgs.cn

PHP:  count($arr);
来源：http://sw.nicolike.cn

JS:   arr.length
来源：http://ta.bookmarksfly.cn

TS:   arr.length
来源：http://ao.521024.cn

Java: list.size();
来源：http://cs.shxzukj.cn

Go:   len(arr)
来源：http://ia.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://gm.wgjwhj.cn

C#:   list.Count;
来源：http://fn.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://eu.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wx.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://al.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://gu.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://rc.colortex.cn

Java: list.subList(1, 4);
来源：http://et.colortex.cn

Go:   arr[1:4]
来源：http://ys.newstarts.cn

Ruby: arr[1, 3]
来源：http://vi.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://qx.shxzukj.cn

[D08] 合并两个数组
来源：http://ws.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://bn.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://rg.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ua.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://cp.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iq.muxihuayi.cn

Go:   append(a, b...)
来源：http://ej.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://mz.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://vr.wgjwhj.cn

[D09] 排序（升序）
来源：http://ir.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://vg.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://rf.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pw.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qz.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hi.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hi.szxytkj.cn

Ruby: arr.sort
来源：http://xd.muxihuayi.cn

C#:   list.Sort();
来源：http://oa.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tr.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cs.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xk.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gz.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tm.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vt.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pe.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rf.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gm.newstarts.cn

[D11] 反转数组
来源：http://hz.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vu.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://nq.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://no.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://cl.nicolike.cn

Java: Collections.reverse(list);
来源：http://ws.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://ut.muxihuayi.cn

Ruby: arr.reverse
来源：http://kt.shxzukj.cn

C#:   list.Reverse();
来源：http://ok.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://bj.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://jw.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oy.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sl.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pm.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mk.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://mv.asd995.cn

Ruby: arr.index(x)
来源：http://ee.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://dv.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://yy.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://am.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ml.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://gz.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://bz.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sw.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://un.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vw.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://og.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pr.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ym.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://et.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://ka.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dd.muxihuayi.cn

Go:   // 手写循环
来源：http://dl.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jj.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bs.chemitech.net.cn

[D15] 去重
来源：http://by.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sp.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://og.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://mr.huanxung.cn

TS:   [...new Set(arr)]
来源：http://rp.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ur.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://og.huixiangedu.cn

Ruby: arr.uniq
来源：http://kc.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://kc.huixiangedu.cn

[D16] 求和与平均值
来源：http://oz.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tv.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ek.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cq.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dz.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yb.szxytkj.cn

Go:   // 手写循环累加
来源：http://kz.yuexingan06.cn


<!-- 参考信息 -->