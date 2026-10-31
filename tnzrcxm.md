代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rw.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wl.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://mp.521024.cn

Py:   list(range(0, 10, 2))
来源：http://ph.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://ec.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ro.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xc.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mm.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hq.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://uz.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aw.panjiajie.cn

[B12] 跳出多层循环
来源：http://xb.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ez.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oo.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sm.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qm.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dx.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ym.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://of.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ia.muxihuayi.cn

[B13] 判断是否为数字
来源：http://nu.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://do.szsharing.cn

PHP:  is_numeric($x)
来源：http://sp.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cx.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://li.muxihuayi.cn

Java: x instanceof Number
来源：http://ms.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pc.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://dx.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://vw.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://gx.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nq.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dv.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://ie.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://pv.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gj.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wc.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ox.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uv.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://sp.jianghongdianzi.cn

Py:   a and b or not c
来源：http://pj.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://iq.panjiajie.cn

JS:   a && b || !c
来源：http://ch.bjjhwx.cn

TS:   a && b || !c
来源：http://ey.9csxet.cn

Java: a && b || !c
来源：http://ao.wgjwhj.cn

Go:   a && b || !c
来源：http://qn.panjiajie.cn

Ruby: a && b || !c
来源：http://pa.colortex.cn

C#:   a && b || !c
来源：http://ha.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nt.yuexingan06.cn

Py:   if not data: return
来源：http://bb.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://kz.bookmarksfly.cn

JS:   if (!data) return;
来源：http://ir.colortex.cn

TS:   if (!data) return;
来源：http://mx.shxzukj.cn

Java: if (data == null) return;
来源：http://vu.szsharing.cn

Go:   if data == nil { return }
来源：http://vj.huanxung.cn

Ruby: return if data.nil?
来源：http://um.szsharing.cn

C#:   if (data == null) return;
来源：http://ik.szxytkj.cn

================================================================================
来源：http://ac.nszjky.cn

C. 函数与作用域
来源：http://kn.bookmarksfly.cn

================================================================================
来源：http://la.chemitech.net.cn

[C01] 定义函数
来源：http://cd.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://dl.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tl.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://xd.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zj.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rt.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hz.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://xi.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nc.huixiangedu.cn

[C02] 默认参数
来源：http://wg.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://im.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ca.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://hv.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vi.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ld.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ur.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://fl.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://pt.shxzskj.cn

[C03] 可变参数
来源：http://np.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://tg.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jg.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://na.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iy.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jz.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aj.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yq.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qx.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://qk.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hx.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kl.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mg.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sa.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://bx.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://ga.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://yt.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://im.shxzskj.cn

[C05] 返回多个值
来源：http://ut.hahajie.cn

Py:   return a, b
来源：http://jo.9csxet.cn

PHP:  return [$a, $b];
来源：http://vj.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mm.shxzskj.cn

TS:   return { a, b };
来源：http://vv.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ti.huanxung.cn

Go:   return a, b
来源：http://xq.nszjky.cn

Ruby: return a, b
来源：http://lp.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://kw.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://uz.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://fg.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dv.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://qu.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://uo.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mx.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bm.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://vv.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ny.nszjky.cn

[C07] 把函数作为参数传入
来源：http://db.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vf.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bx.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iu.shxzukj.cn

TS:   arr.map(String)
来源：http://sl.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hd.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mn.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://ag.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hy.gzmigu.cn

[C08] 闭包
来源：http://df.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cx.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://li.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cf.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pr.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yv.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rn.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dd.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ta.yuntaijiaju.cn

[C09] 递归
来源：http://su.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xd.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hp.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qv.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cb.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dx.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ml.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xd.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://am.huixiangedu.cn

[C10] 变量作用域
来源：http://iz.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lw.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mn.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zo.huixinmuqiang.cn

TS:   同 JS
来源：http://ez.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://vm.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://qp.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wh.panjiajie.cn

C#:   块级作用域
来源：http://ah.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://dm.shtwfgs.cn

Py:   from module import func
来源：http://sh.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vg.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fc.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oi.wgjwhj.cn

Java: import java.util.List;
来源：http://bh.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ai.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://ws.szxytkj.cn

C#:   using System.Text;
来源：http://bg.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://kz.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://zm.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://yh.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://uk.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://yf.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aj.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://rm.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://bo.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://es.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://de.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ch.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rm.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qm.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qv.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://th.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://pr.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tk.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pp.hnjuh.cn

[C14] 泛型函数
来源：http://ur.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zt.521024.cn

PHP:  // 无泛型
来源：http://xh.bookmarksfly.cn

JS:   // 无泛型
来源：http://la.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ic.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ts.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://on.shxzskj.cn

Ruby: # 无泛型
来源：http://rk.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wi.asd995.cn

[C15] 解构 / 展开参数
来源：http://cg.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zj.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://ey.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ml.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://og.chemitech.net.cn

Java: // 无解构
来源：http://pq.lnxyls.cn

Go:   // 无解构
来源：http://ht.szxytkj.cn

Ruby: a, b = pair
来源：http://ic.521024.cn

C#:   var (a, b) = pair;
来源：http://lj.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://ud.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wg.huixiangedu.cn

PHP:  // 无重载
来源：http://se.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lk.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://il.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ix.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://fn.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://qn.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://te.nicolike.cn

================================================================================
来源：http://ry.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://ya.nszjky.cn

================================================================================
来源：http://vi.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://ku.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fm.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zz.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ax.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tl.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lo.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://hy.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://uh.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ht.panjiajie.cn

[D02] 追加元素到末尾
来源：http://qs.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dt.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://po.wgjwhj.cn

JS:   arr.push(4);
来源：http://sh.wgjwhj.cn

TS:   arr.push(4);
来源：http://pa.9csxet.cn

Java: list.add(4);
来源：http://xn.521024.cn

Go:   arr = append(arr, 4)
来源：http://ip.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://zm.bjjhwx.cn

C#:   list.Add(4);
来源：http://gh.521024.cn

[D03] 在指定位置插入元素
来源：http://gg.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://mr.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hy.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zu.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ks.shtwfgs.cn

Java: list.add(0, 0);
来源：http://zv.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ez.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hl.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://hd.shtwfgs.cn

[D04] 删除元素
来源：http://ih.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uo.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yc.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uc.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://lf.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vz.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tc.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oh.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jc.haigaiapp.cn

[D05] 访问与修改元素
来源：http://eq.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tf.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ky.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jj.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://fy.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://wg.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://kb.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xj.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wx.shtwfgs.cn

[D06] 数组长度
来源：http://sn.hnjuh.cn

Py:   len(arr)
来源：http://kr.chemitech.net.cn

PHP:  count($arr);
来源：http://fy.hnjuh.cn

JS:   arr.length
来源：http://jd.jianghongdianzi.cn

TS:   arr.length
来源：http://qj.hahajie.cn

Java: list.size();
来源：http://sh.chemitech.net.cn

Go:   len(arr)
来源：http://gk.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://xz.yuexingan06.cn

C#:   list.Count;
来源：http://sc.hahajie.cn

[D07] 切片 / 取子数组
来源：http://om.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ma.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dw.asd995.cn

JS:   arr.slice(1, 4);
来源：http://nc.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://ci.asd995.cn

Java: list.subList(1, 4);
来源：http://tx.chemitech.net.cn

Go:   arr[1:4]
来源：http://nl.colortex.cn

Ruby: arr[1, 3]
来源：http://ky.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://wq.shxzskj.cn

[D08] 合并两个数组
来源：http://wr.521024.cn

Py:   a + b;  a.extend(b)
来源：http://jv.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://xq.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ce.jctech888.com.cn

TS:   [...a, ...b];
来源：http://qz.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rn.asd995.cn

Go:   append(a, b...)
来源：http://cw.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://ws.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://xn.szsharing.cn

[D09] 排序（升序）
来源：http://uu.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://cc.szsharing.cn

PHP:  sort($arr);
来源：http://wj.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zs.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wf.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://do.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ga.shxzukj.cn

Ruby: arr.sort
来源：http://mb.colortex.cn

C#:   list.Sort();
来源：http://mk.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://al.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gp.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hs.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://np.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ja.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bn.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xc.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://we.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dg.chemitech.net.cn

[D11] 反转数组
来源：http://ct.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nn.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://ua.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lj.shxzskj.cn


<!-- 参考信息 -->