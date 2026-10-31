代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cq.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ra.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://mo.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://jr.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://ki.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vw.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xq.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zk.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fw.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://po.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://go.huanxung.cn

[B12] 跳出多层循环
来源：http://yi.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wq.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cj.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rq.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nd.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://is.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tb.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nj.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nw.wgjwhj.cn

[B13] 判断是否为数字
来源：http://jx.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://ty.szxytkj.cn

PHP:  is_numeric($x)
来源：http://wm.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jw.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wn.lnxyls.cn

Java: x instanceof Number
来源：http://ot.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kx.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://yr.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://vq.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://xn.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tb.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ds.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://hl.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://cr.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bk.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lk.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zu.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ud.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://ou.9csxet.cn

Py:   a and b or not c
来源：http://do.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://qn.panjiajie.cn

JS:   a && b || !c
来源：http://pa.bjjhwx.cn

TS:   a && b || !c
来源：http://fa.chemitech.net.cn

Java: a && b || !c
来源：http://ls.newstarts.cn

Go:   a && b || !c
来源：http://vc.lnxyls.cn

Ruby: a && b || !c
来源：http://nn.newstarts.cn

C#:   a && b || !c
来源：http://zs.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ue.nszjky.cn

Py:   if not data: return
来源：http://oc.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://me.chemitech.net.cn

JS:   if (!data) return;
来源：http://ow.9csxet.cn

TS:   if (!data) return;
来源：http://kg.bookmarksfly.cn

Java: if (data == null) return;
来源：http://wx.newstarts.cn

Go:   if data == nil { return }
来源：http://sz.hahajie.cn

Ruby: return if data.nil?
来源：http://fd.chemitech.net.cn

C#:   if (data == null) return;
来源：http://si.hnjuh.cn

================================================================================
来源：http://vd.bjjhwx.cn

C. 函数与作用域
来源：http://ma.shtwfgs.cn

================================================================================
来源：http://hm.hnjuh.cn

[C01] 定义函数
来源：http://vl.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://bs.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qw.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://ep.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nr.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uf.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vy.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://bt.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tn.yuntaijiaju.cn

[C02] 默认参数
来源：http://eg.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://uh.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ce.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://yi.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wd.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sy.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wd.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://ii.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ud.jctech888.com.cn

[C03] 可变参数
来源：http://tc.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://uy.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://io.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cg.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jj.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mt.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wn.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kc.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ic.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://oc.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oz.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ty.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mx.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ki.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ak.521024.cn

Go:   // 无：用配置结构体参数
来源：http://uu.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://mx.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://rg.shxzskj.cn

[C05] 返回多个值
来源：http://pn.yuexingan06.cn

Py:   return a, b
来源：http://kr.lnxyls.cn

PHP:  return [$a, $b];
来源：http://kq.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sc.szsharing.cn

TS:   return { a, b };
来源：http://cb.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fj.jianghongdianzi.cn

Go:   return a, b
来源：http://gn.9csxet.cn

Ruby: return a, b
来源：http://te.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://ll.521024.cn

[C06] 匿名函数 / lambda
来源：http://kk.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://zi.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xw.asd995.cn

JS:   const square = x => x * x;
来源：http://re.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://sg.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kt.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ng.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://rj.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ku.nicolike.cn

[C07] 把函数作为参数传入
来源：http://yt.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dv.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kf.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yr.bjjhwx.cn

TS:   arr.map(String)
来源：http://ic.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ex.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://km.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://sw.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dn.521024.cn

[C08] 闭包
来源：http://uu.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ps.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lb.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ps.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yx.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ly.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ci.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sl.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dq.shxzukj.cn

[C09] 递归
来源：http://pz.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rd.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ev.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ee.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fp.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pw.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ru.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://at.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gr.lnxyls.cn

[C10] 变量作用域
来源：http://aj.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rg.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ta.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://us.521024.cn

TS:   同 JS
来源：http://eq.nszjky.cn

Java: 方法内为块级作用域
来源：http://fh.hnjuh.cn

Go:   花括号块级作用域
来源：http://ep.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ll.hnjuh.cn

C#:   块级作用域
来源：http://bq.chemitech.net.cn

[C11] 模块导入与导出
来源：http://je.asd995.cn

Py:   from module import func
来源：http://me.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ro.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uw.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pm.bjjhwx.cn

Java: import java.util.List;
来源：http://xj.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mk.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://rw.shtwfgs.cn

C#:   using System.Text;
来源：http://cj.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://bb.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://aw.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://zu.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://uj.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://ws.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wh.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://le.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ho.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xp.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://ca.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ax.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cs.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ug.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ux.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yk.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://zx.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ld.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zg.asd995.cn

[C14] 泛型函数
来源：http://rm.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ak.hahajie.cn

PHP:  // 无泛型
来源：http://ol.521024.cn

JS:   // 无泛型
来源：http://ia.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yc.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ph.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ec.9csxet.cn

Ruby: # 无泛型
来源：http://ac.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rc.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://fn.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gl.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://be.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ql.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ic.lnxyls.cn

Java: // 无解构
来源：http://ta.yuntaijiaju.cn

Go:   // 无解构
来源：http://la.szxytkj.cn

Ruby: a, b = pair
来源：http://sf.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://zu.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://bo.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vi.9csxet.cn

PHP:  // 无重载
来源：http://ri.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dc.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://qv.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jg.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://or.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://ne.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://es.muxihuayi.cn

================================================================================
来源：http://vw.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://rg.muxihuayi.cn

================================================================================
来源：http://tp.newstarts.cn

[D01] 创建数组 / 列表
来源：http://gf.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tx.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ym.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xe.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kk.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kx.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://pr.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://wl.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ho.hnjuh.cn

[D02] 追加元素到末尾
来源：http://if.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qy.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rq.panjiajie.cn

JS:   arr.push(4);
来源：http://bc.wgjwhj.cn

TS:   arr.push(4);
来源：http://kd.jctech888.com.cn

Java: list.add(4);
来源：http://kf.colortex.cn

Go:   arr = append(arr, 4)
来源：http://iv.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://bo.jctech888.com.cn

C#:   list.Add(4);
来源：http://se.hahajie.cn

[D03] 在指定位置插入元素
来源：http://tc.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://gt.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jm.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wk.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://th.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://bw.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zo.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yr.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://gb.szxytkj.cn

[D04] 删除元素
来源：http://jq.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jx.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yr.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://pz.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vc.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://df.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jc.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://we.hnjuh.cn

[D05] 访问与修改元素
来源：http://cv.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jt.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pu.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xe.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://wk.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://hi.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://qg.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xf.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://by.muxihuayi.cn

[D06] 数组长度
来源：http://xx.szsharing.cn

Py:   len(arr)
来源：http://ez.jianghongdianzi.cn

PHP:  count($arr);
来源：http://ug.bookmarksfly.cn

JS:   arr.length
来源：http://do.gzmigu.cn

TS:   arr.length
来源：http://ml.lnxyls.cn

Java: list.size();
来源：http://hb.szxytkj.cn

Go:   len(arr)
来源：http://ik.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://qc.muxihuayi.cn

C#:   list.Count;
来源：http://gk.newstarts.cn

[D07] 切片 / 取子数组
来源：http://sn.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cz.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rd.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://ov.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://ec.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://rb.hahajie.cn

Go:   arr[1:4]
来源：http://go.szxytkj.cn

Ruby: arr[1, 3]
来源：http://sm.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://dg.9csxet.cn

[D08] 合并两个数组
来源：http://yr.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://zp.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://qr.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jf.colortex.cn

TS:   [...a, ...b];
来源：http://dk.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lh.shxzskj.cn

Go:   append(a, b...)
来源：http://dp.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://es.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://bd.lnxyls.cn

[D09] 排序（升序）
来源：http://aj.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://zx.yuexingan06.cn

PHP:  sort($arr);
来源：http://rm.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wk.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://li.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kg.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xl.haigaiapp.cn

Ruby: arr.sort
来源：http://hl.yuntaijiaju.cn

C#:   list.Sort();
来源：http://bz.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yz.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ee.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fx.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cc.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kt.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://du.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ag.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xz.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lp.szsharing.cn

[D11] 反转数组
来源：http://wx.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nv.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://at.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yl.wgjwhj.cn


<!-- 参考信息 -->