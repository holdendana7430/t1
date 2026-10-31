代发 wailian999

PHP:  range(0, 10, 2);
来源：http://mi.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://po.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kd.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ib.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rn.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://iz.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dh.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://uf.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yx.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mh.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nt.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mt.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oy.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rd.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ix.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://up.szsharing.cn

[B13] 判断是否为数字
来源：http://qz.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://qs.shxzskj.cn

PHP:  is_numeric($x)
来源：http://zr.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dz.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tp.wgjwhj.cn

Java: x instanceof Number
来源：http://yr.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://db.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://ic.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://fz.colortex.cn

[B14] 判断值是否在集合内
来源：http://ne.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gr.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dy.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://yn.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://sy.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oj.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pg.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mw.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hb.nszjky.cn

[B15] 布尔运算与取反
来源：http://qp.colortex.cn

Py:   a and b or not c
来源：http://os.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://ye.shtwfgs.cn

JS:   a && b || !c
来源：http://yi.bjjhwx.cn

TS:   a && b || !c
来源：http://bw.muxihuayi.cn

Java: a && b || !c
来源：http://ep.huanxung.cn

Go:   a && b || !c
来源：http://pj.gzmigu.cn

Ruby: a && b || !c
来源：http://wi.chemitech.net.cn

C#:   a && b || !c
来源：http://zc.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kq.shxzskj.cn

Py:   if not data: return
来源：http://jg.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://xd.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://rv.jctech888.com.cn

TS:   if (!data) return;
来源：http://wy.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://wr.hahajie.cn

Go:   if data == nil { return }
来源：http://wk.nszjky.cn

Ruby: return if data.nil?
来源：http://vx.newstarts.cn

C#:   if (data == null) return;
来源：http://zr.521024.cn

================================================================================
来源：http://bc.huixiangedu.cn

C. 函数与作用域
来源：http://at.jianghongdianzi.cn

================================================================================
来源：http://uf.yuntaijiaju.cn

[C01] 定义函数
来源：http://jy.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ro.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wv.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://oc.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sj.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bw.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pt.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://gg.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bz.jianghongdianzi.cn

[C02] 默认参数
来源：http://eo.521024.cn

Py:   def greet(name="World"): return name
来源：http://mo.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ob.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://yg.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bi.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oe.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hj.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://wy.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://wq.jctech888.com.cn

[C03] 可变参数
来源：http://vt.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://vk.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sx.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ak.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mf.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ct.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://td.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yc.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://js.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://gm.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wq.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zb.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://df.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gu.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://lo.521024.cn

Go:   // 无：用配置结构体参数
来源：http://vt.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://vd.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://lj.9csxet.cn

[C05] 返回多个值
来源：http://yt.huixiangedu.cn

Py:   return a, b
来源：http://oi.shxzukj.cn

PHP:  return [$a, $b];
来源：http://nm.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qs.nicolike.cn

TS:   return { a, b };
来源：http://jf.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tx.hahajie.cn

Go:   return a, b
来源：http://ti.chemitech.net.cn

Ruby: return a, b
来源：http://ob.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://xh.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://dg.asd995.cn

Py:   square = lambda x: x * x
来源：http://ce.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jg.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://gu.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://td.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eq.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ug.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://vk.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gr.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://sx.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wj.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wf.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rs.huanxung.cn

TS:   arr.map(String)
来源：http://eb.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nu.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://za.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ia.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ow.hnjuh.cn

[C08] 闭包
来源：http://ui.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ae.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lk.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xe.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ph.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://if.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://st.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fg.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uo.yuntaijiaju.cn

[C09] 递归
来源：http://gp.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ie.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jk.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xu.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mt.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ys.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gs.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qs.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qk.bjjhwx.cn

[C10] 变量作用域
来源：http://rt.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ac.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://so.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wj.wgjwhj.cn

TS:   同 JS
来源：http://tc.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ck.haigaiapp.cn

Go:   花括号块级作用域
来源：http://zu.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zr.wgjwhj.cn

C#:   块级作用域
来源：http://sa.newstarts.cn

[C11] 模块导入与导出
来源：http://rw.huixinmuqiang.cn

Py:   from module import func
来源：http://dw.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zd.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fn.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sw.bjjhwx.cn

Java: import java.util.List;
来源：http://yh.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mc.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://wi.lnxyls.cn

C#:   using System.Text;
来源：http://ph.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://xh.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://rr.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://kd.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://gp.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://hj.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hm.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://cr.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://pt.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tp.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://eb.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tu.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ag.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vx.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tz.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oh.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://hf.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qb.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://og.bookmarksfly.cn

[C14] 泛型函数
来源：http://qe.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fs.muxihuayi.cn

PHP:  // 无泛型
来源：http://tg.newstarts.cn

JS:   // 无泛型
来源：http://wk.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dv.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jr.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ss.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://ad.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ed.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://gx.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jl.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://gy.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://go.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gi.shtwfgs.cn

Java: // 无解构
来源：http://tj.huixinmuqiang.cn

Go:   // 无解构
来源：http://rt.haigaiapp.cn

Ruby: a, b = pair
来源：http://lc.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://hr.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://yp.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://te.shxzukj.cn

PHP:  // 无重载
来源：http://ye.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yr.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://zv.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rb.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://fs.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://zt.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qc.yuntaijiaju.cn

================================================================================
来源：http://gt.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://jc.colortex.cn

================================================================================
来源：http://kb.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://gh.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fh.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vs.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ls.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ud.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ez.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://sr.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://zc.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vw.nicolike.cn

[D02] 追加元素到末尾
来源：http://zz.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xt.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vm.hnjuh.cn

JS:   arr.push(4);
来源：http://tf.muxihuayi.cn

TS:   arr.push(4);
来源：http://se.haigaiapp.cn

Java: list.add(4);
来源：http://jp.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://ny.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://it.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://uw.hahajie.cn

[D03] 在指定位置插入元素
来源：http://nw.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://wo.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dh.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hi.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://cz.hahajie.cn

Java: list.add(0, 0);
来源：http://tg.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xp.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rh.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://bj.lnxyls.cn

[D04] 删除元素
来源：http://lz.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ia.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fy.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dx.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://jn.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oj.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uh.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cj.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xm.shxzukj.cn

[D05] 访问与修改元素
来源：http://vy.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pg.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nj.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ji.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://cj.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://dr.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://yr.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qi.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sb.bookmarksfly.cn

[D06] 数组长度
来源：http://sn.hnjuh.cn

Py:   len(arr)
来源：http://vv.shxzskj.cn

PHP:  count($arr);
来源：http://sr.yuexingan06.cn

JS:   arr.length
来源：http://ds.gzmigu.cn

TS:   arr.length
来源：http://if.jctech888.com.cn

Java: list.size();
来源：http://pv.gzmigu.cn

Go:   len(arr)
来源：http://jt.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://cf.9csxet.cn

C#:   list.Count;
来源：http://ie.hahajie.cn

[D07] 切片 / 取子数组
来源：http://la.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mh.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pg.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://mn.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://gz.hahajie.cn

Java: list.subList(1, 4);
来源：http://ty.shtwfgs.cn

Go:   arr[1:4]
来源：http://fy.shxzskj.cn

Ruby: arr[1, 3]
来源：http://ep.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://ao.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://gv.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://xd.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://jh.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uw.huixiangedu.cn

TS:   [...a, ...b];
来源：http://xk.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rb.hahajie.cn

Go:   append(a, b...)
来源：http://qq.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://iq.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://ic.521024.cn

[D09] 排序（升序）
来源：http://tx.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://sk.huanxung.cn

PHP:  sort($arr);
来源：http://vg.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wg.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ur.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yc.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eb.muxihuayi.cn

Ruby: arr.sort
来源：http://fy.shxzukj.cn

C#:   list.Sort();
来源：http://qr.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://it.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uw.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ay.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xp.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wq.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kv.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vg.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zi.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yg.yuntaijiaju.cn

[D11] 反转数组
来源：http://sl.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://op.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://aq.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jt.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://by.asd995.cn

Java: Collections.reverse(list);
来源：http://pp.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://vi.shtwfgs.cn

Ruby: arr.reverse
来源：http://zm.gzmigu.cn


<!-- 参考信息 -->