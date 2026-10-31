代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://cw.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cy.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cq.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ar.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ef.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oa.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yb.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ba.nicolike.cn

[B13] 判断是否为数字
来源：http://rx.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://zd.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://de.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oi.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pe.lnxyls.cn

Java: x instanceof Number
来源：http://dw.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fj.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://or.shxzskj.cn

C#:   x is int or double or decimal
来源：http://pl.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://vb.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fv.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lz.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://kv.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://cm.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wd.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://av.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qo.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://od.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://xs.521024.cn

Py:   a and b or not c
来源：http://kv.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://zg.lnxyls.cn

JS:   a && b || !c
来源：http://dx.gzmigu.cn

TS:   a && b || !c
来源：http://yo.bookmarksfly.cn

Java: a && b || !c
来源：http://cs.yuexingan06.cn

Go:   a && b || !c
来源：http://rm.szxytkj.cn

Ruby: a && b || !c
来源：http://kl.yuexingan06.cn

C#:   a && b || !c
来源：http://jk.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wu.muxihuayi.cn

Py:   if not data: return
来源：http://xi.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://sk.jctech888.com.cn

JS:   if (!data) return;
来源：http://fx.lnxyls.cn

TS:   if (!data) return;
来源：http://hi.yuexingan06.cn

Java: if (data == null) return;
来源：http://of.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://aa.asd995.cn

Ruby: return if data.nil?
来源：http://jq.panjiajie.cn

C#:   if (data == null) return;
来源：http://ev.jctech888.com.cn

================================================================================
来源：http://bv.newstarts.cn

C. 函数与作用域
来源：http://pw.panjiajie.cn

================================================================================
来源：http://vl.huixinmuqiang.cn

[C01] 定义函数
来源：http://jl.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://fm.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uq.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://xu.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mt.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fl.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cs.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://xg.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mf.yuexingan06.cn

[C02] 默认参数
来源：http://ny.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://yk.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hw.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://nf.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wk.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nn.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jz.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://ku.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://hc.shxzskj.cn

[C03] 可变参数
来源：http://dc.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://gf.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yc.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yc.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ty.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lc.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wg.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cd.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uq.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://ao.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wj.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xb.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://re.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uo.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://br.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://zc.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://ux.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://db.newstarts.cn

[C05] 返回多个值
来源：http://fy.521024.cn

Py:   return a, b
来源：http://ev.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://fq.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pj.hahajie.cn

TS:   return { a, b };
来源：http://qk.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pj.huanxung.cn

Go:   return a, b
来源：http://hw.9csxet.cn

Ruby: return a, b
来源：http://iv.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://bn.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://wh.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://ey.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cs.huanxung.cn

JS:   const square = x => x * x;
来源：http://vo.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://eq.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gq.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uc.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://nc.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qp.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://iy.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ja.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tm.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nl.colortex.cn

TS:   arr.map(String)
来源：http://gp.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vc.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uj.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://ut.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cn.chemitech.net.cn

[C08] 闭包
来源：http://qs.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xj.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wa.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qu.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ps.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iz.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wx.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dm.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vh.huanxung.cn

[C09] 递归
来源：http://da.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ci.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eh.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://su.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wq.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pu.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://di.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fp.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rk.521024.cn

[C10] 变量作用域
来源：http://ov.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mc.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xa.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bn.nszjky.cn

TS:   同 JS
来源：http://ny.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://oj.shtwfgs.cn

Go:   花括号块级作用域
来源：http://pp.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jq.colortex.cn

C#:   块级作用域
来源：http://ho.hahajie.cn

[C11] 模块导入与导出
来源：http://jm.panjiajie.cn

Py:   from module import func
来源：http://dg.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vu.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ll.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zt.shxzukj.cn

Java: import java.util.List;
来源：http://kp.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rz.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://ia.huixinmuqiang.cn

C#:   using System.Text;
来源：http://bo.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://xa.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://ad.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://gv.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://zt.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://vq.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ka.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://sa.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://jj.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cx.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://sw.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://se.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gk.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kh.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gz.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ez.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://fz.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uo.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fp.haigaiapp.cn

[C14] 泛型函数
来源：http://zk.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ub.muxihuayi.cn

PHP:  // 无泛型
来源：http://oo.newstarts.cn

JS:   // 无泛型
来源：http://vu.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kf.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ze.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vz.bjjhwx.cn

Ruby: # 无泛型
来源：http://hr.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://or.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://bf.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tk.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://lp.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vk.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qe.521024.cn

Java: // 无解构
来源：http://aq.bookmarksfly.cn

Go:   // 无解构
来源：http://nz.gzmigu.cn

Ruby: a, b = pair
来源：http://iz.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://en.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://in.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ij.nicolike.cn

PHP:  // 无重载
来源：http://sn.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pf.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://wj.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ul.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://oq.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://nf.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xj.shxzskj.cn

================================================================================
来源：http://cj.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://ll.bookmarksfly.cn

================================================================================
来源：http://uc.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://zj.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ld.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ha.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vr.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kn.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wy.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://td.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://fz.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hp.lnxyls.cn

[D02] 追加元素到末尾
来源：http://pa.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vj.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ja.jctech888.com.cn

JS:   arr.push(4);
来源：http://ky.huixiangedu.cn

TS:   arr.push(4);
来源：http://ge.muxihuayi.cn

Java: list.add(4);
来源：http://kp.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://jr.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://di.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://oc.9csxet.cn

[D03] 在指定位置插入元素
来源：http://vv.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://gf.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ti.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cm.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://et.muxihuayi.cn

Java: list.add(0, 0);
来源：http://kq.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gk.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zs.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://bt.szxytkj.cn

[D04] 删除元素
来源：http://nq.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vg.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://go.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ol.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://ec.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jq.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://su.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://br.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kk.colortex.cn

[D05] 访问与修改元素
来源：http://dy.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bd.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oi.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ax.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://no.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://za.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ln.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://td.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vg.panjiajie.cn

[D06] 数组长度
来源：http://vq.jianghongdianzi.cn

Py:   len(arr)
来源：http://xt.lnxyls.cn

PHP:  count($arr);
来源：http://qq.haigaiapp.cn

JS:   arr.length
来源：http://ui.asd995.cn

TS:   arr.length
来源：http://aw.haigaiapp.cn

Java: list.size();
来源：http://up.panjiajie.cn

Go:   len(arr)
来源：http://rw.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://bp.shxzukj.cn

C#:   list.Count;
来源：http://if.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://cr.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ig.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://es.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://us.521024.cn

TS:   arr.slice(1, 4);
来源：http://oh.shxzukj.cn

Java: list.subList(1, 4);
来源：http://qm.gzmigu.cn

Go:   arr[1:4]
来源：http://ki.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://xr.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://pu.wgjwhj.cn

[D08] 合并两个数组
来源：http://bm.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://is.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://au.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pn.bjjhwx.cn

TS:   [...a, ...b];
来源：http://ru.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ft.szsharing.cn

Go:   append(a, b...)
来源：http://xm.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://dn.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://yn.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://sf.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://ff.bookmarksfly.cn

PHP:  sort($arr);
来源：http://wl.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fa.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ey.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wk.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ra.nszjky.cn

Ruby: arr.sort
来源：http://ba.huixinmuqiang.cn

C#:   list.Sort();
来源：http://jm.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ja.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lu.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qh.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fo.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xd.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hr.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pn.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gx.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ck.colortex.cn

[D11] 反转数组
来源：http://jh.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bw.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://zx.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jl.hnjuh.cn

TS:   [...arr].reverse();
来源：http://we.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://cx.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://ot.muxihuayi.cn

Ruby: arr.reverse
来源：http://we.panjiajie.cn

C#:   list.Reverse();
来源：http://ri.wgjwhj.cn

[D12] 查找元素下标
来源：http://mg.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://fx.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vo.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mw.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rh.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cz.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://gi.huixiangedu.cn


<!-- 参考信息 -->