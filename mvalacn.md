代发 wailian999

PHP:  range(0, 10, 2);
来源：http://ue.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://au.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vc.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zf.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pi.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://yy.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gt.9csxet.cn

[B12] 跳出多层循环
来源：http://wu.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xt.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kc.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jl.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vg.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ze.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ss.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://md.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ba.shxzskj.cn

[B13] 判断是否为数字
来源：http://mm.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://xj.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://uz.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yr.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gg.jctech888.com.cn

Java: x instanceof Number
来源：http://uy.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xg.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://fp.szxytkj.cn

C#:   x is int or double or decimal
来源：http://rd.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://mz.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pp.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yx.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://or.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://jp.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vh.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sr.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qn.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://if.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://xc.yuexingan06.cn

Py:   a and b or not c
来源：http://am.521024.cn

PHP:  $a && $b || !$c
来源：http://gp.hahajie.cn

JS:   a && b || !c
来源：http://ky.lnxyls.cn

TS:   a && b || !c
来源：http://or.gzmigu.cn

Java: a && b || !c
来源：http://lc.huixinmuqiang.cn

Go:   a && b || !c
来源：http://qw.nszjky.cn

Ruby: a && b || !c
来源：http://rw.nszjky.cn

C#:   a && b || !c
来源：http://cn.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nt.wgjwhj.cn

Py:   if not data: return
来源：http://ak.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://xa.newstarts.cn

JS:   if (!data) return;
来源：http://mf.szxytkj.cn

TS:   if (!data) return;
来源：http://ir.hnjuh.cn

Java: if (data == null) return;
来源：http://yo.bjjhwx.cn

Go:   if data == nil { return }
来源：http://nr.bjjhwx.cn

Ruby: return if data.nil?
来源：http://ja.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://ko.asd995.cn

================================================================================
来源：http://jf.gzmigu.cn

C. 函数与作用域
来源：http://ua.newstarts.cn

================================================================================
来源：http://jn.yuexingan06.cn

[C01] 定义函数
来源：http://dc.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://oh.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qd.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://bd.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://me.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uz.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mq.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://pm.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cs.chemitech.net.cn

[C02] 默认参数
来源：http://gm.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://vf.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cc.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://ur.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ah.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xv.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mm.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://di.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://fq.haigaiapp.cn

[C03] 可变参数
来源：http://hk.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://lm.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ii.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hk.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tf.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xd.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ff.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cx.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xr.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://hd.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aa.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ou.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yx.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://do.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://cr.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://zs.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://re.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://xr.jianghongdianzi.cn

[C05] 返回多个值
来源：http://ni.colortex.cn

Py:   return a, b
来源：http://ek.shxzskj.cn

PHP:  return [$a, $b];
来源：http://np.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jw.chemitech.net.cn

TS:   return { a, b };
来源：http://dk.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ju.hahajie.cn

Go:   return a, b
来源：http://jc.hahajie.cn

Ruby: return a, b
来源：http://uc.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ke.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://pb.asd995.cn

Py:   square = lambda x: x * x
来源：http://tb.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mx.asd995.cn

JS:   const square = x => x * x;
来源：http://ls.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ux.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yt.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ut.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://nj.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hb.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://vx.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mo.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nb.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nf.shxzskj.cn

TS:   arr.map(String)
来源：http://uu.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ae.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://af.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://wx.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xi.newstarts.cn

[C08] 闭包
来源：http://nt.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dc.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aj.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ny.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hb.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fl.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tb.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://th.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wi.bookmarksfly.cn

[C09] 递归
来源：http://bq.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zr.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://um.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wi.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sj.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ik.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://es.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pq.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://om.shtwfgs.cn

[C10] 变量作用域
来源：http://ke.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mb.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xs.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bg.szsharing.cn

TS:   同 JS
来源：http://hp.newstarts.cn

Java: 方法内为块级作用域
来源：http://sx.shxzskj.cn

Go:   花括号块级作用域
来源：http://bn.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dv.yuexingan06.cn

C#:   块级作用域
来源：http://it.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://ev.bjjhwx.cn

Py:   from module import func
来源：http://fy.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zf.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kq.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://er.hnjuh.cn

Java: import java.util.List;
来源：http://up.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bh.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://cf.panjiajie.cn

C#:   using System.Text;
来源：http://oa.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://ep.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://wu.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://vi.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://ez.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://ay.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vl.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://pl.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://us.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rn.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://gh.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qw.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zp.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ox.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lc.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wl.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://mh.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ox.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ha.jianghongdianzi.cn

[C14] 泛型函数
来源：http://xd.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://in.lnxyls.cn

PHP:  // 无泛型
来源：http://re.huixiangedu.cn

JS:   // 无泛型
来源：http://jc.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hd.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yc.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ep.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://db.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cr.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://iv.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mt.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://sc.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://et.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cv.muxihuayi.cn

Java: // 无解构
来源：http://qx.9csxet.cn

Go:   // 无解构
来源：http://ly.bjjhwx.cn

Ruby: a, b = pair
来源：http://ln.szsharing.cn

C#:   var (a, b) = pair;
来源：http://zr.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://tm.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tq.lnxyls.cn

PHP:  // 无重载
来源：http://ke.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yo.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://nx.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jn.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://lt.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://cb.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gh.szsharing.cn

================================================================================
来源：http://sp.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://mt.szsharing.cn

================================================================================
来源：http://ca.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://dk.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hs.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ui.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dm.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ot.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lm.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://mu.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://rp.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tw.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://bk.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xh.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wm.hnjuh.cn

JS:   arr.push(4);
来源：http://gb.szxytkj.cn

TS:   arr.push(4);
来源：http://cd.muxihuayi.cn

Java: list.add(4);
来源：http://ec.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://qp.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://er.chemitech.net.cn

C#:   list.Add(4);
来源：http://io.asd995.cn

[D03] 在指定位置插入元素
来源：http://qg.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://mv.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ux.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qq.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://su.colortex.cn

Java: list.add(0, 0);
来源：http://jj.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ri.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ly.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://qt.chemitech.net.cn

[D04] 删除元素
来源：http://ia.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lr.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://db.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bb.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://tm.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lg.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jx.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ur.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zt.panjiajie.cn

[D05] 访问与修改元素
来源：http://rp.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cp.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zq.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mf.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ff.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://nh.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://jm.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xu.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jx.shtwfgs.cn

[D06] 数组长度
来源：http://ds.lnxyls.cn

Py:   len(arr)
来源：http://wm.hahajie.cn

PHP:  count($arr);
来源：http://li.huanxung.cn

JS:   arr.length
来源：http://ig.lnxyls.cn

TS:   arr.length
来源：http://sa.nicolike.cn

Java: list.size();
来源：http://he.colortex.cn

Go:   len(arr)
来源：http://qj.huanxung.cn

Ruby: arr.length; arr.size
来源：http://wm.huanxung.cn

C#:   list.Count;
来源：http://dj.9csxet.cn

[D07] 切片 / 取子数组
来源：http://je.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hc.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ap.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://vh.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://ad.nicolike.cn

Java: list.subList(1, 4);
来源：http://zi.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://ef.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://sc.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://ai.szxytkj.cn

[D08] 合并两个数组
来源：http://qd.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://ce.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://mt.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ki.yuexingan06.cn

TS:   [...a, ...b];
来源：http://ey.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qm.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://up.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://ul.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://qk.hahajie.cn

[D09] 排序（升序）
来源：http://pf.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://ks.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://fr.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rm.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qu.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ch.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hb.szxytkj.cn

Ruby: arr.sort
来源：http://xc.shtwfgs.cn

C#:   list.Sort();
来源：http://pw.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ng.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yh.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gy.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hr.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zs.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pr.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vi.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tr.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jv.panjiajie.cn

[D11] 反转数组
来源：http://bp.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hc.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://lo.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rm.521024.cn

TS:   [...arr].reverse();
来源：http://rj.shxzskj.cn

Java: Collections.reverse(list);
来源：http://qp.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://kq.szxytkj.cn

Ruby: arr.reverse
来源：http://tn.hahajie.cn


<!-- 参考信息 -->