代发 wailian999

C#:   x is int or double or decimal
来源：http://we.nszjky.cn

[B14] 判断值是否在集合内
来源：http://rj.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ze.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://po.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://wc.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://rm.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ue.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nr.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xu.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iw.hahajie.cn

[B15] 布尔运算与取反
来源：http://zf.muxihuayi.cn

Py:   a and b or not c
来源：http://zs.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://qn.521024.cn

JS:   a && b || !c
来源：http://hh.panjiajie.cn

TS:   a && b || !c
来源：http://ad.bookmarksfly.cn

Java: a && b || !c
来源：http://vv.521024.cn

Go:   a && b || !c
来源：http://xq.jctech888.com.cn

Ruby: a && b || !c
来源：http://tz.521024.cn

C#:   a && b || !c
来源：http://er.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xr.colortex.cn

Py:   if not data: return
来源：http://jl.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://su.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://nc.panjiajie.cn

TS:   if (!data) return;
来源：http://rd.hahajie.cn

Java: if (data == null) return;
来源：http://zl.asd995.cn

Go:   if data == nil { return }
来源：http://qy.hahajie.cn

Ruby: return if data.nil?
来源：http://tp.newstarts.cn

C#:   if (data == null) return;
来源：http://zd.gzmigu.cn

================================================================================
来源：http://yd.yuexingan06.cn

C. 函数与作用域
来源：http://ag.521024.cn

================================================================================
来源：http://bf.nszjky.cn

[C01] 定义函数
来源：http://zt.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://ry.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nk.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://di.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ri.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ah.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zh.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://qy.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fu.haigaiapp.cn

[C02] 默认参数
来源：http://px.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://pl.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xv.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ss.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qc.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wb.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mn.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://ds.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://sy.muxihuayi.cn

[C03] 可变参数
来源：http://gx.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://tt.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://if.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aw.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rd.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wi.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yt.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hr.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tf.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://oh.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dz.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jn.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uc.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sb.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://uv.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://ng.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://vt.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://bw.chemitech.net.cn

[C05] 返回多个值
来源：http://yj.shxzskj.cn

Py:   return a, b
来源：http://wh.asd995.cn

PHP:  return [$a, $b];
来源：http://ge.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vi.yuexingan06.cn

TS:   return { a, b };
来源：http://he.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pq.newstarts.cn

Go:   return a, b
来源：http://sn.hahajie.cn

Ruby: return a, b
来源：http://dt.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://kb.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://sd.9csxet.cn

Py:   square = lambda x: x * x
来源：http://xs.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://el.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://yt.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://ff.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://re.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wf.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://qv.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wt.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://fl.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://do.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ra.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uy.asd995.cn

TS:   arr.map(String)
来源：http://th.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ru.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kj.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://lf.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sq.wgjwhj.cn

[C08] 闭包
来源：http://et.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://il.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lo.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rr.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tn.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zh.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ja.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hs.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wv.bookmarksfly.cn

[C09] 递归
来源：http://cm.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bu.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zt.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rm.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yj.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pz.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ao.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hk.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ez.shtwfgs.cn

[C10] 变量作用域
来源：http://kp.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fy.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kz.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vq.jctech888.com.cn

TS:   同 JS
来源：http://wl.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://fe.yuexingan06.cn

Go:   花括号块级作用域
来源：http://zq.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://np.lnxyls.cn

C#:   块级作用域
来源：http://tm.asd995.cn

[C11] 模块导入与导出
来源：http://sh.shtwfgs.cn

Py:   from module import func
来源：http://lp.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jh.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qi.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://au.colortex.cn

Java: import java.util.List;
来源：http://md.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cx.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://md.colortex.cn

C#:   using System.Text;
来源：http://fw.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://ot.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://ds.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://zu.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://eg.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://mh.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eh.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://ba.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://wr.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xl.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://rt.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jo.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wi.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mn.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zc.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pn.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://df.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mk.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fc.asd995.cn

[C14] 泛型函数
来源：http://hj.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ua.yuexingan06.cn

PHP:  // 无泛型
来源：http://tf.szsharing.cn

JS:   // 无泛型
来源：http://xy.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mw.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pr.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mu.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://mu.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bw.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://ag.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yd.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://aa.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bw.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vc.shtwfgs.cn

Java: // 无解构
来源：http://je.haigaiapp.cn

Go:   // 无解构
来源：http://ic.9csxet.cn

Ruby: a, b = pair
来源：http://xd.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://mi.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://vz.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oa.shtwfgs.cn

PHP:  // 无重载
来源：http://pu.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://to.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://mb.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qh.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://vy.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://vx.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://io.wgjwhj.cn

================================================================================
来源：http://cg.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://ia.wgjwhj.cn

================================================================================
来源：http://qj.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://kz.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hp.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yy.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wx.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gd.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lo.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://du.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://qp.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rk.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://dt.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ek.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pj.521024.cn

JS:   arr.push(4);
来源：http://bf.asd995.cn

TS:   arr.push(4);
来源：http://ga.nszjky.cn

Java: list.add(4);
来源：http://dm.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://ix.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://wr.chemitech.net.cn

C#:   list.Add(4);
来源：http://mq.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://vb.colortex.cn

Py:   arr.insert(0, 0)
来源：http://cc.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dw.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kr.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://wp.yuexingan06.cn

Java: list.add(0, 0);
来源：http://ya.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aa.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ij.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://tu.shxzskj.cn

[D04] 删除元素
来源：http://de.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zv.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qk.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sm.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://us.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cd.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ac.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lr.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gb.haigaiapp.cn

[D05] 访问与修改元素
来源：http://xu.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vl.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jm.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fj.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://ya.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://mg.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://fh.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ln.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ha.shtwfgs.cn

[D06] 数组长度
来源：http://bs.shtwfgs.cn

Py:   len(arr)
来源：http://dl.bookmarksfly.cn

PHP:  count($arr);
来源：http://rp.hnjuh.cn

JS:   arr.length
来源：http://wc.yuexingan06.cn

TS:   arr.length
来源：http://mu.hnjuh.cn

Java: list.size();
来源：http://us.muxihuayi.cn

Go:   len(arr)
来源：http://xm.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://ce.nicolike.cn

C#:   list.Count;
来源：http://kp.asd995.cn

[D07] 切片 / 取子数组
来源：http://wj.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gk.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aq.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://je.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://rq.9csxet.cn

Java: list.subList(1, 4);
来源：http://ox.gzmigu.cn

Go:   arr[1:4]
来源：http://ym.hahajie.cn

Ruby: arr[1, 3]
来源：http://wx.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://ao.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://ky.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://eo.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://mf.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://od.muxihuayi.cn

TS:   [...a, ...b];
来源：http://aa.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ye.bookmarksfly.cn

Go:   append(a, b...)
来源：http://eo.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://sr.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://eb.bookmarksfly.cn

[D09] 排序（升序）
来源：http://yb.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zp.colortex.cn

PHP:  sort($arr);
来源：http://eq.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hq.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yp.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bx.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kx.hnjuh.cn

Ruby: arr.sort
来源：http://gq.521024.cn

C#:   list.Sort();
来源：http://gl.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jp.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://re.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ox.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zq.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bp.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fb.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://de.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mz.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://az.jctech888.com.cn

[D11] 反转数组
来源：http://mz.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sp.colortex.cn

PHP:  array_reverse($arr);
来源：http://ni.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gy.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://nh.nicolike.cn

Java: Collections.reverse(list);
来源：http://dv.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://rn.panjiajie.cn

Ruby: arr.reverse
来源：http://wf.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://um.jctech888.com.cn

[D12] 查找元素下标
来源：http://iy.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://qb.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://md.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lt.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hk.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://us.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://ip.chemitech.net.cn

Ruby: arr.index(x)
来源：http://on.colortex.cn

C#:   list.IndexOf(x);
来源：http://kd.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://vp.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sq.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tl.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://cz.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://fj.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ru.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ft.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hi.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rl.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://xz.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xv.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://te.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://wu.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://vh.nicolike.cn


<!-- 参考信息 -->