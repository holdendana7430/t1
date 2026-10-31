代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://az.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ip.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ra.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tn.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xi.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://yg.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nn.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zs.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://di.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eo.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ta.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ge.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xh.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uk.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://ay.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://ng.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://dn.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pn.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kd.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bb.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yv.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://dy.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nc.muxihuayi.cn

[B12] 跳出多层循环
来源：http://mi.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ok.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://so.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rz.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cb.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jk.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ck.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vn.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wz.nszjky.cn

[B13] 判断是否为数字
来源：http://qw.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://lh.szxytkj.cn

PHP:  is_numeric($x)
来源：http://uk.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bh.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gf.shxzukj.cn

Java: x instanceof Number
来源：http://ww.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kc.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://eo.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://fm.hahajie.cn

[B14] 判断值是否在集合内
来源：http://vs.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eb.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ta.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ta.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://qh.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ni.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lm.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pd.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bw.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://uo.muxihuayi.cn

Py:   a and b or not c
来源：http://ei.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://rz.nicolike.cn

JS:   a && b || !c
来源：http://fc.bjjhwx.cn

TS:   a && b || !c
来源：http://oy.muxihuayi.cn

Java: a && b || !c
来源：http://lj.hnjuh.cn

Go:   a && b || !c
来源：http://qa.bookmarksfly.cn

Ruby: a && b || !c
来源：http://fs.huixiangedu.cn

C#:   a && b || !c
来源：http://ab.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fi.colortex.cn

Py:   if not data: return
来源：http://kh.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://co.huixiangedu.cn

JS:   if (!data) return;
来源：http://yn.haigaiapp.cn

TS:   if (!data) return;
来源：http://ot.shxzskj.cn

Java: if (data == null) return;
来源：http://ex.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://iw.shtwfgs.cn

Ruby: return if data.nil?
来源：http://ub.hnjuh.cn

C#:   if (data == null) return;
来源：http://jt.9csxet.cn

================================================================================
来源：http://yl.huixinmuqiang.cn

C. 函数与作用域
来源：http://be.521024.cn

================================================================================
来源：http://hp.wgjwhj.cn

[C01] 定义函数
来源：http://cz.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://mr.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dk.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://me.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zv.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cp.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rz.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://vp.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kj.huixiangedu.cn

[C02] 默认参数
来源：http://wk.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://lv.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mb.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://lz.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://we.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gc.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bn.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://yo.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://qq.nszjky.cn

[C03] 可变参数
来源：http://dh.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://cr.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vy.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rn.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://um.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xv.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wj.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://de.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ab.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://qi.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qk.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aa.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tq.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vj.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ox.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://rq.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://hj.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://fy.huixinmuqiang.cn

[C05] 返回多个值
来源：http://ww.shtwfgs.cn

Py:   return a, b
来源：http://cw.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://ml.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tl.bookmarksfly.cn

TS:   return { a, b };
来源：http://xa.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aq.newstarts.cn

Go:   return a, b
来源：http://hi.521024.cn

Ruby: return a, b
来源：http://cr.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ax.colortex.cn

[C06] 匿名函数 / lambda
来源：http://wy.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://ag.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zb.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://ci.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://wc.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yo.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kq.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://vb.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://up.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://ap.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nn.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wk.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hq.wgjwhj.cn

TS:   arr.map(String)
来源：http://ed.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gm.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yw.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://en.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ii.huixiangedu.cn

[C08] 闭包
来源：http://zr.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hw.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bq.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mr.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gd.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://we.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qi.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cy.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://br.bookmarksfly.cn

[C09] 递归
来源：http://bh.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dp.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yg.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jk.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wp.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xu.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kt.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://st.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cn.muxihuayi.cn

[C10] 变量作用域
来源：http://pr.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zv.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dg.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ye.hnjuh.cn

TS:   同 JS
来源：http://uw.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://jr.gzmigu.cn

Go:   花括号块级作用域
来源：http://qe.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ah.lnxyls.cn

C#:   块级作用域
来源：http://jw.chemitech.net.cn

[C11] 模块导入与导出
来源：http://yw.wgjwhj.cn

Py:   from module import func
来源：http://jz.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gj.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rm.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cs.huixiangedu.cn

Java: import java.util.List;
来源：http://le.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ez.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://kr.haigaiapp.cn

C#:   using System.Text;
来源：http://lr.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://mh.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://vr.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://vx.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://ln.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://yr.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dl.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://iw.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://op.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xu.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://io.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yt.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://db.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dd.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hy.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sa.nicolike.cn

Go:   func add(a, b int) int
来源：http://cp.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kh.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wq.szxytkj.cn

[C14] 泛型函数
来源：http://ia.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jj.nicolike.cn

PHP:  // 无泛型
来源：http://nr.nszjky.cn

JS:   // 无泛型
来源：http://jw.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zv.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mq.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ye.huanxung.cn

Ruby: # 无泛型
来源：http://dx.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dz.521024.cn

[C15] 解构 / 展开参数
来源：http://tp.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bw.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://gl.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ws.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hp.newstarts.cn

Java: // 无解构
来源：http://et.521024.cn

Go:   // 无解构
来源：http://vd.shtwfgs.cn

Ruby: a, b = pair
来源：http://wp.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://px.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://tz.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vy.9csxet.cn

PHP:  // 无重载
来源：http://om.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pd.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://kz.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sf.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://co.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://xo.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dk.huixinmuqiang.cn

================================================================================
来源：http://qy.521024.cn

D. 数组 / 列表 / 集合
来源：http://ox.wgjwhj.cn

================================================================================
来源：http://dx.newstarts.cn

[D01] 创建数组 / 列表
来源：http://qi.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dk.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fo.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sq.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jj.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yj.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://xb.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://pl.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fq.hahajie.cn

[D02] 追加元素到末尾
来源：http://we.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hu.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ub.huanxung.cn

JS:   arr.push(4);
来源：http://qk.yuexingan06.cn

TS:   arr.push(4);
来源：http://uj.haigaiapp.cn

Java: list.add(4);
来源：http://yb.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://dr.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://vd.shxzukj.cn

C#:   list.Add(4);
来源：http://vg.nicolike.cn

[D03] 在指定位置插入元素
来源：http://xg.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://li.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pg.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gm.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://is.panjiajie.cn

Java: list.add(0, 0);
来源：http://wk.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lr.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ci.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://rr.bjjhwx.cn

[D04] 删除元素
来源：http://tr.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rn.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yz.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mk.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://so.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hg.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kq.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uu.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://on.shxzukj.cn

[D05] 访问与修改元素
来源：http://rr.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ig.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lv.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pa.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://og.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://af.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://yc.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://of.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://im.9csxet.cn

[D06] 数组长度
来源：http://vn.huixiangedu.cn

Py:   len(arr)
来源：http://oy.haigaiapp.cn

PHP:  count($arr);
来源：http://no.lnxyls.cn

JS:   arr.length
来源：http://oz.muxihuayi.cn

TS:   arr.length
来源：http://gr.newstarts.cn

Java: list.size();
来源：http://qh.shxzskj.cn

Go:   len(arr)
来源：http://gm.colortex.cn

Ruby: arr.length; arr.size
来源：http://sd.chemitech.net.cn

C#:   list.Count;
来源：http://uz.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://bj.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tx.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nn.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://sy.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://co.colortex.cn

Java: list.subList(1, 4);
来源：http://dc.haigaiapp.cn

Go:   arr[1:4]
来源：http://ld.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://ru.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://vs.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://nc.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://pi.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://gx.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ri.jctech888.com.cn

TS:   [...a, ...b];
来源：http://xs.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ad.nszjky.cn

Go:   append(a, b...)
来源：http://oe.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://ny.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://jp.huixiangedu.cn

[D09] 排序（升序）
来源：http://ci.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://nq.chemitech.net.cn

PHP:  sort($arr);
来源：http://jd.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gh.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://al.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oj.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ek.lnxyls.cn

Ruby: arr.sort
来源：http://xg.newstarts.cn

C#:   list.Sort();
来源：http://tj.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://el.shxzskj.cn


<!-- 参考信息 -->