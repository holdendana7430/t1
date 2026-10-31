代发 wailian999

PHP:  range(0, 10, 2);
来源：http://fy.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pu.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ak.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yi.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sr.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://vn.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bw.9csxet.cn

[B12] 跳出多层循环
来源：http://lb.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://al.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://of.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ar.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zn.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lz.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rx.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jy.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dt.asd995.cn

[B13] 判断是否为数字
来源：http://fm.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://bw.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://xs.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qw.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lz.bjjhwx.cn

Java: x instanceof Number
来源：http://xm.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nl.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://ft.huanxung.cn

C#:   x is int or double or decimal
来源：http://vq.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://ic.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cx.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pl.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://wu.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://vn.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ub.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xh.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rs.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rc.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://br.szxytkj.cn

Py:   a and b or not c
来源：http://zk.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://ho.muxihuayi.cn

JS:   a && b || !c
来源：http://ay.muxihuayi.cn

TS:   a && b || !c
来源：http://wr.newstarts.cn

Java: a && b || !c
来源：http://cf.haigaiapp.cn

Go:   a && b || !c
来源：http://ej.shxzukj.cn

Ruby: a && b || !c
来源：http://uu.wgjwhj.cn

C#:   a && b || !c
来源：http://fk.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cj.shtwfgs.cn

Py:   if not data: return
来源：http://qm.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://sp.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://bd.shtwfgs.cn

TS:   if (!data) return;
来源：http://iw.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://rf.szsharing.cn

Go:   if data == nil { return }
来源：http://nc.huanxung.cn

Ruby: return if data.nil?
来源：http://nh.nszjky.cn

C#:   if (data == null) return;
来源：http://nb.lnxyls.cn

================================================================================
来源：http://pw.bookmarksfly.cn

C. 函数与作用域
来源：http://ol.nszjky.cn

================================================================================
来源：http://uw.yuntaijiaju.cn

[C01] 定义函数
来源：http://to.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://dt.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://hd.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rc.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dr.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ap.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://ww.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://um.wgjwhj.cn

[C02] 默认参数
来源：http://zn.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://we.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cn.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://yp.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nq.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wk.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jx.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://sl.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://ux.chemitech.net.cn

[C03] 可变参数
来源：http://ey.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://zc.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fk.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sj.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wu.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pr.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://no.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mr.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pr.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://up.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nc.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bh.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zs.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pa.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://tn.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://lk.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://xa.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://fd.szsharing.cn

[C05] 返回多个值
来源：http://jh.521024.cn

Py:   return a, b
来源：http://cm.hahajie.cn

PHP:  return [$a, $b];
来源：http://ik.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mv.jianghongdianzi.cn

TS:   return { a, b };
来源：http://bw.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gh.9csxet.cn

Go:   return a, b
来源：http://rj.9csxet.cn

Ruby: return a, b
来源：http://nt.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://co.asd995.cn

[C06] 匿名函数 / lambda
来源：http://hv.newstarts.cn

Py:   square = lambda x: x * x
来源：http://zy.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bl.colortex.cn

JS:   const square = x => x * x;
来源：http://mf.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://og.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sb.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eu.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://wy.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lo.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://cs.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ye.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jk.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dx.nicolike.cn

TS:   arr.map(String)
来源：http://kh.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mn.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://td.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://eb.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dk.szxytkj.cn

[C08] 闭包
来源：http://vb.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ew.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bc.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xw.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qk.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wn.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cb.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dp.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jq.gzmigu.cn

[C09] 递归
来源：http://wv.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tp.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ns.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cf.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://or.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qv.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://my.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://td.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://he.jctech888.com.cn

[C10] 变量作用域
来源：http://zx.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ew.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fo.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fb.szsharing.cn

TS:   同 JS
来源：http://il.hahajie.cn

Java: 方法内为块级作用域
来源：http://xv.szxytkj.cn

Go:   花括号块级作用域
来源：http://up.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xq.jctech888.com.cn

C#:   块级作用域
来源：http://sf.nszjky.cn

[C11] 模块导入与导出
来源：http://qe.huanxung.cn

Py:   from module import func
来源：http://ha.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fu.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cz.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ha.shxzskj.cn

Java: import java.util.List;
来源：http://ji.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ra.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://gk.muxihuayi.cn

C#:   using System.Text;
来源：http://sf.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://iw.521024.cn

Py:   (lambda: print("run"))()
来源：http://rm.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://xk.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://mr.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://zv.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ld.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://kf.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://ld.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lq.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://vl.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jf.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jb.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ip.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kl.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nr.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://wc.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://td.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mz.huanxung.cn

[C14] 泛型函数
来源：http://go.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bc.shxzukj.cn

PHP:  // 无泛型
来源：http://za.muxihuayi.cn

JS:   // 无泛型
来源：http://wu.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vh.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wf.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vl.shtwfgs.cn

Ruby: # 无泛型
来源：http://rj.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ns.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://nk.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jj.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://nv.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ey.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rc.bjjhwx.cn

Java: // 无解构
来源：http://gt.asd995.cn

Go:   // 无解构
来源：http://pl.wgjwhj.cn

Ruby: a, b = pair
来源：http://ps.szsharing.cn

C#:   var (a, b) = pair;
来源：http://nl.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://ou.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jw.wgjwhj.cn

PHP:  // 无重载
来源：http://ma.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rp.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://it.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ud.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://bb.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://vg.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qk.huixiangedu.cn

================================================================================
来源：http://pi.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ah.nicolike.cn

================================================================================
来源：http://qo.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://ts.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sq.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://th.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ih.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tu.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://az.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://xw.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://la.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rm.521024.cn

[D02] 追加元素到末尾
来源：http://lx.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hv.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dk.gzmigu.cn

JS:   arr.push(4);
来源：http://dt.bjjhwx.cn

TS:   arr.push(4);
来源：http://tv.muxihuayi.cn

Java: list.add(4);
来源：http://fo.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://qx.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://nk.nszjky.cn

C#:   list.Add(4);
来源：http://bj.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://tw.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://cf.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nr.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://on.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://ws.hahajie.cn

Java: list.add(0, 0);
来源：http://oj.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://li.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xv.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://hc.shtwfgs.cn

[D04] 删除元素
来源：http://bd.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vo.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iv.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ys.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://yu.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ml.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kr.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xt.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://st.lnxyls.cn

[D05] 访问与修改元素
来源：http://eo.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://og.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tu.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rr.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://at.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://gm.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://to.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cy.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wx.szxytkj.cn

[D06] 数组长度
来源：http://ch.nicolike.cn

Py:   len(arr)
来源：http://ri.szxytkj.cn

PHP:  count($arr);
来源：http://nt.asd995.cn

JS:   arr.length
来源：http://zq.huixiangedu.cn

TS:   arr.length
来源：http://be.chemitech.net.cn

Java: list.size();
来源：http://hc.wgjwhj.cn

Go:   len(arr)
来源：http://mk.9csxet.cn

Ruby: arr.length; arr.size
来源：http://vy.shtwfgs.cn

C#:   list.Count;
来源：http://vy.colortex.cn

[D07] 切片 / 取子数组
来源：http://cc.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://we.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lt.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://cd.colortex.cn

TS:   arr.slice(1, 4);
来源：http://pp.lnxyls.cn

Java: list.subList(1, 4);
来源：http://fn.jctech888.com.cn

Go:   arr[1:4]
来源：http://vr.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://ys.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://ng.panjiajie.cn

[D08] 合并两个数组
来源：http://iz.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://fe.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://fl.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nu.bjjhwx.cn

TS:   [...a, ...b];
来源：http://tb.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ua.shxzukj.cn

Go:   append(a, b...)
来源：http://uw.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://tg.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://gk.chemitech.net.cn

[D09] 排序（升序）
来源：http://es.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://mz.521024.cn

PHP:  sort($arr);
来源：http://uw.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://it.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qq.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cy.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ki.szxytkj.cn

Ruby: arr.sort
来源：http://zs.huixinmuqiang.cn

C#:   list.Sort();
来源：http://gt.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uz.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mg.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rd.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rh.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hq.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dh.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lq.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xa.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oi.colortex.cn

[D11] 反转数组
来源：http://oo.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pt.521024.cn

PHP:  array_reverse($arr);
来源：http://eu.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yi.521024.cn

TS:   [...arr].reverse();
来源：http://fa.hahajie.cn

Java: Collections.reverse(list);
来源：http://qw.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://vk.nszjky.cn

Ruby: arr.reverse
来源：http://ee.shxzukj.cn


<!-- 参考信息 -->