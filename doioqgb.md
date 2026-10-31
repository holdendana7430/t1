代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jz.nszjky.cn

Java: x instanceof Number
来源：http://jg.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kx.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://nf.nicolike.cn

C#:   x is int or double or decimal
来源：http://rp.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://qa.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tf.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bu.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://pl.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://nq.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wn.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zl.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bd.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bk.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://hi.gzmigu.cn

Py:   a and b or not c
来源：http://za.nicolike.cn

PHP:  $a && $b || !$c
来源：http://lc.nszjky.cn

JS:   a && b || !c
来源：http://xl.gzmigu.cn

TS:   a && b || !c
来源：http://je.szsharing.cn

Java: a && b || !c
来源：http://ay.yuntaijiaju.cn

Go:   a && b || !c
来源：http://ui.hahajie.cn

Ruby: a && b || !c
来源：http://jz.szxytkj.cn

C#:   a && b || !c
来源：http://iv.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://io.asd995.cn

Py:   if not data: return
来源：http://vd.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://dl.shxzskj.cn

JS:   if (!data) return;
来源：http://qm.hnjuh.cn

TS:   if (!data) return;
来源：http://nk.bjjhwx.cn

Java: if (data == null) return;
来源：http://xk.huanxung.cn

Go:   if data == nil { return }
来源：http://hb.521024.cn

Ruby: return if data.nil?
来源：http://ds.shtwfgs.cn

C#:   if (data == null) return;
来源：http://ch.jctech888.com.cn

================================================================================
来源：http://lf.huixinmuqiang.cn

C. 函数与作用域
来源：http://mj.asd995.cn

================================================================================
来源：http://ad.gzmigu.cn

[C01] 定义函数
来源：http://he.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://vt.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bd.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://bi.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ve.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bd.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://we.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://fk.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zp.nicolike.cn

[C02] 默认参数
来源：http://qz.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://un.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ow.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://bn.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ij.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ed.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fx.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://do.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://sa.szsharing.cn

[C03] 可变参数
来源：http://xv.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://gi.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bz.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://en.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qx.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mk.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uo.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vh.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gw.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://qo.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dl.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fi.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sh.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xz.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://ml.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://hh.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://re.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://ja.lnxyls.cn

[C05] 返回多个值
来源：http://tl.shtwfgs.cn

Py:   return a, b
来源：http://op.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://df.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ma.nszjky.cn

TS:   return { a, b };
来源：http://ro.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ar.jianghongdianzi.cn

Go:   return a, b
来源：http://xi.shtwfgs.cn

Ruby: return a, b
来源：http://cl.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://br.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://au.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://hx.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wp.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://am.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://nc.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zs.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://af.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://db.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://te.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://bd.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://js.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rd.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tf.szxytkj.cn

TS:   arr.map(String)
来源：http://yg.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dm.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vw.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://pf.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://of.haigaiapp.cn

[C08] 闭包
来源：http://mh.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iu.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eg.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ue.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ve.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sm.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ys.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dc.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vs.panjiajie.cn

[C09] 递归
来源：http://ky.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xu.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bd.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yb.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ss.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://on.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xi.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sq.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ve.wgjwhj.cn

[C10] 变量作用域
来源：http://bp.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ac.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ni.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bm.muxihuayi.cn

TS:   同 JS
来源：http://cg.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ku.gzmigu.cn

Go:   花括号块级作用域
来源：http://sh.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wq.jianghongdianzi.cn

C#:   块级作用域
来源：http://kp.szsharing.cn

[C11] 模块导入与导出
来源：http://au.yuexingan06.cn

Py:   from module import func
来源：http://qb.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tu.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rk.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rs.hahajie.cn

Java: import java.util.List;
来源：http://jo.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ei.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://yf.9csxet.cn

C#:   using System.Text;
来源：http://mb.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://et.asd995.cn

Py:   (lambda: print("run"))()
来源：http://wg.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://kp.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://hp.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://ul.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://go.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://yh.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://gp.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kt.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://pq.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oo.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://su.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ec.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tu.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ma.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://ya.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ef.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yj.bookmarksfly.cn

[C14] 泛型函数
来源：http://qj.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://le.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://xs.521024.cn

JS:   // 无泛型
来源：http://ja.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://te.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tk.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lp.colortex.cn

Ruby: # 无泛型
来源：http://ej.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mr.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://mf.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wr.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://fn.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lm.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fs.huixinmuqiang.cn

Java: // 无解构
来源：http://vt.shtwfgs.cn

Go:   // 无解构
来源：http://om.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://ey.hahajie.cn

C#:   var (a, b) = pair;
来源：http://lx.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://sf.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wv.wgjwhj.cn

PHP:  // 无重载
来源：http://gd.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uw.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://lb.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qq.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://ph.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://lu.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ie.hahajie.cn

================================================================================
来源：http://vk.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://lt.jctech888.com.cn

================================================================================
来源：http://ac.szsharing.cn

[D01] 创建数组 / 列表
来源：http://nz.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zk.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://db.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cc.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ds.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://af.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://dr.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ng.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ah.nszjky.cn

[D02] 追加元素到末尾
来源：http://ya.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://is.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bi.szxytkj.cn

JS:   arr.push(4);
来源：http://sk.szxytkj.cn

TS:   arr.push(4);
来源：http://mo.9csxet.cn

Java: list.add(4);
来源：http://oy.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://nu.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://vu.newstarts.cn

C#:   list.Add(4);
来源：http://nr.9csxet.cn

[D03] 在指定位置插入元素
来源：http://jh.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://pm.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mr.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hh.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://zg.haigaiapp.cn

Java: list.add(0, 0);
来源：http://fl.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gf.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bk.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://aj.szxytkj.cn

[D04] 删除元素
来源：http://oc.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://te.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sl.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://if.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://me.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mp.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ts.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ai.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hb.shxzskj.cn

[D05] 访问与修改元素
来源：http://kw.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://us.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bc.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uo.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ir.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://ca.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://cx.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gn.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sw.shxzskj.cn

[D06] 数组长度
来源：http://tg.wgjwhj.cn

Py:   len(arr)
来源：http://xo.muxihuayi.cn

PHP:  count($arr);
来源：http://bv.haigaiapp.cn

JS:   arr.length
来源：http://bv.jctech888.com.cn

TS:   arr.length
来源：http://fd.shtwfgs.cn

Java: list.size();
来源：http://sk.wgjwhj.cn

Go:   len(arr)
来源：http://bc.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://ez.newstarts.cn

C#:   list.Count;
来源：http://xu.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://dq.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yx.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hw.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://lx.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://at.hnjuh.cn

Java: list.subList(1, 4);
来源：http://ka.bookmarksfly.cn

Go:   arr[1:4]
来源：http://qn.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://nw.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://ua.shxzskj.cn

[D08] 合并两个数组
来源：http://jx.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://iq.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://vx.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qe.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://ru.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fd.hahajie.cn

Go:   append(a, b...)
来源：http://ke.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://mf.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://kg.colortex.cn

[D09] 排序（升序）
来源：http://zx.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://st.haigaiapp.cn

PHP:  sort($arr);
来源：http://aq.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tg.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kw.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lb.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kx.shxzskj.cn

Ruby: arr.sort
来源：http://mr.nszjky.cn

C#:   list.Sort();
来源：http://fu.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://na.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uw.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wl.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sq.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wk.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ka.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dn.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://md.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fx.9csxet.cn

[D11] 反转数组
来源：http://bi.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kn.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://aj.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rz.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://yx.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://by.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://ts.wgjwhj.cn

Ruby: arr.reverse
来源：http://dc.yuexingan06.cn

C#:   list.Reverse();
来源：http://yd.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://vo.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://nv.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hg.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pw.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ik.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fm.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://lc.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://gl.colortex.cn

C#:   list.IndexOf(x);
来源：http://gf.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://lp.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gx.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fo.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://zs.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://jm.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ky.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ex.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vn.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ej.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ig.shxzskj.cn


<!-- 参考信息 -->