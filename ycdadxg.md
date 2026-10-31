代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://np.panjiajie.cn

Java: x instanceof Number
来源：http://ar.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wv.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://pt.9csxet.cn

C#:   x is int or double or decimal
来源：http://pn.hahajie.cn

[B14] 判断值是否在集合内
来源：http://rw.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yn.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gb.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://ed.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://kr.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pg.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ya.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gw.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rm.hahajie.cn

[B15] 布尔运算与取反
来源：http://pk.huixiangedu.cn

Py:   a and b or not c
来源：http://jx.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://re.shxzskj.cn

JS:   a && b || !c
来源：http://mo.huanxung.cn

TS:   a && b || !c
来源：http://va.huixiangedu.cn

Java: a && b || !c
来源：http://ic.9csxet.cn

Go:   a && b || !c
来源：http://cx.shtwfgs.cn

Ruby: a && b || !c
来源：http://vc.huixinmuqiang.cn

C#:   a && b || !c
来源：http://th.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qe.nszjky.cn

Py:   if not data: return
来源：http://vv.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://qs.hnjuh.cn

JS:   if (!data) return;
来源：http://xz.asd995.cn

TS:   if (!data) return;
来源：http://ua.muxihuayi.cn

Java: if (data == null) return;
来源：http://fw.shxzukj.cn

Go:   if data == nil { return }
来源：http://wo.chemitech.net.cn

Ruby: return if data.nil?
来源：http://fv.haigaiapp.cn

C#:   if (data == null) return;
来源：http://ny.9csxet.cn

================================================================================
来源：http://ur.haigaiapp.cn

C. 函数与作用域
来源：http://ia.hahajie.cn

================================================================================
来源：http://oz.hahajie.cn

[C01] 定义函数
来源：http://ya.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://ac.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ld.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ey.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hp.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zz.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xk.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://pp.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://th.szxytkj.cn

[C02] 默认参数
来源：http://xg.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://hk.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gu.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://zw.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bc.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ku.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mj.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://wk.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://oe.asd995.cn

[C03] 可变参数
来源：http://md.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://pq.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ht.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gp.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sn.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xm.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ms.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mg.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ci.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://ph.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hx.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://me.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wm.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://he.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://um.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://co.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://zu.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://hx.9csxet.cn

[C05] 返回多个值
来源：http://ix.bjjhwx.cn

Py:   return a, b
来源：http://ug.hahajie.cn

PHP:  return [$a, $b];
来源：http://fd.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ze.szxytkj.cn

TS:   return { a, b };
来源：http://hn.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ze.bookmarksfly.cn

Go:   return a, b
来源：http://xp.lnxyls.cn

Ruby: return a, b
来源：http://yp.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://dr.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://ke.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://pu.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cg.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://uu.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://tg.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cn.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vx.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://my.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nq.hahajie.cn

[C07] 把函数作为参数传入
来源：http://fr.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zv.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ro.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rq.huixiangedu.cn

TS:   arr.map(String)
来源：http://hp.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ee.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uc.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://nz.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rf.gzmigu.cn

[C08] 闭包
来源：http://uy.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ss.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lf.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fc.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sd.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nt.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mb.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hs.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://op.521024.cn

[C09] 递归
来源：http://fl.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nt.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://my.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qd.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vl.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sr.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hn.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kd.szsharing.cn

[C10] 变量作用域
来源：http://cy.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vv.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ud.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dp.9csxet.cn

TS:   同 JS
来源：http://uh.szxytkj.cn

Java: 方法内为块级作用域
来源：http://rw.shtwfgs.cn

Go:   花括号块级作用域
来源：http://to.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hs.nszjky.cn

C#:   块级作用域
来源：http://qj.hahajie.cn

[C11] 模块导入与导出
来源：http://kw.shxzskj.cn

Py:   from module import func
来源：http://nd.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xr.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ke.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lz.yuntaijiaju.cn

Java: import java.util.List;
来源：http://eu.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uw.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://bn.chemitech.net.cn

C#:   using System.Text;
来源：http://fv.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://hm.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://ok.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://pd.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://nv.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://rg.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bi.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://fq.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://co.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cp.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://lb.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gm.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wy.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ex.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bd.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ap.hnjuh.cn

Go:   func add(a, b int) int
来源：http://ze.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ng.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fk.jianghongdianzi.cn

[C14] 泛型函数
来源：http://cg.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jz.huanxung.cn

PHP:  // 无泛型
来源：http://pq.shtwfgs.cn

JS:   // 无泛型
来源：http://jj.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ix.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vd.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pm.nszjky.cn

Ruby: # 无泛型
来源：http://tv.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lr.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://ik.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tb.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://lv.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bj.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://en.bookmarksfly.cn

Java: // 无解构
来源：http://xk.gzmigu.cn

Go:   // 无解构
来源：http://ek.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://gx.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://pn.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://zh.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qt.yuexingan06.cn

PHP:  // 无重载
来源：http://if.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mp.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://kd.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sn.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://re.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://gf.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zr.colortex.cn

================================================================================
来源：http://sm.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://hl.9csxet.cn

================================================================================
来源：http://gw.huanxung.cn

[D01] 创建数组 / 列表
来源：http://zf.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ph.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://td.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qr.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uu.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yz.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://sg.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://wa.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wy.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://ar.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ej.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://la.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://bk.9csxet.cn

TS:   arr.push(4);
来源：http://mv.jianghongdianzi.cn

Java: list.add(4);
来源：http://fx.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://gq.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://wn.muxihuayi.cn

C#:   list.Add(4);
来源：http://jn.nszjky.cn

[D03] 在指定位置插入元素
来源：http://kl.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://sl.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yu.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mf.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://vc.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://nz.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dw.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bt.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://lv.9csxet.cn

[D04] 删除元素
来源：http://lk.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ut.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dr.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qq.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://zg.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hp.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://km.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wz.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rk.9csxet.cn

[D05] 访问与修改元素
来源：http://tp.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://za.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jk.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kh.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://vf.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ii.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://pj.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lv.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oo.shtwfgs.cn

[D06] 数组长度
来源：http://jz.wgjwhj.cn

Py:   len(arr)
来源：http://cw.jianghongdianzi.cn

PHP:  count($arr);
来源：http://ba.hnjuh.cn

JS:   arr.length
来源：http://na.newstarts.cn

TS:   arr.length
来源：http://me.huixiangedu.cn

Java: list.size();
来源：http://cp.wgjwhj.cn

Go:   len(arr)
来源：http://wp.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://lf.hnjuh.cn

C#:   list.Count;
来源：http://ak.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://bo.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rv.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tj.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://ox.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://kv.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://kw.gzmigu.cn

Go:   arr[1:4]
来源：http://on.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://nq.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://zk.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://yx.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://bq.colortex.cn

PHP:  array_merge($a, $b);
来源：http://ky.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wj.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://lr.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xz.9csxet.cn

Go:   append(a, b...)
来源：http://yp.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://gf.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://vk.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://xi.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://uf.asd995.cn

PHP:  sort($arr);
来源：http://bf.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lz.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://is.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hk.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ej.bjjhwx.cn

Ruby: arr.sort
来源：http://xd.colortex.cn

C#:   list.Sort();
来源：http://kq.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ou.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lj.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dm.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://et.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wk.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gn.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ko.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mz.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hh.wgjwhj.cn

[D11] 反转数组
来源：http://vu.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dn.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://wx.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gm.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://fz.huanxung.cn

Java: Collections.reverse(list);
来源：http://gj.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://jm.huixiangedu.cn

Ruby: arr.reverse
来源：http://bd.shxzskj.cn

C#:   list.Reverse();
来源：http://zz.hahajie.cn

[D12] 查找元素下标
来源：http://yh.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://rt.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bu.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jq.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://db.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://av.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://bq.9csxet.cn

Ruby: arr.index(x)
来源：http://vn.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://xo.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://ei.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wm.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aa.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://vw.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://rc.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://os.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pr.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://do.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mm.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://ig.shxzskj.cn


<!-- 参考信息 -->