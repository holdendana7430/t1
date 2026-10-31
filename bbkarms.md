代发 wailian999

PHP:  range(0, 10, 2);
来源：http://fp.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://by.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zc.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vn.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rl.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://tw.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wl.hahajie.cn

[B12] 跳出多层循环
来源：http://tb.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lx.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nj.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sb.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qj.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wi.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ek.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kw.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jg.chemitech.net.cn

[B13] 判断是否为数字
来源：http://fy.521024.cn

Py:   isinstance(x, (int, float))
来源：http://la.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ua.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ue.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hv.bookmarksfly.cn

Java: x instanceof Number
来源：http://jd.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uf.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://jd.panjiajie.cn

C#:   x is int or double or decimal
来源：http://kb.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://dd.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gj.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lp.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://qy.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://gr.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gu.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mw.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ui.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://re.lnxyls.cn

[B15] 布尔运算与取反
来源：http://kv.yuntaijiaju.cn

Py:   a and b or not c
来源：http://lt.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://cr.szsharing.cn

JS:   a && b || !c
来源：http://ot.lnxyls.cn

TS:   a && b || !c
来源：http://hi.jianghongdianzi.cn

Java: a && b || !c
来源：http://oh.asd995.cn

Go:   a && b || !c
来源：http://gy.szxytkj.cn

Ruby: a && b || !c
来源：http://cx.shxzskj.cn

C#:   a && b || !c
来源：http://rh.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gf.jianghongdianzi.cn

Py:   if not data: return
来源：http://jj.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://rh.chemitech.net.cn

JS:   if (!data) return;
来源：http://xh.shxzukj.cn

TS:   if (!data) return;
来源：http://qa.wgjwhj.cn

Java: if (data == null) return;
来源：http://rq.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://tw.muxihuayi.cn

Ruby: return if data.nil?
来源：http://ez.hnjuh.cn

C#:   if (data == null) return;
来源：http://qn.colortex.cn

================================================================================
来源：http://qb.nicolike.cn

C. 函数与作用域
来源：http://bp.huixiangedu.cn

================================================================================
来源：http://dk.shxzukj.cn

[C01] 定义函数
来源：http://ru.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://ni.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ng.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://tr.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ke.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://de.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ar.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://dm.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://at.panjiajie.cn

[C02] 默认参数
来源：http://lj.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://jg.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ed.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://do.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ft.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ev.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://na.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://ul.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://dg.panjiajie.cn

[C03] 可变参数
来源：http://cd.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://pe.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wx.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rt.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nf.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ba.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mm.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fw.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ty.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://zf.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vp.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cn.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bb.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wc.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ou.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://uh.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://rq.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://ag.nicolike.cn

[C05] 返回多个值
来源：http://yy.9csxet.cn

Py:   return a, b
来源：http://no.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://ni.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mo.colortex.cn

TS:   return { a, b };
来源：http://jd.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://my.colortex.cn

Go:   return a, b
来源：http://dn.9csxet.cn

Ruby: return a, b
来源：http://wq.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://ru.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://id.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://dd.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ah.panjiajie.cn

JS:   const square = x => x * x;
来源：http://wl.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ze.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hp.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://og.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://oq.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vq.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://se.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://js.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ix.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hd.huixiangedu.cn

TS:   arr.map(String)
来源：http://lx.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kn.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://am.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://vz.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hf.shxzskj.cn

[C08] 闭包
来源：http://bu.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fs.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kx.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zo.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vp.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sx.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vq.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yz.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wp.muxihuayi.cn

[C09] 递归
来源：http://tg.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hd.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://il.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vf.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mj.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xl.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mr.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ss.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://we.nicolike.cn

[C10] 变量作用域
来源：http://zx.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://go.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ck.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ws.yuntaijiaju.cn

TS:   同 JS
来源：http://ml.szxytkj.cn

Java: 方法内为块级作用域
来源：http://of.gzmigu.cn

Go:   花括号块级作用域
来源：http://yh.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jt.huixinmuqiang.cn

C#:   块级作用域
来源：http://um.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://bz.haigaiapp.cn

Py:   from module import func
来源：http://di.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ck.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qr.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pj.huanxung.cn

Java: import java.util.List;
来源：http://lm.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://di.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ij.colortex.cn

C#:   using System.Text;
来源：http://ku.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://mn.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://ec.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://wf.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://ye.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://ak.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://up.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://mp.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://px.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dg.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://ya.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xs.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dw.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vq.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lv.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jn.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://lq.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hj.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fk.yuntaijiaju.cn

[C14] 泛型函数
来源：http://lf.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://di.szxytkj.cn

PHP:  // 无泛型
来源：http://nf.asd995.cn

JS:   // 无泛型
来源：http://rq.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yl.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wl.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pg.wgjwhj.cn

Ruby: # 无泛型
来源：http://ka.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://de.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://us.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lw.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://ai.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qg.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rz.jctech888.com.cn

Java: // 无解构
来源：http://jc.huixiangedu.cn

Go:   // 无解构
来源：http://sh.wgjwhj.cn

Ruby: a, b = pair
来源：http://hj.nszjky.cn

C#:   var (a, b) = pair;
来源：http://qv.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://rg.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ix.colortex.cn

PHP:  // 无重载
来源：http://fy.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xt.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ov.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fk.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://kq.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://lk.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bz.yuntaijiaju.cn

================================================================================
来源：http://qe.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://be.hnjuh.cn

================================================================================
来源：http://vk.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://vr.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ci.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xz.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xv.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zp.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hx.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://hl.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://ij.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ds.lnxyls.cn

[D02] 追加元素到末尾
来源：http://pn.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mf.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hx.lnxyls.cn

JS:   arr.push(4);
来源：http://db.szsharing.cn

TS:   arr.push(4);
来源：http://pf.wgjwhj.cn

Java: list.add(4);
来源：http://jb.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://ew.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://ra.hahajie.cn

C#:   list.Add(4);
来源：http://co.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://we.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://ub.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jc.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dq.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://pk.newstarts.cn

Java: list.add(0, 0);
来源：http://hw.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ts.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rr.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://hw.huixiangedu.cn

[D04] 删除元素
来源：http://kj.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qy.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yp.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fd.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://vk.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jc.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pj.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hc.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://on.nszjky.cn

[D05] 访问与修改元素
来源：http://dk.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://on.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nx.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ca.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://cy.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://va.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xb.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bb.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oj.colortex.cn

[D06] 数组长度
来源：http://fh.lnxyls.cn

Py:   len(arr)
来源：http://es.szxytkj.cn

PHP:  count($arr);
来源：http://bs.szxytkj.cn

JS:   arr.length
来源：http://db.colortex.cn

TS:   arr.length
来源：http://st.lnxyls.cn

Java: list.size();
来源：http://yt.huanxung.cn

Go:   len(arr)
来源：http://me.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://mn.nszjky.cn

C#:   list.Count;
来源：http://oe.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://mb.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xd.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ji.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://qx.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://if.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://er.wgjwhj.cn

Go:   arr[1:4]
来源：http://ma.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://ix.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://fe.bjjhwx.cn

[D08] 合并两个数组
来源：http://yp.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://js.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://nr.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fw.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ko.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bj.szxytkj.cn

Go:   append(a, b...)
来源：http://ky.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://hy.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://dl.szsharing.cn

[D09] 排序（升序）
来源：http://yo.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ib.bjjhwx.cn

PHP:  sort($arr);
来源：http://qb.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yu.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nr.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://np.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tv.bookmarksfly.cn

Ruby: arr.sort
来源：http://ct.nszjky.cn

C#:   list.Sort();
来源：http://xw.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://do.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kc.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://af.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xp.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fd.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://so.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ag.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xe.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pc.colortex.cn

[D11] 反转数组
来源：http://aa.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mi.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://ce.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lu.nszjky.cn

TS:   [...arr].reverse();
来源：http://hn.asd995.cn

Java: Collections.reverse(list);
来源：http://tb.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://jv.9csxet.cn

Ruby: arr.reverse
来源：http://na.bjjhwx.cn


<!-- 参考信息 -->