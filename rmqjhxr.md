代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vr.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rx.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vj.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uu.nszjky.cn

[B13] 判断是否为数字
来源：http://zj.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://dt.521024.cn

PHP:  is_numeric($x)
来源：http://ol.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nk.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yl.muxihuayi.cn

Java: x instanceof Number
来源：http://hb.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://id.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://ab.colortex.cn

C#:   x is int or double or decimal
来源：http://dh.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://xi.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ti.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://im.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://us.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://nm.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qo.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ya.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ov.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ej.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://zb.szsharing.cn

Py:   a and b or not c
来源：http://ct.huanxung.cn

PHP:  $a && $b || !$c
来源：http://xr.szsharing.cn

JS:   a && b || !c
来源：http://us.bjjhwx.cn

TS:   a && b || !c
来源：http://oj.9csxet.cn

Java: a && b || !c
来源：http://dn.lnxyls.cn

Go:   a && b || !c
来源：http://hq.bjjhwx.cn

Ruby: a && b || !c
来源：http://eb.bjjhwx.cn

C#:   a && b || !c
来源：http://tx.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rg.521024.cn

Py:   if not data: return
来源：http://eg.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://xt.szsharing.cn

JS:   if (!data) return;
来源：http://re.szsharing.cn

TS:   if (!data) return;
来源：http://en.hahajie.cn

Java: if (data == null) return;
来源：http://gu.haigaiapp.cn

Go:   if data == nil { return }
来源：http://qe.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://en.hnjuh.cn

C#:   if (data == null) return;
来源：http://nj.yuntaijiaju.cn

================================================================================
来源：http://oc.huanxung.cn

C. 函数与作用域
来源：http://dx.chemitech.net.cn

================================================================================
来源：http://rm.haigaiapp.cn

[C01] 定义函数
来源：http://jn.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://fz.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rh.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://pv.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gj.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cw.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://et.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://af.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gi.shtwfgs.cn

[C02] 默认参数
来源：http://mp.521024.cn

Py:   def greet(name="World"): return name
来源：http://zz.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ew.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://vg.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://de.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ei.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zn.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ho.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://uo.yuexingan06.cn

[C03] 可变参数
来源：http://lm.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://ab.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vb.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wn.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yi.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vu.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ac.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uz.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vw.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://ww.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vr.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qz.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bv.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gk.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://fv.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://pf.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://up.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://rm.haigaiapp.cn

[C05] 返回多个值
来源：http://ol.shxzukj.cn

Py:   return a, b
来源：http://cc.panjiajie.cn

PHP:  return [$a, $b];
来源：http://cb.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jf.huixiangedu.cn

TS:   return { a, b };
来源：http://gy.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bc.hahajie.cn

Go:   return a, b
来源：http://cm.panjiajie.cn

Ruby: return a, b
来源：http://zw.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://nx.521024.cn

[C06] 匿名函数 / lambda
来源：http://lj.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://xw.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cm.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://wh.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://el.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ok.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zi.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://dh.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lr.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://or.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vw.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ru.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tt.bookmarksfly.cn

TS:   arr.map(String)
来源：http://pp.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gl.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mo.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://yr.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jd.wgjwhj.cn

[C08] 闭包
来源：http://ey.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://te.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qv.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wh.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xk.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xu.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kh.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ln.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kq.hnjuh.cn

[C09] 递归
来源：http://vh.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qg.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sa.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sj.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zj.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yl.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jv.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://da.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ru.haigaiapp.cn

[C10] 变量作用域
来源：http://qu.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pl.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gd.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yp.huixinmuqiang.cn

TS:   同 JS
来源：http://al.hahajie.cn

Java: 方法内为块级作用域
来源：http://it.huanxung.cn

Go:   花括号块级作用域
来源：http://cc.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ed.nicolike.cn

C#:   块级作用域
来源：http://ei.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://xf.newstarts.cn

Py:   from module import func
来源：http://uh.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kl.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://as.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tl.huanxung.cn

Java: import java.util.List;
来源：http://ap.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://so.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://lx.jctech888.com.cn

C#:   using System.Text;
来源：http://en.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://wf.asd995.cn

Py:   (lambda: print("run"))()
来源：http://xo.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://py.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://lx.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ie.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nm.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://qd.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ae.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cz.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://oj.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ej.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tt.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sa.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pv.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wd.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://tn.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yv.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rq.bookmarksfly.cn

[C14] 泛型函数
来源：http://rz.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nc.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://jr.huixinmuqiang.cn

JS:   // 无泛型
来源：http://ab.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sq.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ni.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rp.lnxyls.cn

Ruby: # 无泛型
来源：http://pn.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hb.521024.cn

[C15] 解构 / 展开参数
来源：http://qb.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rq.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://oa.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lu.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tj.jctech888.com.cn

Java: // 无解构
来源：http://ez.wgjwhj.cn

Go:   // 无解构
来源：http://bb.shxzukj.cn

Ruby: a, b = pair
来源：http://lx.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://hc.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://uy.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tr.bjjhwx.cn

PHP:  // 无重载
来源：http://ve.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ru.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://yv.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rt.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://no.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://bs.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ou.chemitech.net.cn

================================================================================
来源：http://we.colortex.cn

D. 数组 / 列表 / 集合
来源：http://wc.yuexingan06.cn

================================================================================
来源：http://xq.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://ur.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ov.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pa.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qd.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ef.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bc.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://ye.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://iy.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dw.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://xy.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ud.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ae.gzmigu.cn

JS:   arr.push(4);
来源：http://jy.nicolike.cn

TS:   arr.push(4);
来源：http://xk.szsharing.cn

Java: list.add(4);
来源：http://ij.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://xf.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://sw.shtwfgs.cn

C#:   list.Add(4);
来源：http://fx.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://vs.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://lf.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wb.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://te.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ak.shtwfgs.cn

Java: list.add(0, 0);
来源：http://ac.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qw.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xx.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://gj.muxihuayi.cn

[D04] 删除元素
来源：http://sp.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pu.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gu.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fk.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://rt.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hp.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cp.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eq.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cq.lnxyls.cn

[D05] 访问与修改元素
来源：http://yb.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uv.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mc.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ex.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://lx.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ws.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://rd.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hd.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zm.wgjwhj.cn

[D06] 数组长度
来源：http://ct.huixiangedu.cn

Py:   len(arr)
来源：http://yl.nicolike.cn

PHP:  count($arr);
来源：http://ua.jctech888.com.cn

JS:   arr.length
来源：http://nt.colortex.cn

TS:   arr.length
来源：http://ol.asd995.cn

Java: list.size();
来源：http://qz.jctech888.com.cn

Go:   len(arr)
来源：http://fu.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://ns.yuexingan06.cn

C#:   list.Count;
来源：http://wd.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://ab.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ij.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bz.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://ck.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://cb.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://xo.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://ox.nicolike.cn

Ruby: arr[1, 3]
来源：http://ow.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://wq.gzmigu.cn

[D08] 合并两个数组
来源：http://aq.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://mh.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://ii.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lb.chemitech.net.cn

TS:   [...a, ...b];
来源：http://gi.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mp.bookmarksfly.cn

Go:   append(a, b...)
来源：http://hm.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://km.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://up.huanxung.cn

[D09] 排序（升序）
来源：http://uv.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://px.bookmarksfly.cn

PHP:  sort($arr);
来源：http://ql.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sg.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xy.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yx.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dn.muxihuayi.cn

Ruby: arr.sort
来源：http://au.szsharing.cn

C#:   list.Sort();
来源：http://lj.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fc.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://au.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tf.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://in.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eu.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://km.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://im.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pl.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yz.shxzskj.cn

[D11] 反转数组
来源：http://aa.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mw.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://fm.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qk.szxytkj.cn

TS:   [...arr].reverse();
来源：http://it.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://zq.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://es.shtwfgs.cn

Ruby: arr.reverse
来源：http://oh.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://fn.haigaiapp.cn

[D12] 查找元素下标
来源：http://gc.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://ps.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bv.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rx.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yj.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bw.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://rl.newstarts.cn

Ruby: arr.index(x)
来源：http://qd.szsharing.cn

C#:   list.IndexOf(x);
来源：http://nl.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://nd.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cb.shtwfgs.cn


<!-- 参考信息 -->