代发 wailian999

[B13] 判断是否为数字
来源：http://rt.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://bj.hahajie.cn

PHP:  is_numeric($x)
来源：http://xg.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dd.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vi.colortex.cn

Java: x instanceof Number
来源：http://kg.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zq.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://tp.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://ub.nicolike.cn

[B14] 判断值是否在集合内
来源：http://kz.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://br.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://le.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://au.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://wr.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uo.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bw.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uy.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vz.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://uy.chemitech.net.cn

Py:   a and b or not c
来源：http://qs.9csxet.cn

PHP:  $a && $b || !$c
来源：http://wi.muxihuayi.cn

JS:   a && b || !c
来源：http://jh.wgjwhj.cn

TS:   a && b || !c
来源：http://yf.yuexingan06.cn

Java: a && b || !c
来源：http://ys.nszjky.cn

Go:   a && b || !c
来源：http://ks.szxytkj.cn

Ruby: a && b || !c
来源：http://oo.szxytkj.cn

C#:   a && b || !c
来源：http://ws.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qp.hnjuh.cn

Py:   if not data: return
来源：http://fu.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://jx.nszjky.cn

JS:   if (!data) return;
来源：http://zg.hahajie.cn

TS:   if (!data) return;
来源：http://ly.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://af.shxzskj.cn

Go:   if data == nil { return }
来源：http://gp.hahajie.cn

Ruby: return if data.nil?
来源：http://dc.huanxung.cn

C#:   if (data == null) return;
来源：http://uu.hahajie.cn

================================================================================
来源：http://pv.gzmigu.cn

C. 函数与作用域
来源：http://mi.9csxet.cn

================================================================================
来源：http://oh.nszjky.cn

[C01] 定义函数
来源：http://tw.521024.cn

Py:   def add(a, b): return a + b
来源：http://bk.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://je.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://me.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ei.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fx.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uh.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://zk.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://le.hahajie.cn

[C02] 默认参数
来源：http://pp.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://xi.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hv.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://du.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kr.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ss.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cd.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://bh.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://qb.huixinmuqiang.cn

[C03] 可变参数
来源：http://xe.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://gg.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mg.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hk.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vx.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rk.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dy.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cw.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ft.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://jy.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mf.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kg.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ut.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ua.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://aw.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://sq.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://wc.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://ni.9csxet.cn

[C05] 返回多个值
来源：http://su.nszjky.cn

Py:   return a, b
来源：http://lp.shxzukj.cn

PHP:  return [$a, $b];
来源：http://ma.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jp.newstarts.cn

TS:   return { a, b };
来源：http://sg.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ra.9csxet.cn

Go:   return a, b
来源：http://ja.shxzskj.cn

Ruby: return a, b
来源：http://ey.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://li.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://vq.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://tb.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yt.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://ba.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://il.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tl.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://td.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://rw.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://of.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://ka.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ph.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dk.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wr.asd995.cn

TS:   arr.map(String)
来源：http://ey.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dm.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xq.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://hc.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hb.lnxyls.cn

[C08] 闭包
来源：http://zg.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ix.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nh.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tr.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dv.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://op.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jh.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://he.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xr.gzmigu.cn

[C09] 递归
来源：http://oa.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mk.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mr.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fa.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bp.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tp.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eg.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mf.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qh.bjjhwx.cn

[C10] 变量作用域
来源：http://gh.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ny.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jb.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qx.newstarts.cn

TS:   同 JS
来源：http://ng.9csxet.cn

Java: 方法内为块级作用域
来源：http://yc.hnjuh.cn

Go:   花括号块级作用域
来源：http://he.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://an.shxzukj.cn

C#:   块级作用域
来源：http://dd.hahajie.cn

[C11] 模块导入与导出
来源：http://bf.hahajie.cn

Py:   from module import func
来源：http://rd.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bb.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nn.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mh.bjjhwx.cn

Java: import java.util.List;
来源：http://yu.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://it.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://hi.hnjuh.cn

C#:   using System.Text;
来源：http://pj.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://bd.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://tg.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://gk.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://ue.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://mc.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nn.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://gc.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://bv.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jx.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://fb.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yg.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vs.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dn.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wb.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ax.gzmigu.cn

Go:   func add(a, b int) int
来源：http://za.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wy.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bj.szsharing.cn

[C14] 泛型函数
来源：http://sz.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vm.bjjhwx.cn

PHP:  // 无泛型
来源：http://kw.nicolike.cn

JS:   // 无泛型
来源：http://yz.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hc.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lm.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bn.huixiangedu.cn

Ruby: # 无泛型
来源：http://ew.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pk.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://ez.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eo.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://ul.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sx.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ap.bookmarksfly.cn

Java: // 无解构
来源：http://lx.chemitech.net.cn

Go:   // 无解构
来源：http://on.huixiangedu.cn

Ruby: a, b = pair
来源：http://st.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://fz.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://ym.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wl.colortex.cn

PHP:  // 无重载
来源：http://hp.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jw.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://sf.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ea.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://ak.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://ec.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ni.muxihuayi.cn

================================================================================
来源：http://oo.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://cr.huanxung.cn

================================================================================
来源：http://to.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://rl.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fq.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pd.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eb.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rk.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wr.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ii.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://to.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tw.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://hy.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mk.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xn.haigaiapp.cn

JS:   arr.push(4);
来源：http://cp.gzmigu.cn

TS:   arr.push(4);
来源：http://xu.wgjwhj.cn

Java: list.add(4);
来源：http://as.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://yd.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://jl.9csxet.cn

C#:   list.Add(4);
来源：http://do.nszjky.cn

[D03] 在指定位置插入元素
来源：http://xb.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://zj.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yo.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sl.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://ww.521024.cn

Java: list.add(0, 0);
来源：http://xd.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sj.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xj.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://xs.chemitech.net.cn

[D04] 删除元素
来源：http://jp.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ad.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qa.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gr.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://le.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://if.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bc.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://js.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qd.9csxet.cn

[D05] 访问与修改元素
来源：http://mi.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ra.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ow.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sq.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://bp.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://pf.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ij.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wo.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zq.shtwfgs.cn

[D06] 数组长度
来源：http://ic.lnxyls.cn

Py:   len(arr)
来源：http://ms.bookmarksfly.cn

PHP:  count($arr);
来源：http://ji.yuntaijiaju.cn

JS:   arr.length
来源：http://ue.521024.cn

TS:   arr.length
来源：http://sh.newstarts.cn

Java: list.size();
来源：http://eg.shxzskj.cn

Go:   len(arr)
来源：http://oq.521024.cn

Ruby: arr.length; arr.size
来源：http://ug.szsharing.cn

C#:   list.Count;
来源：http://yj.colortex.cn

[D07] 切片 / 取子数组
来源：http://pb.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iu.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ac.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://lw.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://um.shxzukj.cn

Java: list.subList(1, 4);
来源：http://jl.panjiajie.cn

Go:   arr[1:4]
来源：http://zd.shxzskj.cn

Ruby: arr[1, 3]
来源：http://zq.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://ju.szxytkj.cn

[D08] 合并两个数组
来源：http://oa.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://qv.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://gg.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bh.muxihuayi.cn

TS:   [...a, ...b];
来源：http://ge.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dw.lnxyls.cn

Go:   append(a, b...)
来源：http://bu.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://fd.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://cy.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://oc.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://lw.shtwfgs.cn

PHP:  sort($arr);
来源：http://jo.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xw.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nk.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ll.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jn.lnxyls.cn

Ruby: arr.sort
来源：http://hi.shtwfgs.cn

C#:   list.Sort();
来源：http://wt.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vw.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sy.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fv.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kk.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://js.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sm.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://df.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://td.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ec.shtwfgs.cn

[D11] 反转数组
来源：http://bj.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wj.nicolike.cn

PHP:  array_reverse($arr);
来源：http://wj.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tq.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://br.hnjuh.cn

Java: Collections.reverse(list);
来源：http://tw.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://jh.wgjwhj.cn

Ruby: arr.reverse
来源：http://xq.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://as.yuexingan06.cn

[D12] 查找元素下标
来源：http://df.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://lj.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kj.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wy.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rc.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wz.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://zo.asd995.cn

Ruby: arr.index(x)
来源：http://jp.newstarts.cn

C#:   list.IndexOf(x);
来源：http://za.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://lb.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://me.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nh.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://ps.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://yp.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rs.szsharing.cn


<!-- 参考信息 -->