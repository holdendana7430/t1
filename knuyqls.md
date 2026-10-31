代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vx.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xn.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ar.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fx.521024.cn

[B13] 判断是否为数字
来源：http://nd.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://co.hahajie.cn

PHP:  is_numeric($x)
来源：http://lw.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vz.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dm.9csxet.cn

Java: x instanceof Number
来源：http://xz.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nk.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://ha.szsharing.cn

C#:   x is int or double or decimal
来源：http://dg.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://qx.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sv.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ce.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://bk.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://mk.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mw.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fi.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pj.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jr.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://sa.yuntaijiaju.cn

Py:   a and b or not c
来源：http://xo.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://nu.nicolike.cn

JS:   a && b || !c
来源：http://ok.newstarts.cn

TS:   a && b || !c
来源：http://qh.bjjhwx.cn

Java: a && b || !c
来源：http://ha.newstarts.cn

Go:   a && b || !c
来源：http://sb.521024.cn

Ruby: a && b || !c
来源：http://ea.hahajie.cn

C#:   a && b || !c
来源：http://jb.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gg.jianghongdianzi.cn

Py:   if not data: return
来源：http://vw.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://dr.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://pj.shxzukj.cn

TS:   if (!data) return;
来源：http://ne.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://qo.521024.cn

Go:   if data == nil { return }
来源：http://cr.szxytkj.cn

Ruby: return if data.nil?
来源：http://rg.shxzskj.cn

C#:   if (data == null) return;
来源：http://hl.asd995.cn

================================================================================
来源：http://cm.chemitech.net.cn

C. 函数与作用域
来源：http://lu.shxzukj.cn

================================================================================
来源：http://gn.colortex.cn

[C01] 定义函数
来源：http://xw.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://rm.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cs.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://cf.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mh.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wy.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zs.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://ei.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nr.asd995.cn

[C02] 默认参数
来源：http://pv.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://zw.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qn.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://ku.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dk.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cb.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ry.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://rh.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://ya.wgjwhj.cn

[C03] 可变参数
来源：http://jn.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://zt.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qc.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://th.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://je.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zc.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://no.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sw.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zx.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://oq.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sz.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bl.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dy.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sl.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ne.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://cl.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://ii.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://gc.lnxyls.cn

[C05] 返回多个值
来源：http://bl.panjiajie.cn

Py:   return a, b
来源：http://eu.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://hb.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://il.szxytkj.cn

TS:   return { a, b };
来源：http://uh.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pv.bookmarksfly.cn

Go:   return a, b
来源：http://xt.shtwfgs.cn

Ruby: return a, b
来源：http://gk.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://ce.colortex.cn

[C06] 匿名函数 / lambda
来源：http://jb.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://ii.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pb.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://ss.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://ak.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uu.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uj.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://cu.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kn.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://xa.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://af.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qj.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wo.huixiangedu.cn

TS:   arr.map(String)
来源：http://ga.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fe.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ux.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://oe.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sj.shxzukj.cn

[C08] 闭包
来源：http://vy.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://te.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://co.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xa.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ap.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ao.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rz.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oy.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fx.huanxung.cn

[C09] 递归
来源：http://kd.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vw.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wz.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bv.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pi.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oo.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gj.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bm.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tn.nicolike.cn

[C10] 变量作用域
来源：http://bp.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wo.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ce.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lv.shxzskj.cn

TS:   同 JS
来源：http://vq.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://lu.newstarts.cn

Go:   花括号块级作用域
来源：http://nh.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zj.hnjuh.cn

C#:   块级作用域
来源：http://bn.bjjhwx.cn

[C11] 模块导入与导出
来源：http://lj.bjjhwx.cn

Py:   from module import func
来源：http://uw.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cc.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dr.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oy.bookmarksfly.cn

Java: import java.util.List;
来源：http://xs.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fe.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://fm.colortex.cn

C#:   using System.Text;
来源：http://za.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://ib.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://lo.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://ca.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://ln.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://bk.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ov.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://zo.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://sq.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cf.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://kb.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eu.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fb.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oy.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ui.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kt.hnjuh.cn

Go:   func add(a, b int) int
来源：http://on.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wy.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vi.panjiajie.cn

[C14] 泛型函数
来源：http://md.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ed.newstarts.cn

PHP:  // 无泛型
来源：http://lq.newstarts.cn

JS:   // 无泛型
来源：http://rf.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ld.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fk.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dw.shxzskj.cn

Ruby: # 无泛型
来源：http://ub.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://us.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://vg.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rt.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://qo.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bu.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ku.wgjwhj.cn

Java: // 无解构
来源：http://jt.szxytkj.cn

Go:   // 无解构
来源：http://qu.haigaiapp.cn

Ruby: a, b = pair
来源：http://qi.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://fz.szsharing.cn

[C16] 函数 / 方法重载
来源：http://xz.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nn.bjjhwx.cn

PHP:  // 无重载
来源：http://tb.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sz.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://zt.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gz.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://oj.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://ui.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://av.colortex.cn

================================================================================
来源：http://jj.asd995.cn

D. 数组 / 列表 / 集合
来源：http://ao.huanxung.cn

================================================================================
来源：http://vz.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://lq.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wh.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cq.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mz.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yq.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vz.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://bk.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://cm.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cd.asd995.cn

[D02] 追加元素到末尾
来源：http://nh.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lr.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bw.szxytkj.cn

JS:   arr.push(4);
来源：http://eo.huixiangedu.cn

TS:   arr.push(4);
来源：http://ut.szxytkj.cn

Java: list.add(4);
来源：http://gu.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://xh.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://gh.jctech888.com.cn

C#:   list.Add(4);
来源：http://cj.hahajie.cn

[D03] 在指定位置插入元素
来源：http://sf.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://bm.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nn.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ko.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://wu.chemitech.net.cn

Java: list.add(0, 0);
来源：http://am.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ar.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ca.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://we.asd995.cn

[D04] 删除元素
来源：http://iu.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lh.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fm.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://et.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://db.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mz.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wv.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hn.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ut.szsharing.cn

[D05] 访问与修改元素
来源：http://de.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mj.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uq.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ho.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://fv.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://fo.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://lm.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vj.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oa.hahajie.cn

[D06] 数组长度
来源：http://mr.bjjhwx.cn

Py:   len(arr)
来源：http://pv.9csxet.cn

PHP:  count($arr);
来源：http://rj.haigaiapp.cn

JS:   arr.length
来源：http://cr.huixiangedu.cn

TS:   arr.length
来源：http://et.colortex.cn

Java: list.size();
来源：http://kt.chemitech.net.cn

Go:   len(arr)
来源：http://gk.huanxung.cn

Ruby: arr.length; arr.size
来源：http://ar.nszjky.cn

C#:   list.Count;
来源：http://xs.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://vn.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fn.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://av.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://jy.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://bb.hahajie.cn

Java: list.subList(1, 4);
来源：http://mx.asd995.cn

Go:   arr[1:4]
来源：http://gn.huanxung.cn

Ruby: arr[1, 3]
来源：http://pw.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://uf.yuexingan06.cn

[D08] 合并两个数组
来源：http://sh.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://pf.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://ic.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ak.asd995.cn

TS:   [...a, ...b];
来源：http://yz.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mb.colortex.cn

Go:   append(a, b...)
来源：http://sm.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://bx.521024.cn

C#:   a.Concat(b).ToList()
来源：http://yw.szsharing.cn

[D09] 排序（升序）
来源：http://fr.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://um.newstarts.cn

PHP:  sort($arr);
来源：http://sn.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dp.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gt.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wq.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ql.szxytkj.cn

Ruby: arr.sort
来源：http://hg.asd995.cn

C#:   list.Sort();
来源：http://nn.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dp.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oe.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yc.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://it.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fm.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qx.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jj.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pr.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xv.gzmigu.cn

[D11] 反转数组
来源：http://yl.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ym.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://en.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ji.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://gi.szxytkj.cn

Java: Collections.reverse(list);
来源：http://ha.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://il.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://wn.colortex.cn

C#:   list.Reverse();
来源：http://ym.gzmigu.cn

[D12] 查找元素下标
来源：http://gr.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://yl.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bb.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rn.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ez.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eg.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://lt.chemitech.net.cn

Ruby: arr.index(x)
来源：http://gp.asd995.cn

C#:   list.IndexOf(x);
来源：http://sk.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://yf.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vq.jianghongdianzi.cn


<!-- 参考信息 -->