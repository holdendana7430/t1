代发 wailian999

[B09] break 与 continue
来源：http://um.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tc.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vt.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tr.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vo.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tm.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vm.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yx.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://db.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://pv.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://by.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://el.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ym.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hc.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nl.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rb.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hg.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ii.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://xt.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://qu.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://wo.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zz.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cy.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sw.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://av.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://lo.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hv.shxzukj.cn

[B12] 跳出多层循环
来源：http://lc.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jl.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tu.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mb.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zi.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gw.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ki.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://or.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ol.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://gk.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://po.nicolike.cn

PHP:  is_numeric($x)
来源：http://wb.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xp.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ym.jianghongdianzi.cn

Java: x instanceof Number
来源：http://ue.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://go.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://yn.nszjky.cn

C#:   x is int or double or decimal
来源：http://me.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://qb.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ce.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mb.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://cp.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://nh.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wt.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oo.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rr.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cv.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://qn.jctech888.com.cn

Py:   a and b or not c
来源：http://to.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://la.shxzskj.cn

JS:   a && b || !c
来源：http://ir.nicolike.cn

TS:   a && b || !c
来源：http://nn.shxzukj.cn

Java: a && b || !c
来源：http://za.colortex.cn

Go:   a && b || !c
来源：http://oi.shxzukj.cn

Ruby: a && b || !c
来源：http://pw.muxihuayi.cn

C#:   a && b || !c
来源：http://zp.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sw.hahajie.cn

Py:   if not data: return
来源：http://rb.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://bg.shtwfgs.cn

JS:   if (!data) return;
来源：http://zn.shxzukj.cn

TS:   if (!data) return;
来源：http://xt.lnxyls.cn

Java: if (data == null) return;
来源：http://vd.521024.cn

Go:   if data == nil { return }
来源：http://ie.hahajie.cn

Ruby: return if data.nil?
来源：http://qm.gzmigu.cn

C#:   if (data == null) return;
来源：http://mc.newstarts.cn

================================================================================
来源：http://ab.jianghongdianzi.cn

C. 函数与作用域
来源：http://ix.szsharing.cn

================================================================================
来源：http://gd.hnjuh.cn

[C01] 定义函数
来源：http://mi.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://ls.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kb.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://ts.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fp.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ep.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mr.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://rc.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dr.jianghongdianzi.cn

[C02] 默认参数
来源：http://rn.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://bu.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mj.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://tz.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bc.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ky.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bb.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ht.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://iq.haigaiapp.cn

[C03] 可变参数
来源：http://yw.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://ji.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vp.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cy.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yk.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qz.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pi.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qm.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qc.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://tl.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zt.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dp.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bo.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ty.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://zj.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://wx.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://ua.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://kv.yuntaijiaju.cn

[C05] 返回多个值
来源：http://rs.lnxyls.cn

Py:   return a, b
来源：http://eu.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://hs.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xd.szxytkj.cn

TS:   return { a, b };
来源：http://ub.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ra.yuexingan06.cn

Go:   return a, b
来源：http://tt.nszjky.cn

Ruby: return a, b
来源：http://bv.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://ga.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://co.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://wl.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gq.shxzskj.cn

JS:   const square = x => x * x;
来源：http://qe.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://sl.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rq.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pm.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://bd.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://js.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://nu.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gj.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://to.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yb.muxihuayi.cn

TS:   arr.map(String)
来源：http://vm.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wb.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://og.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://wl.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fc.shxzskj.cn

[C08] 闭包
来源：http://bf.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://si.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hc.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ui.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://up.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vk.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vm.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xx.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ye.nszjky.cn

[C09] 递归
来源：http://sy.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kw.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ex.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ef.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xi.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ia.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sw.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kl.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pa.huixinmuqiang.cn

[C10] 变量作用域
来源：http://nh.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sc.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hd.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gg.jctech888.com.cn

TS:   同 JS
来源：http://du.lnxyls.cn

Java: 方法内为块级作用域
来源：http://ym.huanxung.cn

Go:   花括号块级作用域
来源：http://pr.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ej.jctech888.com.cn

C#:   块级作用域
来源：http://hh.shtwfgs.cn

[C11] 模块导入与导出
来源：http://tp.wgjwhj.cn

Py:   from module import func
来源：http://om.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bh.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ug.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sp.hahajie.cn

Java: import java.util.List;
来源：http://yj.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vp.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://ay.shxzukj.cn

C#:   using System.Text;
来源：http://jf.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://xn.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://cp.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://kn.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://bf.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://ca.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lw.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://xj.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://sl.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oa.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://hg.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cl.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xp.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://it.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bp.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://co.hahajie.cn

Go:   func add(a, b int) int
来源：http://cv.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jx.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nc.521024.cn

[C14] 泛型函数
来源：http://bo.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ev.colortex.cn

PHP:  // 无泛型
来源：http://do.shxzskj.cn

JS:   // 无泛型
来源：http://gh.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fw.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ok.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://df.bjjhwx.cn

Ruby: # 无泛型
来源：http://av.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://og.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://fx.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sg.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://hj.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xy.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ur.panjiajie.cn

Java: // 无解构
来源：http://uz.nicolike.cn

Go:   // 无解构
来源：http://iu.bjjhwx.cn

Ruby: a, b = pair
来源：http://so.szsharing.cn

C#:   var (a, b) = pair;
来源：http://xi.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://as.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xm.szxytkj.cn

PHP:  // 无重载
来源：http://sm.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vk.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://hu.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nt.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://oo.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://hx.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ny.wgjwhj.cn

================================================================================
来源：http://iu.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://pn.panjiajie.cn

================================================================================
来源：http://bp.9csxet.cn

[D01] 创建数组 / 列表
来源：http://jn.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://se.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fu.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hw.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xt.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pj.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://hk.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://tp.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hb.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://jr.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zt.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cl.szxytkj.cn

JS:   arr.push(4);
来源：http://ff.9csxet.cn

TS:   arr.push(4);
来源：http://qo.hahajie.cn

Java: list.add(4);
来源：http://wh.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://kw.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://no.yuexingan06.cn

C#:   list.Add(4);
来源：http://fq.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://yq.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://sk.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jz.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fv.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ai.lnxyls.cn

Java: list.add(0, 0);
来源：http://ko.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cd.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mg.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://or.huanxung.cn

[D04] 删除元素
来源：http://pe.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gi.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vf.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dw.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://hq.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ug.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mg.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sm.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ht.hnjuh.cn

[D05] 访问与修改元素
来源：http://cj.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mc.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qd.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gz.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://al.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://gr.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://kb.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bg.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dr.yuntaijiaju.cn

[D06] 数组长度
来源：http://ep.huanxung.cn

Py:   len(arr)
来源：http://be.wgjwhj.cn

PHP:  count($arr);
来源：http://rg.asd995.cn

JS:   arr.length
来源：http://dm.asd995.cn

TS:   arr.length
来源：http://pq.9csxet.cn

Java: list.size();
来源：http://dq.huixinmuqiang.cn

Go:   len(arr)
来源：http://um.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://db.szxytkj.cn

C#:   list.Count;
来源：http://wv.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://na.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hw.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vl.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://gi.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://yz.colortex.cn

Java: list.subList(1, 4);
来源：http://bh.huixiangedu.cn

Go:   arr[1:4]
来源：http://yj.szxytkj.cn

Ruby: arr[1, 3]
来源：http://my.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://if.lnxyls.cn

[D08] 合并两个数组
来源：http://pc.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://xk.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://sh.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kw.szxytkj.cn

TS:   [...a, ...b];
来源：http://xy.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://va.521024.cn

Go:   append(a, b...)
来源：http://ti.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://oi.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://hl.521024.cn

[D09] 排序（升序）
来源：http://sj.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://qj.wgjwhj.cn

PHP:  sort($arr);
来源：http://pd.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hi.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pp.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://py.bjjhwx.cn


<!-- 参考信息 -->