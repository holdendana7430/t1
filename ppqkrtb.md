代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://rw.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zh.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xi.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tp.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jn.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qg.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iv.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://er.panjiajie.cn

[B13] 判断是否为数字
来源：http://fe.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://tb.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://ry.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qd.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xx.9csxet.cn

Java: x instanceof Number
来源：http://wb.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uk.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://sr.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://yf.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://we.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dx.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mq.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://ip.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://yn.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lk.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jo.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://be.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qq.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://uf.haigaiapp.cn

Py:   a and b or not c
来源：http://ij.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://ex.nszjky.cn

JS:   a && b || !c
来源：http://eq.yuntaijiaju.cn

TS:   a && b || !c
来源：http://dz.huanxung.cn

Java: a && b || !c
来源：http://gk.lnxyls.cn

Go:   a && b || !c
来源：http://it.bjjhwx.cn

Ruby: a && b || !c
来源：http://xr.wgjwhj.cn

C#:   a && b || !c
来源：http://gp.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sb.bookmarksfly.cn

Py:   if not data: return
来源：http://sn.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://dp.haigaiapp.cn

JS:   if (!data) return;
来源：http://ql.521024.cn

TS:   if (!data) return;
来源：http://se.hahajie.cn

Java: if (data == null) return;
来源：http://gm.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://ok.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://dl.shtwfgs.cn

C#:   if (data == null) return;
来源：http://pj.hahajie.cn

================================================================================
来源：http://tx.9csxet.cn

C. 函数与作用域
来源：http://je.bjjhwx.cn

================================================================================
来源：http://pa.newstarts.cn

[C01] 定义函数
来源：http://ed.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://ca.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oq.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://qh.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gc.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gx.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ol.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://dv.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gp.hahajie.cn

[C02] 默认参数
来源：http://pt.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://xn.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nq.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://my.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yu.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://el.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dj.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://ni.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://mj.shtwfgs.cn

[C03] 可变参数
来源：http://bk.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://nc.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wz.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hh.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uf.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vm.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pg.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mj.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ex.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://ji.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nk.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nx.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bw.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ny.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://bb.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://si.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://nz.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://mr.lnxyls.cn

[C05] 返回多个值
来源：http://ns.jctech888.com.cn

Py:   return a, b
来源：http://ss.huanxung.cn

PHP:  return [$a, $b];
来源：http://yx.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lx.haigaiapp.cn

TS:   return { a, b };
来源：http://gp.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://da.colortex.cn

Go:   return a, b
来源：http://hv.shxzukj.cn

Ruby: return a, b
来源：http://ju.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://pk.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://wn.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://xw.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xd.hahajie.cn

JS:   const square = x => x * x;
来源：http://zk.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://of.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ge.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bn.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://vt.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vm.9csxet.cn

[C07] 把函数作为参数传入
来源：http://rt.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tq.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vh.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kt.hahajie.cn

TS:   arr.map(String)
来源：http://bt.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oj.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ep.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://ph.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mg.colortex.cn

[C08] 闭包
来源：http://av.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ag.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://re.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xk.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rv.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bu.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://px.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vm.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yv.huanxung.cn

[C09] 递归
来源：http://we.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pu.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ts.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://my.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yl.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fu.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cv.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yb.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oh.9csxet.cn

[C10] 变量作用域
来源：http://sm.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xf.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qg.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kr.szsharing.cn

TS:   同 JS
来源：http://sx.nszjky.cn

Java: 方法内为块级作用域
来源：http://xu.bjjhwx.cn

Go:   花括号块级作用域
来源：http://me.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ah.yuexingan06.cn

C#:   块级作用域
来源：http://kz.panjiajie.cn

[C11] 模块导入与导出
来源：http://es.colortex.cn

Py:   from module import func
来源：http://vx.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zi.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ir.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nn.muxihuayi.cn

Java: import java.util.List;
来源：http://cx.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qp.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://ga.9csxet.cn

C#:   using System.Text;
来源：http://zg.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://cp.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://km.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://du.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://ia.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://nj.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ke.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://kl.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://mv.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ir.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://mh.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vk.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mj.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mz.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qs.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dw.szxytkj.cn

Go:   func add(a, b int) int
来源：http://je.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bw.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fl.yuntaijiaju.cn

[C14] 泛型函数
来源：http://hr.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rq.szxytkj.cn

PHP:  // 无泛型
来源：http://uc.newstarts.cn

JS:   // 无泛型
来源：http://yf.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ah.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vw.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ms.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://at.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mk.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://dx.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://us.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://wb.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vj.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gn.panjiajie.cn

Java: // 无解构
来源：http://bw.huanxung.cn

Go:   // 无解构
来源：http://dx.hahajie.cn

Ruby: a, b = pair
来源：http://wf.newstarts.cn

C#:   var (a, b) = pair;
来源：http://vt.colortex.cn

[C16] 函数 / 方法重载
来源：http://gk.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sh.muxihuayi.cn

PHP:  // 无重载
来源：http://mw.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cb.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://zl.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ce.521024.cn

Go:   // 无重载：用不同函数名
来源：http://gg.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://vs.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yh.9csxet.cn

================================================================================
来源：http://bk.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://cr.jctech888.com.cn

================================================================================
来源：http://bc.asd995.cn

[D01] 创建数组 / 列表
来源：http://rj.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rw.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vp.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vj.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kq.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://to.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ho.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://ar.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ej.shxzukj.cn

[D02] 追加元素到末尾
来源：http://kl.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ye.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bp.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://nl.jctech888.com.cn

TS:   arr.push(4);
来源：http://ee.asd995.cn

Java: list.add(4);
来源：http://ud.521024.cn

Go:   arr = append(arr, 4)
来源：http://af.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://et.lnxyls.cn

C#:   list.Add(4);
来源：http://hs.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://kn.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://yq.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fc.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ts.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ht.gzmigu.cn

Java: list.add(0, 0);
来源：http://ri.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jn.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sa.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://gz.panjiajie.cn

[D04] 删除元素
来源：http://yo.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hk.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gb.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jq.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://sb.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vu.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://om.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vr.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://di.shtwfgs.cn

[D05] 访问与修改元素
来源：http://pe.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fm.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bi.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sj.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://nz.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ya.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://ig.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jc.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ah.wgjwhj.cn

[D06] 数组长度
来源：http://qb.bookmarksfly.cn

Py:   len(arr)
来源：http://bv.hnjuh.cn

PHP:  count($arr);
来源：http://wd.9csxet.cn

JS:   arr.length
来源：http://sq.hnjuh.cn

TS:   arr.length
来源：http://uv.jianghongdianzi.cn

Java: list.size();
来源：http://uz.jctech888.com.cn

Go:   len(arr)
来源：http://bb.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://yz.hnjuh.cn

C#:   list.Count;
来源：http://sa.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://vp.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vh.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hj.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://mu.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://sl.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://lz.521024.cn

Go:   arr[1:4]
来源：http://qh.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://xb.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://vv.huanxung.cn

[D08] 合并两个数组
来源：http://in.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://hg.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://ls.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yo.9csxet.cn

TS:   [...a, ...b];
来源：http://wl.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rr.bookmarksfly.cn

Go:   append(a, b...)
来源：http://ui.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://wh.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://sj.shxzukj.cn

[D09] 排序（升序）
来源：http://og.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://aq.jctech888.com.cn

PHP:  sort($arr);
来源：http://bw.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ij.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://si.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uk.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kw.muxihuayi.cn

Ruby: arr.sort
来源：http://hf.jianghongdianzi.cn

C#:   list.Sort();
来源：http://ht.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://po.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ju.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ib.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yl.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xg.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ty.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ud.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wj.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jc.szsharing.cn

[D11] 反转数组
来源：http://iq.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pg.asd995.cn

PHP:  array_reverse($arr);
来源：http://vj.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qq.huanxung.cn

TS:   [...arr].reverse();
来源：http://au.shxzukj.cn

Java: Collections.reverse(list);
来源：http://rt.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://ey.jctech888.com.cn

Ruby: arr.reverse
来源：http://fp.hnjuh.cn

C#:   list.Reverse();
来源：http://uc.bjjhwx.cn

[D12] 查找元素下标
来源：http://db.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://po.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wa.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zg.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yx.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bl.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://gj.huanxung.cn


<!-- 参考信息 -->