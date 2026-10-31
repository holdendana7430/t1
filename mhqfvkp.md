代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://tm.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mi.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://zb.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://og.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://fb.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mh.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xo.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://dv.asd995.cn

[B09] break 与 continue
来源：http://yj.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wf.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lj.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://db.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wk.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rt.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://il.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rm.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cu.asd995.cn

[B10] 遍历同时拿索引
来源：http://tn.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kl.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ok.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aq.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xc.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vn.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qq.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dk.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tc.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://kq.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://ki.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://pn.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ax.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tt.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ha.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nk.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://pf.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pr.haigaiapp.cn

[B12] 跳出多层循环
来源：http://gf.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jk.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pi.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ul.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wl.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://os.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ps.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ot.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xa.huixiangedu.cn

[B13] 判断是否为数字
来源：http://uw.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://dm.nicolike.cn

PHP:  is_numeric($x)
来源：http://hd.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bf.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kp.9csxet.cn

Java: x instanceof Number
来源：http://cj.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://va.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://gd.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://xz.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://ty.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xn.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ga.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://bj.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://oq.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iq.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tz.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ha.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ib.newstarts.cn

[B15] 布尔运算与取反
来源：http://fl.huixiangedu.cn

Py:   a and b or not c
来源：http://lt.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://fk.jctech888.com.cn

JS:   a && b || !c
来源：http://lv.bookmarksfly.cn

TS:   a && b || !c
来源：http://ma.asd995.cn

Java: a && b || !c
来源：http://ei.wgjwhj.cn

Go:   a && b || !c
来源：http://mn.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://dm.lnxyls.cn

C#:   a && b || !c
来源：http://sk.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pr.lnxyls.cn

Py:   if not data: return
来源：http://zw.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://wk.huanxung.cn

JS:   if (!data) return;
来源：http://mw.yuexingan06.cn

TS:   if (!data) return;
来源：http://tu.szxytkj.cn

Java: if (data == null) return;
来源：http://en.shtwfgs.cn

Go:   if data == nil { return }
来源：http://im.9csxet.cn

Ruby: return if data.nil?
来源：http://on.haigaiapp.cn

C#:   if (data == null) return;
来源：http://ao.panjiajie.cn

================================================================================
来源：http://ho.colortex.cn

C. 函数与作用域
来源：http://wf.hnjuh.cn

================================================================================
来源：http://ow.gzmigu.cn

[C01] 定义函数
来源：http://qf.colortex.cn

Py:   def add(a, b): return a + b
来源：http://bi.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nr.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://lp.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uk.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dk.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cb.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://gp.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dk.huixiangedu.cn

[C02] 默认参数
来源：http://jn.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://nq.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://km.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://tn.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pj.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ub.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tb.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ib.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://dt.shxzskj.cn

[C03] 可变参数
来源：http://tj.521024.cn

Py:   def total(*args): return sum(args)
来源：http://dj.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ga.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iw.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cz.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rs.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vp.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uy.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ph.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://of.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://es.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ni.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ir.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tn.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://av.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://aa.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://uq.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://nl.jctech888.com.cn

[C05] 返回多个值
来源：http://um.shtwfgs.cn

Py:   return a, b
来源：http://tu.shxzskj.cn

PHP:  return [$a, $b];
来源：http://qj.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qn.lnxyls.cn

TS:   return { a, b };
来源：http://oe.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pk.huanxung.cn

Go:   return a, b
来源：http://fi.521024.cn

Ruby: return a, b
来源：http://sm.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://wo.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://po.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://qf.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ax.asd995.cn

JS:   const square = x => x * x;
来源：http://tb.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://ld.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fm.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ch.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://tv.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ws.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://hn.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yq.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mh.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pk.hahajie.cn

TS:   arr.map(String)
来源：http://lb.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lw.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pc.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://el.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xf.colortex.cn

[C08] 闭包
来源：http://jv.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rj.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ys.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qk.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qa.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://el.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zn.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gx.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ks.jctech888.com.cn

[C09] 递归
来源：http://ud.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sm.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xd.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wp.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gj.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ig.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rz.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xg.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rv.szxytkj.cn

[C10] 变量作用域
来源：http://qp.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kg.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xr.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dh.chemitech.net.cn

TS:   同 JS
来源：http://tb.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://yg.muxihuayi.cn

Go:   花括号块级作用域
来源：http://ud.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hk.panjiajie.cn

C#:   块级作用域
来源：http://lk.jctech888.com.cn

[C11] 模块导入与导出
来源：http://oc.huixiangedu.cn

Py:   from module import func
来源：http://pf.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kp.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hp.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xq.bookmarksfly.cn

Java: import java.util.List;
来源：http://ah.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wk.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://zf.yuexingan06.cn

C#:   using System.Text;
来源：http://qh.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://km.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://re.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://dl.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://xj.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://ug.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://al.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://km.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://uu.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ni.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://lk.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jh.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wc.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ki.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mb.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zq.shxzskj.cn

Go:   func add(a, b int) int
来源：http://fe.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zl.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qm.huanxung.cn

[C14] 泛型函数
来源：http://tq.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vh.nszjky.cn

PHP:  // 无泛型
来源：http://vq.szsharing.cn

JS:   // 无泛型
来源：http://ih.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pe.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tk.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://po.szxytkj.cn

Ruby: # 无泛型
来源：http://sp.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qn.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://em.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qt.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://wg.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bv.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tq.nicolike.cn

Java: // 无解构
来源：http://az.newstarts.cn

Go:   // 无解构
来源：http://ad.chemitech.net.cn

Ruby: a, b = pair
来源：http://vs.nicolike.cn

C#:   var (a, b) = pair;
来源：http://rw.521024.cn

[C16] 函数 / 方法重载
来源：http://pn.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sg.yuntaijiaju.cn

PHP:  // 无重载
来源：http://bx.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ps.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://uo.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tc.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://lv.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://ie.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zx.szsharing.cn

================================================================================
来源：http://wa.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://bw.lnxyls.cn

================================================================================
来源：http://qx.szsharing.cn

[D01] 创建数组 / 列表
来源：http://nu.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yi.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://op.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kq.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rf.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dw.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ib.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://wa.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wt.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://wa.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ff.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wt.shxzukj.cn

JS:   arr.push(4);
来源：http://pu.bookmarksfly.cn

TS:   arr.push(4);
来源：http://cf.jctech888.com.cn

Java: list.add(4);
来源：http://lg.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://pt.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://vp.yuexingan06.cn

C#:   list.Add(4);
来源：http://mu.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://nh.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://wi.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xc.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ca.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://xd.haigaiapp.cn

Java: list.add(0, 0);
来源：http://hx.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://go.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ik.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://jo.huixinmuqiang.cn

[D04] 删除元素
来源：http://xz.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bf.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zr.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zu.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://ve.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vl.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nw.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bx.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vg.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://nv.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rf.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yu.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hh.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://cw.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://je.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://no.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oe.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://om.colortex.cn

[D06] 数组长度
来源：http://sw.yuexingan06.cn

Py:   len(arr)
来源：http://sm.szxytkj.cn

PHP:  count($arr);
来源：http://yh.9csxet.cn

JS:   arr.length
来源：http://pj.haigaiapp.cn

TS:   arr.length
来源：http://tk.shtwfgs.cn

Java: list.size();
来源：http://sr.lnxyls.cn

Go:   len(arr)
来源：http://jz.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://vb.nicolike.cn

C#:   list.Count;
来源：http://ra.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://pt.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dw.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cg.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://xd.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://tv.szsharing.cn

Java: list.subList(1, 4);
来源：http://sb.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://fz.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://sg.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://mi.hahajie.cn

[D08] 合并两个数组
来源：http://ya.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://in.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://dk.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sg.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://ne.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wc.9csxet.cn

Go:   append(a, b...)
来源：http://hw.jctech888.com.cn


<!-- 参考信息 -->