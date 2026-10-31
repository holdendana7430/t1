代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sq.shxzukj.cn

Java: x instanceof Number
来源：http://tx.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://op.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://gj.nicolike.cn

C#:   x is int or double or decimal
来源：http://zn.asd995.cn

[B14] 判断值是否在集合内
来源：http://hs.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iu.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sg.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ze.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://hl.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vu.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mt.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://te.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wj.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://dq.nicolike.cn

Py:   a and b or not c
来源：http://lg.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://gt.521024.cn

JS:   a && b || !c
来源：http://xy.huanxung.cn

TS:   a && b || !c
来源：http://nj.shxzukj.cn

Java: a && b || !c
来源：http://lo.nicolike.cn

Go:   a && b || !c
来源：http://sw.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://jl.bjjhwx.cn

C#:   a && b || !c
来源：http://hq.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dg.shtwfgs.cn

Py:   if not data: return
来源：http://vy.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://mm.9csxet.cn

JS:   if (!data) return;
来源：http://rn.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://eq.haigaiapp.cn

Java: if (data == null) return;
来源：http://zp.nicolike.cn

Go:   if data == nil { return }
来源：http://ct.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://da.colortex.cn

C#:   if (data == null) return;
来源：http://fd.panjiajie.cn

================================================================================
来源：http://ae.newstarts.cn

C. 函数与作用域
来源：http://fk.asd995.cn

================================================================================
来源：http://bo.gzmigu.cn

[C01] 定义函数
来源：http://dm.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://oo.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://np.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://qd.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xc.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pf.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://is.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://er.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://no.huixiangedu.cn

[C02] 默认参数
来源：http://vt.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://qc.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wq.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://xj.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xx.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://od.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xi.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://zt.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://lp.jctech888.com.cn

[C03] 可变参数
来源：http://xu.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://wd.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ij.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wh.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wa.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cj.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gh.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qs.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wz.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://pv.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cv.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lu.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rt.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kj.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://sc.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://hn.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://lz.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://sf.huixiangedu.cn

[C05] 返回多个值
来源：http://gh.shxzukj.cn

Py:   return a, b
来源：http://ks.panjiajie.cn

PHP:  return [$a, $b];
来源：http://ec.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mr.huixiangedu.cn

TS:   return { a, b };
来源：http://iq.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jn.jctech888.com.cn

Go:   return a, b
来源：http://qv.nicolike.cn

Ruby: return a, b
来源：http://de.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://nh.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://gy.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://wq.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mj.huanxung.cn

JS:   const square = x => x * x;
来源：http://wl.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://ei.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tu.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yq.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://zd.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wc.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://ln.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zk.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kp.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hg.hahajie.cn

TS:   arr.map(String)
来源：http://gs.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bz.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vs.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://kl.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ys.hnjuh.cn

[C08] 闭包
来源：http://uj.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dd.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gw.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ev.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ty.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rw.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qf.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://or.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gj.haigaiapp.cn

[C09] 递归
来源：http://vz.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jj.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rr.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zf.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://es.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mg.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oz.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sf.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iq.bookmarksfly.cn

[C10] 变量作用域
来源：http://wk.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ob.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hc.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cw.gzmigu.cn

TS:   同 JS
来源：http://wn.szsharing.cn

Java: 方法内为块级作用域
来源：http://xp.muxihuayi.cn

Go:   花括号块级作用域
来源：http://ne.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wu.huixinmuqiang.cn

C#:   块级作用域
来源：http://np.nicolike.cn

[C11] 模块导入与导出
来源：http://mn.yuexingan06.cn

Py:   from module import func
来源：http://nj.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hi.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yf.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ml.yuntaijiaju.cn

Java: import java.util.List;
来源：http://qe.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tx.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://yn.521024.cn

C#:   using System.Text;
来源：http://qs.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://ec.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://uv.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://dg.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://je.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://vm.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ay.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://py.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://vr.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yq.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://au.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yz.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lt.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jr.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://we.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lm.asd995.cn

Go:   func add(a, b int) int
来源：http://tq.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pl.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uw.lnxyls.cn

[C14] 泛型函数
来源：http://yn.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jx.haigaiapp.cn

PHP:  // 无泛型
来源：http://zu.shtwfgs.cn

JS:   // 无泛型
来源：http://bn.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hh.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yg.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qq.yuexingan06.cn

Ruby: # 无泛型
来源：http://zi.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://if.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://th.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ce.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://gu.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vr.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bn.haigaiapp.cn

Java: // 无解构
来源：http://nq.colortex.cn

Go:   // 无解构
来源：http://he.shxzukj.cn

Ruby: a, b = pair
来源：http://th.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://rd.asd995.cn

[C16] 函数 / 方法重载
来源：http://ol.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vv.jctech888.com.cn

PHP:  // 无重载
来源：http://uw.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ja.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://rn.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dq.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://ds.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://qv.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ke.gzmigu.cn

================================================================================
来源：http://vj.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://cg.nicolike.cn

================================================================================
来源：http://ii.huanxung.cn

[D01] 创建数组 / 列表
来源：http://oi.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ig.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ix.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cm.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oe.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xq.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://xo.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://pt.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kg.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://bv.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vh.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://es.shtwfgs.cn

JS:   arr.push(4);
来源：http://an.shtwfgs.cn

TS:   arr.push(4);
来源：http://nu.lnxyls.cn

Java: list.add(4);
来源：http://xs.asd995.cn

Go:   arr = append(arr, 4)
来源：http://de.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://yf.colortex.cn

C#:   list.Add(4);
来源：http://qe.nicolike.cn

[D03] 在指定位置插入元素
来源：http://ot.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://yw.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vy.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yx.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://nd.haigaiapp.cn

Java: list.add(0, 0);
来源：http://ix.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ol.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ec.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://sk.521024.cn

[D04] 删除元素
来源：http://ox.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ez.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rd.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yj.colortex.cn

TS:   arr.splice(0, 1);
来源：http://mj.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qy.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oc.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lk.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zu.haigaiapp.cn

[D05] 访问与修改元素
来源：http://yf.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jw.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eq.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tn.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://am.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://re.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://on.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://on.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zd.wgjwhj.cn

[D06] 数组长度
来源：http://fe.panjiajie.cn

Py:   len(arr)
来源：http://zr.muxihuayi.cn

PHP:  count($arr);
来源：http://be.gzmigu.cn

JS:   arr.length
来源：http://be.nszjky.cn

TS:   arr.length
来源：http://vw.shxzukj.cn

Java: list.size();
来源：http://pe.shxzskj.cn

Go:   len(arr)
来源：http://us.asd995.cn

Ruby: arr.length; arr.size
来源：http://ve.jctech888.com.cn

C#:   list.Count;
来源：http://xd.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://am.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rk.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jj.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://ko.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://ga.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://ye.hahajie.cn

Go:   arr[1:4]
来源：http://qm.szxytkj.cn

Ruby: arr[1, 3]
来源：http://mu.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://yj.huixiangedu.cn

[D08] 合并两个数组
来源：http://nx.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://eb.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://ew.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qh.nicolike.cn

TS:   [...a, ...b];
来源：http://ha.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qd.asd995.cn

Go:   append(a, b...)
来源：http://hb.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://bo.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://dz.chemitech.net.cn

[D09] 排序（升序）
来源：http://mh.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://un.bjjhwx.cn

PHP:  sort($arr);
来源：http://rm.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zi.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ri.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rp.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ik.newstarts.cn

Ruby: arr.sort
来源：http://gz.asd995.cn

C#:   list.Sort();
来源：http://lk.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tt.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rf.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cl.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pq.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yl.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ov.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eg.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wp.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wf.hnjuh.cn

[D11] 反转数组
来源：http://bs.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ws.newstarts.cn

PHP:  array_reverse($arr);
来源：http://ty.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zx.gzmigu.cn

TS:   [...arr].reverse();
来源：http://qv.hahajie.cn

Java: Collections.reverse(list);
来源：http://ha.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://zg.huixiangedu.cn

Ruby: arr.reverse
来源：http://uf.yuexingan06.cn

C#:   list.Reverse();
来源：http://xk.yuexingan06.cn

[D12] 查找元素下标
来源：http://mx.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://ro.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ko.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ut.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hb.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qk.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://wy.jctech888.com.cn

Ruby: arr.index(x)
来源：http://ob.huanxung.cn

C#:   list.IndexOf(x);
来源：http://nw.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://xa.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://un.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zl.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://ft.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://kg.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ab.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://il.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yh.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bh.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://gw.shxzukj.cn


<!-- 参考信息 -->