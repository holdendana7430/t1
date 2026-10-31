代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cl.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://gx.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://je.521024.cn

[B08] do-while（至少执行一次）
来源：http://hf.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ni.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pp.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://ow.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://ro.521024.cn

Java: do { i++; } while (i < 10);
来源：http://gh.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gz.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tu.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://fc.haigaiapp.cn

[B09] break 与 continue
来源：http://oa.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kh.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://st.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fi.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ss.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ox.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eb.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qk.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.newstarts.cn

[B10] 遍历同时拿索引
来源：http://qb.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jz.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kn.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pr.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rr.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cy.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oi.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wu.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jn.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://uk.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://qi.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://nl.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qr.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fc.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://si.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ej.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://vc.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sb.chemitech.net.cn

[B12] 跳出多层循环
来源：http://ev.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ym.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fq.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gs.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gx.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fm.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gn.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://up.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gh.nszjky.cn

[B13] 判断是否为数字
来源：http://kb.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://ty.nicolike.cn

PHP:  is_numeric($x)
来源：http://rj.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kk.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oe.muxihuayi.cn

Java: x instanceof Number
来源：http://dh.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lq.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://xi.hahajie.cn

C#:   x is int or double or decimal
来源：http://of.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://zk.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qg.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tc.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://lm.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://bs.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ky.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zn.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gq.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://am.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://ss.chemitech.net.cn

Py:   a and b or not c
来源：http://bu.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://gd.hahajie.cn

JS:   a && b || !c
来源：http://qq.huixinmuqiang.cn

TS:   a && b || !c
来源：http://jl.panjiajie.cn

Java: a && b || !c
来源：http://eo.wgjwhj.cn

Go:   a && b || !c
来源：http://vo.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://zg.szsharing.cn

C#:   a && b || !c
来源：http://rp.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qf.hnjuh.cn

Py:   if not data: return
来源：http://qe.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://wy.chemitech.net.cn

JS:   if (!data) return;
来源：http://dl.bjjhwx.cn

TS:   if (!data) return;
来源：http://kb.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://em.newstarts.cn

Go:   if data == nil { return }
来源：http://wn.lnxyls.cn

Ruby: return if data.nil?
来源：http://hr.wgjwhj.cn

C#:   if (data == null) return;
来源：http://zv.huixiangedu.cn

================================================================================
来源：http://te.newstarts.cn

C. 函数与作用域
来源：http://cq.9csxet.cn

================================================================================
来源：http://ab.shxzskj.cn

[C01] 定义函数
来源：http://xx.colortex.cn

Py:   def add(a, b): return a + b
来源：http://qd.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wv.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://xw.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ug.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nl.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hk.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://eb.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gy.newstarts.cn

[C02] 默认参数
来源：http://do.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://pw.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ki.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://gt.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vq.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qk.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ip.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://bl.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://gq.shxzskj.cn

[C03] 可变参数
来源：http://lq.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://jl.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fy.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rx.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fb.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pk.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pb.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hq.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qm.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://tb.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bf.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qb.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cb.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vo.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://td.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://us.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://ms.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://rw.szsharing.cn

[C05] 返回多个值
来源：http://mj.newstarts.cn

Py:   return a, b
来源：http://xz.9csxet.cn

PHP:  return [$a, $b];
来源：http://ov.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xr.hahajie.cn

TS:   return { a, b };
来源：http://wv.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zy.9csxet.cn

Go:   return a, b
来源：http://cm.lnxyls.cn

Ruby: return a, b
来源：http://tb.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://my.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://uv.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://km.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xz.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://sr.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ml.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ze.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fg.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://xh.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://el.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://ih.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yn.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tz.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://im.hahajie.cn

TS:   arr.map(String)
来源：http://gw.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wg.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bk.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://df.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pj.nicolike.cn

[C08] 闭包
来源：http://pj.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eq.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cw.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ik.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dq.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ba.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ls.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gn.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qz.gzmigu.cn

[C09] 递归
来源：http://hx.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://su.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nn.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zv.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ia.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cr.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ov.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ug.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sa.huixinmuqiang.cn

[C10] 变量作用域
来源：http://rj.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nu.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://on.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ag.hnjuh.cn

TS:   同 JS
来源：http://vl.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://cc.hahajie.cn

Go:   花括号块级作用域
来源：http://dy.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yu.szxytkj.cn

C#:   块级作用域
来源：http://me.shtwfgs.cn

[C11] 模块导入与导出
来源：http://ht.newstarts.cn

Py:   from module import func
来源：http://av.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mh.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hi.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cx.nicolike.cn

Java: import java.util.List;
来源：http://kk.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vt.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://rn.szxytkj.cn

C#:   using System.Text;
来源：http://uu.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://ap.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://wv.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://qy.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://md.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://te.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yj.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://ak.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://jf.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ev.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://aj.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lv.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zm.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kh.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nf.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zg.asd995.cn

Go:   func add(a, b int) int
来源：http://xc.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ic.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wv.asd995.cn

[C14] 泛型函数
来源：http://ia.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yz.huanxung.cn

PHP:  // 无泛型
来源：http://am.shxzskj.cn

JS:   // 无泛型
来源：http://cv.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xl.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sl.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vj.muxihuayi.cn

Ruby: # 无泛型
来源：http://vi.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ut.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://nu.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oc.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://vh.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xb.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ee.muxihuayi.cn

Java: // 无解构
来源：http://ga.shxzskj.cn

Go:   // 无解构
来源：http://ip.shxzskj.cn

Ruby: a, b = pair
来源：http://nf.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://cp.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://va.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wz.nszjky.cn

PHP:  // 无重载
来源：http://gl.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kp.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://qt.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yw.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://nd.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://xr.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fy.521024.cn

================================================================================
来源：http://hg.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://yt.panjiajie.cn

================================================================================
来源：http://lx.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://kd.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ph.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vf.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nv.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vl.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wz.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://jk.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://zs.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hk.nszjky.cn

[D02] 追加元素到末尾
来源：http://qz.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vb.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bx.colortex.cn

JS:   arr.push(4);
来源：http://yu.huixiangedu.cn

TS:   arr.push(4);
来源：http://ia.huanxung.cn

Java: list.add(4);
来源：http://pq.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://nv.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://gs.bookmarksfly.cn

C#:   list.Add(4);
来源：http://hm.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://js.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://ng.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iv.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sb.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://bo.colortex.cn

Java: list.add(0, 0);
来源：http://ng.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nf.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eg.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://jk.gzmigu.cn

[D04] 删除元素
来源：http://at.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ha.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kb.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hi.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://of.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mz.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nj.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ja.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ox.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://bl.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oo.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yh.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yz.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://wy.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://oc.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://ai.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lr.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aa.yuntaijiaju.cn

[D06] 数组长度
来源：http://jn.yuntaijiaju.cn

Py:   len(arr)
来源：http://eq.huanxung.cn

PHP:  count($arr);
来源：http://je.asd995.cn

JS:   arr.length
来源：http://wq.colortex.cn

TS:   arr.length
来源：http://oq.jianghongdianzi.cn

Java: list.size();
来源：http://oy.bjjhwx.cn

Go:   len(arr)
来源：http://so.asd995.cn

Ruby: arr.length; arr.size
来源：http://uc.yuexingan06.cn

C#:   list.Count;
来源：http://oe.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://og.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pe.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ki.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://fn.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://ft.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://bw.bookmarksfly.cn

Go:   arr[1:4]
来源：http://yf.colortex.cn

Ruby: arr[1, 3]
来源：http://jj.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://ge.hnjuh.cn

[D08] 合并两个数组
来源：http://pl.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://gt.asd995.cn

PHP:  array_merge($a, $b);
来源：http://up.521024.cn


<!-- 参考信息 -->