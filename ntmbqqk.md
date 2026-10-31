代发 wailian999

PHP:  range(0, 10, 2);
来源：http://nn.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cd.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gp.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ga.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oj.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://gy.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tl.jctech888.com.cn

[B12] 跳出多层循环
来源：http://si.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ya.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uz.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ov.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bq.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nl.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gd.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yn.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hg.huixiangedu.cn

[B13] 判断是否为数字
来源：http://bz.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://hw.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://wi.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dc.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eh.colortex.cn

Java: x instanceof Number
来源：http://od.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://np.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://cv.szxytkj.cn

C#:   x is int or double or decimal
来源：http://bm.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://vt.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ke.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pk.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://zi.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://xx.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rq.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mo.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zx.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qb.hnjuh.cn

[B15] 布尔运算与取反
来源：http://ag.gzmigu.cn

Py:   a and b or not c
来源：http://nq.colortex.cn

PHP:  $a && $b || !$c
来源：http://kx.colortex.cn

JS:   a && b || !c
来源：http://cz.hnjuh.cn

TS:   a && b || !c
来源：http://kj.bookmarksfly.cn

Java: a && b || !c
来源：http://uf.shxzukj.cn

Go:   a && b || !c
来源：http://po.huanxung.cn

Ruby: a && b || !c
来源：http://ik.shtwfgs.cn

C#:   a && b || !c
来源：http://fd.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xc.szsharing.cn

Py:   if not data: return
来源：http://cw.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://vn.wgjwhj.cn

JS:   if (!data) return;
来源：http://pz.bookmarksfly.cn

TS:   if (!data) return;
来源：http://ic.panjiajie.cn

Java: if (data == null) return;
来源：http://kk.chemitech.net.cn

Go:   if data == nil { return }
来源：http://ar.9csxet.cn

Ruby: return if data.nil?
来源：http://fp.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://cu.hahajie.cn

================================================================================
来源：http://ds.lnxyls.cn

C. 函数与作用域
来源：http://zn.hnjuh.cn

================================================================================
来源：http://dk.jctech888.com.cn

[C01] 定义函数
来源：http://pq.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://dy.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ar.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://ha.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yp.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rp.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://go.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://hg.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lf.jianghongdianzi.cn

[C02] 默认参数
来源：http://um.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://hj.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qu.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://vl.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qq.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lx.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nv.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://uq.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://yg.chemitech.net.cn

[C03] 可变参数
来源：http://tp.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://yz.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ah.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xj.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ld.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fj.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kk.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vn.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dg.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://kg.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fs.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gw.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://br.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nu.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://pq.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://id.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://mj.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://sv.colortex.cn

[C05] 返回多个值
来源：http://xx.haigaiapp.cn

Py:   return a, b
来源：http://wz.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://mj.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fv.shtwfgs.cn

TS:   return { a, b };
来源：http://aw.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ir.lnxyls.cn

Go:   return a, b
来源：http://fk.newstarts.cn

Ruby: return a, b
来源：http://wt.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://bj.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://ro.nszjky.cn

Py:   square = lambda x: x * x
来源：http://jv.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ow.newstarts.cn

JS:   const square = x => x * x;
来源：http://ea.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://ys.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ld.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nk.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://op.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ta.asd995.cn

[C07] 把函数作为参数传入
来源：http://lk.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oz.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lu.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://li.nszjky.cn

TS:   arr.map(String)
来源：http://no.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cz.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ry.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://hs.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cs.gzmigu.cn

[C08] 闭包
来源：http://wr.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ub.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ze.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zr.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fu.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://id.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gz.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rp.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uj.hnjuh.cn

[C09] 递归
来源：http://pd.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hc.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bi.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ts.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ap.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jl.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xp.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wm.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gd.9csxet.cn

[C10] 变量作用域
来源：http://tl.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hh.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dn.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cc.haigaiapp.cn

TS:   同 JS
来源：http://pn.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://wm.wgjwhj.cn

Go:   花括号块级作用域
来源：http://st.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://du.9csxet.cn

C#:   块级作用域
来源：http://gc.gzmigu.cn

[C11] 模块导入与导出
来源：http://yy.colortex.cn

Py:   from module import func
来源：http://ay.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gj.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jn.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zq.lnxyls.cn

Java: import java.util.List;
来源：http://fy.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://va.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://tm.huixiangedu.cn

C#:   using System.Text;
来源：http://ol.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://ce.colortex.cn

Py:   (lambda: print("run"))()
来源：http://kb.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://qs.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://db.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://kz.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sy.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://kd.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://ld.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ui.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://gu.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zs.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ed.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jt.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sz.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dl.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://ku.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gu.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://do.colortex.cn

[C14] 泛型函数
来源：http://jr.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ag.newstarts.cn

PHP:  // 无泛型
来源：http://ye.szsharing.cn

JS:   // 无泛型
来源：http://ry.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ta.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ca.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lk.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://su.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zo.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://wp.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ec.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://so.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rv.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zr.bookmarksfly.cn

Java: // 无解构
来源：http://rc.hnjuh.cn

Go:   // 无解构
来源：http://do.bjjhwx.cn

Ruby: a, b = pair
来源：http://aa.asd995.cn

C#:   var (a, b) = pair;
来源：http://jf.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://rh.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rb.szsharing.cn

PHP:  // 无重载
来源：http://pg.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nv.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://wx.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bw.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://un.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://le.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yf.panjiajie.cn

================================================================================
来源：http://pp.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://cx.nicolike.cn

================================================================================
来源：http://fn.asd995.cn

[D01] 创建数组 / 列表
来源：http://km.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ee.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dt.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ai.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bg.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dh.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://ub.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://hl.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wd.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://dg.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ww.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gu.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://ka.jctech888.com.cn

TS:   arr.push(4);
来源：http://ox.nicolike.cn

Java: list.add(4);
来源：http://oz.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://sb.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://hl.huixiangedu.cn

C#:   list.Add(4);
来源：http://er.hahajie.cn

[D03] 在指定位置插入元素
来源：http://hd.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://vg.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yj.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mv.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://hu.gzmigu.cn

Java: list.add(0, 0);
来源：http://tb.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vw.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gi.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://wx.gzmigu.cn

[D04] 删除元素
来源：http://wl.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yg.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jw.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jw.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://dw.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gq.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ml.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://of.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bp.shtwfgs.cn

[D05] 访问与修改元素
来源：http://jd.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fk.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pb.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mh.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://xw.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://yp.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://cw.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pv.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ob.bookmarksfly.cn

[D06] 数组长度
来源：http://ly.huanxung.cn

Py:   len(arr)
来源：http://bx.shxzskj.cn

PHP:  count($arr);
来源：http://lc.huixinmuqiang.cn

JS:   arr.length
来源：http://tc.colortex.cn

TS:   arr.length
来源：http://ny.9csxet.cn

Java: list.size();
来源：http://aj.newstarts.cn

Go:   len(arr)
来源：http://qx.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://wc.szxytkj.cn

C#:   list.Count;
来源：http://on.nicolike.cn

[D07] 切片 / 取子数组
来源：http://jr.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vl.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rd.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://rq.asd995.cn

TS:   arr.slice(1, 4);
来源：http://vc.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://cu.shxzskj.cn

Go:   arr[1:4]
来源：http://gw.colortex.cn

Ruby: arr[1, 3]
来源：http://sc.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://tq.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://ac.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://rk.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://qf.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ew.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://qs.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fn.shtwfgs.cn

Go:   append(a, b...)
来源：http://gd.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://jw.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://ko.szsharing.cn

[D09] 排序（升序）
来源：http://ry.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://nc.haigaiapp.cn

PHP:  sort($arr);
来源：http://aq.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://du.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rc.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bw.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rk.haigaiapp.cn

Ruby: arr.sort
来源：http://sp.huixiangedu.cn

C#:   list.Sort();
来源：http://vw.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sb.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uq.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ij.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://li.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oq.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xx.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lu.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uv.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tx.huixinmuqiang.cn

[D11] 反转数组
来源：http://hs.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ry.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://hl.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://re.panjiajie.cn

TS:   [...arr].reverse();
来源：http://ac.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://xa.521024.cn

Go:   slices.Reverse(arr)
来源：http://sm.muxihuayi.cn

Ruby: arr.reverse
来源：http://bd.wgjwhj.cn


<!-- 参考信息 -->