代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://km.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wz.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://hs.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://cw.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://oc.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qx.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://db.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://wr.shxzskj.cn

[B09] break 与 continue
来源：http://sp.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dz.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sw.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ep.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bq.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wt.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ug.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yp.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://re.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://ch.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://az.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lb.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rh.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rz.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://de.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ni.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uu.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://az.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://gg.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://je.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://gw.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wi.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://az.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bn.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rg.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://ti.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cr.gzmigu.cn

[B12] 跳出多层循环
来源：http://ye.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ow.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qa.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bb.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lx.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ki.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qa.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nx.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vo.chemitech.net.cn

[B13] 判断是否为数字
来源：http://st.521024.cn

Py:   isinstance(x, (int, float))
来源：http://qb.lnxyls.cn

PHP:  is_numeric($x)
来源：http://ic.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ez.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ve.wgjwhj.cn

Java: x instanceof Number
来源：http://ek.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rv.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://ke.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://nv.521024.cn

[B14] 判断值是否在集合内
来源：http://wj.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ls.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zq.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://tt.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://uc.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://td.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vj.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ko.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cl.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://wh.hahajie.cn

Py:   a and b or not c
来源：http://hi.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://dt.jianghongdianzi.cn

JS:   a && b || !c
来源：http://jb.9csxet.cn

TS:   a && b || !c
来源：http://od.nicolike.cn

Java: a && b || !c
来源：http://yr.gzmigu.cn

Go:   a && b || !c
来源：http://xa.shxzskj.cn

Ruby: a && b || !c
来源：http://qe.gzmigu.cn

C#:   a && b || !c
来源：http://ll.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uq.huanxung.cn

Py:   if not data: return
来源：http://mt.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://qd.nszjky.cn

JS:   if (!data) return;
来源：http://ef.shxzukj.cn

TS:   if (!data) return;
来源：http://ud.hnjuh.cn

Java: if (data == null) return;
来源：http://ra.asd995.cn

Go:   if data == nil { return }
来源：http://zc.hnjuh.cn

Ruby: return if data.nil?
来源：http://if.shtwfgs.cn

C#:   if (data == null) return;
来源：http://nn.shxzskj.cn

================================================================================
来源：http://cp.521024.cn

C. 函数与作用域
来源：http://rk.lnxyls.cn

================================================================================
来源：http://vb.shxzskj.cn

[C01] 定义函数
来源：http://na.asd995.cn

Py:   def add(a, b): return a + b
来源：http://pb.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jl.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://po.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gv.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dg.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hw.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://ca.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vu.nicolike.cn

[C02] 默认参数
来源：http://sd.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://yf.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ca.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://pn.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vl.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eu.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yu.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://bn.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://qn.chemitech.net.cn

[C03] 可变参数
来源：http://kl.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://ih.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://io.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aq.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ic.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kv.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sn.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ud.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lv.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://sz.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ss.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ow.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ly.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kj.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://zl.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://gd.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://vx.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://mw.muxihuayi.cn

[C05] 返回多个值
来源：http://ic.gzmigu.cn

Py:   return a, b
来源：http://ns.hnjuh.cn

PHP:  return [$a, $b];
来源：http://oa.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zk.yuntaijiaju.cn

TS:   return { a, b };
来源：http://as.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ig.bjjhwx.cn

Go:   return a, b
来源：http://uw.nszjky.cn

Ruby: return a, b
来源：http://cq.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://qi.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://dt.521024.cn

Py:   square = lambda x: x * x
来源：http://ig.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ay.szsharing.cn

JS:   const square = x => x * x;
来源：http://lv.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://xg.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fc.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mj.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://so.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zi.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://sn.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vz.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xw.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tt.bookmarksfly.cn

TS:   arr.map(String)
来源：http://op.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://is.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://li.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://tt.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fb.yuntaijiaju.cn

[C08] 闭包
来源：http://go.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hg.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://me.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fx.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dn.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vt.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fc.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ow.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://we.szsharing.cn

[C09] 递归
来源：http://io.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xi.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rv.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xe.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zr.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://in.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kr.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dg.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ym.9csxet.cn

[C10] 变量作用域
来源：http://ey.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jc.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vx.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uc.9csxet.cn

TS:   同 JS
来源：http://wr.9csxet.cn

Java: 方法内为块级作用域
来源：http://vh.panjiajie.cn

Go:   花括号块级作用域
来源：http://hv.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ze.9csxet.cn

C#:   块级作用域
来源：http://og.yuexingan06.cn

[C11] 模块导入与导出
来源：http://he.huixinmuqiang.cn

Py:   from module import func
来源：http://gk.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xx.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ws.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ww.jianghongdianzi.cn

Java: import java.util.List;
来源：http://xz.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ng.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://dq.panjiajie.cn

C#:   using System.Text;
来源：http://uy.521024.cn

[C12] 立即执行函数 IIFE
来源：http://ma.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://am.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://nr.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://zr.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://lb.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tx.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://be.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://hp.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cu.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://sk.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ju.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uz.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wz.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wq.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xe.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://cl.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nw.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ub.521024.cn

[C14] 泛型函数
来源：http://ob.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vp.nicolike.cn

PHP:  // 无泛型
来源：http://sm.huixinmuqiang.cn

JS:   // 无泛型
来源：http://jt.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dy.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yi.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xf.newstarts.cn

Ruby: # 无泛型
来源：http://hc.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dk.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://yo.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pm.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://cn.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nt.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qf.nszjky.cn

Java: // 无解构
来源：http://wr.nszjky.cn

Go:   // 无解构
来源：http://sc.yuexingan06.cn

Ruby: a, b = pair
来源：http://fl.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://gw.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://yh.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ll.colortex.cn

PHP:  // 无重载
来源：http://ja.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zm.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://vt.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gs.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://la.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://rz.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mt.jctech888.com.cn

================================================================================
来源：http://he.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://ph.shtwfgs.cn

================================================================================
来源：http://mz.asd995.cn

[D01] 创建数组 / 列表
来源：http://il.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ie.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ei.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oj.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tl.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bt.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://uh.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://xs.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gd.hnjuh.cn

[D02] 追加元素到末尾
来源：http://ko.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xi.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rn.newstarts.cn

JS:   arr.push(4);
来源：http://yo.huanxung.cn

TS:   arr.push(4);
来源：http://od.hnjuh.cn

Java: list.add(4);
来源：http://uo.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://vp.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ac.huanxung.cn

C#:   list.Add(4);
来源：http://bg.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://tm.asd995.cn

Py:   arr.insert(0, 0)
来源：http://qn.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pe.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jg.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://qh.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://zv.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nz.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nr.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://et.9csxet.cn

[D04] 删除元素
来源：http://ng.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ry.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hu.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aq.colortex.cn

TS:   arr.splice(0, 1);
来源：http://bp.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gm.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://za.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kx.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wx.521024.cn

[D05] 访问与修改元素
来源：http://bj.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oa.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vd.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vg.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://dc.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ex.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://xa.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ee.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qw.panjiajie.cn

[D06] 数组长度
来源：http://id.521024.cn

Py:   len(arr)
来源：http://jl.asd995.cn

PHP:  count($arr);
来源：http://aa.bookmarksfly.cn

JS:   arr.length
来源：http://cb.newstarts.cn

TS:   arr.length
来源：http://hx.szsharing.cn

Java: list.size();
来源：http://dk.shxzskj.cn

Go:   len(arr)
来源：http://ai.nszjky.cn

Ruby: arr.length; arr.size
来源：http://wh.jctech888.com.cn

C#:   list.Count;
来源：http://qs.huanxung.cn

[D07] 切片 / 取子数组
来源：http://my.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://te.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ei.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://bp.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://gv.lnxyls.cn

Java: list.subList(1, 4);
来源：http://qe.szxytkj.cn

Go:   arr[1:4]
来源：http://ii.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://yl.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://at.wgjwhj.cn

[D08] 合并两个数组
来源：http://jp.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://na.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://wa.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vx.colortex.cn

TS:   [...a, ...b];
来源：http://cp.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ns.hahajie.cn

Go:   append(a, b...)
来源：http://ki.asd995.cn


<!-- 参考信息 -->