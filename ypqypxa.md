代发 wailian999

[B09] break 与 continue
来源：http://fc.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fd.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ge.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qs.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eq.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fk.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gk.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ye.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xk.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://ll.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jk.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ti.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://di.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iq.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nz.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nz.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hv.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kv.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://mo.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://ke.asd995.cn

PHP:  range(0, 10, 2);
来源：http://cx.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qh.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xc.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vz.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bc.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://cj.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ue.panjiajie.cn

[B12] 跳出多层循环
来源：http://bb.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gg.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xx.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vl.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xb.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rx.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://go.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://py.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ya.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://vo.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://ru.9csxet.cn

PHP:  is_numeric($x)
来源：http://zc.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dl.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ps.jctech888.com.cn

Java: x instanceof Number
来源：http://zq.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bt.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://wu.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://gc.asd995.cn

[B14] 判断值是否在集合内
来源：http://xa.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rw.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oy.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://um.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://yd.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gw.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yk.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zr.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://co.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://rg.huanxung.cn

Py:   a and b or not c
来源：http://dp.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://uz.yuntaijiaju.cn

JS:   a && b || !c
来源：http://mn.huixiangedu.cn

TS:   a && b || !c
来源：http://aj.gzmigu.cn

Java: a && b || !c
来源：http://rk.szsharing.cn

Go:   a && b || !c
来源：http://gs.shtwfgs.cn

Ruby: a && b || !c
来源：http://ak.colortex.cn

C#:   a && b || !c
来源：http://vr.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ls.asd995.cn

Py:   if not data: return
来源：http://iw.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://ip.nicolike.cn

JS:   if (!data) return;
来源：http://ip.szxytkj.cn

TS:   if (!data) return;
来源：http://wo.jctech888.com.cn

Java: if (data == null) return;
来源：http://na.szxytkj.cn

Go:   if data == nil { return }
来源：http://eh.nicolike.cn

Ruby: return if data.nil?
来源：http://nb.shxzskj.cn

C#:   if (data == null) return;
来源：http://ee.muxihuayi.cn

================================================================================
来源：http://wf.hahajie.cn

C. 函数与作用域
来源：http://sa.muxihuayi.cn

================================================================================
来源：http://zu.hnjuh.cn

[C01] 定义函数
来源：http://xv.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://to.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hq.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://jp.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hr.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ks.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sp.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://rd.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tq.colortex.cn

[C02] 默认参数
来源：http://pt.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://mg.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sx.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://ch.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cj.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tt.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cs.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://zu.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://eo.yuntaijiaju.cn

[C03] 可变参数
来源：http://wq.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://tk.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ae.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dx.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rj.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vp.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://br.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dd.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://un.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://xh.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gs.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rt.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nu.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fd.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://ge.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://pv.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://zf.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://fk.huixiangedu.cn

[C05] 返回多个值
来源：http://fm.haigaiapp.cn

Py:   return a, b
来源：http://qz.hahajie.cn

PHP:  return [$a, $b];
来源：http://ph.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pr.muxihuayi.cn

TS:   return { a, b };
来源：http://cb.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oz.szxytkj.cn

Go:   return a, b
来源：http://ur.nszjky.cn

Ruby: return a, b
来源：http://pq.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://ch.asd995.cn

[C06] 匿名函数 / lambda
来源：http://cg.9csxet.cn

Py:   square = lambda x: x * x
来源：http://zj.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ek.nicolike.cn

JS:   const square = x => x * x;
来源：http://mi.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://hd.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kk.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xy.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://xf.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yj.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://kw.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cj.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jf.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dn.yuexingan06.cn

TS:   arr.map(String)
来源：http://sc.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xf.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fm.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://kg.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pr.huixiangedu.cn

[C08] 闭包
来源：http://hg.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gt.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fz.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mo.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xs.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mx.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oj.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ic.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sq.9csxet.cn

[C09] 递归
来源：http://dy.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hu.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ba.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vx.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vl.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yg.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qh.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qa.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yy.nszjky.cn

[C10] 变量作用域
来源：http://es.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iz.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://la.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xf.hahajie.cn

TS:   同 JS
来源：http://av.szxytkj.cn

Java: 方法内为块级作用域
来源：http://ov.haigaiapp.cn

Go:   花括号块级作用域
来源：http://ye.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uo.huixiangedu.cn

C#:   块级作用域
来源：http://qi.huanxung.cn

[C11] 模块导入与导出
来源：http://gm.szsharing.cn

Py:   from module import func
来源：http://tc.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bl.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ji.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://em.hnjuh.cn

Java: import java.util.List;
来源：http://ct.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ze.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://dv.521024.cn

C#:   using System.Text;
来源：http://dy.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://au.521024.cn

Py:   (lambda: print("run"))()
来源：http://px.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://wh.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://bb.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://sb.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vg.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://xd.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://qn.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://am.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://wb.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wk.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sd.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uu.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rq.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iw.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://he.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yu.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://io.shxzukj.cn

[C14] 泛型函数
来源：http://pw.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ei.colortex.cn

PHP:  // 无泛型
来源：http://oq.huixiangedu.cn

JS:   // 无泛型
来源：http://hk.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://er.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gm.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bu.huanxung.cn

Ruby: # 无泛型
来源：http://ca.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sm.nicolike.cn

[C15] 解构 / 展开参数
来源：http://so.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yw.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://yx.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pz.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ss.9csxet.cn

Java: // 无解构
来源：http://bk.bookmarksfly.cn

Go:   // 无解构
来源：http://af.nszjky.cn

Ruby: a, b = pair
来源：http://tu.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://gc.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://sn.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gh.wgjwhj.cn

PHP:  // 无重载
来源：http://ne.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wh.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://vi.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://go.521024.cn

Go:   // 无重载：用不同函数名
来源：http://ol.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://wy.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fl.colortex.cn

================================================================================
来源：http://kp.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://ih.huanxung.cn

================================================================================
来源：http://pp.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://by.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://et.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vq.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zo.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://he.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lq.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://cn.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://iz.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://og.szxytkj.cn

[D02] 追加元素到末尾
来源：http://sc.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gs.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qe.hahajie.cn

JS:   arr.push(4);
来源：http://qa.newstarts.cn

TS:   arr.push(4);
来源：http://xg.huanxung.cn

Java: list.add(4);
来源：http://tp.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://an.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://oi.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://xk.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://yt.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://gi.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lz.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wo.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://mp.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://df.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xn.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ji.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://hl.haigaiapp.cn

[D04] 删除元素
来源：http://va.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sp.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mf.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wx.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://wt.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jf.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dn.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cw.521024.cn

[D05] 访问与修改元素
来源：http://xw.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nu.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sw.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zl.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://qb.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://mg.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://vx.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ag.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://md.yuntaijiaju.cn

[D06] 数组长度
来源：http://br.bookmarksfly.cn

Py:   len(arr)
来源：http://oa.shxzskj.cn

PHP:  count($arr);
来源：http://by.huanxung.cn

JS:   arr.length
来源：http://ck.szsharing.cn

TS:   arr.length
来源：http://ex.shxzukj.cn

Java: list.size();
来源：http://vk.shxzskj.cn

Go:   len(arr)
来源：http://dk.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://lt.huixiangedu.cn

C#:   list.Count;
来源：http://dd.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://el.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pj.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gc.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://zb.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://us.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://oq.lnxyls.cn

Go:   arr[1:4]
来源：http://bp.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://et.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://qz.szsharing.cn

[D08] 合并两个数组
来源：http://mn.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://dw.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://hr.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ov.muxihuayi.cn

TS:   [...a, ...b];
来源：http://er.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fa.muxihuayi.cn

Go:   append(a, b...)
来源：http://vz.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://hg.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://bq.shxzukj.cn

[D09] 排序（升序）
来源：http://vz.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://mg.muxihuayi.cn

PHP:  sort($arr);
来源：http://hj.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://se.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qq.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pn.shxzskj.cn


<!-- 参考信息 -->