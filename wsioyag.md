代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jw.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ex.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yb.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gn.nszjky.cn

[B13] 判断是否为数字
来源：http://hn.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://hi.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://an.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yh.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sq.huixinmuqiang.cn

Java: x instanceof Number
来源：http://uu.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qk.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://zp.newstarts.cn

C#:   x is int or double or decimal
来源：http://jp.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://wl.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ki.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ql.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ya.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://mp.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vk.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ke.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mq.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gl.lnxyls.cn

[B15] 布尔运算与取反
来源：http://fl.jianghongdianzi.cn

Py:   a and b or not c
来源：http://mx.colortex.cn

PHP:  $a && $b || !$c
来源：http://se.9csxet.cn

JS:   a && b || !c
来源：http://yx.jctech888.com.cn

TS:   a && b || !c
来源：http://uq.shxzskj.cn

Java: a && b || !c
来源：http://jb.hnjuh.cn

Go:   a && b || !c
来源：http://fh.shtwfgs.cn

Ruby: a && b || !c
来源：http://tz.lnxyls.cn

C#:   a && b || !c
来源：http://nj.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jn.hnjuh.cn

Py:   if not data: return
来源：http://zu.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://fu.gzmigu.cn

JS:   if (!data) return;
来源：http://tx.9csxet.cn

TS:   if (!data) return;
来源：http://vu.colortex.cn

Java: if (data == null) return;
来源：http://jr.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://iu.shxzskj.cn

Ruby: return if data.nil?
来源：http://yg.muxihuayi.cn

C#:   if (data == null) return;
来源：http://wn.asd995.cn

================================================================================
来源：http://ua.chemitech.net.cn

C. 函数与作用域
来源：http://en.huixiangedu.cn

================================================================================
来源：http://jf.jctech888.com.cn

[C01] 定义函数
来源：http://jy.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://xd.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://is.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://na.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cc.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wo.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zv.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://hj.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gg.colortex.cn

[C02] 默认参数
来源：http://kj.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://mj.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zq.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ii.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fy.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bb.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uk.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://sj.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://cq.gzmigu.cn

[C03] 可变参数
来源：http://fp.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://gc.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mb.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dh.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://md.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://el.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wo.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://js.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ux.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://eq.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ev.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eb.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vu.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wm.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://nh.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://dx.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://vq.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://tg.hnjuh.cn

[C05] 返回多个值
来源：http://si.shtwfgs.cn

Py:   return a, b
来源：http://my.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://vi.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sx.asd995.cn

TS:   return { a, b };
来源：http://sb.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qj.bookmarksfly.cn

Go:   return a, b
来源：http://rd.wgjwhj.cn

Ruby: return a, b
来源：http://wr.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://nj.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://hq.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://dt.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pd.panjiajie.cn

JS:   const square = x => x * x;
来源：http://mn.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://vs.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xu.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vy.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://xm.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xi.newstarts.cn

[C07] 把函数作为参数传入
来源：http://lo.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pa.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aa.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yw.chemitech.net.cn

TS:   arr.map(String)
来源：http://eo.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nf.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jn.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://eu.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wx.shxzukj.cn

[C08] 闭包
来源：http://aj.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hc.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vx.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nc.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mh.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kg.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wd.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kf.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ia.newstarts.cn

[C09] 递归
来源：http://wi.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nm.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lz.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ir.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rl.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mc.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cs.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kk.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fe.panjiajie.cn

[C10] 变量作用域
来源：http://pb.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ys.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gq.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ps.jianghongdianzi.cn

TS:   同 JS
来源：http://el.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://eu.szxytkj.cn

Go:   花括号块级作用域
来源：http://bb.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xr.bookmarksfly.cn

C#:   块级作用域
来源：http://tl.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://yv.chemitech.net.cn

Py:   from module import func
来源：http://mz.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qf.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uw.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uv.panjiajie.cn

Java: import java.util.List;
来源：http://qf.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dp.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://po.szxytkj.cn

C#:   using System.Text;
来源：http://zv.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://iq.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://jo.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://cw.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://nm.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://uh.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://un.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ez.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://gp.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ll.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://vi.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ot.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wr.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jg.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sw.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bc.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://es.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ag.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rv.bookmarksfly.cn

[C14] 泛型函数
来源：http://kl.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fo.lnxyls.cn

PHP:  // 无泛型
来源：http://mh.521024.cn

JS:   // 无泛型
来源：http://go.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cq.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yi.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fr.shxzskj.cn

Ruby: # 无泛型
来源：http://qw.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hl.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://qd.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nq.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://zq.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oh.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qs.haigaiapp.cn

Java: // 无解构
来源：http://ub.bookmarksfly.cn

Go:   // 无解构
来源：http://ny.shtwfgs.cn

Ruby: a, b = pair
来源：http://mf.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://oi.9csxet.cn

[C16] 函数 / 方法重载
来源：http://ax.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ko.521024.cn

PHP:  // 无重载
来源：http://uw.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qy.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://wm.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://si.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://xw.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://dn.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oq.yuntaijiaju.cn

================================================================================
来源：http://vi.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://zf.huixiangedu.cn

================================================================================
来源：http://fi.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://hy.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://za.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://se.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ec.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kx.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gv.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://rp.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://se.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cz.gzmigu.cn

[D02] 追加元素到末尾
来源：http://pk.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dt.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ot.chemitech.net.cn

JS:   arr.push(4);
来源：http://wx.gzmigu.cn

TS:   arr.push(4);
来源：http://uo.nicolike.cn

Java: list.add(4);
来源：http://ae.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://qo.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://ew.jctech888.com.cn

C#:   list.Add(4);
来源：http://ha.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://pb.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://ij.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://da.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aq.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://os.panjiajie.cn

Java: list.add(0, 0);
来源：http://cs.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tc.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gl.asd995.cn

C#:   list.Insert(0, 0);
来源：http://is.shtwfgs.cn

[D04] 删除元素
来源：http://xa.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rh.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ct.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cb.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://uw.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zy.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vp.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ld.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sx.newstarts.cn

[D05] 访问与修改元素
来源：http://nc.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vs.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yk.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aw.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://dh.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://oo.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://nz.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://by.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ho.haigaiapp.cn

[D06] 数组长度
来源：http://si.asd995.cn

Py:   len(arr)
来源：http://gb.yuexingan06.cn

PHP:  count($arr);
来源：http://zw.szxytkj.cn

JS:   arr.length
来源：http://pg.szxytkj.cn

TS:   arr.length
来源：http://zi.shxzukj.cn

Java: list.size();
来源：http://me.hnjuh.cn

Go:   len(arr)
来源：http://np.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://ir.huixiangedu.cn

C#:   list.Count;
来源：http://xs.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://ih.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kq.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mr.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://vv.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://hs.gzmigu.cn

Java: list.subList(1, 4);
来源：http://bs.lnxyls.cn

Go:   arr[1:4]
来源：http://un.nszjky.cn

Ruby: arr[1, 3]
来源：http://rb.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://to.shxzukj.cn

[D08] 合并两个数组
来源：http://qx.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://eo.521024.cn

PHP:  array_merge($a, $b);
来源：http://ka.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sq.szxytkj.cn

TS:   [...a, ...b];
来源：http://dl.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kl.huanxung.cn

Go:   append(a, b...)
来源：http://gm.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://ip.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://is.shtwfgs.cn

[D09] 排序（升序）
来源：http://me.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://pz.shtwfgs.cn

PHP:  sort($arr);
来源：http://mx.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mt.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fo.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xc.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uk.lnxyls.cn

Ruby: arr.sort
来源：http://fl.haigaiapp.cn

C#:   list.Sort();
来源：http://wl.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zs.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wv.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vf.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eu.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ew.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bk.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hg.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jo.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zy.9csxet.cn

[D11] 反转数组
来源：http://on.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zm.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://du.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bq.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://sm.9csxet.cn

Java: Collections.reverse(list);
来源：http://gg.colortex.cn

Go:   slices.Reverse(arr)
来源：http://dw.szsharing.cn

Ruby: arr.reverse
来源：http://pc.szxytkj.cn

C#:   list.Reverse();
来源：http://kr.shtwfgs.cn

[D12] 查找元素下标
来源：http://ci.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://wj.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://od.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vx.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ki.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://od.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://bd.521024.cn

Ruby: arr.index(x)
来源：http://jo.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://wk.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://nl.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uh.lnxyls.cn


<!-- 参考信息 -->