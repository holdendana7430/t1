代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gb.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://qp.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ka.huixiangedu.cn

[B12] 跳出多层循环
来源：http://ex.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xm.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://py.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uz.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ze.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mi.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hb.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oy.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fk.colortex.cn

[B13] 判断是否为数字
来源：http://nv.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://lo.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://zt.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mq.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gt.szxytkj.cn

Java: x instanceof Number
来源：http://ap.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sb.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://av.huanxung.cn

C#:   x is int or double or decimal
来源：http://qg.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://by.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tg.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wn.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://yn.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://at.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lt.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ps.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://px.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zv.shxzukj.cn

[B15] 布尔运算与取反
来源：http://ws.bookmarksfly.cn

Py:   a and b or not c
来源：http://te.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://wb.bjjhwx.cn

JS:   a && b || !c
来源：http://tv.haigaiapp.cn

TS:   a && b || !c
来源：http://ka.szsharing.cn

Java: a && b || !c
来源：http://si.521024.cn

Go:   a && b || !c
来源：http://nb.lnxyls.cn

Ruby: a && b || !c
来源：http://pb.nicolike.cn

C#:   a && b || !c
来源：http://is.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://td.hahajie.cn

Py:   if not data: return
来源：http://vb.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://fv.colortex.cn

JS:   if (!data) return;
来源：http://pp.shtwfgs.cn

TS:   if (!data) return;
来源：http://zi.yuexingan06.cn

Java: if (data == null) return;
来源：http://ac.szxytkj.cn

Go:   if data == nil { return }
来源：http://du.wgjwhj.cn

Ruby: return if data.nil?
来源：http://yf.muxihuayi.cn

C#:   if (data == null) return;
来源：http://up.bjjhwx.cn

================================================================================
来源：http://gu.hahajie.cn

C. 函数与作用域
来源：http://gw.hahajie.cn

================================================================================
来源：http://li.huanxung.cn

[C01] 定义函数
来源：http://uw.colortex.cn

Py:   def add(a, b): return a + b
来源：http://bn.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://da.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://cf.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iw.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lo.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jj.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://zz.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dm.gzmigu.cn

[C02] 默认参数
来源：http://ej.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://cd.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gv.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://rl.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ke.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ek.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://js.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://gv.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://vp.wgjwhj.cn

[C03] 可变参数
来源：http://uk.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://lz.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bw.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vv.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xc.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bw.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xr.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://df.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ih.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://ml.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://na.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xi.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wk.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://td.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://tk.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://nw.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://ln.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://kj.haigaiapp.cn

[C05] 返回多个值
来源：http://oj.9csxet.cn

Py:   return a, b
来源：http://ku.szxytkj.cn

PHP:  return [$a, $b];
来源：http://ea.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lv.huixiangedu.cn

TS:   return { a, b };
来源：http://om.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ct.shxzukj.cn

Go:   return a, b
来源：http://zt.bookmarksfly.cn

Ruby: return a, b
来源：http://le.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://ve.asd995.cn

[C06] 匿名函数 / lambda
来源：http://qu.asd995.cn

Py:   square = lambda x: x * x
来源：http://ss.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://te.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://wr.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://gn.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ui.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fa.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://jt.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fb.hahajie.cn

[C07] 把函数作为参数传入
来源：http://ic.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hm.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://es.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uw.521024.cn

TS:   arr.map(String)
来源：http://fw.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sw.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ym.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://dc.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eb.hahajie.cn

[C08] 闭包
来源：http://in.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hl.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yd.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ii.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ee.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sg.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kq.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ny.newstarts.cn

[C09] 递归
来源：http://rp.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://za.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ah.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ux.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bw.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nl.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ph.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://to.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ow.muxihuayi.cn

[C10] 变量作用域
来源：http://il.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nx.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jr.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sn.huanxung.cn

TS:   同 JS
来源：http://ju.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://cy.muxihuayi.cn

Go:   花括号块级作用域
来源：http://zp.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vd.shtwfgs.cn

C#:   块级作用域
来源：http://az.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://nl.szsharing.cn

Py:   from module import func
来源：http://ck.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hq.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rg.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xb.hnjuh.cn

Java: import java.util.List;
来源：http://dw.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yq.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://nu.chemitech.net.cn

C#:   using System.Text;
来源：http://zh.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://ph.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://kn.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://du.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://pq.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://yn.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://or.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://km.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://fn.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bi.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://px.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rj.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://en.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ni.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ot.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ik.panjiajie.cn

Go:   func add(a, b int) int
来源：http://sz.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bc.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zt.wgjwhj.cn

[C14] 泛型函数
来源：http://qc.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ra.bjjhwx.cn

PHP:  // 无泛型
来源：http://pr.panjiajie.cn

JS:   // 无泛型
来源：http://tp.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dc.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xp.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rq.hnjuh.cn

Ruby: # 无泛型
来源：http://xv.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dk.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://kt.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://up.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://ke.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rx.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ak.9csxet.cn

Java: // 无解构
来源：http://yt.521024.cn

Go:   // 无解构
来源：http://bp.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://ls.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://vz.9csxet.cn

[C16] 函数 / 方法重载
来源：http://zz.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ij.chemitech.net.cn

PHP:  // 无重载
来源：http://rh.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nd.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ka.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ho.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://xf.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://zb.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gq.newstarts.cn

================================================================================
来源：http://sv.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://jr.huixiangedu.cn

================================================================================
来源：http://uq.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://ys.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ua.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rq.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ds.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pk.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vo.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://de.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://fi.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://in.asd995.cn

[D02] 追加元素到末尾
来源：http://qm.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://si.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gz.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://dm.lnxyls.cn

TS:   arr.push(4);
来源：http://uo.gzmigu.cn

Java: list.add(4);
来源：http://cr.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://pj.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://yw.shxzskj.cn

C#:   list.Add(4);
来源：http://ny.szsharing.cn

[D03] 在指定位置插入元素
来源：http://cm.asd995.cn

Py:   arr.insert(0, 0)
来源：http://vr.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aw.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zg.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://bs.gzmigu.cn

Java: list.add(0, 0);
来源：http://av.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bu.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vl.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://pt.wgjwhj.cn

[D04] 删除元素
来源：http://px.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://al.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tz.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hv.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://wo.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ah.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://by.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vw.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pn.szxytkj.cn

[D05] 访问与修改元素
来源：http://zc.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ss.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oz.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://om.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://vw.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://mm.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://ng.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nz.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kz.lnxyls.cn

[D06] 数组长度
来源：http://gh.lnxyls.cn

Py:   len(arr)
来源：http://wl.wgjwhj.cn

PHP:  count($arr);
来源：http://jn.chemitech.net.cn

JS:   arr.length
来源：http://uc.nicolike.cn

TS:   arr.length
来源：http://vg.hahajie.cn

Java: list.size();
来源：http://zo.panjiajie.cn

Go:   len(arr)
来源：http://wm.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://kb.panjiajie.cn

C#:   list.Count;
来源：http://ss.nszjky.cn

[D07] 切片 / 取子数组
来源：http://nr.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wv.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vn.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://rt.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://vs.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://qg.shxzukj.cn

Go:   arr[1:4]
来源：http://xn.newstarts.cn

Ruby: arr[1, 3]
来源：http://oz.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://ws.shxzskj.cn

[D08] 合并两个数组
来源：http://fv.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://cv.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://gm.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sj.shtwfgs.cn

TS:   [...a, ...b];
来源：http://ls.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yi.bookmarksfly.cn

Go:   append(a, b...)
来源：http://jb.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://qr.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://ki.hahajie.cn

[D09] 排序（升序）
来源：http://ou.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://je.lnxyls.cn

PHP:  sort($arr);
来源：http://dr.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cq.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jr.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aj.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ej.hnjuh.cn

Ruby: arr.sort
来源：http://jj.jianghongdianzi.cn

C#:   list.Sort();
来源：http://ol.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ei.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vi.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gu.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rh.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xt.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qm.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://og.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gi.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jg.hahajie.cn

[D11] 反转数组
来源：http://id.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://po.colortex.cn

PHP:  array_reverse($arr);
来源：http://bm.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hk.huanxung.cn

TS:   [...arr].reverse();
来源：http://qb.hnjuh.cn

Java: Collections.reverse(list);
来源：http://pd.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://on.yuexingan06.cn

Ruby: arr.reverse
来源：http://jo.nicolike.cn

C#:   list.Reverse();
来源：http://is.gzmigu.cn

[D12] 查找元素下标
来源：http://nc.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://tk.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dh.asd995.cn


<!-- 参考信息 -->