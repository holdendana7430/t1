代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kt.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zd.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zk.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ny.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vz.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yo.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://es.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://zo.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://uh.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uk.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jz.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://js.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ih.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://lv.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hs.lnxyls.cn

[B12] 跳出多层循环
来源：http://qe.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rl.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wf.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hr.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sn.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aw.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://la.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pu.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ld.bjjhwx.cn

[B13] 判断是否为数字
来源：http://pd.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://fs.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://cs.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ox.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sm.asd995.cn

Java: x instanceof Number
来源：http://hu.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://om.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://rl.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://qx.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://ey.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ha.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rf.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://lz.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://lj.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kn.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wo.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vb.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gs.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://cj.shxzukj.cn

Py:   a and b or not c
来源：http://gm.colortex.cn

PHP:  $a && $b || !$c
来源：http://vg.asd995.cn

JS:   a && b || !c
来源：http://pl.gzmigu.cn

TS:   a && b || !c
来源：http://to.9csxet.cn

Java: a && b || !c
来源：http://di.haigaiapp.cn

Go:   a && b || !c
来源：http://ri.hnjuh.cn

Ruby: a && b || !c
来源：http://na.asd995.cn

C#:   a && b || !c
来源：http://oz.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wh.hnjuh.cn

Py:   if not data: return
来源：http://oi.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://wq.nicolike.cn

JS:   if (!data) return;
来源：http://gt.hahajie.cn

TS:   if (!data) return;
来源：http://oy.newstarts.cn

Java: if (data == null) return;
来源：http://gp.bjjhwx.cn

Go:   if data == nil { return }
来源：http://wz.panjiajie.cn

Ruby: return if data.nil?
来源：http://zk.shxzukj.cn

C#:   if (data == null) return;
来源：http://ng.yuntaijiaju.cn

================================================================================
来源：http://da.hahajie.cn

C. 函数与作用域
来源：http://qp.colortex.cn

================================================================================
来源：http://gm.muxihuayi.cn

[C01] 定义函数
来源：http://ie.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://ml.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hs.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://bo.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wt.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zy.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tg.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://xh.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ck.nszjky.cn

[C02] 默认参数
来源：http://kl.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://yf.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dg.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://nv.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tk.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kh.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rp.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://vq.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://zr.colortex.cn

[C03] 可变参数
来源：http://xu.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://cj.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://en.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zf.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vu.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rd.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ig.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qo.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rl.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://zs.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vm.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oc.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mr.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://af.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ev.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://pu.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://qh.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://em.asd995.cn

[C05] 返回多个值
来源：http://tl.yuexingan06.cn

Py:   return a, b
来源：http://ao.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://kj.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dl.bjjhwx.cn

TS:   return { a, b };
来源：http://ae.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://an.jctech888.com.cn

Go:   return a, b
来源：http://ty.muxihuayi.cn

Ruby: return a, b
来源：http://eo.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://rv.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://wt.newstarts.cn

Py:   square = lambda x: x * x
来源：http://vj.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cg.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://mi.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://op.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rh.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mz.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://yv.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ue.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://ay.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tp.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ay.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mm.gzmigu.cn

TS:   arr.map(String)
来源：http://wx.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://id.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oe.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://ud.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://aj.bjjhwx.cn

[C08] 闭包
来源：http://ek.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vr.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lo.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hi.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pu.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://om.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vv.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xi.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yt.lnxyls.cn

[C09] 递归
来源：http://um.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qz.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cg.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qi.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://we.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nq.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wy.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zu.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tc.chemitech.net.cn

[C10] 变量作用域
来源：http://lz.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://de.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kg.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sl.colortex.cn

TS:   同 JS
来源：http://lu.asd995.cn

Java: 方法内为块级作用域
来源：http://sp.szsharing.cn

Go:   花括号块级作用域
来源：http://sx.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kc.yuntaijiaju.cn

C#:   块级作用域
来源：http://zq.bjjhwx.cn

[C11] 模块导入与导出
来源：http://dl.panjiajie.cn

Py:   from module import func
来源：http://yv.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lg.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mn.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fe.colortex.cn

Java: import java.util.List;
来源：http://tv.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hx.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://bu.huixinmuqiang.cn

C#:   using System.Text;
来源：http://wk.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://am.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://gy.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://ha.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ec.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://uw.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rm.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://hb.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://ry.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mb.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://vp.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bn.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yx.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bv.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lw.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ea.521024.cn

Go:   func add(a, b int) int
来源：http://sa.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://os.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ya.huanxung.cn

[C14] 泛型函数
来源：http://xx.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bx.hnjuh.cn

PHP:  // 无泛型
来源：http://ux.chemitech.net.cn

JS:   // 无泛型
来源：http://ol.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wv.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ws.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ar.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://th.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ya.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://wm.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://df.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://yw.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ng.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sh.colortex.cn

Java: // 无解构
来源：http://ah.bookmarksfly.cn

Go:   // 无解构
来源：http://qf.gzmigu.cn

Ruby: a, b = pair
来源：http://qh.huanxung.cn

C#:   var (a, b) = pair;
来源：http://ot.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://ja.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nv.szxytkj.cn

PHP:  // 无重载
来源：http://gg.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tc.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://gc.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ie.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://wg.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://uc.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dz.panjiajie.cn

================================================================================
来源：http://xu.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://td.bookmarksfly.cn

================================================================================
来源：http://io.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://hf.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pr.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sj.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ih.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dq.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yq.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://su.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://er.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bg.9csxet.cn

[D02] 追加元素到末尾
来源：http://ii.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pc.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uw.bjjhwx.cn

JS:   arr.push(4);
来源：http://jv.bjjhwx.cn

TS:   arr.push(4);
来源：http://er.nicolike.cn

Java: list.add(4);
来源：http://ut.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://ax.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://ds.bjjhwx.cn

C#:   list.Add(4);
来源：http://tp.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://eu.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://ib.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oz.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uy.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://ud.jctech888.com.cn

Java: list.add(0, 0);
来源：http://dp.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ak.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pd.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://vd.jianghongdianzi.cn

[D04] 删除元素
来源：http://cg.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ag.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://so.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oj.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://tw.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xz.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bc.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vt.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hu.newstarts.cn

[D05] 访问与修改元素
来源：http://zw.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dv.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pm.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xm.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://vf.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://qe.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://kr.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tc.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hm.521024.cn

[D06] 数组长度
来源：http://nl.asd995.cn

Py:   len(arr)
来源：http://xo.panjiajie.cn

PHP:  count($arr);
来源：http://cz.haigaiapp.cn

JS:   arr.length
来源：http://ay.asd995.cn

TS:   arr.length
来源：http://hh.asd995.cn

Java: list.size();
来源：http://gz.yuntaijiaju.cn

Go:   len(arr)
来源：http://on.nicolike.cn

Ruby: arr.length; arr.size
来源：http://bu.chemitech.net.cn

C#:   list.Count;
来源：http://pl.newstarts.cn

[D07] 切片 / 取子数组
来源：http://vb.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uh.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://in.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://tj.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://ba.szxytkj.cn

Java: list.subList(1, 4);
来源：http://pk.szsharing.cn

Go:   arr[1:4]
来源：http://lh.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://su.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://lo.shtwfgs.cn

[D08] 合并两个数组
来源：http://va.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://tg.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://qe.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bb.nicolike.cn

TS:   [...a, ...b];
来源：http://cu.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rp.nicolike.cn

Go:   append(a, b...)
来源：http://ds.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://cf.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://va.bjjhwx.cn

[D09] 排序（升序）
来源：http://pp.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ee.wgjwhj.cn

PHP:  sort($arr);
来源：http://rg.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sg.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ls.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pc.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://om.muxihuayi.cn

Ruby: arr.sort
来源：http://in.huixiangedu.cn

C#:   list.Sort();
来源：http://xx.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yl.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lq.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pp.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://un.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hm.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mk.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ef.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fi.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tt.shxzskj.cn


<!-- 参考信息 -->