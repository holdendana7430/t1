代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rp.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://ne.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ls.nicolike.cn

[B12] 跳出多层循环
来源：http://jz.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cr.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ze.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ln.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tf.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qc.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rr.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yn.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dc.nszjky.cn

[B13] 判断是否为数字
来源：http://ih.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://uz.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://yo.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ks.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vn.huixinmuqiang.cn

Java: x instanceof Number
来源：http://mt.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mi.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://no.521024.cn

C#:   x is int or double or decimal
来源：http://il.newstarts.cn

[B14] 判断值是否在集合内
来源：http://nj.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nr.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pv.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://oa.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ke.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ft.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tg.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xr.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lt.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://he.nszjky.cn

Py:   a and b or not c
来源：http://ab.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://ng.nicolike.cn

JS:   a && b || !c
来源：http://wy.shxzukj.cn

TS:   a && b || !c
来源：http://rc.muxihuayi.cn

Java: a && b || !c
来源：http://zj.bjjhwx.cn

Go:   a && b || !c
来源：http://gp.lnxyls.cn

Ruby: a && b || !c
来源：http://mj.hahajie.cn

C#:   a && b || !c
来源：http://jc.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yn.9csxet.cn

Py:   if not data: return
来源：http://iw.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://gh.hahajie.cn

JS:   if (!data) return;
来源：http://sl.hnjuh.cn

TS:   if (!data) return;
来源：http://mu.asd995.cn

Java: if (data == null) return;
来源：http://bo.gzmigu.cn

Go:   if data == nil { return }
来源：http://cj.nicolike.cn

Ruby: return if data.nil?
来源：http://ae.jctech888.com.cn

C#:   if (data == null) return;
来源：http://rw.yuexingan06.cn

================================================================================
来源：http://tc.wgjwhj.cn

C. 函数与作用域
来源：http://wn.lnxyls.cn

================================================================================
来源：http://tg.shxzskj.cn

[C01] 定义函数
来源：http://md.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://rm.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cx.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ny.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jc.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yj.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tx.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://dc.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aj.asd995.cn

[C02] 默认参数
来源：http://am.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://vc.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jv.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://je.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bj.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rt.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ho.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://hs.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://dj.nicolike.cn

[C03] 可变参数
来源：http://lp.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://me.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pq.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jh.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vf.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lq.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nn.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ow.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://el.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://ql.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://op.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jf.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ro.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zj.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://ce.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://qy.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://td.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://zk.szsharing.cn

[C05] 返回多个值
来源：http://ne.wgjwhj.cn

Py:   return a, b
来源：http://zc.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://bt.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wl.szsharing.cn

TS:   return { a, b };
来源：http://qt.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wb.gzmigu.cn

Go:   return a, b
来源：http://on.shxzukj.cn

Ruby: return a, b
来源：http://gl.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://yl.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://lp.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://yu.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sn.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://mt.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ox.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wy.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ff.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://lj.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jn.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://in.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ty.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ay.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ra.bjjhwx.cn

TS:   arr.map(String)
来源：http://ib.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cf.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wt.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://zq.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sm.haigaiapp.cn

[C08] 闭包
来源：http://ur.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bd.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oa.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://at.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nf.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://st.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pe.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wb.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wy.szxytkj.cn

[C09] 递归
来源：http://yg.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jr.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://or.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://av.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xs.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ce.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fw.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yl.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yr.huixinmuqiang.cn

[C10] 变量作用域
来源：http://ds.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ic.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://va.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zo.bookmarksfly.cn

TS:   同 JS
来源：http://xp.nicolike.cn

Java: 方法内为块级作用域
来源：http://hh.szxytkj.cn

Go:   花括号块级作用域
来源：http://si.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xu.bjjhwx.cn

C#:   块级作用域
来源：http://fa.szsharing.cn

[C11] 模块导入与导出
来源：http://gk.9csxet.cn

Py:   from module import func
来源：http://og.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mz.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://db.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ja.wgjwhj.cn

Java: import java.util.List;
来源：http://lb.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cb.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://ek.nicolike.cn

C#:   using System.Text;
来源：http://yf.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://ie.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://yq.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://zj.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://sc.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://ba.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fy.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://tq.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://rl.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rg.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://kf.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vz.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bs.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fj.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ry.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dx.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://mr.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cp.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rs.jianghongdianzi.cn

[C14] 泛型函数
来源：http://dg.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://po.panjiajie.cn

PHP:  // 无泛型
来源：http://ti.nszjky.cn

JS:   // 无泛型
来源：http://ji.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://es.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wt.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ox.9csxet.cn

Ruby: # 无泛型
来源：http://pn.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://se.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://gn.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ss.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://yr.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ua.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://up.shxzukj.cn

Java: // 无解构
来源：http://mt.jianghongdianzi.cn

Go:   // 无解构
来源：http://hh.huixiangedu.cn

Ruby: a, b = pair
来源：http://xs.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://lj.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://sl.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ev.chemitech.net.cn

PHP:  // 无重载
来源：http://gb.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uq.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://pq.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jv.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://ji.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://rf.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ld.9csxet.cn

================================================================================
来源：http://ao.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://tf.colortex.cn

================================================================================
来源：http://li.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://gq.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zj.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fr.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mu.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ph.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ad.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://so.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://to.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ly.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://zp.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://et.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://me.lnxyls.cn

JS:   arr.push(4);
来源：http://jq.bjjhwx.cn

TS:   arr.push(4);
来源：http://ho.jianghongdianzi.cn

Java: list.add(4);
来源：http://dc.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://hv.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://rx.shxzskj.cn

C#:   list.Add(4);
来源：http://cb.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://tt.colortex.cn

Py:   arr.insert(0, 0)
来源：http://fz.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fy.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cs.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://jn.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://tx.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ym.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kj.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://nt.chemitech.net.cn

[D04] 删除元素
来源：http://gc.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://es.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nk.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qk.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://hn.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oh.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zw.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kd.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ko.bjjhwx.cn

[D05] 访问与修改元素
来源：http://ep.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pr.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rc.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://go.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://ac.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://lr.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://uj.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://my.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tw.521024.cn

[D06] 数组长度
来源：http://bu.haigaiapp.cn

Py:   len(arr)
来源：http://cg.muxihuayi.cn

PHP:  count($arr);
来源：http://gs.gzmigu.cn

JS:   arr.length
来源：http://ny.gzmigu.cn

TS:   arr.length
来源：http://bt.newstarts.cn

Java: list.size();
来源：http://ky.colortex.cn

Go:   len(arr)
来源：http://ev.colortex.cn

Ruby: arr.length; arr.size
来源：http://zt.wgjwhj.cn

C#:   list.Count;
来源：http://md.nicolike.cn

[D07] 切片 / 取子数组
来源：http://sd.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mf.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ta.asd995.cn

JS:   arr.slice(1, 4);
来源：http://sz.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://ok.newstarts.cn

Java: list.subList(1, 4);
来源：http://ah.hnjuh.cn

Go:   arr[1:4]
来源：http://ci.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://uv.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://ou.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://gc.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://te.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://vt.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ml.shxzukj.cn

TS:   [...a, ...b];
来源：http://ch.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kq.bjjhwx.cn

Go:   append(a, b...)
来源：http://ap.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://gr.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://mp.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://ig.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://dx.yuexingan06.cn

PHP:  sort($arr);
来源：http://pg.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fv.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wc.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ct.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fv.haigaiapp.cn

Ruby: arr.sort
来源：http://bv.bjjhwx.cn

C#:   list.Sort();
来源：http://sh.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://os.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fr.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lg.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ng.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cr.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ih.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://or.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ee.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pa.szxytkj.cn

[D11] 反转数组
来源：http://mz.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bn.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://ii.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yb.gzmigu.cn

TS:   [...arr].reverse();
来源：http://gg.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://ao.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://ls.huixiangedu.cn

Ruby: arr.reverse
来源：http://zw.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://ha.9csxet.cn

[D12] 查找元素下标
来源：http://ym.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://ez.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ah.haigaiapp.cn


<!-- 参考信息 -->