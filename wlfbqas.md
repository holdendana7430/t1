代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hq.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vb.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xw.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sb.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eb.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xn.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://uu.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://cd.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://yt.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ov.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hm.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ux.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fu.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://xz.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://on.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://rq.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ho.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yz.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ko.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zv.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hp.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ro.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ki.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qv.jctech888.com.cn

[B13] 判断是否为数字
来源：http://op.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://ka.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://tl.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kq.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sw.wgjwhj.cn

Java: x instanceof Number
来源：http://gl.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xq.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://pp.colortex.cn

C#:   x is int or double or decimal
来源：http://zf.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://vm.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tx.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qw.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://ii.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://ff.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ol.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cf.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zd.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eh.nicolike.cn

[B15] 布尔运算与取反
来源：http://fx.yuntaijiaju.cn

Py:   a and b or not c
来源：http://oa.colortex.cn

PHP:  $a && $b || !$c
来源：http://tf.gzmigu.cn

JS:   a && b || !c
来源：http://kk.bookmarksfly.cn

TS:   a && b || !c
来源：http://ps.jianghongdianzi.cn

Java: a && b || !c
来源：http://hj.asd995.cn

Go:   a && b || !c
来源：http://zn.colortex.cn

Ruby: a && b || !c
来源：http://ov.9csxet.cn

C#:   a && b || !c
来源：http://dx.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zu.hnjuh.cn

Py:   if not data: return
来源：http://ai.521024.cn

PHP:  if (!$data) { return; }
来源：http://zc.asd995.cn

JS:   if (!data) return;
来源：http://ht.huixiangedu.cn

TS:   if (!data) return;
来源：http://ng.yuexingan06.cn

Java: if (data == null) return;
来源：http://ck.panjiajie.cn

Go:   if data == nil { return }
来源：http://if.shxzukj.cn

Ruby: return if data.nil?
来源：http://ov.szxytkj.cn

C#:   if (data == null) return;
来源：http://gi.chemitech.net.cn

================================================================================
来源：http://ar.haigaiapp.cn

C. 函数与作用域
来源：http://do.huixiangedu.cn

================================================================================
来源：http://jk.huanxung.cn

[C01] 定义函数
来源：http://gv.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://ib.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yi.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://le.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nu.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wz.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eu.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://zz.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sx.colortex.cn

[C02] 默认参数
来源：http://ez.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://rp.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ox.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ys.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nm.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://td.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cv.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://tj.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://jm.nicolike.cn

[C03] 可变参数
来源：http://ag.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://tl.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hc.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fe.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kz.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hv.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xx.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cd.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fd.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://dp.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://um.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mm.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xh.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kc.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://hp.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://dl.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://ao.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://bv.jianghongdianzi.cn

[C05] 返回多个值
来源：http://qf.huanxung.cn

Py:   return a, b
来源：http://nf.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://mc.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ph.hahajie.cn

TS:   return { a, b };
来源：http://ic.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bt.szsharing.cn

Go:   return a, b
来源：http://yt.jctech888.com.cn

Ruby: return a, b
来源：http://tg.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://dj.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://qv.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://gu.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pv.shxzukj.cn

JS:   const square = x => x * x;
来源：http://vq.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ra.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ft.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wz.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://dm.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vw.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://ds.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ka.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ss.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xb.shtwfgs.cn

TS:   arr.map(String)
来源：http://li.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mk.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ye.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://dr.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wo.yuexingan06.cn

[C08] 闭包
来源：http://df.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ss.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aj.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fr.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vb.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kv.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sg.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ax.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tv.chemitech.net.cn

[C09] 递归
来源：http://xm.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sb.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tb.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ys.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uv.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qx.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://du.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ir.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ox.szsharing.cn

[C10] 变量作用域
来源：http://bo.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://et.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yl.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nf.huixiangedu.cn

TS:   同 JS
来源：http://qb.shxzukj.cn

Java: 方法内为块级作用域
来源：http://qu.521024.cn

Go:   花括号块级作用域
来源：http://aq.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ko.shxzskj.cn

C#:   块级作用域
来源：http://by.lnxyls.cn

[C11] 模块导入与导出
来源：http://zr.yuntaijiaju.cn

Py:   from module import func
来源：http://uh.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tw.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ui.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tk.jianghongdianzi.cn

Java: import java.util.List;
来源：http://dq.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rq.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ba.nszjky.cn

C#:   using System.Text;
来源：http://gz.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://tw.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://mn.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://xr.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://yh.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://mt.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aq.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://ww.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://kn.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://di.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://kr.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qn.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://se.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tr.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ha.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yu.shxzukj.cn

Go:   func add(a, b int) int
来源：http://nq.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ma.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://an.huanxung.cn

[C14] 泛型函数
来源：http://hb.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yc.huanxung.cn

PHP:  // 无泛型
来源：http://yi.huixiangedu.cn

JS:   // 无泛型
来源：http://ev.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nn.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gf.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://td.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://wa.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nt.9csxet.cn

[C15] 解构 / 展开参数
来源：http://mn.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://of.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://xq.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://go.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ka.shtwfgs.cn

Java: // 无解构
来源：http://ua.colortex.cn

Go:   // 无解构
来源：http://bx.shtwfgs.cn

Ruby: a, b = pair
来源：http://gi.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://po.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://ib.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xz.nszjky.cn

PHP:  // 无重载
来源：http://oi.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wg.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://pk.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ql.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://xs.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ar.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vl.gzmigu.cn

================================================================================
来源：http://vi.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://dl.jianghongdianzi.cn

================================================================================
来源：http://hq.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://pq.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rs.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mn.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mw.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ei.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://am.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://si.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://dy.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gi.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://jw.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lz.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tf.bookmarksfly.cn

JS:   arr.push(4);
来源：http://nq.hahajie.cn

TS:   arr.push(4);
来源：http://xr.huixiangedu.cn

Java: list.add(4);
来源：http://jv.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://cy.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://or.9csxet.cn

C#:   list.Add(4);
来源：http://wc.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://zt.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://pl.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ec.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xm.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://tg.gzmigu.cn

Java: list.add(0, 0);
来源：http://rf.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nb.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bb.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://bw.huixinmuqiang.cn

[D04] 删除元素
来源：http://cg.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uy.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://av.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gd.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://xr.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ik.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jc.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lg.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zn.muxihuayi.cn

[D05] 访问与修改元素
来源：http://xt.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ej.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jt.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wv.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://iv.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://vb.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://cv.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mg.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mw.yuexingan06.cn

[D06] 数组长度
来源：http://ki.nicolike.cn

Py:   len(arr)
来源：http://ax.chemitech.net.cn

PHP:  count($arr);
来源：http://eb.hahajie.cn

JS:   arr.length
来源：http://ip.521024.cn

TS:   arr.length
来源：http://mw.muxihuayi.cn

Java: list.size();
来源：http://cr.jianghongdianzi.cn

Go:   len(arr)
来源：http://xj.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://vj.shxzukj.cn

C#:   list.Count;
来源：http://fk.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://cd.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iv.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://el.521024.cn

JS:   arr.slice(1, 4);
来源：http://fz.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://bi.hnjuh.cn

Java: list.subList(1, 4);
来源：http://kg.szxytkj.cn

Go:   arr[1:4]
来源：http://ml.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://rt.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://si.lnxyls.cn

[D08] 合并两个数组
来源：http://of.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://xi.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://fr.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://or.huanxung.cn

TS:   [...a, ...b];
来源：http://ww.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://no.521024.cn

Go:   append(a, b...)
来源：http://yk.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://ar.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://sv.9csxet.cn

[D09] 排序（升序）
来源：http://ob.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ct.huixiangedu.cn

PHP:  sort($arr);
来源：http://kz.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://we.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dh.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iv.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ha.panjiajie.cn

Ruby: arr.sort
来源：http://xh.nszjky.cn

C#:   list.Sort();
来源：http://qb.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pk.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yc.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yc.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://de.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rf.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ls.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ej.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hx.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oh.huixinmuqiang.cn


<!-- 参考信息 -->