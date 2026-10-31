代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://pf.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vv.hnjuh.cn

[B15] 布尔运算与取反
来源：http://zy.yuntaijiaju.cn

Py:   a and b or not c
来源：http://bp.nicolike.cn

PHP:  $a && $b || !$c
来源：http://wu.chemitech.net.cn

JS:   a && b || !c
来源：http://cd.jianghongdianzi.cn

TS:   a && b || !c
来源：http://zc.asd995.cn

Java: a && b || !c
来源：http://fb.yuntaijiaju.cn

Go:   a && b || !c
来源：http://ty.muxihuayi.cn

Ruby: a && b || !c
来源：http://vf.wgjwhj.cn

C#:   a && b || !c
来源：http://bf.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tq.bookmarksfly.cn

Py:   if not data: return
来源：http://kg.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://td.lnxyls.cn

JS:   if (!data) return;
来源：http://mx.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://ax.bookmarksfly.cn

Java: if (data == null) return;
来源：http://df.bjjhwx.cn

Go:   if data == nil { return }
来源：http://eo.shtwfgs.cn

Ruby: return if data.nil?
来源：http://zd.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://pw.hahajie.cn

================================================================================
来源：http://qq.haigaiapp.cn

C. 函数与作用域
来源：http://wh.colortex.cn

================================================================================
来源：http://ch.nicolike.cn

[C01] 定义函数
来源：http://jj.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://uj.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oh.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://dv.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://th.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hk.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zn.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://mo.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ql.9csxet.cn

[C02] 默认参数
来源：http://iw.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://lw.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wt.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://oz.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fn.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ro.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hc.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://yk.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ed.9csxet.cn

[C03] 可变参数
来源：http://sy.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://bb.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gw.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://in.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ix.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sz.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rh.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yr.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ds.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://gi.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vw.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://au.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ik.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fx.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://cr.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://gf.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://lb.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://cp.szsharing.cn

[C05] 返回多个值
来源：http://sq.haigaiapp.cn

Py:   return a, b
来源：http://xb.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://wo.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bt.asd995.cn

TS:   return { a, b };
来源：http://lh.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ns.shtwfgs.cn

Go:   return a, b
来源：http://hg.szxytkj.cn

Ruby: return a, b
来源：http://an.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://lb.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://xm.newstarts.cn

Py:   square = lambda x: x * x
来源：http://kh.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jv.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://rx.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://wq.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://te.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://du.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://pr.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://em.hahajie.cn

[C07] 把函数作为参数传入
来源：http://jl.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xp.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rj.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hq.bookmarksfly.cn

TS:   arr.map(String)
来源：http://kz.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ub.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mr.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://cw.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qz.nszjky.cn

[C08] 闭包
来源：http://yp.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nu.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vv.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qh.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mt.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uu.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jz.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fn.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://em.wgjwhj.cn

[C09] 递归
来源：http://on.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iw.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sy.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tp.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ph.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yl.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qo.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rf.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ah.shtwfgs.cn

[C10] 变量作用域
来源：http://oe.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xn.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jf.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vn.bjjhwx.cn

TS:   同 JS
来源：http://ot.hnjuh.cn

Java: 方法内为块级作用域
来源：http://kh.gzmigu.cn

Go:   花括号块级作用域
来源：http://db.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ig.asd995.cn

C#:   块级作用域
来源：http://nb.gzmigu.cn

[C11] 模块导入与导出
来源：http://gm.newstarts.cn

Py:   from module import func
来源：http://ul.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nt.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vr.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fa.lnxyls.cn

Java: import java.util.List;
来源：http://xq.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fe.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://je.szsharing.cn

C#:   using System.Text;
来源：http://lo.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://nv.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://zp.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://qj.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://ox.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://gq.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ks.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://ny.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://ws.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iw.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://tu.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rl.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xq.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qp.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xr.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uy.huanxung.cn

Go:   func add(a, b int) int
来源：http://gc.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://un.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xc.bookmarksfly.cn

[C14] 泛型函数
来源：http://mo.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.colortex.cn

PHP:  // 无泛型
来源：http://rb.newstarts.cn

JS:   // 无泛型
来源：http://qy.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ku.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kq.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dw.panjiajie.cn

Ruby: # 无泛型
来源：http://zf.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bb.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://qw.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lp.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://ig.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ki.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zb.9csxet.cn

Java: // 无解构
来源：http://sf.jianghongdianzi.cn

Go:   // 无解构
来源：http://pv.shtwfgs.cn

Ruby: a, b = pair
来源：http://wf.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://za.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://xe.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pa.newstarts.cn

PHP:  // 无重载
来源：http://qg.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ru.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://iz.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://se.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://ty.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://po.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xb.lnxyls.cn

================================================================================
来源：http://hn.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://em.hnjuh.cn

================================================================================
来源：http://hu.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://df.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hr.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rh.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nr.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ic.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qg.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://px.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://yj.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fl.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://jc.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yc.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hd.lnxyls.cn

JS:   arr.push(4);
来源：http://dt.muxihuayi.cn

TS:   arr.push(4);
来源：http://il.9csxet.cn

Java: list.add(4);
来源：http://em.521024.cn

Go:   arr = append(arr, 4)
来源：http://zb.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://wc.shxzskj.cn

C#:   list.Add(4);
来源：http://fm.9csxet.cn

[D03] 在指定位置插入元素
来源：http://fe.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://ih.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://da.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wl.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://te.shxzskj.cn

Java: list.add(0, 0);
来源：http://vq.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://si.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ii.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://lt.bookmarksfly.cn

[D04] 删除元素
来源：http://ac.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ef.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://au.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jz.asd995.cn

TS:   arr.splice(0, 1);
来源：http://au.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pi.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vq.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gk.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gl.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://ok.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qq.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oq.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://av.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://xg.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://cc.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://uy.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ud.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lv.521024.cn

[D06] 数组长度
来源：http://bh.hahajie.cn

Py:   len(arr)
来源：http://lq.lnxyls.cn

PHP:  count($arr);
来源：http://lr.9csxet.cn

JS:   arr.length
来源：http://aw.colortex.cn

TS:   arr.length
来源：http://mu.wgjwhj.cn

Java: list.size();
来源：http://kq.gzmigu.cn

Go:   len(arr)
来源：http://nw.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://tm.hahajie.cn

C#:   list.Count;
来源：http://mn.colortex.cn

[D07] 切片 / 取子数组
来源：http://oc.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ft.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cv.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://nd.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://nt.nicolike.cn

Java: list.subList(1, 4);
来源：http://jo.szsharing.cn

Go:   arr[1:4]
来源：http://xr.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://oc.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://cb.yuexingan06.cn

[D08] 合并两个数组
来源：http://br.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://gk.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://fg.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ax.shxzukj.cn

TS:   [...a, ...b];
来源：http://hz.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uu.jctech888.com.cn

Go:   append(a, b...)
来源：http://ax.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://qz.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://hg.nszjky.cn

[D09] 排序（升序）
来源：http://uo.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://yx.newstarts.cn

PHP:  sort($arr);
来源：http://zx.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gs.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ng.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fi.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kl.huixiangedu.cn

Ruby: arr.sort
来源：http://wa.nszjky.cn

C#:   list.Sort();
来源：http://ry.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pr.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nm.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iw.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kl.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rw.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ul.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cg.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jt.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bf.colortex.cn

[D11] 反转数组
来源：http://bp.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://no.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://dv.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sg.panjiajie.cn

TS:   [...arr].reverse();
来源：http://lt.newstarts.cn

Java: Collections.reverse(list);
来源：http://eb.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://ka.hahajie.cn

Ruby: arr.reverse
来源：http://lq.colortex.cn

C#:   list.Reverse();
来源：http://zu.shxzskj.cn

[D12] 查找元素下标
来源：http://gg.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://mn.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eq.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tr.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qt.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mt.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://el.hahajie.cn

Ruby: arr.index(x)
来源：http://ut.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://yi.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://zg.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ne.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uj.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://pv.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://pq.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ml.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://th.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yo.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cn.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://yi.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zf.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bz.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://bt.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://mz.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jp.jianghongdianzi.cn

Go:   // 手写循环
来源：http://td.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fv.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oc.nszjky.cn

[D15] 去重
来源：http://gk.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ce.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://jc.nicolike.cn

JS:   [...new Set(arr)]
来源：http://gn.shxzukj.cn


<!-- 参考信息 -->