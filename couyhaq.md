代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xy.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jh.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://qh.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://xo.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://fj.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xj.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ji.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://za.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ga.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://ly.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iz.haigaiapp.cn

[B12] 跳出多层循环
来源：http://kb.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://td.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sy.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wl.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jr.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gd.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zr.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xl.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wm.hahajie.cn

[B13] 判断是否为数字
来源：http://mo.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://er.nicolike.cn

PHP:  is_numeric($x)
来源：http://ka.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ty.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ve.521024.cn

Java: x instanceof Number
来源：http://vi.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://up.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://uu.nicolike.cn

C#:   x is int or double or decimal
来源：http://yv.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://jq.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ko.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tc.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://if.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ip.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://we.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ah.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qw.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nv.shxzskj.cn

[B15] 布尔运算与取反
来源：http://ra.colortex.cn

Py:   a and b or not c
来源：http://so.nszjky.cn

PHP:  $a && $b || !$c
来源：http://ke.wgjwhj.cn

JS:   a && b || !c
来源：http://vo.colortex.cn

TS:   a && b || !c
来源：http://qx.muxihuayi.cn

Java: a && b || !c
来源：http://fr.hahajie.cn

Go:   a && b || !c
来源：http://ja.huixiangedu.cn

Ruby: a && b || !c
来源：http://gg.huanxung.cn

C#:   a && b || !c
来源：http://kh.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jt.szxytkj.cn

Py:   if not data: return
来源：http://xb.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://rm.nszjky.cn

JS:   if (!data) return;
来源：http://qp.newstarts.cn

TS:   if (!data) return;
来源：http://cp.newstarts.cn

Java: if (data == null) return;
来源：http://to.nszjky.cn

Go:   if data == nil { return }
来源：http://ah.szsharing.cn

Ruby: return if data.nil?
来源：http://wt.hahajie.cn

C#:   if (data == null) return;
来源：http://wk.colortex.cn

================================================================================
来源：http://sp.wgjwhj.cn

C. 函数与作用域
来源：http://nl.szsharing.cn

================================================================================
来源：http://lv.shxzskj.cn

[C01] 定义函数
来源：http://gz.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://xv.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bq.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://xo.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zj.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mo.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kn.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://bj.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fv.bjjhwx.cn

[C02] 默认参数
来源：http://lq.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://xj.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ad.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://fk.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ov.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lz.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cw.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://yz.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://mr.9csxet.cn

[C03] 可变参数
来源：http://tz.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://dz.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iw.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nv.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xg.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lp.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://he.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pr.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qj.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://ib.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jk.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xl.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aw.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vi.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://cq.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://ko.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://ic.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://it.521024.cn

[C05] 返回多个值
来源：http://yi.bookmarksfly.cn

Py:   return a, b
来源：http://vz.huanxung.cn

PHP:  return [$a, $b];
来源：http://ed.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uq.huanxung.cn

TS:   return { a, b };
来源：http://px.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sa.bjjhwx.cn

Go:   return a, b
来源：http://jk.haigaiapp.cn

Ruby: return a, b
来源：http://dj.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ll.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://jx.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://sg.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://in.panjiajie.cn

JS:   const square = x => x * x;
来源：http://gl.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://ri.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vd.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uf.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://rn.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://en.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://mq.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sk.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pw.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dy.521024.cn

TS:   arr.map(String)
来源：http://mw.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bk.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oh.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://mr.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fx.521024.cn

[C08] 闭包
来源：http://se.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xw.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vs.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rc.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://om.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sd.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lt.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rb.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tl.szsharing.cn

[C09] 递归
来源：http://fe.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ga.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://du.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ur.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bd.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qs.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kw.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pc.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hk.yuntaijiaju.cn

[C10] 变量作用域
来源：http://vo.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ib.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ia.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nu.wgjwhj.cn

TS:   同 JS
来源：http://gb.panjiajie.cn

Java: 方法内为块级作用域
来源：http://rt.asd995.cn

Go:   花括号块级作用域
来源：http://jx.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pa.lnxyls.cn

C#:   块级作用域
来源：http://pv.lnxyls.cn

[C11] 模块导入与导出
来源：http://aq.jctech888.com.cn

Py:   from module import func
来源：http://aw.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gu.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lc.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qh.asd995.cn

Java: import java.util.List;
来源：http://le.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kf.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://nr.lnxyls.cn

C#:   using System.Text;
来源：http://np.521024.cn

[C12] 立即执行函数 IIFE
来源：http://ad.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://ab.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://br.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://wn.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://li.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ry.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://xy.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://tc.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xj.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://qx.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wz.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xx.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qu.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sd.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://we.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://xw.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cj.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zt.bjjhwx.cn

[C14] 泛型函数
来源：http://di.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pw.shxzukj.cn

PHP:  // 无泛型
来源：http://nn.9csxet.cn

JS:   // 无泛型
来源：http://gs.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://up.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yz.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tw.yuexingan06.cn

Ruby: # 无泛型
来源：http://wb.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ny.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://kv.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uz.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://jr.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bu.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gd.bjjhwx.cn

Java: // 无解构
来源：http://ue.nszjky.cn

Go:   // 无解构
来源：http://ht.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://mn.nszjky.cn

C#:   var (a, b) = pair;
来源：http://fo.hahajie.cn

[C16] 函数 / 方法重载
来源：http://kv.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xg.panjiajie.cn

PHP:  // 无重载
来源：http://ef.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gw.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://yy.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qi.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://og.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://up.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zx.shtwfgs.cn

================================================================================
来源：http://mr.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://bw.huanxung.cn

================================================================================
来源：http://nc.asd995.cn

[D01] 创建数组 / 列表
来源：http://lr.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zz.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wc.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zw.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bo.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://er.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://nh.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://uj.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nn.newstarts.cn

[D02] 追加元素到末尾
来源：http://sl.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bm.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gp.shxzskj.cn

JS:   arr.push(4);
来源：http://jb.wgjwhj.cn

TS:   arr.push(4);
来源：http://bx.szxytkj.cn

Java: list.add(4);
来源：http://vj.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://th.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://cd.huixiangedu.cn

C#:   list.Add(4);
来源：http://fg.nicolike.cn

[D03] 在指定位置插入元素
来源：http://al.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://ob.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uk.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oc.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://dn.hahajie.cn

Java: list.add(0, 0);
来源：http://wn.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wg.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ej.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://pq.jctech888.com.cn

[D04] 删除元素
来源：http://al.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xk.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lq.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qd.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://kc.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rf.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qe.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ut.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pk.szsharing.cn

[D05] 访问与修改元素
来源：http://uf.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://di.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://co.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ir.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://wd.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://tq.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://dk.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ae.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lf.newstarts.cn

[D06] 数组长度
来源：http://in.wgjwhj.cn

Py:   len(arr)
来源：http://ou.hnjuh.cn

PHP:  count($arr);
来源：http://wj.muxihuayi.cn

JS:   arr.length
来源：http://fh.hahajie.cn

TS:   arr.length
来源：http://fm.shtwfgs.cn

Java: list.size();
来源：http://qt.yuexingan06.cn

Go:   len(arr)
来源：http://ra.9csxet.cn

Ruby: arr.length; arr.size
来源：http://de.colortex.cn

C#:   list.Count;
来源：http://ms.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://zi.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wv.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://le.521024.cn

JS:   arr.slice(1, 4);
来源：http://zb.asd995.cn

TS:   arr.slice(1, 4);
来源：http://xt.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://ob.hahajie.cn

Go:   arr[1:4]
来源：http://mk.szxytkj.cn

Ruby: arr[1, 3]
来源：http://bv.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://jh.bjjhwx.cn

[D08] 合并两个数组
来源：http://by.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://jq.colortex.cn

PHP:  array_merge($a, $b);
来源：http://cp.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ra.shxzskj.cn

TS:   [...a, ...b];
来源：http://eq.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oq.szxytkj.cn

Go:   append(a, b...)
来源：http://hl.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://zs.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://ku.chemitech.net.cn

[D09] 排序（升序）
来源：http://ww.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://fz.jctech888.com.cn

PHP:  sort($arr);
来源：http://kc.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ju.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ea.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sg.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vx.asd995.cn

Ruby: arr.sort
来源：http://eq.jctech888.com.cn

C#:   list.Sort();
来源：http://of.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cn.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ml.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oi.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ro.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://po.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ki.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bw.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mi.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mv.bookmarksfly.cn

[D11] 反转数组
来源：http://jq.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qb.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://wh.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nc.newstarts.cn


<!-- 参考信息 -->