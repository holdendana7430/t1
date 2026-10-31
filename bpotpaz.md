代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ss.jctech888.com.cn

Java: x instanceof Number
来源：http://em.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eu.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://ja.shxzukj.cn

C#:   x is int or double or decimal
来源：http://fe.newstarts.cn

[B14] 判断值是否在集合内
来源：http://de.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qn.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://en.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://xy.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://wb.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vv.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vp.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qf.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rm.521024.cn

[B15] 布尔运算与取反
来源：http://ho.panjiajie.cn

Py:   a and b or not c
来源：http://aw.huanxung.cn

PHP:  $a && $b || !$c
来源：http://nv.yuntaijiaju.cn

JS:   a && b || !c
来源：http://dq.gzmigu.cn

TS:   a && b || !c
来源：http://at.chemitech.net.cn

Java: a && b || !c
来源：http://fn.chemitech.net.cn

Go:   a && b || !c
来源：http://ge.asd995.cn

Ruby: a && b || !c
来源：http://kg.bjjhwx.cn

C#:   a && b || !c
来源：http://bs.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://su.jctech888.com.cn

Py:   if not data: return
来源：http://pk.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://lq.hnjuh.cn

JS:   if (!data) return;
来源：http://uo.shxzukj.cn

TS:   if (!data) return;
来源：http://qi.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://un.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://io.newstarts.cn

Ruby: return if data.nil?
来源：http://cn.shtwfgs.cn

C#:   if (data == null) return;
来源：http://uz.hahajie.cn

================================================================================
来源：http://sz.wgjwhj.cn

C. 函数与作用域
来源：http://ti.gzmigu.cn

================================================================================
来源：http://mp.newstarts.cn

[C01] 定义函数
来源：http://iq.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://fs.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xw.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://lb.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xh.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eb.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wy.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://gf.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ho.shxzukj.cn

[C02] 默认参数
来源：http://nl.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://rv.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cl.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://ag.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://id.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lv.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hy.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://ol.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://ne.asd995.cn

[C03] 可变参数
来源：http://rc.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://ab.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ia.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wi.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jz.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sz.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wx.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rv.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ox.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://bm.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://df.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lt.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pf.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aj.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://nm.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://tf.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://uo.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://wh.hnjuh.cn

[C05] 返回多个值
来源：http://xb.gzmigu.cn

Py:   return a, b
来源：http://ey.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://is.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sm.haigaiapp.cn

TS:   return { a, b };
来源：http://xc.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ut.jianghongdianzi.cn

Go:   return a, b
来源：http://id.yuntaijiaju.cn

Ruby: return a, b
来源：http://db.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://eg.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://qm.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://xy.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bs.521024.cn

JS:   const square = x => x * x;
来源：http://ub.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://aa.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wa.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ct.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://yn.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kg.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://ad.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ei.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zk.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ga.huanxung.cn

TS:   arr.map(String)
来源：http://ic.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qd.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zx.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://oh.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wf.9csxet.cn

[C08] 闭包
来源：http://oo.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ek.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eq.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://et.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xc.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gy.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hm.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lz.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eb.gzmigu.cn

[C09] 递归
来源：http://rc.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xr.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lt.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iu.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nr.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cq.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gs.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jb.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qk.shxzukj.cn

[C10] 变量作用域
来源：http://xj.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wi.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ih.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tk.bjjhwx.cn

TS:   同 JS
来源：http://ye.lnxyls.cn

Java: 方法内为块级作用域
来源：http://hy.hahajie.cn

Go:   花括号块级作用域
来源：http://ye.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wn.hahajie.cn

C#:   块级作用域
来源：http://ck.panjiajie.cn

[C11] 模块导入与导出
来源：http://lo.shtwfgs.cn

Py:   from module import func
来源：http://ze.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nz.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rz.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kz.colortex.cn

Java: import java.util.List;
来源：http://li.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zm.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://no.521024.cn

C#:   using System.Text;
来源：http://ez.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://fe.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://ct.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://bq.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://pu.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://zq.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yc.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://kl.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://da.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wx.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://fs.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ei.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tz.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nb.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zk.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xu.shxzskj.cn

Go:   func add(a, b int) int
来源：http://qd.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iz.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jx.gzmigu.cn

[C14] 泛型函数
来源：http://ul.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fw.huanxung.cn

PHP:  // 无泛型
来源：http://sa.panjiajie.cn

JS:   // 无泛型
来源：http://ub.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gu.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vh.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wt.muxihuayi.cn

Ruby: # 无泛型
来源：http://dz.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kw.colortex.cn

[C15] 解构 / 展开参数
来源：http://wh.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uh.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://nd.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gb.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ae.nicolike.cn

Java: // 无解构
来源：http://ty.huixinmuqiang.cn

Go:   // 无解构
来源：http://lu.haigaiapp.cn

Ruby: a, b = pair
来源：http://on.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://mu.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://zo.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yv.lnxyls.cn

PHP:  // 无重载
来源：http://cl.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oh.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://sw.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://co.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://bt.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://ne.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aq.bookmarksfly.cn

================================================================================
来源：http://ca.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://nz.jianghongdianzi.cn

================================================================================
来源：http://fh.asd995.cn

[D01] 创建数组 / 列表
来源：http://ky.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sz.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ub.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bj.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ul.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qv.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://qe.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://nv.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://el.521024.cn

[D02] 追加元素到末尾
来源：http://fv.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qr.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://th.yuexingan06.cn

JS:   arr.push(4);
来源：http://aq.colortex.cn

TS:   arr.push(4);
来源：http://oi.huixinmuqiang.cn

Java: list.add(4);
来源：http://ri.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://wt.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ex.521024.cn

C#:   list.Add(4);
来源：http://su.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://vx.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://rx.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oo.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qn.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://ls.szxytkj.cn

Java: list.add(0, 0);
来源：http://sm.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tt.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mh.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://ej.yuntaijiaju.cn

[D04] 删除元素
来源：http://em.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ep.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jl.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gk.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://tn.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://un.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vu.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ok.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ed.chemitech.net.cn

[D05] 访问与修改元素
来源：http://zb.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pt.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hg.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lu.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://ao.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://nu.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://wa.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gc.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nk.yuexingan06.cn

[D06] 数组长度
来源：http://rg.panjiajie.cn

Py:   len(arr)
来源：http://kt.yuexingan06.cn

PHP:  count($arr);
来源：http://lw.jianghongdianzi.cn

JS:   arr.length
来源：http://fo.lnxyls.cn

TS:   arr.length
来源：http://ph.hahajie.cn

Java: list.size();
来源：http://au.jctech888.com.cn

Go:   len(arr)
来源：http://hx.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://yq.muxihuayi.cn

C#:   list.Count;
来源：http://mt.nicolike.cn

[D07] 切片 / 取子数组
来源：http://xk.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://no.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gg.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://kw.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://hk.panjiajie.cn

Java: list.subList(1, 4);
来源：http://tn.jctech888.com.cn

Go:   arr[1:4]
来源：http://vc.panjiajie.cn

Ruby: arr[1, 3]
来源：http://om.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://ox.muxihuayi.cn

[D08] 合并两个数组
来源：http://yo.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://mx.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://re.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cu.muxihuayi.cn

TS:   [...a, ...b];
来源：http://xu.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vk.hahajie.cn

Go:   append(a, b...)
来源：http://hf.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://cc.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://cl.huanxung.cn

[D09] 排序（升序）
来源：http://dv.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://fq.chemitech.net.cn

PHP:  sort($arr);
来源：http://ux.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uq.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hq.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bd.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gr.asd995.cn

Ruby: arr.sort
来源：http://ct.shxzukj.cn

C#:   list.Sort();
来源：http://cq.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gb.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zt.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ur.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://es.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qr.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sc.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cl.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ue.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dq.huixinmuqiang.cn

[D11] 反转数组
来源：http://oo.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://js.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://wd.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uv.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://to.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://mw.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://ml.hnjuh.cn

Ruby: arr.reverse
来源：http://ax.jctech888.com.cn

C#:   list.Reverse();
来源：http://ey.gzmigu.cn

[D12] 查找元素下标
来源：http://va.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://eq.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://of.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uh.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fr.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ny.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://pf.newstarts.cn

Ruby: arr.index(x)
来源：http://pr.szsharing.cn

C#:   list.IndexOf(x);
来源：http://mv.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://pb.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sd.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iy.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://ff.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://gm.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dc.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ev.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zs.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hd.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://yt.hnjuh.cn


<!-- 参考信息 -->