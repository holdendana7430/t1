代发 wailian999

[B13] 判断是否为数字
来源：http://ya.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://sd.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://ox.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vq.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fa.huanxung.cn

Java: x instanceof Number
来源：http://bc.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sd.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://dr.huanxung.cn

C#:   x is int or double or decimal
来源：http://ap.asd995.cn

[B14] 判断值是否在集合内
来源：http://dj.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pw.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iy.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://ix.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://gy.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cy.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gi.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qe.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sx.shxzukj.cn

[B15] 布尔运算与取反
来源：http://uk.nszjky.cn

Py:   a and b or not c
来源：http://dz.hahajie.cn

PHP:  $a && $b || !$c
来源：http://dx.521024.cn

JS:   a && b || !c
来源：http://bj.yuntaijiaju.cn

TS:   a && b || !c
来源：http://vm.panjiajie.cn

Java: a && b || !c
来源：http://os.yuexingan06.cn

Go:   a && b || !c
来源：http://rt.huixiangedu.cn

Ruby: a && b || !c
来源：http://qq.panjiajie.cn

C#:   a && b || !c
来源：http://mt.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rf.haigaiapp.cn

Py:   if not data: return
来源：http://il.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://zr.lnxyls.cn

JS:   if (!data) return;
来源：http://wq.muxihuayi.cn

TS:   if (!data) return;
来源：http://sn.newstarts.cn

Java: if (data == null) return;
来源：http://it.shtwfgs.cn

Go:   if data == nil { return }
来源：http://nx.hnjuh.cn

Ruby: return if data.nil?
来源：http://pr.huixiangedu.cn

C#:   if (data == null) return;
来源：http://rw.yuexingan06.cn

================================================================================
来源：http://nu.shxzskj.cn

C. 函数与作用域
来源：http://iw.szxytkj.cn

================================================================================
来源：http://yx.bookmarksfly.cn

[C01] 定义函数
来源：http://gm.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://vg.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://as.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://og.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fk.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fd.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cf.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://sz.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uw.521024.cn

[C02] 默认参数
来源：http://zt.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://ul.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tg.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://dq.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pu.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ja.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yn.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://la.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://dk.szxytkj.cn

[C03] 可变参数
来源：http://vk.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://ly.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jw.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ks.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aa.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lb.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nj.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://se.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bg.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://ph.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zb.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ji.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vh.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dt.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://ca.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://us.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://wl.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://hh.nszjky.cn

[C05] 返回多个值
来源：http://aj.yuexingan06.cn

Py:   return a, b
来源：http://ji.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://yt.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://km.nszjky.cn

TS:   return { a, b };
来源：http://em.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uo.chemitech.net.cn

Go:   return a, b
来源：http://yi.hnjuh.cn

Ruby: return a, b
来源：http://ll.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://vu.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://yu.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://ql.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vl.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://ad.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://nb.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qx.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vv.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://td.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tx.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://gs.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ns.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qi.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lg.szxytkj.cn

TS:   arr.map(String)
来源：http://kz.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rs.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://do.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://yk.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ka.wgjwhj.cn

[C08] 闭包
来源：http://ql.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lg.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ap.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hh.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jw.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ld.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bw.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vb.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tp.huixiangedu.cn

[C09] 递归
来源：http://gc.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ka.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nj.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tt.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hh.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gm.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uo.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tm.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ct.chemitech.net.cn

[C10] 变量作用域
来源：http://sv.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dl.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sx.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dz.yuntaijiaju.cn

TS:   同 JS
来源：http://px.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://se.521024.cn

Go:   花括号块级作用域
来源：http://tn.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hc.szsharing.cn

C#:   块级作用域
来源：http://ya.huanxung.cn

[C11] 模块导入与导出
来源：http://tv.shxzskj.cn

Py:   from module import func
来源：http://vs.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cu.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mj.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ji.yuexingan06.cn

Java: import java.util.List;
来源：http://cv.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lf.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://mx.wgjwhj.cn

C#:   using System.Text;
来源：http://ia.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://nv.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://qb.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://xv.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://ui.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://ak.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ik.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://oh.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://my.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xw.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://wo.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uh.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mq.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vp.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kj.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jf.newstarts.cn

Go:   func add(a, b int) int
来源：http://qs.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fe.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lu.bjjhwx.cn

[C14] 泛型函数
来源：http://to.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jv.9csxet.cn

PHP:  // 无泛型
来源：http://an.haigaiapp.cn

JS:   // 无泛型
来源：http://rs.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fp.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dm.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pe.jctech888.com.cn

Ruby: # 无泛型
来源：http://zo.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wj.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://kz.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xz.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://id.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mp.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mq.shxzskj.cn

Java: // 无解构
来源：http://oh.nicolike.cn

Go:   // 无解构
来源：http://cm.shtwfgs.cn

Ruby: a, b = pair
来源：http://oq.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://gm.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://si.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pe.yuexingan06.cn

PHP:  // 无重载
来源：http://ct.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://np.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://ak.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pd.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://zg.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://rz.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ug.lnxyls.cn

================================================================================
来源：http://on.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://su.bjjhwx.cn

================================================================================
来源：http://kp.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://gj.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qw.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://po.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qt.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://if.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cv.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://hj.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://iv.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vl.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://ee.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ix.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xc.nicolike.cn

JS:   arr.push(4);
来源：http://jb.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://so.nszjky.cn

Java: list.add(4);
来源：http://go.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://ky.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://dp.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://kg.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://yt.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://ja.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dg.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nb.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://vq.jctech888.com.cn

Java: list.add(0, 0);
来源：http://fo.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zi.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ov.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://ig.colortex.cn

[D04] 删除元素
来源：http://ma.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pt.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yx.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fy.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://ms.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tj.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nw.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bt.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cs.chemitech.net.cn

[D05] 访问与修改元素
来源：http://mc.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sz.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vq.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rf.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://gp.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://ew.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://cp.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ca.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jn.haigaiapp.cn

[D06] 数组长度
来源：http://wx.yuntaijiaju.cn

Py:   len(arr)
来源：http://px.lnxyls.cn

PHP:  count($arr);
来源：http://nx.shxzskj.cn

JS:   arr.length
来源：http://ey.colortex.cn

TS:   arr.length
来源：http://kh.szsharing.cn

Java: list.size();
来源：http://yz.lnxyls.cn

Go:   len(arr)
来源：http://hf.nicolike.cn

Ruby: arr.length; arr.size
来源：http://bq.muxihuayi.cn

C#:   list.Count;
来源：http://pf.huanxung.cn

[D07] 切片 / 取子数组
来源：http://hm.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://er.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qv.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://qh.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ke.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://xz.521024.cn

Go:   arr[1:4]
来源：http://tu.newstarts.cn

Ruby: arr[1, 3]
来源：http://ay.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://rl.yuexingan06.cn

[D08] 合并两个数组
来源：http://dz.521024.cn

Py:   a + b;  a.extend(b)
来源：http://mp.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://sd.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://az.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ie.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xu.hahajie.cn

Go:   append(a, b...)
来源：http://dn.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://wp.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://jz.haigaiapp.cn

[D09] 排序（升序）
来源：http://bg.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://sa.haigaiapp.cn

PHP:  sort($arr);
来源：http://vk.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eu.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yq.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uz.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://af.muxihuayi.cn

Ruby: arr.sort
来源：http://oe.jianghongdianzi.cn

C#:   list.Sort();
来源：http://yl.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mn.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ws.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iw.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mj.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oq.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xg.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yl.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sd.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sc.szxytkj.cn

[D11] 反转数组
来源：http://xa.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aw.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://hj.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dw.panjiajie.cn

TS:   [...arr].reverse();
来源：http://ut.szsharing.cn

Java: Collections.reverse(list);
来源：http://ps.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://gu.nszjky.cn

Ruby: arr.reverse
来源：http://te.hnjuh.cn

C#:   list.Reverse();
来源：http://bi.hnjuh.cn

[D12] 查找元素下标
来源：http://ke.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ko.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uz.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rp.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sh.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ek.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://fw.colortex.cn

Ruby: arr.index(x)
来源：http://gm.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://af.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://om.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zv.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oy.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://yh.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://fz.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://st.521024.cn


<!-- 参考信息 -->