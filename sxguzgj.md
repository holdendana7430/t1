代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://za.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://os.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://wd.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://cp.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vc.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://zb.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://gg.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://zi.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://tn.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ie.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://jb.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://gf.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://zt.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wv.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ef.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://by.jianghongdianzi.cn

[B09] break 与 continue
来源：http://wq.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ot.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ah.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dk.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nj.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://um.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vr.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xs.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hf.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://vw.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vi.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ml.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://az.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vc.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xw.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ye.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ze.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gi.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://gj.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://on.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://rm.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vx.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qm.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fy.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xw.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://hw.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zr.521024.cn

[B12] 跳出多层循环
来源：http://mj.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dj.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rc.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yb.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nh.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zg.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ws.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://li.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://il.jctech888.com.cn

[B13] 判断是否为数字
来源：http://vu.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://no.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://cs.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vn.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xz.nicolike.cn

Java: x instanceof Number
来源：http://nc.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ak.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://ki.panjiajie.cn

C#:   x is int or double or decimal
来源：http://bv.asd995.cn

[B14] 判断值是否在集合内
来源：http://sn.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pe.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bx.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://px.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://dm.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sz.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jo.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gm.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oe.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://zi.hnjuh.cn

Py:   a and b or not c
来源：http://fo.521024.cn

PHP:  $a && $b || !$c
来源：http://rn.szsharing.cn

JS:   a && b || !c
来源：http://bw.hnjuh.cn

TS:   a && b || !c
来源：http://xr.panjiajie.cn

Java: a && b || !c
来源：http://za.bookmarksfly.cn

Go:   a && b || !c
来源：http://kv.bjjhwx.cn

Ruby: a && b || !c
来源：http://lh.szxytkj.cn

C#:   a && b || !c
来源：http://xk.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://py.bjjhwx.cn

Py:   if not data: return
来源：http://cm.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://qg.haigaiapp.cn

JS:   if (!data) return;
来源：http://og.haigaiapp.cn

TS:   if (!data) return;
来源：http://uu.newstarts.cn

Java: if (data == null) return;
来源：http://sg.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://po.panjiajie.cn

Ruby: return if data.nil?
来源：http://sk.yuexingan06.cn

C#:   if (data == null) return;
来源：http://ni.huixiangedu.cn

================================================================================
来源：http://ae.yuntaijiaju.cn

C. 函数与作用域
来源：http://ot.bookmarksfly.cn

================================================================================
来源：http://lc.haigaiapp.cn

[C01] 定义函数
来源：http://pe.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://wh.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aq.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://ck.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://en.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yc.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://in.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://ik.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ar.bookmarksfly.cn

[C02] 默认参数
来源：http://gf.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://px.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jy.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://dv.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fl.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zt.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mc.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://gx.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://ef.huanxung.cn

[C03] 可变参数
来源：http://ob.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://jm.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gl.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jm.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rq.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tt.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rp.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pe.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oy.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://el.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://no.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fz.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nb.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://te.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://fm.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://qr.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://pt.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://uv.newstarts.cn

[C05] 返回多个值
来源：http://yh.wgjwhj.cn

Py:   return a, b
来源：http://jd.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://pt.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mv.szxytkj.cn

TS:   return { a, b };
来源：http://ml.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pq.newstarts.cn

Go:   return a, b
来源：http://ax.newstarts.cn

Ruby: return a, b
来源：http://ur.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://dr.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://jr.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://td.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wg.panjiajie.cn

JS:   const square = x => x * x;
来源：http://bp.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://rn.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qz.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iq.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://du.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hk.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://nd.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qo.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vr.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://in.shxzskj.cn

TS:   arr.map(String)
来源：http://cg.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ob.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fp.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://uo.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://de.muxihuayi.cn

[C08] 闭包
来源：http://ie.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mj.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vv.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xq.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rc.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sq.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jy.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vx.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bx.shxzskj.cn

[C09] 递归
来源：http://nv.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iq.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nz.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kx.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ai.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ui.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xs.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qc.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nu.panjiajie.cn

[C10] 变量作用域
来源：http://bt.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ox.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uo.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zh.huanxung.cn

TS:   同 JS
来源：http://zc.hnjuh.cn

Java: 方法内为块级作用域
来源：http://yp.521024.cn

Go:   花括号块级作用域
来源：http://bi.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rd.huixinmuqiang.cn

C#:   块级作用域
来源：http://ux.colortex.cn

[C11] 模块导入与导出
来源：http://ld.panjiajie.cn

Py:   from module import func
来源：http://jj.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qf.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hh.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lx.jianghongdianzi.cn

Java: import java.util.List;
来源：http://ea.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ye.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://vy.jctech888.com.cn

C#:   using System.Text;
来源：http://eg.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://cl.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://ja.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://pb.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://gp.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://rr.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rz.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://jn.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://lr.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wj.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://ji.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://la.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sr.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lv.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qe.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fr.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://pt.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ix.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rt.yuntaijiaju.cn

[C14] 泛型函数
来源：http://qb.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://by.shtwfgs.cn

PHP:  // 无泛型
来源：http://bi.shxzukj.cn

JS:   // 无泛型
来源：http://zc.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gl.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fp.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tw.panjiajie.cn

Ruby: # 无泛型
来源：http://ju.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://py.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://np.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://he.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://pf.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sb.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pq.yuntaijiaju.cn

Java: // 无解构
来源：http://sv.huixinmuqiang.cn

Go:   // 无解构
来源：http://hp.newstarts.cn

Ruby: a, b = pair
来源：http://yq.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://zn.huanxung.cn

[C16] 函数 / 方法重载
来源：http://jw.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jb.gzmigu.cn

PHP:  // 无重载
来源：http://vu.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tj.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://nm.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gv.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://sy.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://he.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://re.jianghongdianzi.cn

================================================================================
来源：http://sy.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://xf.yuexingan06.cn

================================================================================
来源：http://rn.nszjky.cn

[D01] 创建数组 / 列表
来源：http://ir.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sf.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wc.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://da.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ts.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mr.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://uj.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://ab.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ts.shxzskj.cn

[D02] 追加元素到末尾
来源：http://eo.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nm.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lh.shxzskj.cn

JS:   arr.push(4);
来源：http://tt.521024.cn

TS:   arr.push(4);
来源：http://wt.chemitech.net.cn

Java: list.add(4);
来源：http://mj.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://zx.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://xk.szsharing.cn

C#:   list.Add(4);
来源：http://aq.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://fr.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://vz.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://th.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://av.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://vu.nicolike.cn

Java: list.add(0, 0);
来源：http://bt.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kx.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fu.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://ou.wgjwhj.cn

[D04] 删除元素
来源：http://dx.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cy.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yv.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rc.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://vr.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gm.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://io.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ic.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ce.hahajie.cn

[D05] 访问与修改元素
来源：http://zc.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fx.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kv.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yn.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://fv.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://yl.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://zg.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vl.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vw.gzmigu.cn

[D06] 数组长度
来源：http://dd.yuexingan06.cn

Py:   len(arr)
来源：http://mw.jctech888.com.cn

PHP:  count($arr);
来源：http://ig.hahajie.cn

JS:   arr.length
来源：http://nk.yuntaijiaju.cn

TS:   arr.length
来源：http://qi.nicolike.cn

Java: list.size();
来源：http://kd.gzmigu.cn

Go:   len(arr)
来源：http://uz.szsharing.cn

Ruby: arr.length; arr.size
来源：http://fr.muxihuayi.cn

C#:   list.Count;
来源：http://jm.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://kk.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wy.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oh.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://tn.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://dk.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://pq.huanxung.cn

Go:   arr[1:4]
来源：http://jj.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://rf.bookmarksfly.cn


<!-- 参考信息 -->