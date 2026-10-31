代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ug.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://xm.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zi.shxzskj.cn

[B12] 跳出多层循环
来源：http://fi.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pk.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ok.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ul.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xv.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cz.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kw.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bs.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ak.gzmigu.cn

[B13] 判断是否为数字
来源：http://ge.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://ad.panjiajie.cn

PHP:  is_numeric($x)
来源：http://md.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tx.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ny.nicolike.cn

Java: x instanceof Number
来源：http://cc.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ru.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://ss.szxytkj.cn

C#:   x is int or double or decimal
来源：http://eh.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://qp.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ae.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wo.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://bj.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://wx.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yt.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://du.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://px.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ro.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://jl.bookmarksfly.cn

Py:   a and b or not c
来源：http://iz.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://rp.haigaiapp.cn

JS:   a && b || !c
来源：http://jf.asd995.cn

TS:   a && b || !c
来源：http://ks.yuntaijiaju.cn

Java: a && b || !c
来源：http://eq.muxihuayi.cn

Go:   a && b || !c
来源：http://gp.newstarts.cn

Ruby: a && b || !c
来源：http://ue.nicolike.cn

C#:   a && b || !c
来源：http://ma.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ml.jianghongdianzi.cn

Py:   if not data: return
来源：http://pp.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://bv.asd995.cn

JS:   if (!data) return;
来源：http://xi.9csxet.cn

TS:   if (!data) return;
来源：http://df.bjjhwx.cn

Java: if (data == null) return;
来源：http://xd.colortex.cn

Go:   if data == nil { return }
来源：http://mc.szxytkj.cn

Ruby: return if data.nil?
来源：http://bi.szsharing.cn

C#:   if (data == null) return;
来源：http://qh.nszjky.cn

================================================================================
来源：http://yq.bjjhwx.cn

C. 函数与作用域
来源：http://pv.huixinmuqiang.cn

================================================================================
来源：http://pz.newstarts.cn

[C01] 定义函数
来源：http://jj.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://eq.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gt.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://jk.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fj.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ig.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vv.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://hi.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://av.huixinmuqiang.cn

[C02] 默认参数
来源：http://rc.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://wf.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ig.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://tb.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vc.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ox.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://js.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://wd.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://zc.shxzukj.cn

[C03] 可变参数
来源：http://eh.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://tr.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yr.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sm.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wo.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ee.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bf.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tc.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tq.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://ea.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://up.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ci.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dc.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yn.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://vm.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://lf.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://on.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://th.haigaiapp.cn

[C05] 返回多个值
来源：http://ow.asd995.cn

Py:   return a, b
来源：http://nk.hnjuh.cn

PHP:  return [$a, $b];
来源：http://uw.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mh.huixiangedu.cn

TS:   return { a, b };
来源：http://zv.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ly.yuntaijiaju.cn

Go:   return a, b
来源：http://wn.hahajie.cn

Ruby: return a, b
来源：http://xx.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://vi.asd995.cn

[C06] 匿名函数 / lambda
来源：http://lg.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://up.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tr.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://eg.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://om.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wz.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rc.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://pi.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vt.nszjky.cn

[C07] 把函数作为参数传入
来源：http://wr.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nq.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sm.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xg.huanxung.cn

TS:   arr.map(String)
来源：http://ev.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qh.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xr.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://ko.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xo.shxzskj.cn

[C08] 闭包
来源：http://aj.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xk.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gs.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nz.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://du.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lq.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hd.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sa.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sf.wgjwhj.cn

[C09] 递归
来源：http://sg.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vt.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jj.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lb.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sa.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://et.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eq.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zt.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hi.shxzukj.cn

[C10] 变量作用域
来源：http://ll.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://up.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kf.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ow.wgjwhj.cn

TS:   同 JS
来源：http://ww.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://rj.haigaiapp.cn

Go:   花括号块级作用域
来源：http://ze.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fx.chemitech.net.cn

C#:   块级作用域
来源：http://vg.shxzukj.cn

[C11] 模块导入与导出
来源：http://hr.9csxet.cn

Py:   from module import func
来源：http://wo.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://de.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rb.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ca.gzmigu.cn

Java: import java.util.List;
来源：http://ig.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wx.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://je.haigaiapp.cn

C#:   using System.Text;
来源：http://hp.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://rr.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://bj.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://js.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://hk.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://lw.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qo.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://ul.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://lm.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gd.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://nb.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vq.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ag.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tt.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ta.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hr.panjiajie.cn

Go:   func add(a, b int) int
来源：http://sv.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sl.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mc.nszjky.cn

[C14] 泛型函数
来源：http://xy.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yi.bookmarksfly.cn

PHP:  // 无泛型
来源：http://gk.huixinmuqiang.cn

JS:   // 无泛型
来源：http://li.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://re.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mh.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ap.shxzukj.cn

Ruby: # 无泛型
来源：http://ju.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://da.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://ps.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mj.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://gi.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hy.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vf.gzmigu.cn

Java: // 无解构
来源：http://pe.huanxung.cn

Go:   // 无解构
来源：http://kv.panjiajie.cn

Ruby: a, b = pair
来源：http://ys.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://jc.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://fc.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zl.shxzukj.cn

PHP:  // 无重载
来源：http://is.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zo.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://bq.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://va.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://zd.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://yr.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://an.chemitech.net.cn

================================================================================
来源：http://wn.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://zq.gzmigu.cn

================================================================================
来源：http://ta.colortex.cn

[D01] 创建数组 / 列表
来源：http://yf.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ij.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ge.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lm.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ja.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://li.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://nj.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://rr.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lq.521024.cn

[D02] 追加元素到末尾
来源：http://kz.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kg.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lp.haigaiapp.cn

JS:   arr.push(4);
来源：http://xr.lnxyls.cn

TS:   arr.push(4);
来源：http://yx.bookmarksfly.cn

Java: list.add(4);
来源：http://us.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://su.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://rh.haigaiapp.cn

C#:   list.Add(4);
来源：http://qw.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://nq.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://sc.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bm.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nr.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://tb.hahajie.cn

Java: list.add(0, 0);
来源：http://sa.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qh.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sa.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://ca.asd995.cn

[D04] 删除元素
来源：http://me.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jv.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hr.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://at.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://ot.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yx.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cu.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lo.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qb.nicolike.cn

[D05] 访问与修改元素
来源：http://pg.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ry.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ib.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vt.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://li.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://pl.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://aa.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ou.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cl.hahajie.cn

[D06] 数组长度
来源：http://nl.huanxung.cn

Py:   len(arr)
来源：http://ya.panjiajie.cn

PHP:  count($arr);
来源：http://fy.nszjky.cn

JS:   arr.length
来源：http://rj.chemitech.net.cn

TS:   arr.length
来源：http://ie.huixiangedu.cn

Java: list.size();
来源：http://gp.bjjhwx.cn

Go:   len(arr)
来源：http://yr.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://xq.huanxung.cn

C#:   list.Count;
来源：http://mv.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://vn.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://he.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xa.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://rv.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://eq.9csxet.cn

Java: list.subList(1, 4);
来源：http://xp.haigaiapp.cn

Go:   arr[1:4]
来源：http://zq.szxytkj.cn

Ruby: arr[1, 3]
来源：http://ax.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://nl.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://av.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://lg.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://ix.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ra.haigaiapp.cn

TS:   [...a, ...b];
来源：http://mg.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hu.hnjuh.cn

Go:   append(a, b...)
来源：http://jx.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://hw.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://ix.jctech888.com.cn

[D09] 排序（升序）
来源：http://bt.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://up.szsharing.cn

PHP:  sort($arr);
来源：http://qh.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ne.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ng.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://li.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gn.haigaiapp.cn

Ruby: arr.sort
来源：http://cz.muxihuayi.cn

C#:   list.Sort();
来源：http://ij.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ks.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tk.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pv.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cu.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ds.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gr.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ff.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ip.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ik.bookmarksfly.cn

[D11] 反转数组
来源：http://mh.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mn.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://uh.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kd.newstarts.cn

TS:   [...arr].reverse();
来源：http://jd.9csxet.cn

Java: Collections.reverse(list);
来源：http://wd.521024.cn

Go:   slices.Reverse(arr)
来源：http://kh.huanxung.cn

Ruby: arr.reverse
来源：http://ep.bjjhwx.cn

C#:   list.Reverse();
来源：http://rc.shtwfgs.cn

[D12] 查找元素下标
来源：http://ko.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://yv.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uv.bjjhwx.cn


<!-- 参考信息 -->