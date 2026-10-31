代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xf.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fg.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://yg.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://we.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://yw.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wk.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ct.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ad.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fx.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://cn.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dy.newstarts.cn

[B12] 跳出多层循环
来源：http://kj.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bj.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gc.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://to.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gr.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xz.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wk.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oc.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://am.muxihuayi.cn

[B13] 判断是否为数字
来源：http://uo.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://qu.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://im.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tp.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cl.yuntaijiaju.cn

Java: x instanceof Number
来源：http://ux.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ny.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://cg.szsharing.cn

C#:   x is int or double or decimal
来源：http://oy.hahajie.cn

[B14] 判断值是否在集合内
来源：http://sy.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yx.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yu.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://cz.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://jv.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://og.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://km.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sx.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pw.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://mg.muxihuayi.cn

Py:   a and b or not c
来源：http://yk.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://vz.gzmigu.cn

JS:   a && b || !c
来源：http://or.huanxung.cn

TS:   a && b || !c
来源：http://ve.haigaiapp.cn

Java: a && b || !c
来源：http://ry.muxihuayi.cn

Go:   a && b || !c
来源：http://dn.shxzukj.cn

Ruby: a && b || !c
来源：http://ax.bookmarksfly.cn

C#:   a && b || !c
来源：http://lr.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lj.521024.cn

Py:   if not data: return
来源：http://ti.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://za.szsharing.cn

JS:   if (!data) return;
来源：http://zy.colortex.cn

TS:   if (!data) return;
来源：http://wb.yuexingan06.cn

Java: if (data == null) return;
来源：http://hq.muxihuayi.cn

Go:   if data == nil { return }
来源：http://hg.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://bc.muxihuayi.cn

C#:   if (data == null) return;
来源：http://ps.hahajie.cn

================================================================================
来源：http://df.yuntaijiaju.cn

C. 函数与作用域
来源：http://cq.jctech888.com.cn

================================================================================
来源：http://fu.shxzukj.cn

[C01] 定义函数
来源：http://bi.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ao.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ri.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://cf.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://il.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qw.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pb.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://zb.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bj.bookmarksfly.cn

[C02] 默认参数
来源：http://tk.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://so.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ki.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://bv.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ws.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vk.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ym.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://nk.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://qd.nszjky.cn

[C03] 可变参数
来源：http://nx.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://eh.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hy.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hb.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zi.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fd.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ux.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qk.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://db.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://dd.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uk.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ji.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sm.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gw.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://uu.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://kw.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://cr.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://yt.panjiajie.cn

[C05] 返回多个值
来源：http://em.shtwfgs.cn

Py:   return a, b
来源：http://lx.huanxung.cn

PHP:  return [$a, $b];
来源：http://gw.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wo.nszjky.cn

TS:   return { a, b };
来源：http://mu.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xw.lnxyls.cn

Go:   return a, b
来源：http://gm.muxihuayi.cn

Ruby: return a, b
来源：http://wk.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://lc.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://tr.huanxung.cn

Py:   square = lambda x: x * x
来源：http://fg.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vf.gzmigu.cn

JS:   const square = x => x * x;
来源：http://cl.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://rx.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nt.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://os.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://ab.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ok.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://ku.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hd.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vq.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mu.szxytkj.cn

TS:   arr.map(String)
来源：http://mh.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://du.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mo.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://vp.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://if.yuntaijiaju.cn

[C08] 闭包
来源：http://rw.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dc.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jh.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vf.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://on.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rz.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oa.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wa.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bs.hnjuh.cn

[C09] 递归
来源：http://yr.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iy.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bj.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://id.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://np.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gx.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sm.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tw.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yc.bookmarksfly.cn

[C10] 变量作用域
来源：http://xy.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gf.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ik.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xj.9csxet.cn

TS:   同 JS
来源：http://ge.nszjky.cn

Java: 方法内为块级作用域
来源：http://zw.lnxyls.cn

Go:   花括号块级作用域
来源：http://wg.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sm.bookmarksfly.cn

C#:   块级作用域
来源：http://bu.chemitech.net.cn

[C11] 模块导入与导出
来源：http://pz.521024.cn

Py:   from module import func
来源：http://px.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eq.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fq.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gp.9csxet.cn

Java: import java.util.List;
来源：http://uv.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qy.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://yh.huixinmuqiang.cn

C#:   using System.Text;
来源：http://tx.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://my.asd995.cn

Py:   (lambda: print("run"))()
来源：http://gq.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://sr.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://xu.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://if.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ym.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ot.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://qg.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xs.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://ay.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rp.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ec.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sg.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dv.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gf.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://ew.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dx.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yp.wgjwhj.cn

[C14] 泛型函数
来源：http://ml.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lx.newstarts.cn

PHP:  // 无泛型
来源：http://uw.shxzskj.cn

JS:   // 无泛型
来源：http://fq.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qn.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dy.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ke.521024.cn

Ruby: # 无泛型
来源：http://mx.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wq.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://tj.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tc.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://ke.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fq.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rm.asd995.cn

Java: // 无解构
来源：http://yy.shtwfgs.cn

Go:   // 无解构
来源：http://ou.newstarts.cn

Ruby: a, b = pair
来源：http://kw.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://gb.hahajie.cn

[C16] 函数 / 方法重载
来源：http://nf.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eg.huixinmuqiang.cn

PHP:  // 无重载
来源：http://xr.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bj.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://tk.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://im.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://fg.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://wi.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lh.521024.cn

================================================================================
来源：http://jw.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://pu.szxytkj.cn

================================================================================
来源：http://rk.colortex.cn

[D01] 创建数组 / 列表
来源：http://no.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://un.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zy.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://us.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wp.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zm.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ar.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://ml.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hg.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://ev.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vq.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ag.huixiangedu.cn

JS:   arr.push(4);
来源：http://lk.chemitech.net.cn

TS:   arr.push(4);
来源：http://zy.newstarts.cn

Java: list.add(4);
来源：http://yl.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://ec.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://dr.huanxung.cn

C#:   list.Add(4);
来源：http://uf.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://oh.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://fa.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rs.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ec.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://uf.shxzskj.cn

Java: list.add(0, 0);
来源：http://sh.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ci.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pn.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://si.asd995.cn

[D04] 删除元素
来源：http://zr.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fn.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yr.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kt.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://yg.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bt.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://am.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qx.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eh.nicolike.cn

[D05] 访问与修改元素
来源：http://yx.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ci.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://po.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ga.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://cw.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://ex.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://qc.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fi.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ml.hnjuh.cn

[D06] 数组长度
来源：http://ey.newstarts.cn

Py:   len(arr)
来源：http://ka.hahajie.cn

PHP:  count($arr);
来源：http://lb.huixiangedu.cn

JS:   arr.length
来源：http://df.muxihuayi.cn

TS:   arr.length
来源：http://zv.hnjuh.cn

Java: list.size();
来源：http://ww.lnxyls.cn

Go:   len(arr)
来源：http://la.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://wd.jianghongdianzi.cn

C#:   list.Count;
来源：http://lg.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://df.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kx.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hd.asd995.cn

JS:   arr.slice(1, 4);
来源：http://hx.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://ba.lnxyls.cn

Java: list.subList(1, 4);
来源：http://nj.jctech888.com.cn

Go:   arr[1:4]
来源：http://mi.asd995.cn

Ruby: arr[1, 3]
来源：http://hi.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://cq.nszjky.cn

[D08] 合并两个数组
来源：http://bp.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://de.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://uo.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mu.szxytkj.cn

TS:   [...a, ...b];
来源：http://lv.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sj.jctech888.com.cn

Go:   append(a, b...)
来源：http://oj.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://py.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://gw.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://yh.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://jm.shxzukj.cn

PHP:  sort($arr);
来源：http://qb.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eg.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ql.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tm.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://up.asd995.cn

Ruby: arr.sort
来源：http://gc.nszjky.cn

C#:   list.Sort();
来源：http://xr.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ao.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uc.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bx.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ug.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hp.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xu.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jh.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://go.yuntaijiaju.cn

[D11] 反转数组
来源：http://lt.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xd.asd995.cn

PHP:  array_reverse($arr);
来源：http://sw.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ne.newstarts.cn


<!-- 参考信息 -->