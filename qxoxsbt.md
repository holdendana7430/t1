代发 wailian999

[B13] 判断是否为数字
来源：http://wq.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://jz.asd995.cn

PHP:  is_numeric($x)
来源：http://ks.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ja.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wq.nicolike.cn

Java: x instanceof Number
来源：http://ck.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ec.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://oi.nszjky.cn

C#:   x is int or double or decimal
来源：http://or.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://tr.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hy.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ou.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://ic.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://of.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nf.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fb.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wt.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wg.huanxung.cn

[B15] 布尔运算与取反
来源：http://wm.muxihuayi.cn

Py:   a and b or not c
来源：http://pc.hahajie.cn

PHP:  $a && $b || !$c
来源：http://lb.yuexingan06.cn

JS:   a && b || !c
来源：http://ok.shxzskj.cn

TS:   a && b || !c
来源：http://vd.nicolike.cn

Java: a && b || !c
来源：http://yc.nszjky.cn

Go:   a && b || !c
来源：http://ik.shxzskj.cn

Ruby: a && b || !c
来源：http://ym.muxihuayi.cn

C#:   a && b || !c
来源：http://lt.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vc.asd995.cn

Py:   if not data: return
来源：http://ol.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://wa.shxzukj.cn

JS:   if (!data) return;
来源：http://yl.9csxet.cn

TS:   if (!data) return;
来源：http://ue.asd995.cn

Java: if (data == null) return;
来源：http://hn.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://yb.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://tp.bjjhwx.cn

C#:   if (data == null) return;
来源：http://ye.yuexingan06.cn

================================================================================
来源：http://fj.muxihuayi.cn

C. 函数与作用域
来源：http://md.muxihuayi.cn

================================================================================
来源：http://eh.szxytkj.cn

[C01] 定义函数
来源：http://tx.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://sc.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://es.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://yi.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yn.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ja.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cn.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://on.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kt.huixinmuqiang.cn

[C02] 默认参数
来源：http://dv.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://kj.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lw.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://hb.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://on.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dk.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://db.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://lk.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://aj.wgjwhj.cn

[C03] 可变参数
来源：http://ws.521024.cn

Py:   def total(*args): return sum(args)
来源：http://hh.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kq.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kf.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wi.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ik.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ie.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ud.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hr.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://to.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://le.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ok.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wk.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ce.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://pz.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://li.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://tc.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://np.haigaiapp.cn

[C05] 返回多个值
来源：http://nu.chemitech.net.cn

Py:   return a, b
来源：http://bw.panjiajie.cn

PHP:  return [$a, $b];
来源：http://ud.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ep.shxzukj.cn

TS:   return { a, b };
来源：http://xa.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yt.szxytkj.cn

Go:   return a, b
来源：http://ek.muxihuayi.cn

Ruby: return a, b
来源：http://xb.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://xj.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://ua.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://bw.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iq.9csxet.cn

JS:   const square = x => x * x;
来源：http://jt.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://gq.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ce.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ft.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://bw.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sz.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://sg.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cj.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://do.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://do.szxytkj.cn

TS:   arr.map(String)
来源：http://dq.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aa.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ay.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://xd.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qb.gzmigu.cn

[C08] 闭包
来源：http://zt.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uf.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ir.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ot.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ju.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sd.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gw.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ny.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sw.huixinmuqiang.cn

[C09] 递归
来源：http://ap.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qq.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rs.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iv.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vy.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pk.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fg.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cm.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lx.521024.cn

[C10] 变量作用域
来源：http://ja.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://va.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sq.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cm.muxihuayi.cn

TS:   同 JS
来源：http://zg.hahajie.cn

Java: 方法内为块级作用域
来源：http://hv.jctech888.com.cn

Go:   花括号块级作用域
来源：http://iq.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ka.gzmigu.cn

C#:   块级作用域
来源：http://al.panjiajie.cn

[C11] 模块导入与导出
来源：http://jb.huanxung.cn

Py:   from module import func
来源：http://zv.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dg.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ow.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sy.newstarts.cn

Java: import java.util.List;
来源：http://uo.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sh.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://hr.yuexingan06.cn

C#:   using System.Text;
来源：http://tm.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://cu.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://zl.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://xw.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://ro.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://sg.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ci.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://jw.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://df.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dx.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://yn.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yv.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ki.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ug.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gp.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://ow.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ni.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sg.asd995.cn

[C14] 泛型函数
来源：http://nr.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ni.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://vr.9csxet.cn

JS:   // 无泛型
来源：http://ba.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dp.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wq.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://im.521024.cn

Ruby: # 无泛型
来源：http://ea.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pk.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://uy.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dl.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://za.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bc.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ss.huixinmuqiang.cn

Java: // 无解构
来源：http://xm.yuexingan06.cn

Go:   // 无解构
来源：http://ni.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://jb.9csxet.cn

C#:   var (a, b) = pair;
来源：http://la.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://bu.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gw.nszjky.cn

PHP:  // 无重载
来源：http://oo.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bv.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://cn.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rs.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://ta.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://xv.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yr.hnjuh.cn

================================================================================
来源：http://kg.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://dr.nicolike.cn

================================================================================
来源：http://yv.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://ze.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qq.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wn.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uu.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bd.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yk.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://ft.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://pt.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fg.nszjky.cn

[D02] 追加元素到末尾
来源：http://od.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ze.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gi.nicolike.cn

JS:   arr.push(4);
来源：http://pj.haigaiapp.cn

TS:   arr.push(4);
来源：http://vz.szxytkj.cn

Java: list.add(4);
来源：http://cs.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://zw.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://wa.bjjhwx.cn

C#:   list.Add(4);
来源：http://ey.9csxet.cn

[D03] 在指定位置插入元素
来源：http://qy.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://wk.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bc.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pf.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://iv.haigaiapp.cn

Java: list.add(0, 0);
来源：http://jy.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dz.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qe.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://wr.shxzskj.cn

[D04] 删除元素
来源：http://ba.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ak.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aq.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://as.521024.cn

TS:   arr.splice(0, 1);
来源：http://rv.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ao.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ra.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ul.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ej.jctech888.com.cn

[D05] 访问与修改元素
来源：http://kj.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vi.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mb.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kd.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://pz.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://wg.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ap.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rl.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zn.panjiajie.cn

[D06] 数组长度
来源：http://dj.shtwfgs.cn

Py:   len(arr)
来源：http://ek.panjiajie.cn

PHP:  count($arr);
来源：http://vs.szsharing.cn

JS:   arr.length
来源：http://fu.huanxung.cn

TS:   arr.length
来源：http://lu.jctech888.com.cn

Java: list.size();
来源：http://mj.9csxet.cn

Go:   len(arr)
来源：http://cl.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://hn.bjjhwx.cn

C#:   list.Count;
来源：http://ub.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://ap.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tn.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cu.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://lz.asd995.cn

TS:   arr.slice(1, 4);
来源：http://ou.9csxet.cn

Java: list.subList(1, 4);
来源：http://gm.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://ta.shxzukj.cn

Ruby: arr[1, 3]
来源：http://hf.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://js.shxzskj.cn

[D08] 合并两个数组
来源：http://xm.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://sp.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://ac.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vg.muxihuayi.cn

TS:   [...a, ...b];
来源：http://xe.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ax.huanxung.cn

Go:   append(a, b...)
来源：http://lb.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://dm.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://xu.panjiajie.cn

[D09] 排序（升序）
来源：http://yy.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://bz.gzmigu.cn

PHP:  sort($arr);
来源：http://cm.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cj.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gf.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nv.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vy.wgjwhj.cn

Ruby: arr.sort
来源：http://bv.gzmigu.cn

C#:   list.Sort();
来源：http://kx.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tr.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ss.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kp.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pb.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ws.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qu.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zu.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xh.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://et.huixiangedu.cn

[D11] 反转数组
来源：http://fd.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xn.szsharing.cn

PHP:  array_reverse($arr);
来源：http://py.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jy.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://nw.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://tc.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://yi.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://tj.521024.cn

C#:   list.Reverse();
来源：http://xn.shxzukj.cn

[D12] 查找元素下标
来源：http://un.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://bn.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://md.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cv.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ou.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://az.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://et.nicolike.cn

Ruby: arr.index(x)
来源：http://qk.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://si.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://yk.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://on.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gc.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://bg.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://ec.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uf.huanxung.cn


<!-- 参考信息 -->