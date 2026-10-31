代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tq.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://tg.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jp.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://ch.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qs.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://co.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fm.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dl.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ql.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tn.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://is.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zs.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://py.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://ze.huanxung.cn

PHP:  is_numeric($x)
来源：http://or.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uq.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ay.shtwfgs.cn

Java: x instanceof Number
来源：http://bm.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aj.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://oq.huanxung.cn

C#:   x is int or double or decimal
来源：http://ke.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://sn.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rm.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qj.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://cl.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://rj.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ee.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pc.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lg.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://og.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://jh.muxihuayi.cn

Py:   a and b or not c
来源：http://rv.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://xm.shtwfgs.cn

JS:   a && b || !c
来源：http://wx.nicolike.cn

TS:   a && b || !c
来源：http://ux.bookmarksfly.cn

Java: a && b || !c
来源：http://gb.shxzskj.cn

Go:   a && b || !c
来源：http://we.muxihuayi.cn

Ruby: a && b || !c
来源：http://tw.hahajie.cn

C#:   a && b || !c
来源：http://ik.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dy.lnxyls.cn

Py:   if not data: return
来源：http://zy.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://oe.huanxung.cn

JS:   if (!data) return;
来源：http://hl.hnjuh.cn

TS:   if (!data) return;
来源：http://lq.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://by.panjiajie.cn

Go:   if data == nil { return }
来源：http://vx.9csxet.cn

Ruby: return if data.nil?
来源：http://su.jctech888.com.cn

C#:   if (data == null) return;
来源：http://wg.9csxet.cn

================================================================================
来源：http://ao.gzmigu.cn

C. 函数与作用域
来源：http://xv.panjiajie.cn

================================================================================
来源：http://ge.bookmarksfly.cn

[C01] 定义函数
来源：http://yh.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://de.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ep.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ui.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sr.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mw.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nu.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://fz.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rs.newstarts.cn

[C02] 默认参数
来源：http://en.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://jb.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kn.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://vl.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ex.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://de.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eu.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://ti.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://pj.wgjwhj.cn

[C03] 可变参数
来源：http://th.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://nx.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qm.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gy.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xh.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nz.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zq.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ag.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zx.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://zx.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kh.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nc.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ha.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lk.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://be.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://sr.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://qp.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://vs.yuntaijiaju.cn

[C05] 返回多个值
来源：http://vg.lnxyls.cn

Py:   return a, b
来源：http://gk.gzmigu.cn

PHP:  return [$a, $b];
来源：http://oy.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gz.hnjuh.cn

TS:   return { a, b };
来源：http://ty.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ae.gzmigu.cn

Go:   return a, b
来源：http://ko.huanxung.cn

Ruby: return a, b
来源：http://rz.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://dl.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://ho.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://qj.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lm.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://gt.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://cw.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jq.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zh.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://jk.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://az.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://oa.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sk.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cf.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jb.bookmarksfly.cn

TS:   arr.map(String)
来源：http://hj.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wj.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cv.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://oh.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uw.colortex.cn

[C08] 闭包
来源：http://lx.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qm.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vf.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ht.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jy.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mb.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fa.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ir.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wl.panjiajie.cn

[C09] 递归
来源：http://mp.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bp.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yq.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ex.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://re.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oh.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hm.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zs.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tf.bjjhwx.cn

[C10] 变量作用域
来源：http://me.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://do.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gq.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yx.newstarts.cn

TS:   同 JS
来源：http://nl.shxzskj.cn

Java: 方法内为块级作用域
来源：http://vi.shxzskj.cn

Go:   花括号块级作用域
来源：http://bw.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qb.chemitech.net.cn

C#:   块级作用域
来源：http://hm.lnxyls.cn

[C11] 模块导入与导出
来源：http://az.huixinmuqiang.cn

Py:   from module import func
来源：http://up.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kh.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ea.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://za.newstarts.cn

Java: import java.util.List;
来源：http://iu.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dg.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://mi.haigaiapp.cn

C#:   using System.Text;
来源：http://aa.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://uv.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://oo.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://zh.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://jp.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://br.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lw.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://sd.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://rb.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qc.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://zk.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pl.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mi.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ks.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wh.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tz.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://yh.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ol.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jh.panjiajie.cn

[C14] 泛型函数
来源：http://ff.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wf.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://lx.shtwfgs.cn

JS:   // 无泛型
来源：http://qq.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xm.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mt.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lq.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://xa.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ai.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://vi.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ie.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://pq.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zo.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gc.nszjky.cn

Java: // 无解构
来源：http://cv.9csxet.cn

Go:   // 无解构
来源：http://at.bookmarksfly.cn

Ruby: a, b = pair
来源：http://hg.nicolike.cn

C#:   var (a, b) = pair;
来源：http://zl.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://bd.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jk.haigaiapp.cn

PHP:  // 无重载
来源：http://mk.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zj.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://np.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://av.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://kf.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://lc.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hg.521024.cn

================================================================================
来源：http://rv.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ay.521024.cn

================================================================================
来源：http://di.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://cy.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uz.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cy.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://km.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ng.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lk.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://tz.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://wo.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wk.shxzukj.cn

[D02] 追加元素到末尾
来源：http://ty.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vk.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nc.lnxyls.cn

JS:   arr.push(4);
来源：http://dz.gzmigu.cn

TS:   arr.push(4);
来源：http://tm.shtwfgs.cn

Java: list.add(4);
来源：http://gi.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://ce.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://yy.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://qq.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://ln.521024.cn

Py:   arr.insert(0, 0)
来源：http://wq.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yr.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ok.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ej.hnjuh.cn

Java: list.add(0, 0);
来源：http://wx.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wp.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ss.asd995.cn

C#:   list.Insert(0, 0);
来源：http://gb.huanxung.cn

[D04] 删除元素
来源：http://hw.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rr.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fq.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jm.colortex.cn

TS:   arr.splice(0, 1);
来源：http://dg.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zn.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xy.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ca.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://un.lnxyls.cn

[D05] 访问与修改元素
来源：http://ze.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rj.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fr.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ff.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://rm.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ow.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://hr.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gx.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rc.huixiangedu.cn

[D06] 数组长度
来源：http://qk.huanxung.cn

Py:   len(arr)
来源：http://nm.shtwfgs.cn

PHP:  count($arr);
来源：http://qi.jctech888.com.cn

JS:   arr.length
来源：http://hc.9csxet.cn

TS:   arr.length
来源：http://rn.jctech888.com.cn

Java: list.size();
来源：http://yv.521024.cn

Go:   len(arr)
来源：http://pi.nszjky.cn

Ruby: arr.length; arr.size
来源：http://xt.huixinmuqiang.cn

C#:   list.Count;
来源：http://mp.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://li.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vm.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://un.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://mx.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://jl.nszjky.cn

Java: list.subList(1, 4);
来源：http://ew.yuexingan06.cn

Go:   arr[1:4]
来源：http://ru.colortex.cn

Ruby: arr[1, 3]
来源：http://lc.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://mu.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://dv.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://pd.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://lb.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dr.shxzukj.cn

TS:   [...a, ...b];
来源：http://zw.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bl.bjjhwx.cn

Go:   append(a, b...)
来源：http://sq.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://hl.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://yr.shtwfgs.cn

[D09] 排序（升序）
来源：http://ps.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://rs.jctech888.com.cn

PHP:  sort($arr);
来源：http://yx.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wj.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jg.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vp.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qf.jianghongdianzi.cn

Ruby: arr.sort
来源：http://la.shxzskj.cn

C#:   list.Sort();
来源：http://fs.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wb.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pj.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zb.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ul.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gz.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://te.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ci.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lh.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mm.shxzskj.cn

[D11] 反转数组
来源：http://sk.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://au.nicolike.cn

PHP:  array_reverse($arr);
来源：http://pp.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yb.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://wu.521024.cn

Java: Collections.reverse(list);
来源：http://vu.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://tw.panjiajie.cn

Ruby: arr.reverse
来源：http://rc.lnxyls.cn

C#:   list.Reverse();
来源：http://kf.shtwfgs.cn

[D12] 查找元素下标
来源：http://as.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://yd.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gb.asd995.cn


<!-- 参考信息 -->