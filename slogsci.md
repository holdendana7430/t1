代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xu.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://ug.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://je.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://yu.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://oi.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gl.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://qy.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://nf.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://qr.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xb.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xi.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ym.szsharing.cn

[B09] break 与 continue
来源：http://xc.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rt.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gg.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bm.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ou.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://su.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kn.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yv.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vc.huanxung.cn

[B10] 遍历同时拿索引
来源：http://dc.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ew.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hc.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vz.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qe.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sd.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nh.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vv.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ut.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://es.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://zv.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://mm.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ob.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cf.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rp.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gg.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://sk.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yv.szxytkj.cn

[B12] 跳出多层循环
来源：http://fo.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://me.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ti.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lk.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gb.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ho.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fn.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sk.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bb.colortex.cn

[B13] 判断是否为数字
来源：http://cm.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://ao.asd995.cn

PHP:  is_numeric($x)
来源：http://ua.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yj.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ym.panjiajie.cn

Java: x instanceof Number
来源：http://kl.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fp.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://ii.hahajie.cn

C#:   x is int or double or decimal
来源：http://yz.newstarts.cn

[B14] 判断值是否在集合内
来源：http://bn.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pq.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bi.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://rg.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://im.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xd.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hx.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eh.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kn.panjiajie.cn

[B15] 布尔运算与取反
来源：http://rz.bjjhwx.cn

Py:   a and b or not c
来源：http://az.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://ys.hnjuh.cn

JS:   a && b || !c
来源：http://ny.chemitech.net.cn

TS:   a && b || !c
来源：http://ix.bjjhwx.cn

Java: a && b || !c
来源：http://xq.9csxet.cn

Go:   a && b || !c
来源：http://bk.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://vy.shxzskj.cn

C#:   a && b || !c
来源：http://il.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zw.muxihuayi.cn

Py:   if not data: return
来源：http://na.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://bs.huixiangedu.cn

JS:   if (!data) return;
来源：http://zq.bjjhwx.cn

TS:   if (!data) return;
来源：http://xb.nszjky.cn

Java: if (data == null) return;
来源：http://ml.bjjhwx.cn

Go:   if data == nil { return }
来源：http://ja.bjjhwx.cn

Ruby: return if data.nil?
来源：http://pw.colortex.cn

C#:   if (data == null) return;
来源：http://rp.521024.cn

================================================================================
来源：http://fp.shtwfgs.cn

C. 函数与作用域
来源：http://ph.bjjhwx.cn

================================================================================
来源：http://pe.bjjhwx.cn

[C01] 定义函数
来源：http://af.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://zw.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gf.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://th.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fu.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aw.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bs.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://sd.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vk.colortex.cn

[C02] 默认参数
来源：http://sa.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://sk.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oi.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://rn.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sx.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xi.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ky.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://xk.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://dq.chemitech.net.cn

[C03] 可变参数
来源：http://qb.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://yw.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://da.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rm.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hg.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ry.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lu.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vx.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yr.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://bk.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bh.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pi.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wb.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jh.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://cc.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://op.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://nq.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://sc.asd995.cn

[C05] 返回多个值
来源：http://kv.nicolike.cn

Py:   return a, b
来源：http://pp.newstarts.cn

PHP:  return [$a, $b];
来源：http://ok.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yp.muxihuayi.cn

TS:   return { a, b };
来源：http://so.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fx.bookmarksfly.cn

Go:   return a, b
来源：http://zj.bookmarksfly.cn

Ruby: return a, b
来源：http://qb.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://do.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://pr.newstarts.cn

Py:   square = lambda x: x * x
来源：http://ka.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gt.panjiajie.cn

JS:   const square = x => x * x;
来源：http://yg.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://kw.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ek.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oa.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://qs.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kg.newstarts.cn

[C07] 把函数作为参数传入
来源：http://hb.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vv.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bi.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fx.panjiajie.cn

TS:   arr.map(String)
来源：http://wc.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qz.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vx.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://uj.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kx.chemitech.net.cn

[C08] 闭包
来源：http://ul.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fo.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xh.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ge.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rj.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qo.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qt.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ol.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zw.huixinmuqiang.cn

[C09] 递归
来源：http://ws.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sy.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://if.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xw.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ol.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ge.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nb.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gt.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wp.nszjky.cn

[C10] 变量作用域
来源：http://rf.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tp.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bo.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aw.colortex.cn

TS:   同 JS
来源：http://zh.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://qi.nicolike.cn

Go:   花括号块级作用域
来源：http://da.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jg.hahajie.cn

C#:   块级作用域
来源：http://xz.hnjuh.cn

[C11] 模块导入与导出
来源：http://zp.nicolike.cn

Py:   from module import func
来源：http://dw.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wv.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ne.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ox.haigaiapp.cn

Java: import java.util.List;
来源：http://cm.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jc.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://ap.521024.cn

C#:   using System.Text;
来源：http://hd.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://qi.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://lh.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://zl.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://zj.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://rn.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ys.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ae.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://ik.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hj.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://hz.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gi.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jw.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eh.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hn.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gh.szxytkj.cn

Go:   func add(a, b int) int
来源：http://gk.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bc.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://if.chemitech.net.cn

[C14] 泛型函数
来源：http://wl.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fl.nszjky.cn

PHP:  // 无泛型
来源：http://xp.wgjwhj.cn

JS:   // 无泛型
来源：http://cc.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://no.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://se.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sr.huanxung.cn

Ruby: # 无泛型
来源：http://bi.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://md.asd995.cn

[C15] 解构 / 展开参数
来源：http://up.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xs.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://pb.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oq.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vj.nszjky.cn

Java: // 无解构
来源：http://dl.muxihuayi.cn

Go:   // 无解构
来源：http://pl.hahajie.cn

Ruby: a, b = pair
来源：http://sv.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://wl.newstarts.cn

[C16] 函数 / 方法重载
来源：http://jw.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vk.nszjky.cn

PHP:  // 无重载
来源：http://ew.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://za.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://jz.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://at.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://ym.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://wv.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hn.hnjuh.cn

================================================================================
来源：http://iw.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://jt.newstarts.cn

================================================================================
来源：http://qv.9csxet.cn

[D01] 创建数组 / 列表
来源：http://lh.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cs.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xu.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ve.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ib.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dh.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://gt.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://ai.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ue.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://vm.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ec.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hf.9csxet.cn

JS:   arr.push(4);
来源：http://qe.hahajie.cn

TS:   arr.push(4);
来源：http://bb.shxzskj.cn

Java: list.add(4);
来源：http://sa.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://as.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://au.wgjwhj.cn

C#:   list.Add(4);
来源：http://bw.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://yv.colortex.cn

Py:   arr.insert(0, 0)
来源：http://uj.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ll.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uh.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ep.huixiangedu.cn

Java: list.add(0, 0);
来源：http://xr.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lh.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xp.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://ja.huixinmuqiang.cn

[D04] 删除元素
来源：http://xn.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ok.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cr.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ng.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://em.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oz.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bo.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pc.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xh.szxytkj.cn

[D05] 访问与修改元素
来源：http://qc.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://re.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rn.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qr.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://lg.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://oc.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://sv.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wl.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xy.gzmigu.cn

[D06] 数组长度
来源：http://cm.lnxyls.cn

Py:   len(arr)
来源：http://lk.szxytkj.cn

PHP:  count($arr);
来源：http://of.bjjhwx.cn

JS:   arr.length
来源：http://bj.wgjwhj.cn

TS:   arr.length
来源：http://pm.shtwfgs.cn

Java: list.size();
来源：http://ya.yuexingan06.cn

Go:   len(arr)
来源：http://ru.nszjky.cn

Ruby: arr.length; arr.size
来源：http://aw.jianghongdianzi.cn

C#:   list.Count;
来源：http://db.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://td.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fa.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rt.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://hs.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://mu.panjiajie.cn

Java: list.subList(1, 4);
来源：http://wg.hahajie.cn

Go:   arr[1:4]
来源：http://wv.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://he.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://od.shxzukj.cn

[D08] 合并两个数组
来源：http://xu.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://mk.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://ss.huixiangedu.cn


<!-- 参考信息 -->