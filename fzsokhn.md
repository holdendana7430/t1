代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://ff.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yj.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://ll.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://ks.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://ce.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ik.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mu.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://ca.hnjuh.cn

[B09] break 与 continue
来源：http://cx.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ju.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ee.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vp.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xh.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gy.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aj.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mg.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sk.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ac.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gp.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://im.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dn.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xr.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oi.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rt.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wx.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cc.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://or.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://ks.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://yw.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uz.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sf.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bj.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tb.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://cd.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dz.shxzskj.cn

[B12] 跳出多层循环
来源：http://ah.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tp.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gj.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rh.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qa.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ro.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pu.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ko.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ga.muxihuayi.cn

[B13] 判断是否为数字
来源：http://dd.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://as.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://up.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://of.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wr.bookmarksfly.cn

Java: x instanceof Number
来源：http://el.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tq.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://xv.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ii.hahajie.cn

[B14] 判断值是否在集合内
来源：http://tt.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hv.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ir.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://ag.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://ar.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rv.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jh.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lp.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tw.panjiajie.cn

[B15] 布尔运算与取反
来源：http://yu.szsharing.cn

Py:   a and b or not c
来源：http://zz.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://yr.521024.cn

JS:   a && b || !c
来源：http://zu.chemitech.net.cn

TS:   a && b || !c
来源：http://th.hahajie.cn

Java: a && b || !c
来源：http://hk.huixiangedu.cn

Go:   a && b || !c
来源：http://ag.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://hr.huixiangedu.cn

C#:   a && b || !c
来源：http://gm.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ef.nicolike.cn

Py:   if not data: return
来源：http://mk.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://mp.asd995.cn

JS:   if (!data) return;
来源：http://so.panjiajie.cn

TS:   if (!data) return;
来源：http://ks.jctech888.com.cn

Java: if (data == null) return;
来源：http://yb.huanxung.cn

Go:   if data == nil { return }
来源：http://ac.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://kq.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://lf.wgjwhj.cn

================================================================================
来源：http://qz.chemitech.net.cn

C. 函数与作用域
来源：http://ob.jctech888.com.cn

================================================================================
来源：http://md.newstarts.cn

[C01] 定义函数
来源：http://uy.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://ca.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sq.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://xz.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ax.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ok.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tp.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://pq.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ok.asd995.cn

[C02] 默认参数
来源：http://lu.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://aa.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wb.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://iw.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ea.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sl.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yu.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://xk.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://bf.asd995.cn

[C03] 可变参数
来源：http://nm.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://im.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://md.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kf.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gs.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fl.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gv.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hx.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eg.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://va.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tw.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qu.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fj.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jh.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://vs.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://gy.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://fq.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://xu.521024.cn

[C05] 返回多个值
来源：http://ug.chemitech.net.cn

Py:   return a, b
来源：http://aw.lnxyls.cn

PHP:  return [$a, $b];
来源：http://jn.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fd.bjjhwx.cn

TS:   return { a, b };
来源：http://jm.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tq.huixinmuqiang.cn

Go:   return a, b
来源：http://ip.asd995.cn

Ruby: return a, b
来源：http://ol.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://de.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://gv.nicolike.cn

Py:   square = lambda x: x * x
来源：http://vd.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dd.szxytkj.cn

JS:   const square = x => x * x;
来源：http://yd.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://nm.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bb.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kw.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://lz.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://de.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://jq.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sg.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ql.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://on.gzmigu.cn

TS:   arr.map(String)
来源：http://yt.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nx.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://op.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://pi.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zw.huanxung.cn

[C08] 闭包
来源：http://cn.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tx.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zv.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://al.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mw.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://da.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hl.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://co.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ki.szxytkj.cn

[C09] 递归
来源：http://py.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://si.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fu.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rt.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yj.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rq.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ba.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xt.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ib.hnjuh.cn

[C10] 变量作用域
来源：http://jw.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gy.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nm.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://om.yuntaijiaju.cn

TS:   同 JS
来源：http://ul.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://wh.yuexingan06.cn

Go:   花括号块级作用域
来源：http://gz.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dm.9csxet.cn

C#:   块级作用域
来源：http://xu.chemitech.net.cn

[C11] 模块导入与导出
来源：http://vi.asd995.cn

Py:   from module import func
来源：http://sd.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tz.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yn.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ne.huanxung.cn

Java: import java.util.List;
来源：http://wd.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ks.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://ir.bjjhwx.cn

C#:   using System.Text;
来源：http://hp.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://hb.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://sx.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://te.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://mc.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://oq.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cw.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ym.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://yv.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://to.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://fv.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dk.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yd.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ew.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uo.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ct.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://kq.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bf.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://du.nszjky.cn

[C14] 泛型函数
来源：http://dr.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kg.yuexingan06.cn

PHP:  // 无泛型
来源：http://xb.hnjuh.cn

JS:   // 无泛型
来源：http://bg.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ep.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ta.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kr.gzmigu.cn

Ruby: # 无泛型
来源：http://xo.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oy.colortex.cn

[C15] 解构 / 展开参数
来源：http://ua.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bk.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://gt.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://es.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cw.wgjwhj.cn

Java: // 无解构
来源：http://jm.bjjhwx.cn

Go:   // 无解构
来源：http://fn.asd995.cn

Ruby: a, b = pair
来源：http://zs.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://hj.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://tn.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vg.szxytkj.cn

PHP:  // 无重载
来源：http://ie.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kh.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://wf.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yt.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://ci.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://gz.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iv.nszjky.cn

================================================================================
来源：http://gl.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://pa.panjiajie.cn

================================================================================
来源：http://uv.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://ft.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://am.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nw.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qs.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tz.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qn.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ny.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://hp.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ss.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://wm.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qf.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ub.muxihuayi.cn

JS:   arr.push(4);
来源：http://mn.wgjwhj.cn

TS:   arr.push(4);
来源：http://is.asd995.cn

Java: list.add(4);
来源：http://pd.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://be.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://wc.521024.cn

C#:   list.Add(4);
来源：http://ls.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://wr.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://hu.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lm.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ur.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://cv.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://bz.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gd.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ez.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://qj.jctech888.com.cn

[D04] 删除元素
来源：http://mz.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dg.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hc.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dr.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://pj.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zs.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qw.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nt.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://de.yuexingan06.cn

[D05] 访问与修改元素
来源：http://ww.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jl.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hi.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zq.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://oi.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://gb.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://un.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ya.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ut.jianghongdianzi.cn

[D06] 数组长度
来源：http://ve.yuntaijiaju.cn

Py:   len(arr)
来源：http://jm.panjiajie.cn

PHP:  count($arr);
来源：http://ro.bjjhwx.cn

JS:   arr.length
来源：http://no.haigaiapp.cn

TS:   arr.length
来源：http://wj.muxihuayi.cn

Java: list.size();
来源：http://ai.shtwfgs.cn

Go:   len(arr)
来源：http://hc.szsharing.cn

Ruby: arr.length; arr.size
来源：http://um.jianghongdianzi.cn

C#:   list.Count;
来源：http://fw.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://pi.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sf.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ud.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://rw.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://kf.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://hd.asd995.cn

Go:   arr[1:4]
来源：http://fj.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://oa.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://dt.yuexingan06.cn

[D08] 合并两个数组
来源：http://zu.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://vz.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://qn.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uz.9csxet.cn

TS:   [...a, ...b];
来源：http://vl.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bf.lnxyls.cn

Go:   append(a, b...)
来源：http://xs.nszjky.cn


<!-- 参考信息 -->