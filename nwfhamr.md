代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://py.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mb.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://ap.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://fx.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://rf.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jo.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bb.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://lx.shxzukj.cn

[B09] break 与 continue
来源：http://ep.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yt.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kl.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sz.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fn.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fw.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sb.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://su.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ka.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://lt.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iq.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ug.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wg.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ix.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uc.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xf.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ny.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wk.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://xh.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://di.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://co.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zp.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nz.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://my.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hr.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://qg.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rd.521024.cn

[B12] 跳出多层循环
来源：http://kv.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ir.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ax.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ao.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://us.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ea.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aj.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cm.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zg.nicolike.cn

[B13] 判断是否为数字
来源：http://vj.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://wb.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://zb.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iv.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wb.asd995.cn

Java: x instanceof Number
来源：http://qx.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lo.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://fv.hahajie.cn

C#:   x is int or double or decimal
来源：http://le.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://cc.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cn.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://em.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://hx.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://lv.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rw.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bg.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rc.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fn.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://gg.bjjhwx.cn

Py:   a and b or not c
来源：http://zj.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://ln.bjjhwx.cn

JS:   a && b || !c
来源：http://yy.9csxet.cn

TS:   a && b || !c
来源：http://jr.521024.cn

Java: a && b || !c
来源：http://bj.panjiajie.cn

Go:   a && b || !c
来源：http://im.shxzskj.cn

Ruby: a && b || !c
来源：http://wz.szsharing.cn

C#:   a && b || !c
来源：http://st.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uk.asd995.cn

Py:   if not data: return
来源：http://zp.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://bb.bookmarksfly.cn

JS:   if (!data) return;
来源：http://qv.gzmigu.cn

TS:   if (!data) return;
来源：http://yg.yuexingan06.cn

Java: if (data == null) return;
来源：http://ic.szsharing.cn

Go:   if data == nil { return }
来源：http://ib.szxytkj.cn

Ruby: return if data.nil?
来源：http://gj.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://af.shxzukj.cn

================================================================================
来源：http://tv.bjjhwx.cn

C. 函数与作用域
来源：http://kq.shtwfgs.cn

================================================================================
来源：http://ko.shxzukj.cn

[C01] 定义函数
来源：http://fk.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://br.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vw.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://aj.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pe.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ls.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wi.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://vn.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vh.lnxyls.cn

[C02] 默认参数
来源：http://ee.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://ch.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lz.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://dh.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yt.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fe.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jd.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://eb.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://iq.huixiangedu.cn

[C03] 可变参数
来源：http://ft.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://pu.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wo.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qi.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qu.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zq.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rw.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xb.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ci.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://xo.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qf.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wq.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ay.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kq.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://jf.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://oy.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://wa.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://ed.jctech888.com.cn

[C05] 返回多个值
来源：http://jz.newstarts.cn

Py:   return a, b
来源：http://cc.newstarts.cn

PHP:  return [$a, $b];
来源：http://nc.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xw.gzmigu.cn

TS:   return { a, b };
来源：http://sz.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://md.wgjwhj.cn

Go:   return a, b
来源：http://nj.bookmarksfly.cn

Ruby: return a, b
来源：http://jf.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://wq.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://uv.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://ae.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gv.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://uy.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://sl.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ow.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rl.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://qr.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gh.9csxet.cn

[C07] 把函数作为参数传入
来源：http://hr.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sg.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rp.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://un.yuexingan06.cn

TS:   arr.map(String)
来源：http://uc.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://au.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ts.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://qf.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wl.nicolike.cn

[C08] 闭包
来源：http://ns.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ps.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qt.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hl.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mg.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mn.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xi.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zj.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://md.521024.cn

[C09] 递归
来源：http://uy.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ga.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mc.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jp.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vh.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lh.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xl.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bw.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ry.yuexingan06.cn

[C10] 变量作用域
来源：http://ti.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xn.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nx.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vu.nszjky.cn

TS:   同 JS
来源：http://ws.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://ze.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://jh.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://de.nicolike.cn

C#:   块级作用域
来源：http://dy.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://gx.huanxung.cn

Py:   from module import func
来源：http://lm.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://le.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ba.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ye.hahajie.cn

Java: import java.util.List;
来源：http://bl.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qm.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://kx.jianghongdianzi.cn

C#:   using System.Text;
来源：http://tn.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://ba.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://vq.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://yu.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://ip.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://ku.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jo.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://ju.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://be.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bp.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://kk.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hs.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pb.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://df.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ux.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fg.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://zh.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xk.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ld.9csxet.cn

[C14] 泛型函数
来源：http://ws.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qk.lnxyls.cn

PHP:  // 无泛型
来源：http://jo.gzmigu.cn

JS:   // 无泛型
来源：http://ni.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xu.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ba.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mu.asd995.cn

Ruby: # 无泛型
来源：http://wd.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dc.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://ym.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gu.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://dn.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sh.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yg.muxihuayi.cn

Java: // 无解构
来源：http://ci.shtwfgs.cn

Go:   // 无解构
来源：http://mz.huanxung.cn

Ruby: a, b = pair
来源：http://qu.colortex.cn

C#:   var (a, b) = pair;
来源：http://dn.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://xc.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nf.nszjky.cn

PHP:  // 无重载
来源：http://ex.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tx.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://hz.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bp.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://pc.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://sp.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ir.haigaiapp.cn

================================================================================
来源：http://di.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://fk.yuntaijiaju.cn

================================================================================
来源：http://wu.nicolike.cn

[D01] 创建数组 / 列表
来源：http://by.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://im.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://al.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://of.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dx.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qy.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://he.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://ft.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://el.521024.cn

[D02] 追加元素到末尾
来源：http://iy.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://na.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ku.bookmarksfly.cn

JS:   arr.push(4);
来源：http://ik.hnjuh.cn

TS:   arr.push(4);
来源：http://pt.muxihuayi.cn

Java: list.add(4);
来源：http://fa.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://gu.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://jd.lnxyls.cn

C#:   list.Add(4);
来源：http://eb.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://wa.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://ht.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ov.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vb.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://rk.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://hm.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ze.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://po.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://ir.szxytkj.cn

[D04] 删除元素
来源：http://il.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zv.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ih.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://en.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://yw.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gg.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ro.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iz.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tm.haigaiapp.cn

[D05] 访问与修改元素
来源：http://lq.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sm.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://up.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://du.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://qb.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://py.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://zy.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hu.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ei.szsharing.cn

[D06] 数组长度
来源：http://au.szxytkj.cn

Py:   len(arr)
来源：http://or.gzmigu.cn

PHP:  count($arr);
来源：http://fa.muxihuayi.cn

JS:   arr.length
来源：http://nr.hahajie.cn

TS:   arr.length
来源：http://bq.shtwfgs.cn

Java: list.size();
来源：http://eq.jctech888.com.cn

Go:   len(arr)
来源：http://mm.szsharing.cn

Ruby: arr.length; arr.size
来源：http://rx.jianghongdianzi.cn

C#:   list.Count;
来源：http://zs.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://cc.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ih.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jv.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://wx.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://ca.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://oh.huanxung.cn

Go:   arr[1:4]
来源：http://gh.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://qp.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://ap.nicolike.cn

[D08] 合并两个数组
来源：http://la.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://le.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://jo.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lm.nicolike.cn

TS:   [...a, ...b];
来源：http://vp.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kd.nicolike.cn

Go:   append(a, b...)
来源：http://xv.hahajie.cn


<!-- 参考信息 -->