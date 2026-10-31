代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://ak.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xy.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vn.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vw.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://he.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wx.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ll.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tk.shtwfgs.cn

[B13] 判断是否为数字
来源：http://ny.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://nn.szsharing.cn

PHP:  is_numeric($x)
来源：http://si.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oi.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://px.szsharing.cn

Java: x instanceof Number
来源：http://vy.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vh.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://bi.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://sq.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://nm.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pl.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qo.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://ny.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://eq.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://th.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xw.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sl.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://od.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://vp.muxihuayi.cn

Py:   a and b or not c
来源：http://xr.9csxet.cn

PHP:  $a && $b || !$c
来源：http://yh.newstarts.cn

JS:   a && b || !c
来源：http://mg.jianghongdianzi.cn

TS:   a && b || !c
来源：http://hp.bookmarksfly.cn

Java: a && b || !c
来源：http://yn.huixinmuqiang.cn

Go:   a && b || !c
来源：http://cx.szsharing.cn

Ruby: a && b || !c
来源：http://mb.gzmigu.cn

C#:   a && b || !c
来源：http://er.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://da.haigaiapp.cn

Py:   if not data: return
来源：http://gn.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://de.huixiangedu.cn

JS:   if (!data) return;
来源：http://py.bjjhwx.cn

TS:   if (!data) return;
来源：http://zs.newstarts.cn

Java: if (data == null) return;
来源：http://pc.wgjwhj.cn

Go:   if data == nil { return }
来源：http://kj.colortex.cn

Ruby: return if data.nil?
来源：http://vd.newstarts.cn

C#:   if (data == null) return;
来源：http://ol.huixiangedu.cn

================================================================================
来源：http://xm.huanxung.cn

C. 函数与作用域
来源：http://ur.huixiangedu.cn

================================================================================
来源：http://dj.hahajie.cn

[C01] 定义函数
来源：http://nb.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://lk.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ar.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://qd.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ib.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cj.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tq.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://ji.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hv.shxzskj.cn

[C02] 默认参数
来源：http://ln.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://gh.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ro.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://yk.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rf.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ux.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yp.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://fa.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://im.nicolike.cn

[C03] 可变参数
来源：http://mm.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://li.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aq.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ok.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sk.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://la.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gg.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xa.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cm.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://rp.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xk.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cw.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uc.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xl.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://af.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://gp.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://bt.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://wi.lnxyls.cn

[C05] 返回多个值
来源：http://js.yuexingan06.cn

Py:   return a, b
来源：http://sy.hnjuh.cn

PHP:  return [$a, $b];
来源：http://xv.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bx.newstarts.cn

TS:   return { a, b };
来源：http://rh.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rb.shxzukj.cn

Go:   return a, b
来源：http://bz.szxytkj.cn

Ruby: return a, b
来源：http://cu.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://wl.colortex.cn

[C06] 匿名函数 / lambda
来源：http://kf.asd995.cn

Py:   square = lambda x: x * x
来源：http://oi.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ti.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://cv.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://op.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nn.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gu.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://er.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oj.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://sl.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jj.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kl.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ii.asd995.cn

TS:   arr.map(String)
来源：http://qa.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bm.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cy.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://jn.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ba.panjiajie.cn

[C08] 闭包
来源：http://fe.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ll.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ec.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ia.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aw.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ip.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cd.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dg.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hb.yuntaijiaju.cn

[C09] 递归
来源：http://ae.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eh.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ek.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://or.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ph.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fb.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wd.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jm.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mv.shxzskj.cn

[C10] 变量作用域
来源：http://nw.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ji.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mg.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xr.shxzskj.cn

TS:   同 JS
来源：http://rt.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://hb.panjiajie.cn

Go:   花括号块级作用域
来源：http://fe.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://df.521024.cn

C#:   块级作用域
来源：http://qo.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://es.hahajie.cn

Py:   from module import func
来源：http://nm.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nw.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pr.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bc.521024.cn

Java: import java.util.List;
来源：http://mi.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wa.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://cq.gzmigu.cn

C#:   using System.Text;
来源：http://pf.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://vf.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://vl.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://cj.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://hr.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://sm.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cg.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://kd.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://cw.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://om.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://hn.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eu.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mr.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bv.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ay.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://td.szsharing.cn

Go:   func add(a, b int) int
来源：http://pc.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://io.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kw.hahajie.cn

[C14] 泛型函数
来源：http://vf.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://up.colortex.cn

PHP:  // 无泛型
来源：http://nh.panjiajie.cn

JS:   // 无泛型
来源：http://co.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jp.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ll.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hs.hnjuh.cn

Ruby: # 无泛型
来源：http://qk.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oq.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://hw.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ei.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://yd.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sk.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yz.haigaiapp.cn

Java: // 无解构
来源：http://eg.szxytkj.cn

Go:   // 无解构
来源：http://ph.szsharing.cn

Ruby: a, b = pair
来源：http://du.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://hl.nicolike.cn

[C16] 函数 / 方法重载
来源：http://ew.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qw.huixiangedu.cn

PHP:  // 无重载
来源：http://cp.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zc.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://go.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://od.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://hu.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://ur.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uz.nszjky.cn

================================================================================
来源：http://yq.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://db.chemitech.net.cn

================================================================================
来源：http://of.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://tb.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qz.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fc.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tk.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wg.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ap.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://dr.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://mc.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oy.gzmigu.cn

[D02] 追加元素到末尾
来源：http://od.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kb.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mo.bookmarksfly.cn

JS:   arr.push(4);
来源：http://xx.wgjwhj.cn

TS:   arr.push(4);
来源：http://gw.szsharing.cn

Java: list.add(4);
来源：http://fn.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://ow.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://sa.lnxyls.cn

C#:   list.Add(4);
来源：http://kd.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://yu.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://yz.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qk.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lf.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://ez.hahajie.cn

Java: list.add(0, 0);
来源：http://do.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uw.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wy.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://nl.hahajie.cn

[D04] 删除元素
来源：http://wb.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wa.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hc.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://vg.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ao.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gh.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oo.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kz.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://ej.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://un.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xb.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://li.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://hm.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://jj.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://zo.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fn.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fc.hahajie.cn

[D06] 数组长度
来源：http://qr.jctech888.com.cn

Py:   len(arr)
来源：http://gx.shxzskj.cn

PHP:  count($arr);
来源：http://oc.wgjwhj.cn

JS:   arr.length
来源：http://uj.huixiangedu.cn

TS:   arr.length
来源：http://bx.szsharing.cn

Java: list.size();
来源：http://av.hahajie.cn

Go:   len(arr)
来源：http://uc.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://md.wgjwhj.cn

C#:   list.Count;
来源：http://qz.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://ws.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lq.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zg.asd995.cn

JS:   arr.slice(1, 4);
来源：http://dl.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://wg.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://dj.shxzukj.cn

Go:   arr[1:4]
来源：http://ys.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://bs.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://vq.9csxet.cn

[D08] 合并两个数组
来源：http://yr.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://gp.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://zk.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zn.jctech888.com.cn

TS:   [...a, ...b];
来源：http://fu.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rn.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://ml.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://sk.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://ea.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://se.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://gy.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://uo.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lo.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pj.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sc.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ji.szsharing.cn

Ruby: arr.sort
来源：http://hl.haigaiapp.cn

C#:   list.Sort();
来源：http://qz.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://my.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yg.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pl.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mg.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mw.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sb.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zv.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aq.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hv.lnxyls.cn

[D11] 反转数组
来源：http://nj.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ke.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://hf.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dl.hahajie.cn

TS:   [...arr].reverse();
来源：http://fg.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://uh.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://cu.szxytkj.cn

Ruby: arr.reverse
来源：http://ck.nszjky.cn

C#:   list.Reverse();
来源：http://qy.hahajie.cn

[D12] 查找元素下标
来源：http://wv.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://qy.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hs.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qb.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pr.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://so.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://ni.huanxung.cn


<!-- 参考信息 -->