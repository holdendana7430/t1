代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xx.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://uq.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://ky.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://qv.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://us.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jc.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://pd.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://ch.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://hx.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qr.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sz.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://dp.shtwfgs.cn

[B09] break 与 continue
来源：http://se.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yq.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zl.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lm.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ki.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ta.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bo.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bo.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://aa.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gd.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qd.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://st.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wm.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cw.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dy.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zx.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eq.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://zi.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://jy.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://rt.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oh.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jt.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cm.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vj.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://to.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ey.yuexingan06.cn

[B12] 跳出多层循环
来源：http://kn.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xx.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zi.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sc.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sf.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zp.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nq.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cf.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sa.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://tg.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://zw.9csxet.cn

PHP:  is_numeric($x)
来源：http://ss.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sa.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ta.huixiangedu.cn

Java: x instanceof Number
来源：http://yz.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ab.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://ez.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://mt.asd995.cn

[B14] 判断值是否在集合内
来源：http://kt.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ic.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ml.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://ft.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://on.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qa.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zk.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wm.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nz.521024.cn

[B15] 布尔运算与取反
来源：http://rt.wgjwhj.cn

Py:   a and b or not c
来源：http://qx.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://zt.bookmarksfly.cn

JS:   a && b || !c
来源：http://fj.panjiajie.cn

TS:   a && b || !c
来源：http://ly.hnjuh.cn

Java: a && b || !c
来源：http://ro.nszjky.cn

Go:   a && b || !c
来源：http://tk.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://kf.shtwfgs.cn

C#:   a && b || !c
来源：http://aj.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oz.chemitech.net.cn

Py:   if not data: return
来源：http://lq.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://bi.gzmigu.cn

JS:   if (!data) return;
来源：http://zg.szsharing.cn

TS:   if (!data) return;
来源：http://ts.nicolike.cn

Java: if (data == null) return;
来源：http://rf.wgjwhj.cn

Go:   if data == nil { return }
来源：http://bj.huanxung.cn

Ruby: return if data.nil?
来源：http://kl.9csxet.cn

C#:   if (data == null) return;
来源：http://bq.szsharing.cn

================================================================================
来源：http://im.9csxet.cn

C. 函数与作用域
来源：http://gx.nszjky.cn

================================================================================
来源：http://fd.jianghongdianzi.cn

[C01] 定义函数
来源：http://ad.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://iq.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://md.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://dg.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hf.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ne.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dm.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://sg.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://es.nszjky.cn

[C02] 默认参数
来源：http://mk.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://el.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ja.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://kh.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ri.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ao.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fk.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://fv.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://zi.jianghongdianzi.cn

[C03] 可变参数
来源：http://ka.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://ek.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kl.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hw.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://by.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pd.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gv.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iq.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mn.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://nn.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hu.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kh.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bz.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://es.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ab.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://cy.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://on.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://hx.521024.cn

[C05] 返回多个值
来源：http://pf.newstarts.cn

Py:   return a, b
来源：http://ud.colortex.cn

PHP:  return [$a, $b];
来源：http://wp.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://js.shxzukj.cn

TS:   return { a, b };
来源：http://sm.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lv.nicolike.cn

Go:   return a, b
来源：http://du.9csxet.cn

Ruby: return a, b
来源：http://dp.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://bi.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://hn.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://or.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xp.nszjky.cn

JS:   const square = x => x * x;
来源：http://sm.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://qm.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ak.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hx.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://rg.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oc.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://rm.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ke.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hv.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sw.shxzukj.cn

TS:   arr.map(String)
来源：http://ih.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qj.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pb.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://ef.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gj.newstarts.cn

[C08] 闭包
来源：http://ph.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ek.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tz.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lt.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://th.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ab.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pu.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sq.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kx.szsharing.cn

[C09] 递归
来源：http://ph.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gr.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hm.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jf.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bx.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gd.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gm.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wu.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wq.lnxyls.cn

[C10] 变量作用域
来源：http://qb.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pz.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ez.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hf.shtwfgs.cn

TS:   同 JS
来源：http://sz.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ly.shxzukj.cn

Go:   花括号块级作用域
来源：http://lo.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xk.shxzskj.cn

C#:   块级作用域
来源：http://si.shxzukj.cn

[C11] 模块导入与导出
来源：http://ct.muxihuayi.cn

Py:   from module import func
来源：http://sc.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ub.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vi.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eq.wgjwhj.cn

Java: import java.util.List;
来源：http://us.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fy.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://ps.haigaiapp.cn

C#:   using System.Text;
来源：http://po.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://mc.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://hk.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://ue.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://lz.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://os.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://na.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://wu.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://rx.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tc.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://kw.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ro.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ob.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://po.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nx.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gc.asd995.cn

Go:   func add(a, b int) int
来源：http://xi.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wc.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ny.haigaiapp.cn

[C14] 泛型函数
来源：http://sb.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fi.newstarts.cn

PHP:  // 无泛型
来源：http://xo.shtwfgs.cn

JS:   // 无泛型
来源：http://qc.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ew.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ry.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kw.newstarts.cn

Ruby: # 无泛型
来源：http://qy.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eq.9csxet.cn

[C15] 解构 / 展开参数
来源：http://op.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ng.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://dk.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gq.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kg.nicolike.cn

Java: // 无解构
来源：http://lf.gzmigu.cn

Go:   // 无解构
来源：http://kh.newstarts.cn

Ruby: a, b = pair
来源：http://mi.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://sj.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://vm.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yz.huixiangedu.cn

PHP:  // 无重载
来源：http://dh.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dg.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://tp.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rl.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://tw.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://xk.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zf.521024.cn

================================================================================
来源：http://qs.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://rn.nicolike.cn

================================================================================
来源：http://mh.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://ct.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tt.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kk.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zw.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qu.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lf.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ml.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://tu.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mb.nszjky.cn

[D02] 追加元素到末尾
来源：http://mv.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cu.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ut.nszjky.cn

JS:   arr.push(4);
来源：http://ta.chemitech.net.cn

TS:   arr.push(4);
来源：http://hg.asd995.cn

Java: list.add(4);
来源：http://gu.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://tq.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://kj.521024.cn

C#:   list.Add(4);
来源：http://rz.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://vh.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://hx.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wj.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ac.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://cc.wgjwhj.cn

Java: list.add(0, 0);
来源：http://ty.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cq.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qr.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://kw.huanxung.cn

[D04] 删除元素
来源：http://wt.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uz.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mu.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lw.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://oq.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vt.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rp.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ln.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fs.wgjwhj.cn

[D05] 访问与修改元素
来源：http://re.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zm.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dv.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uh.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://hd.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://vm.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://dv.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mm.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qi.yuntaijiaju.cn

[D06] 数组长度
来源：http://nf.521024.cn

Py:   len(arr)
来源：http://cm.newstarts.cn

PHP:  count($arr);
来源：http://nn.bjjhwx.cn

JS:   arr.length
来源：http://hj.lnxyls.cn

TS:   arr.length
来源：http://jg.chemitech.net.cn

Java: list.size();
来源：http://yq.chemitech.net.cn

Go:   len(arr)
来源：http://kd.9csxet.cn

Ruby: arr.length; arr.size
来源：http://jc.yuntaijiaju.cn

C#:   list.Count;
来源：http://cu.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://hg.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cg.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uu.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://fh.asd995.cn

TS:   arr.slice(1, 4);
来源：http://gc.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://fp.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://uo.521024.cn

Ruby: arr[1, 3]
来源：http://on.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://zz.muxihuayi.cn

[D08] 合并两个数组
来源：http://cq.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://sb.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://yr.yuntaijiaju.cn


<!-- 参考信息 -->