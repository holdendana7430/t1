代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://qv.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hw.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nv.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uy.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://my.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kd.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ov.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ux.huixiangedu.cn

[B13] 判断是否为数字
来源：http://nl.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ut.lnxyls.cn

PHP:  is_numeric($x)
来源：http://ap.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://el.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ss.lnxyls.cn

Java: x instanceof Number
来源：http://uf.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hs.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://is.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://va.huanxung.cn

[B14] 判断值是否在集合内
来源：http://yz.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jk.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ye.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://kc.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://vf.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jp.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hq.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gq.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ig.huanxung.cn

[B15] 布尔运算与取反
来源：http://aa.huixiangedu.cn

Py:   a and b or not c
来源：http://vl.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://fk.lnxyls.cn

JS:   a && b || !c
来源：http://vw.521024.cn

TS:   a && b || !c
来源：http://fx.bookmarksfly.cn

Java: a && b || !c
来源：http://ti.huixiangedu.cn

Go:   a && b || !c
来源：http://vr.muxihuayi.cn

Ruby: a && b || !c
来源：http://ra.colortex.cn

C#:   a && b || !c
来源：http://al.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rl.colortex.cn

Py:   if not data: return
来源：http://ox.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://dl.hahajie.cn

JS:   if (!data) return;
来源：http://hc.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://es.shxzskj.cn

Java: if (data == null) return;
来源：http://mk.nicolike.cn

Go:   if data == nil { return }
来源：http://nu.hnjuh.cn

Ruby: return if data.nil?
来源：http://ol.shxzskj.cn

C#:   if (data == null) return;
来源：http://qb.bjjhwx.cn

================================================================================
来源：http://et.521024.cn

C. 函数与作用域
来源：http://hz.panjiajie.cn

================================================================================
来源：http://sw.szxytkj.cn

[C01] 定义函数
来源：http://vm.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://xn.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mt.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://lg.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sf.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hj.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ww.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://un.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ci.jianghongdianzi.cn

[C02] 默认参数
来源：http://wi.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://ch.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dl.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://ap.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://me.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://en.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ar.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://zk.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://fh.shxzskj.cn

[C03] 可变参数
来源：http://cu.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://bv.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uv.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dn.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uu.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bh.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rn.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hp.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wg.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://qf.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pv.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fb.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xa.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oo.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://iy.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://ao.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://wj.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://st.yuntaijiaju.cn

[C05] 返回多个值
来源：http://fs.jctech888.com.cn

Py:   return a, b
来源：http://wg.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://cb.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vg.521024.cn

TS:   return { a, b };
来源：http://wo.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ma.huixiangedu.cn

Go:   return a, b
来源：http://hy.huixiangedu.cn

Ruby: return a, b
来源：http://tn.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://cp.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://oz.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://va.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wj.szsharing.cn

JS:   const square = x => x * x;
来源：http://og.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://ec.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pu.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ow.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://eq.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://in.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://nk.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://km.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sl.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ea.haigaiapp.cn

TS:   arr.map(String)
来源：http://ma.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fl.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pd.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://cm.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jn.colortex.cn

[C08] 闭包
来源：http://wg.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://va.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rg.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cy.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nh.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zt.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zx.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wa.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mb.gzmigu.cn

[C09] 递归
来源：http://ek.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zn.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pe.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mg.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fn.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uz.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cu.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cs.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ii.nszjky.cn

[C10] 变量作用域
来源：http://qh.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wd.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uz.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ri.huanxung.cn

TS:   同 JS
来源：http://mx.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://tx.shxzskj.cn

Go:   花括号块级作用域
来源：http://sz.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qq.haigaiapp.cn

C#:   块级作用域
来源：http://mg.muxihuayi.cn

[C11] 模块导入与导出
来源：http://fk.shxzskj.cn

Py:   from module import func
来源：http://bw.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bd.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ip.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://th.chemitech.net.cn

Java: import java.util.List;
来源：http://dr.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yh.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://bc.huixinmuqiang.cn

C#:   using System.Text;
来源：http://vs.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://eu.asd995.cn

Py:   (lambda: print("run"))()
来源：http://lt.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://pj.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://pl.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://wh.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qu.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://zn.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://tg.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ro.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://la.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gt.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ux.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mb.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yi.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vn.9csxet.cn

Go:   func add(a, b int) int
来源：http://hn.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tg.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sd.bookmarksfly.cn

[C14] 泛型函数
来源：http://mm.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ae.bjjhwx.cn

PHP:  // 无泛型
来源：http://ix.yuntaijiaju.cn

JS:   // 无泛型
来源：http://wk.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ex.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vr.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mn.hnjuh.cn

Ruby: # 无泛型
来源：http://sd.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wc.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://vi.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://no.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://xo.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://js.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iu.huixinmuqiang.cn

Java: // 无解构
来源：http://wo.huixinmuqiang.cn

Go:   // 无解构
来源：http://fj.9csxet.cn

Ruby: a, b = pair
来源：http://rn.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://sk.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://ow.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ef.panjiajie.cn

PHP:  // 无重载
来源：http://ud.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ge.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ez.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yv.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://hz.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://kh.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wd.hahajie.cn

================================================================================
来源：http://wh.asd995.cn

D. 数组 / 列表 / 集合
来源：http://tf.colortex.cn

================================================================================
来源：http://lq.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://et.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tg.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wb.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zi.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://os.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qj.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://yg.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://hd.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uo.hnjuh.cn

[D02] 追加元素到末尾
来源：http://yq.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jj.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dn.szsharing.cn

JS:   arr.push(4);
来源：http://jx.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://aa.gzmigu.cn

Java: list.add(4);
来源：http://bz.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://xd.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://ys.bjjhwx.cn

C#:   list.Add(4);
来源：http://wz.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://hl.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://tu.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ww.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://de.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://rh.colortex.cn

Java: list.add(0, 0);
来源：http://bq.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ga.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zt.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://jl.yuntaijiaju.cn

[D04] 删除元素
来源：http://va.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yy.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://th.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ak.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://kz.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ph.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ds.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pf.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yn.521024.cn

[D05] 访问与修改元素
来源：http://qy.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vi.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xg.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fc.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ii.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://im.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://sx.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vj.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kb.shtwfgs.cn

[D06] 数组长度
来源：http://td.shxzukj.cn

Py:   len(arr)
来源：http://gq.huixinmuqiang.cn

PHP:  count($arr);
来源：http://ie.nszjky.cn

JS:   arr.length
来源：http://sq.shtwfgs.cn

TS:   arr.length
来源：http://ww.shtwfgs.cn

Java: list.size();
来源：http://oc.asd995.cn

Go:   len(arr)
来源：http://rl.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://om.newstarts.cn

C#:   list.Count;
来源：http://yo.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://vr.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qg.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zs.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://qb.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://sn.shxzskj.cn

Java: list.subList(1, 4);
来源：http://so.wgjwhj.cn

Go:   arr[1:4]
来源：http://ir.shxzskj.cn

Ruby: arr[1, 3]
来源：http://cs.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://aw.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://xw.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://if.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://sk.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://le.nicolike.cn

TS:   [...a, ...b];
来源：http://hw.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gd.newstarts.cn

Go:   append(a, b...)
来源：http://oj.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://ua.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://np.hahajie.cn

[D09] 排序（升序）
来源：http://tn.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://nd.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://pd.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dn.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xm.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rl.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sv.bookmarksfly.cn

Ruby: arr.sort
来源：http://ef.lnxyls.cn

C#:   list.Sort();
来源：http://jy.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://um.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yw.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sj.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rx.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pa.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bn.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gz.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xr.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://en.nszjky.cn

[D11] 反转数组
来源：http://ur.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iu.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://gv.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gr.newstarts.cn

TS:   [...arr].reverse();
来源：http://dk.521024.cn

Java: Collections.reverse(list);
来源：http://er.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://xm.szxytkj.cn

Ruby: arr.reverse
来源：http://oz.chemitech.net.cn

C#:   list.Reverse();
来源：http://ex.panjiajie.cn

[D12] 查找元素下标
来源：http://mh.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://nv.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gs.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wj.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xr.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pj.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://sv.colortex.cn


<!-- 参考信息 -->