代发 wailian999

PHP:  range(0, 10, 2);
来源：http://pk.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iq.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lt.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tk.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bt.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://qp.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fe.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://nj.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gs.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gr.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uc.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qh.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ap.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://du.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jl.huixiangedu.cn

[B13] 判断是否为数字
来源：http://qr.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://sq.newstarts.cn

PHP:  is_numeric($x)
来源：http://hm.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pz.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rk.muxihuayi.cn

Java: x instanceof Number
来源：http://ov.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fn.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://ud.nicolike.cn

C#:   x is int or double or decimal
来源：http://vg.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://wn.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xs.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gk.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://qd.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://qn.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hi.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://js.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xb.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bh.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://xz.haigaiapp.cn

Py:   a and b or not c
来源：http://rt.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://hh.huixinmuqiang.cn

JS:   a && b || !c
来源：http://rk.colortex.cn

TS:   a && b || !c
来源：http://nz.chemitech.net.cn

Java: a && b || !c
来源：http://xl.bookmarksfly.cn

Go:   a && b || !c
来源：http://cx.haigaiapp.cn

Ruby: a && b || !c
来源：http://ee.shtwfgs.cn

C#:   a && b || !c
来源：http://dk.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ur.wgjwhj.cn

Py:   if not data: return
来源：http://gd.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://oj.bookmarksfly.cn

JS:   if (!data) return;
来源：http://fl.nszjky.cn

TS:   if (!data) return;
来源：http://rx.wgjwhj.cn

Java: if (data == null) return;
来源：http://tq.colortex.cn

Go:   if data == nil { return }
来源：http://qd.nicolike.cn

Ruby: return if data.nil?
来源：http://rk.huixiangedu.cn

C#:   if (data == null) return;
来源：http://qu.bookmarksfly.cn

================================================================================
来源：http://uj.huixinmuqiang.cn

C. 函数与作用域
来源：http://ql.hahajie.cn

================================================================================
来源：http://en.huixinmuqiang.cn

[C01] 定义函数
来源：http://dy.asd995.cn

Py:   def add(a, b): return a + b
来源：http://tg.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hd.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://pw.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pb.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bz.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ut.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://qp.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oa.bookmarksfly.cn

[C02] 默认参数
来源：http://kd.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://gx.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fk.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://oh.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pj.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wt.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cw.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ws.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://wq.muxihuayi.cn

[C03] 可变参数
来源：http://kb.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://wu.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eq.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://km.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://it.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ni.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://se.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gi.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mm.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://hi.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://id.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dk.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kr.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jk.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ck.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://jm.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://xt.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://iu.hnjuh.cn

[C05] 返回多个值
来源：http://jn.szxytkj.cn

Py:   return a, b
来源：http://yv.lnxyls.cn

PHP:  return [$a, $b];
来源：http://ua.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uq.bookmarksfly.cn

TS:   return { a, b };
来源：http://vj.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kf.yuexingan06.cn

Go:   return a, b
来源：http://xn.gzmigu.cn

Ruby: return a, b
来源：http://ze.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://gh.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://cd.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://rl.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ow.gzmigu.cn

JS:   const square = x => x * x;
来源：http://jp.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://im.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ma.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dg.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://nf.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fz.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://ze.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ck.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://an.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wj.gzmigu.cn

TS:   arr.map(String)
来源：http://ru.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ir.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pq.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://oa.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lm.haigaiapp.cn

[C08] 闭包
来源：http://ba.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pa.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yi.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mb.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vx.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://td.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dy.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cq.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tq.jctech888.com.cn

[C09] 递归
来源：http://ql.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pf.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://am.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rz.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cm.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xr.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yw.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bw.wgjwhj.cn

[C10] 变量作用域
来源：http://zt.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rk.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://py.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tx.colortex.cn

TS:   同 JS
来源：http://zn.szsharing.cn

Java: 方法内为块级作用域
来源：http://zy.huixiangedu.cn

Go:   花括号块级作用域
来源：http://wa.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ti.521024.cn

C#:   块级作用域
来源：http://hn.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://og.gzmigu.cn

Py:   from module import func
来源：http://bj.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ey.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rs.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uk.jianghongdianzi.cn

Java: import java.util.List;
来源：http://lp.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zl.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://bi.asd995.cn

C#:   using System.Text;
来源：http://zn.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://pb.521024.cn

Py:   (lambda: print("run"))()
来源：http://qa.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://wu.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://yd.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://lw.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jd.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://cm.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://lz.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://we.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://pr.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xd.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yq.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ov.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ig.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jp.nszjky.cn

Go:   func add(a, b int) int
来源：http://ij.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hb.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tk.bookmarksfly.cn

[C14] 泛型函数
来源：http://kg.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fl.chemitech.net.cn

PHP:  // 无泛型
来源：http://em.haigaiapp.cn

JS:   // 无泛型
来源：http://cb.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uk.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gs.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ax.9csxet.cn

Ruby: # 无泛型
来源：http://it.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bw.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://tk.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mj.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://rb.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fe.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://if.shxzskj.cn

Java: // 无解构
来源：http://wu.gzmigu.cn

Go:   // 无解构
来源：http://xd.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://aj.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://dm.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://wp.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://of.yuexingan06.cn

PHP:  // 无重载
来源：http://vo.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qo.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://bh.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://og.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://rp.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://ut.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fr.yuexingan06.cn

================================================================================
来源：http://ch.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://ei.nszjky.cn

================================================================================
来源：http://yk.9csxet.cn

[D01] 创建数组 / 列表
来源：http://jv.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xp.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://us.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://va.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dm.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sp.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://qc.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://gv.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uv.szxytkj.cn

[D02] 追加元素到末尾
来源：http://yj.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wv.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rc.9csxet.cn

JS:   arr.push(4);
来源：http://vj.9csxet.cn

TS:   arr.push(4);
来源：http://hn.hnjuh.cn

Java: list.add(4);
来源：http://za.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://cf.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://hi.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://od.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://hh.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://mp.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hx.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bq.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://vn.gzmigu.cn

Java: list.add(0, 0);
来源：http://sl.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kq.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bo.asd995.cn

C#:   list.Insert(0, 0);
来源：http://yf.huixiangedu.cn

[D04] 删除元素
来源：http://id.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gy.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lb.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aj.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://iq.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lv.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fc.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gi.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vb.huixiangedu.cn

[D05] 访问与修改元素
来源：http://mv.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://co.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wg.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zx.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://ob.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://pn.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://cu.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yz.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mt.yuntaijiaju.cn

[D06] 数组长度
来源：http://ja.panjiajie.cn

Py:   len(arr)
来源：http://mj.yuntaijiaju.cn

PHP:  count($arr);
来源：http://vq.szxytkj.cn

JS:   arr.length
来源：http://rc.shxzskj.cn

TS:   arr.length
来源：http://ci.huixiangedu.cn

Java: list.size();
来源：http://kn.haigaiapp.cn

Go:   len(arr)
来源：http://ot.hahajie.cn

Ruby: arr.length; arr.size
来源：http://hx.shxzukj.cn

C#:   list.Count;
来源：http://hq.nicolike.cn

[D07] 切片 / 取子数组
来源：http://xj.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mz.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wq.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://my.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://rs.nszjky.cn

Java: list.subList(1, 4);
来源：http://uv.nicolike.cn

Go:   arr[1:4]
来源：http://hv.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://xz.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://pk.521024.cn

[D08] 合并两个数组
来源：http://jo.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://ca.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://zx.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://we.szsharing.cn

TS:   [...a, ...b];
来源：http://tv.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nn.9csxet.cn

Go:   append(a, b...)
来源：http://ft.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://gd.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://db.shxzskj.cn

[D09] 排序（升序）
来源：http://kd.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://if.gzmigu.cn

PHP:  sort($arr);
来源：http://zc.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tf.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kh.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bz.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ec.jianghongdianzi.cn

Ruby: arr.sort
来源：http://nh.521024.cn

C#:   list.Sort();
来源：http://ha.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uo.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pe.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tt.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dj.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ly.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tu.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://az.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vr.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nc.jianghongdianzi.cn

[D11] 反转数组
来源：http://tt.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uu.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://bt.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aa.9csxet.cn

TS:   [...arr].reverse();
来源：http://uq.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://kd.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://ag.521024.cn

Ruby: arr.reverse
来源：http://hv.wgjwhj.cn


<!-- 参考信息 -->