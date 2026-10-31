代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://su.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ms.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cp.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://yx.bookmarksfly.cn

[B09] break 与 continue
来源：http://wv.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cx.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vv.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ir.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tq.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mp.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eb.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tt.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qb.asd995.cn

[B10] 遍历同时拿索引
来源：http://qf.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qm.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mr.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qc.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ea.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oe.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jw.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sw.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rm.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://jy.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://jr.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://kz.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ux.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vm.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tx.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dt.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://xv.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qa.huixiangedu.cn

[B12] 跳出多层循环
来源：http://zw.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sc.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ps.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ij.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jw.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ox.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jp.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kk.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wx.hnjuh.cn

[B13] 判断是否为数字
来源：http://rq.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://hr.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://py.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://af.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xw.bjjhwx.cn

Java: x instanceof Number
来源：http://yv.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zw.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://cc.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://br.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://ub.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bx.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qo.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://rn.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://vq.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zp.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hl.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rh.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sm.panjiajie.cn

[B15] 布尔运算与取反
来源：http://au.asd995.cn

Py:   a and b or not c
来源：http://qu.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://zw.szsharing.cn

JS:   a && b || !c
来源：http://wy.huanxung.cn

TS:   a && b || !c
来源：http://fl.colortex.cn

Java: a && b || !c
来源：http://ge.shxzskj.cn

Go:   a && b || !c
来源：http://ys.gzmigu.cn

Ruby: a && b || !c
来源：http://lw.hahajie.cn

C#:   a && b || !c
来源：http://gx.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jo.asd995.cn

Py:   if not data: return
来源：http://qs.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://eu.bookmarksfly.cn

JS:   if (!data) return;
来源：http://jy.haigaiapp.cn

TS:   if (!data) return;
来源：http://zo.521024.cn

Java: if (data == null) return;
来源：http://iy.colortex.cn

Go:   if data == nil { return }
来源：http://up.colortex.cn

Ruby: return if data.nil?
来源：http://io.panjiajie.cn

C#:   if (data == null) return;
来源：http://ep.huixinmuqiang.cn

================================================================================
来源：http://kk.bookmarksfly.cn

C. 函数与作用域
来源：http://jq.jianghongdianzi.cn

================================================================================
来源：http://tc.yuexingan06.cn

[C01] 定义函数
来源：http://ln.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://zn.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yr.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://yw.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rs.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ji.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ln.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://kd.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ku.521024.cn

[C02] 默认参数
来源：http://wn.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://iy.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zf.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://nz.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ja.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qb.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ya.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://zb.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://to.hahajie.cn

[C03] 可变参数
来源：http://jd.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://ux.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cb.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tw.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lw.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oq.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mn.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wy.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ay.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://gi.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cy.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xl.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ya.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zw.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://nr.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://kf.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://tn.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://qc.521024.cn

[C05] 返回多个值
来源：http://tc.muxihuayi.cn

Py:   return a, b
来源：http://tu.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://zh.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kw.yuexingan06.cn

TS:   return { a, b };
来源：http://ts.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ip.huixiangedu.cn

Go:   return a, b
来源：http://wm.panjiajie.cn

Ruby: return a, b
来源：http://ax.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://tc.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://ri.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://fu.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://em.hahajie.cn

JS:   const square = x => x * x;
来源：http://su.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ew.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ap.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sb.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://il.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nx.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://xd.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hc.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hv.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nd.gzmigu.cn

TS:   arr.map(String)
来源：http://pr.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jg.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ue.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://de.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ek.asd995.cn

[C08] 闭包
来源：http://xa.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rx.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bk.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ki.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wh.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pr.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://he.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aq.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hv.hahajie.cn

[C09] 递归
来源：http://gh.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ey.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xr.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pz.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fw.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ae.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qy.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ju.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xc.jianghongdianzi.cn

[C10] 变量作用域
来源：http://yr.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cv.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qr.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xi.huanxung.cn

TS:   同 JS
来源：http://jn.9csxet.cn

Java: 方法内为块级作用域
来源：http://uu.asd995.cn

Go:   花括号块级作用域
来源：http://sx.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rq.shtwfgs.cn

C#:   块级作用域
来源：http://dh.shxzskj.cn

[C11] 模块导入与导出
来源：http://ds.521024.cn

Py:   from module import func
来源：http://yb.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eb.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yu.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mb.bjjhwx.cn

Java: import java.util.List;
来源：http://ib.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gl.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://gc.yuexingan06.cn

C#:   using System.Text;
来源：http://ow.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://oq.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://vb.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://kh.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://dt.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://kb.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://me.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://os.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://fe.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pg.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://rv.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qw.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ci.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pq.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pa.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nc.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://lw.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qf.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yc.shxzukj.cn

[C14] 泛型函数
来源：http://kv.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uu.hnjuh.cn

PHP:  // 无泛型
来源：http://ri.bjjhwx.cn

JS:   // 无泛型
来源：http://ez.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://re.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vi.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zq.jctech888.com.cn

Ruby: # 无泛型
来源：http://de.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dd.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://om.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mz.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://pc.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://to.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ry.jctech888.com.cn

Java: // 无解构
来源：http://az.nszjky.cn

Go:   // 无解构
来源：http://nw.lnxyls.cn

Ruby: a, b = pair
来源：http://ad.521024.cn

C#:   var (a, b) = pair;
来源：http://wi.hahajie.cn

[C16] 函数 / 方法重载
来源：http://xj.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sx.521024.cn

PHP:  // 无重载
来源：http://za.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lj.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://gc.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hg.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://us.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://su.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wj.panjiajie.cn

================================================================================
来源：http://ex.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://px.huixiangedu.cn

================================================================================
来源：http://wx.521024.cn

[D01] 创建数组 / 列表
来源：http://dn.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fe.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://im.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vz.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://do.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qf.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://bi.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://nd.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://am.lnxyls.cn

[D02] 追加元素到末尾
来源：http://su.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ue.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yd.chemitech.net.cn

JS:   arr.push(4);
来源：http://ng.huixiangedu.cn

TS:   arr.push(4);
来源：http://ho.jctech888.com.cn

Java: list.add(4);
来源：http://ah.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://fb.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://ol.nszjky.cn

C#:   list.Add(4);
来源：http://mz.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://fi.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://yv.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ld.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://td.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://ng.gzmigu.cn

Java: list.add(0, 0);
来源：http://fp.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mo.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ya.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://nj.yuntaijiaju.cn

[D04] 删除元素
来源：http://ne.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cv.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ub.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ny.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://tf.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yc.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://na.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hd.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://af.nicolike.cn

[D05] 访问与修改元素
来源：http://jb.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ed.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://io.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://do.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://ez.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://vn.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://pc.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kc.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ml.hahajie.cn

[D06] 数组长度
来源：http://aq.lnxyls.cn

Py:   len(arr)
来源：http://oj.szxytkj.cn

PHP:  count($arr);
来源：http://ao.yuntaijiaju.cn

JS:   arr.length
来源：http://my.huixiangedu.cn

TS:   arr.length
来源：http://ak.shtwfgs.cn

Java: list.size();
来源：http://sx.chemitech.net.cn

Go:   len(arr)
来源：http://es.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://xn.panjiajie.cn

C#:   list.Count;
来源：http://xh.nszjky.cn

[D07] 切片 / 取子数组
来源：http://gh.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ow.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yu.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://il.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://lb.asd995.cn

Java: list.subList(1, 4);
来源：http://da.shxzskj.cn

Go:   arr[1:4]
来源：http://qe.newstarts.cn

Ruby: arr[1, 3]
来源：http://qt.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://ps.shxzukj.cn

[D08] 合并两个数组
来源：http://bl.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://nk.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://uo.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kj.521024.cn

TS:   [...a, ...b];
来源：http://sd.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vt.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://qm.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://er.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://tw.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://ek.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ti.gzmigu.cn


<!-- 参考信息 -->