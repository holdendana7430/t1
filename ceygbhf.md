代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://kh.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://at.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ax.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://df.nszjky.cn

[B09] break 与 continue
来源：http://qg.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vh.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://id.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rl.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xv.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vt.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hd.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tb.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pw.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://ab.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dh.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rv.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qo.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kk.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://od.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qs.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lx.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tl.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://qe.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://zj.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://pi.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jd.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kt.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://de.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mr.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://iw.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xu.hahajie.cn

[B12] 跳出多层循环
来源：http://lg.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lk.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gq.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cd.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dr.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tm.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kh.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sh.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gv.muxihuayi.cn

[B13] 判断是否为数字
来源：http://vd.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://rt.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://hq.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vy.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ac.bookmarksfly.cn

Java: x instanceof Number
来源：http://nc.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iv.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://xa.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://vg.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://nn.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hn.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://id.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://rt.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://dv.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lo.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uc.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://et.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pv.shxzskj.cn

[B15] 布尔运算与取反
来源：http://vc.colortex.cn

Py:   a and b or not c
来源：http://nx.huanxung.cn

PHP:  $a && $b || !$c
来源：http://nz.yuntaijiaju.cn

JS:   a && b || !c
来源：http://xi.colortex.cn

TS:   a && b || !c
来源：http://mg.panjiajie.cn

Java: a && b || !c
来源：http://vh.szsharing.cn

Go:   a && b || !c
来源：http://dy.hahajie.cn

Ruby: a && b || !c
来源：http://hy.wgjwhj.cn

C#:   a && b || !c
来源：http://ch.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gq.jctech888.com.cn

Py:   if not data: return
来源：http://cx.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://og.gzmigu.cn

JS:   if (!data) return;
来源：http://ge.nszjky.cn

TS:   if (!data) return;
来源：http://wk.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://gu.hnjuh.cn

Go:   if data == nil { return }
来源：http://qj.nicolike.cn

Ruby: return if data.nil?
来源：http://wf.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://rc.shxzukj.cn

================================================================================
来源：http://km.huixiangedu.cn

C. 函数与作用域
来源：http://mw.wgjwhj.cn

================================================================================
来源：http://kh.panjiajie.cn

[C01] 定义函数
来源：http://jr.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://bn.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://if.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://sl.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fz.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hb.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nq.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://wr.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nk.gzmigu.cn

[C02] 默认参数
来源：http://yv.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://dm.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sx.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://br.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vq.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tk.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://se.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://vo.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://dl.hnjuh.cn

[C03] 可变参数
来源：http://ps.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://er.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zr.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qk.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dm.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dz.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ts.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ju.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mx.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://ne.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qd.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hv.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qs.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gp.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://je.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://dn.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://uh.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://sz.muxihuayi.cn

[C05] 返回多个值
来源：http://ht.9csxet.cn

Py:   return a, b
来源：http://uz.9csxet.cn

PHP:  return [$a, $b];
来源：http://sh.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qb.yuntaijiaju.cn

TS:   return { a, b };
来源：http://nl.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ir.muxihuayi.cn

Go:   return a, b
来源：http://do.wgjwhj.cn

Ruby: return a, b
来源：http://lx.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://hi.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://cf.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://vt.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uy.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://nh.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://ud.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wk.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pa.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://sz.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hi.9csxet.cn

[C07] 把函数作为参数传入
来源：http://io.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xz.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://db.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kn.panjiajie.cn

TS:   arr.map(String)
来源：http://xa.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aj.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kk.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://hw.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rm.bookmarksfly.cn

[C08] 闭包
来源：http://bf.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wu.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aa.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jt.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cr.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://up.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jc.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cw.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fl.wgjwhj.cn

[C09] 递归
来源：http://hn.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zz.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mv.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jf.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ye.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mj.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wp.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ik.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pa.colortex.cn

[C10] 变量作用域
来源：http://sh.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qz.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xr.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ww.newstarts.cn

TS:   同 JS
来源：http://wx.panjiajie.cn

Java: 方法内为块级作用域
来源：http://ov.yuexingan06.cn

Go:   花括号块级作用域
来源：http://en.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://na.jctech888.com.cn

C#:   块级作用域
来源：http://ec.szxytkj.cn

[C11] 模块导入与导出
来源：http://ks.newstarts.cn

Py:   from module import func
来源：http://tk.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tr.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mb.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mc.szsharing.cn

Java: import java.util.List;
来源：http://db.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yk.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://pe.jctech888.com.cn

C#:   using System.Text;
来源：http://vp.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ck.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://xf.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://tc.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://nv.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://hf.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nm.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ya.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://yy.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wv.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://hd.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pf.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vr.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yr.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oe.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xq.shxzskj.cn

Go:   func add(a, b int) int
来源：http://zb.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sr.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wv.szsharing.cn

[C14] 泛型函数
来源：http://or.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://is.hnjuh.cn

PHP:  // 无泛型
来源：http://st.haigaiapp.cn

JS:   // 无泛型
来源：http://ex.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dd.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://je.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fd.nicolike.cn

Ruby: # 无泛型
来源：http://rr.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://or.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://ok.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ft.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://ff.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ld.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ae.nszjky.cn

Java: // 无解构
来源：http://tn.muxihuayi.cn

Go:   // 无解构
来源：http://ot.bookmarksfly.cn

Ruby: a, b = pair
来源：http://gy.szsharing.cn

C#:   var (a, b) = pair;
来源：http://ev.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://ok.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ks.shtwfgs.cn

PHP:  // 无重载
来源：http://xj.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tt.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://af.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ow.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://ez.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://jg.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fw.nicolike.cn

================================================================================
来源：http://ps.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://zw.asd995.cn

================================================================================
来源：http://ti.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://en.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ay.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://al.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qi.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wc.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gn.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://kg.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://gh.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mu.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://km.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ph.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://og.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://hu.nszjky.cn

TS:   arr.push(4);
来源：http://bq.szsharing.cn

Java: list.add(4);
来源：http://pm.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://ih.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://wc.chemitech.net.cn

C#:   list.Add(4);
来源：http://rd.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://fi.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://yp.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wq.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gu.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://li.szxytkj.cn

Java: list.add(0, 0);
来源：http://hw.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rc.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ls.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://ya.szsharing.cn

[D04] 删除元素
来源：http://mk.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tk.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mx.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://tu.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lo.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://do.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dt.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vg.nszjky.cn

[D05] 访问与修改元素
来源：http://nw.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ag.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zl.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tt.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://iv.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://la.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://sh.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bt.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kt.colortex.cn

[D06] 数组长度
来源：http://cp.colortex.cn

Py:   len(arr)
来源：http://wt.wgjwhj.cn

PHP:  count($arr);
来源：http://xw.gzmigu.cn

JS:   arr.length
来源：http://bs.lnxyls.cn

TS:   arr.length
来源：http://yz.521024.cn

Java: list.size();
来源：http://fw.panjiajie.cn

Go:   len(arr)
来源：http://am.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://yb.huixiangedu.cn

C#:   list.Count;
来源：http://ej.nszjky.cn

[D07] 切片 / 取子数组
来源：http://fk.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tx.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://um.521024.cn

JS:   arr.slice(1, 4);
来源：http://es.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://uf.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://ja.nszjky.cn

Go:   arr[1:4]
来源：http://qz.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://if.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ju.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://gv.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://pw.colortex.cn

PHP:  array_merge($a, $b);
来源：http://yq.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tr.nicolike.cn

TS:   [...a, ...b];
来源：http://en.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ce.haigaiapp.cn

Go:   append(a, b...)
来源：http://vs.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://ze.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://df.chemitech.net.cn

[D09] 排序（升序）
来源：http://cq.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://wq.shxzukj.cn


<!-- 参考信息 -->