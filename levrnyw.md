代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lp.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mq.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lc.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dd.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ri.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mo.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ph.hnjuh.cn

[B13] 判断是否为数字
来源：http://db.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://ul.panjiajie.cn

PHP:  is_numeric($x)
来源：http://xv.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bv.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hv.bookmarksfly.cn

Java: x instanceof Number
来源：http://cc.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nj.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://kk.szsharing.cn

C#:   x is int or double or decimal
来源：http://qr.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://kq.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hq.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vm.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://up.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://hq.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sg.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://co.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tt.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fc.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://rg.chemitech.net.cn

Py:   a and b or not c
来源：http://jk.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://tk.szxytkj.cn

JS:   a && b || !c
来源：http://wz.shtwfgs.cn

TS:   a && b || !c
来源：http://ax.jianghongdianzi.cn

Java: a && b || !c
来源：http://gu.9csxet.cn

Go:   a && b || !c
来源：http://bh.muxihuayi.cn

Ruby: a && b || !c
来源：http://ue.lnxyls.cn

C#:   a && b || !c
来源：http://dq.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wk.bookmarksfly.cn

Py:   if not data: return
来源：http://he.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://qt.bookmarksfly.cn

JS:   if (!data) return;
来源：http://bx.huixiangedu.cn

TS:   if (!data) return;
来源：http://ni.szsharing.cn

Java: if (data == null) return;
来源：http://xm.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://bc.asd995.cn

Ruby: return if data.nil?
来源：http://fa.huixiangedu.cn

C#:   if (data == null) return;
来源：http://xj.bjjhwx.cn

================================================================================
来源：http://dz.gzmigu.cn

C. 函数与作用域
来源：http://ge.jctech888.com.cn

================================================================================
来源：http://zs.bjjhwx.cn

[C01] 定义函数
来源：http://fv.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://fy.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lj.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://mo.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qk.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wp.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iu.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://wc.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vl.asd995.cn

[C02] 默认参数
来源：http://nv.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://ya.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kn.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://cs.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ni.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zd.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cc.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://ox.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://pg.chemitech.net.cn

[C03] 可变参数
来源：http://mt.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://it.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nu.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wx.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xx.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uw.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yc.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://na.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zv.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://id.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gg.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ac.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eg.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tb.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://sk.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://px.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://yv.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://ye.nicolike.cn

[C05] 返回多个值
来源：http://sz.shxzukj.cn

Py:   return a, b
来源：http://xq.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://fn.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yh.hnjuh.cn

TS:   return { a, b };
来源：http://eb.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sj.hnjuh.cn

Go:   return a, b
来源：http://gg.huixiangedu.cn

Ruby: return a, b
来源：http://wc.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://oc.colortex.cn

[C06] 匿名函数 / lambda
来源：http://us.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://hg.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cq.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://vd.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://hr.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vj.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oe.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://ll.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ou.newstarts.cn

[C07] 把函数作为参数传入
来源：http://tm.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hh.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gr.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gj.huanxung.cn

TS:   arr.map(String)
来源：http://dk.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kf.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dr.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://ka.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hm.shxzukj.cn

[C08] 闭包
来源：http://et.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ht.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rm.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ju.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yw.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dk.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://es.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kb.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fr.wgjwhj.cn

[C09] 递归
来源：http://fe.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hu.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ep.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ms.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zn.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cd.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://na.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ib.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ex.9csxet.cn

[C10] 变量作用域
来源：http://jb.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://te.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jx.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gq.hahajie.cn

TS:   同 JS
来源：http://gt.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://uw.panjiajie.cn

Go:   花括号块级作用域
来源：http://xj.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qw.521024.cn

C#:   块级作用域
来源：http://ej.chemitech.net.cn

[C11] 模块导入与导出
来源：http://gd.hnjuh.cn

Py:   from module import func
来源：http://hf.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ds.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cw.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uk.shxzskj.cn

Java: import java.util.List;
来源：http://jv.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://br.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://tq.chemitech.net.cn

C#:   using System.Text;
来源：http://uu.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://vl.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://eu.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://vd.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://oa.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://yy.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ki.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://bo.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://bx.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xg.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://et.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vk.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dx.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ig.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ej.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ff.shxzukj.cn

Go:   func add(a, b int) int
来源：http://pc.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sb.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pm.wgjwhj.cn

[C14] 泛型函数
来源：http://fv.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ui.bookmarksfly.cn

PHP:  // 无泛型
来源：http://vm.panjiajie.cn

JS:   // 无泛型
来源：http://qv.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ly.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gs.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bh.521024.cn

Ruby: # 无泛型
来源：http://or.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gj.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://gn.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://po.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://hx.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://co.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nb.bjjhwx.cn

Java: // 无解构
来源：http://zk.bjjhwx.cn

Go:   // 无解构
来源：http://mt.nszjky.cn

Ruby: a, b = pair
来源：http://xf.nszjky.cn

C#:   var (a, b) = pair;
来源：http://el.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://xi.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ud.huanxung.cn

PHP:  // 无重载
来源：http://fh.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ae.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://po.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wn.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://iz.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://na.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nz.lnxyls.cn

================================================================================
来源：http://uy.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://tz.shtwfgs.cn

================================================================================
来源：http://yi.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://nl.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fg.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nh.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oc.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sg.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ff.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://wc.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://ex.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ce.521024.cn

[D02] 追加元素到末尾
来源：http://iu.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://io.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qh.wgjwhj.cn

JS:   arr.push(4);
来源：http://pq.huixiangedu.cn

TS:   arr.push(4);
来源：http://io.haigaiapp.cn

Java: list.add(4);
来源：http://zi.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://nz.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ex.nszjky.cn

C#:   list.Add(4);
来源：http://ih.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://zc.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://ha.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://al.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zi.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://gz.szsharing.cn

Java: list.add(0, 0);
来源：http://ow.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fy.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oh.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://yj.huanxung.cn

[D04] 删除元素
来源：http://je.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ys.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rm.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rw.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://ey.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zs.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://al.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vi.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uf.lnxyls.cn

[D05] 访问与修改元素
来源：http://gv.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nj.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://of.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gs.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://wc.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://aa.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://gb.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hn.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ax.colortex.cn

[D06] 数组长度
来源：http://io.521024.cn

Py:   len(arr)
来源：http://tu.9csxet.cn

PHP:  count($arr);
来源：http://di.colortex.cn

JS:   arr.length
来源：http://hg.huixinmuqiang.cn

TS:   arr.length
来源：http://ax.panjiajie.cn

Java: list.size();
来源：http://wz.9csxet.cn

Go:   len(arr)
来源：http://ib.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://qz.bjjhwx.cn

C#:   list.Count;
来源：http://wt.colortex.cn

[D07] 切片 / 取子数组
来源：http://wm.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bz.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bh.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://ve.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://jk.szxytkj.cn

Java: list.subList(1, 4);
来源：http://bz.shxzskj.cn

Go:   arr[1:4]
来源：http://cv.colortex.cn

Ruby: arr[1, 3]
来源：http://nt.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://op.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://zp.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://iy.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://nb.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zj.shxzskj.cn

TS:   [...a, ...b];
来源：http://nw.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://da.hnjuh.cn

Go:   append(a, b...)
来源：http://ne.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://tz.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://sr.yuexingan06.cn

[D09] 排序（升序）
来源：http://tj.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://tl.jctech888.com.cn

PHP:  sort($arr);
来源：http://zg.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sl.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ay.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bj.panjiajie.cn

Ruby: arr.sort
来源：http://uw.yuntaijiaju.cn

C#:   list.Sort();
来源：http://zk.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qn.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yd.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mv.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cw.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yq.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ev.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ki.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qb.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kc.bookmarksfly.cn

[D11] 反转数组
来源：http://tb.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wm.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://on.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://do.szsharing.cn

TS:   [...arr].reverse();
来源：http://jx.521024.cn

Java: Collections.reverse(list);
来源：http://on.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://yo.hnjuh.cn

Ruby: arr.reverse
来源：http://ok.asd995.cn

C#:   list.Reverse();
来源：http://ru.shtwfgs.cn

[D12] 查找元素下标
来源：http://ke.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://dc.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yi.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xg.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://at.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tp.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://sh.newstarts.cn


<!-- 参考信息 -->