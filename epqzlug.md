代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nv.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dq.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dr.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dz.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://as.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mh.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://gb.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://ee.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://ur.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://td.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qv.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yi.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cx.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://eq.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dr.chemitech.net.cn

[B12] 跳出多层循环
来源：http://ay.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zi.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kd.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nu.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fh.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kw.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nv.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hq.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gi.9csxet.cn

[B13] 判断是否为数字
来源：http://gq.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://bw.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://eg.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ml.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bp.asd995.cn

Java: x instanceof Number
来源：http://di.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ox.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://lp.huanxung.cn

C#:   x is int or double or decimal
来源：http://ia.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://hq.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vr.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dj.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://uv.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://at.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wo.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://be.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://al.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aq.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://cg.asd995.cn

Py:   a and b or not c
来源：http://qk.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://bm.shtwfgs.cn

JS:   a && b || !c
来源：http://ey.huanxung.cn

TS:   a && b || !c
来源：http://tr.szsharing.cn

Java: a && b || !c
来源：http://kn.lnxyls.cn

Go:   a && b || !c
来源：http://pb.szsharing.cn

Ruby: a && b || !c
来源：http://pe.colortex.cn

C#:   a && b || !c
来源：http://rk.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lh.nszjky.cn

Py:   if not data: return
来源：http://ht.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://lv.newstarts.cn

JS:   if (!data) return;
来源：http://nb.jctech888.com.cn

TS:   if (!data) return;
来源：http://xd.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://xc.gzmigu.cn

Go:   if data == nil { return }
来源：http://mj.lnxyls.cn

Ruby: return if data.nil?
来源：http://mj.shxzskj.cn

C#:   if (data == null) return;
来源：http://it.asd995.cn

================================================================================
来源：http://yb.asd995.cn

C. 函数与作用域
来源：http://de.jianghongdianzi.cn

================================================================================
来源：http://fi.bookmarksfly.cn

[C01] 定义函数
来源：http://qi.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://ch.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qw.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://fz.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ej.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ml.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qw.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://hl.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nz.jianghongdianzi.cn

[C02] 默认参数
来源：http://xm.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://ha.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cu.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://rs.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mb.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ld.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://on.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://jo.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ho.lnxyls.cn

[C03] 可变参数
来源：http://dv.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://ud.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jw.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eq.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bz.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ir.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rp.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gg.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ud.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://vm.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xz.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fr.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kv.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vy.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ij.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://sf.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://gw.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://ay.haigaiapp.cn

[C05] 返回多个值
来源：http://uy.nicolike.cn

Py:   return a, b
来源：http://cl.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://nr.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cz.chemitech.net.cn

TS:   return { a, b };
来源：http://wo.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ji.jianghongdianzi.cn

Go:   return a, b
来源：http://hi.chemitech.net.cn

Ruby: return a, b
来源：http://tj.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://op.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://og.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://ag.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://up.521024.cn

JS:   const square = x => x * x;
来源：http://zw.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://su.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xl.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cz.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://sj.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://da.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://fn.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rl.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bb.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yuexingan06.cn

TS:   arr.map(String)
来源：http://vz.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jh.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gf.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://qa.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hg.yuntaijiaju.cn

[C08] 闭包
来源：http://wu.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ts.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ar.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wz.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://im.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vo.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mi.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qf.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nz.shxzskj.cn

[C09] 递归
来源：http://km.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ib.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ez.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jp.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ce.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ff.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pg.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xj.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://le.shxzukj.cn

[C10] 变量作用域
来源：http://zb.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kp.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://az.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cx.asd995.cn

TS:   同 JS
来源：http://wf.lnxyls.cn

Java: 方法内为块级作用域
来源：http://qi.lnxyls.cn

Go:   花括号块级作用域
来源：http://oq.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fg.haigaiapp.cn

C#:   块级作用域
来源：http://pi.yuexingan06.cn

[C11] 模块导入与导出
来源：http://ls.bjjhwx.cn

Py:   from module import func
来源：http://ax.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ek.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kd.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lb.colortex.cn

Java: import java.util.List;
来源：http://ui.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bh.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://kl.yuntaijiaju.cn

C#:   using System.Text;
来源：http://gg.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://we.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://yb.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://jp.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ve.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://uh.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wy.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ja.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://az.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hu.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://kx.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qi.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gh.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fg.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://po.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mx.521024.cn

Go:   func add(a, b int) int
来源：http://tt.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ov.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://am.hahajie.cn

[C14] 泛型函数
来源：http://cv.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hg.muxihuayi.cn

PHP:  // 无泛型
来源：http://hk.newstarts.cn

JS:   // 无泛型
来源：http://gf.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yr.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mt.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://al.shxzskj.cn

Ruby: # 无泛型
来源：http://jw.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bo.nicolike.cn

[C15] 解构 / 展开参数
来源：http://ks.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mu.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://gv.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vo.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ig.hnjuh.cn

Java: // 无解构
来源：http://dm.jctech888.com.cn

Go:   // 无解构
来源：http://su.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://oj.colortex.cn

C#:   var (a, b) = pair;
来源：http://oy.szsharing.cn

[C16] 函数 / 方法重载
来源：http://tx.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://de.521024.cn

PHP:  // 无重载
来源：http://yn.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://py.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://uc.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qx.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://se.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://kg.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tv.newstarts.cn

================================================================================
来源：http://sc.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://wh.shtwfgs.cn

================================================================================
来源：http://tz.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://pm.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ai.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sx.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://by.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bw.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pr.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://lu.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://tz.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fe.colortex.cn

[D02] 追加元素到末尾
来源：http://ac.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oa.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lk.panjiajie.cn

JS:   arr.push(4);
来源：http://ro.9csxet.cn

TS:   arr.push(4);
来源：http://vu.bookmarksfly.cn

Java: list.add(4);
来源：http://gu.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://yj.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://ff.bookmarksfly.cn

C#:   list.Add(4);
来源：http://zm.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://wd.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://vb.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dt.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gb.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://xw.shtwfgs.cn

Java: list.add(0, 0);
来源：http://oa.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qn.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wh.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://mr.bookmarksfly.cn

[D04] 删除元素
来源：http://on.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aj.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://md.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ik.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://nz.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zr.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bg.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nq.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pk.shxzukj.cn

[D05] 访问与修改元素
来源：http://st.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ze.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fx.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pn.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://xn.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://tx.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://rn.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dm.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vl.colortex.cn

[D06] 数组长度
来源：http://jk.gzmigu.cn

Py:   len(arr)
来源：http://ii.asd995.cn

PHP:  count($arr);
来源：http://cs.gzmigu.cn

JS:   arr.length
来源：http://af.jianghongdianzi.cn

TS:   arr.length
来源：http://jl.hnjuh.cn

Java: list.size();
来源：http://oq.haigaiapp.cn

Go:   len(arr)
来源：http://lc.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://uw.huixinmuqiang.cn

C#:   list.Count;
来源：http://yw.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://zv.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zh.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ph.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://vp.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://eq.panjiajie.cn

Java: list.subList(1, 4);
来源：http://xq.nszjky.cn

Go:   arr[1:4]
来源：http://yv.szxytkj.cn

Ruby: arr[1, 3]
来源：http://ap.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://aa.shxzskj.cn

[D08] 合并两个数组
来源：http://fg.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://nb.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://rd.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qa.jctech888.com.cn

TS:   [...a, ...b];
来源：http://bi.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yf.gzmigu.cn

Go:   append(a, b...)
来源：http://zg.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://zo.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://fh.nszjky.cn

[D09] 排序（升序）
来源：http://om.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://zr.yuexingan06.cn

PHP:  sort($arr);
来源：http://jv.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iw.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://su.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iw.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cs.hahajie.cn

Ruby: arr.sort
来源：http://hm.szsharing.cn

C#:   list.Sort();
来源：http://hd.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lu.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sv.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zf.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ld.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ei.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vn.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sl.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eq.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wk.nszjky.cn


<!-- 参考信息 -->