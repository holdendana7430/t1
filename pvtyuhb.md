代发 wailian999

PHP:  range(0, 10, 2);
来源：http://lp.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pr.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fa.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lq.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://po.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://vz.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kj.jctech888.com.cn

[B12] 跳出多层循环
来源：http://qc.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nj.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://az.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lj.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qt.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fr.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ql.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zh.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bg.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://ei.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://wk.nszjky.cn

PHP:  is_numeric($x)
来源：http://cu.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jy.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vn.wgjwhj.cn

Java: x instanceof Number
来源：http://qs.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vu.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://hx.9csxet.cn

C#:   x is int or double or decimal
来源：http://qc.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://ok.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dw.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oe.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://xb.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://vz.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hc.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iw.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jx.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uy.shxzukj.cn

[B15] 布尔运算与取反
来源：http://jb.newstarts.cn

Py:   a and b or not c
来源：http://op.newstarts.cn

PHP:  $a && $b || !$c
来源：http://fq.gzmigu.cn

JS:   a && b || !c
来源：http://gx.chemitech.net.cn

TS:   a && b || !c
来源：http://cb.lnxyls.cn

Java: a && b || !c
来源：http://bc.shtwfgs.cn

Go:   a && b || !c
来源：http://xr.bjjhwx.cn

Ruby: a && b || !c
来源：http://is.9csxet.cn

C#:   a && b || !c
来源：http://uc.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aq.lnxyls.cn

Py:   if not data: return
来源：http://wp.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://pn.wgjwhj.cn

JS:   if (!data) return;
来源：http://ra.hnjuh.cn

TS:   if (!data) return;
来源：http://gt.yuexingan06.cn

Java: if (data == null) return;
来源：http://ky.chemitech.net.cn

Go:   if data == nil { return }
来源：http://gl.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://mw.shtwfgs.cn

C#:   if (data == null) return;
来源：http://br.huixiangedu.cn

================================================================================
来源：http://dz.hahajie.cn

C. 函数与作用域
来源：http://wc.yuntaijiaju.cn

================================================================================
来源：http://nl.yuexingan06.cn

[C01] 定义函数
来源：http://ls.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://aw.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ab.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://jv.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ui.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ab.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zq.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://kx.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ao.bjjhwx.cn

[C02] 默认参数
来源：http://gb.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://fp.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://on.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://ns.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lg.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wf.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wg.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://wr.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://dm.nszjky.cn

[C03] 可变参数
来源：http://ti.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://ro.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nc.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bp.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bm.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mo.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cj.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qf.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bu.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://ms.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uq.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ce.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://op.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nl.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://mm.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://la.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://xy.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://im.colortex.cn

[C05] 返回多个值
来源：http://jx.521024.cn

Py:   return a, b
来源：http://co.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://ub.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ni.shxzukj.cn

TS:   return { a, b };
来源：http://bv.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ee.muxihuayi.cn

Go:   return a, b
来源：http://tf.yuexingan06.cn

Ruby: return a, b
来源：http://kh.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://bq.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://qw.huanxung.cn

Py:   square = lambda x: x * x
来源：http://jc.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rh.asd995.cn

JS:   const square = x => x * x;
来源：http://nb.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://xp.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sd.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yf.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://xl.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ic.9csxet.cn

[C07] 把函数作为参数传入
来源：http://di.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nt.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ov.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xk.nicolike.cn

TS:   arr.map(String)
来源：http://uq.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zo.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://es.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://ey.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ax.hnjuh.cn

[C08] 闭包
来源：http://fw.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nu.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jn.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://at.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ii.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aq.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hp.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ip.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ak.bookmarksfly.cn

[C09] 递归
来源：http://fx.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uc.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fs.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kx.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bj.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tb.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lo.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mv.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hn.muxihuayi.cn

[C10] 变量作用域
来源：http://nt.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kr.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://my.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cr.jctech888.com.cn

TS:   同 JS
来源：http://az.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://ip.newstarts.cn

Go:   花括号块级作用域
来源：http://fw.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hq.panjiajie.cn

C#:   块级作用域
来源：http://rk.szxytkj.cn

[C11] 模块导入与导出
来源：http://bc.nszjky.cn

Py:   from module import func
来源：http://um.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jf.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qu.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lj.yuntaijiaju.cn

Java: import java.util.List;
来源：http://xl.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hp.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://im.lnxyls.cn

C#:   using System.Text;
来源：http://nr.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://qe.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://fs.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://bs.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://im.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://kx.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bs.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://jl.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://sy.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oi.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://mt.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ca.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iu.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://at.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://or.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ui.lnxyls.cn

Go:   func add(a, b int) int
来源：http://cw.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jg.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sz.9csxet.cn

[C14] 泛型函数
来源：http://ld.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zd.asd995.cn

PHP:  // 无泛型
来源：http://yv.shxzskj.cn

JS:   // 无泛型
来源：http://oa.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vf.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nr.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ev.shtwfgs.cn

Ruby: # 无泛型
来源：http://ce.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://es.521024.cn

[C15] 解构 / 展开参数
来源：http://el.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qf.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://yd.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qr.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rl.hnjuh.cn

Java: // 无解构
来源：http://ro.huanxung.cn

Go:   // 无解构
来源：http://iv.hnjuh.cn

Ruby: a, b = pair
来源：http://tc.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://su.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://qh.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xp.jctech888.com.cn

PHP:  // 无重载
来源：http://oi.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xj.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ju.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rc.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://aq.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://is.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xo.nszjky.cn

================================================================================
来源：http://sx.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://pm.jctech888.com.cn

================================================================================
来源：http://lg.9csxet.cn

[D01] 创建数组 / 列表
来源：http://ik.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hn.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pd.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pq.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qc.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rp.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://at.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://rl.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yn.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://ct.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dr.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ad.chemitech.net.cn

JS:   arr.push(4);
来源：http://ut.nicolike.cn

TS:   arr.push(4);
来源：http://yh.shtwfgs.cn

Java: list.add(4);
来源：http://jq.colortex.cn

Go:   arr = append(arr, 4)
来源：http://cv.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://xj.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://qw.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://gr.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://ne.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ij.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://za.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://dg.szsharing.cn

Java: list.add(0, 0);
来源：http://pl.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wk.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sg.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://sf.bookmarksfly.cn

[D04] 删除元素
来源：http://oc.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xt.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://by.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://np.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://gt.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tn.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://al.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kp.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://de.szsharing.cn

[D05] 访问与修改元素
来源：http://se.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gd.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nm.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sw.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://ik.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://ai.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://ig.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tq.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qv.jianghongdianzi.cn

[D06] 数组长度
来源：http://jv.hahajie.cn

Py:   len(arr)
来源：http://ik.szxytkj.cn

PHP:  count($arr);
来源：http://qs.haigaiapp.cn

JS:   arr.length
来源：http://uu.521024.cn

TS:   arr.length
来源：http://kz.haigaiapp.cn

Java: list.size();
来源：http://no.muxihuayi.cn

Go:   len(arr)
来源：http://ab.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://yr.panjiajie.cn

C#:   list.Count;
来源：http://rm.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://ca.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rt.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ey.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://ul.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://yp.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://on.shxzukj.cn

Go:   arr[1:4]
来源：http://vw.shxzskj.cn

Ruby: arr[1, 3]
来源：http://sm.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://vz.szxytkj.cn

[D08] 合并两个数组
来源：http://fq.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://gh.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://de.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ft.huixiangedu.cn

TS:   [...a, ...b];
来源：http://by.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oe.shxzskj.cn

Go:   append(a, b...)
来源：http://tv.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://og.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://ip.521024.cn

[D09] 排序（升序）
来源：http://xy.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://yj.bjjhwx.cn

PHP:  sort($arr);
来源：http://fs.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cz.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cu.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lc.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ul.nszjky.cn

Ruby: arr.sort
来源：http://ln.lnxyls.cn

C#:   list.Sort();
来源：http://gs.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xa.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tc.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oo.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cs.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ag.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wx.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bk.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pk.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xi.bookmarksfly.cn

[D11] 反转数组
来源：http://gw.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ej.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://tl.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vb.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://ep.panjiajie.cn

Java: Collections.reverse(list);
来源：http://rs.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://ua.bjjhwx.cn

Ruby: arr.reverse
来源：http://so.521024.cn


<!-- 参考信息 -->