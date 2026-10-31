代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://ru.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jo.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ao.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://ns.asd995.cn

[B09] break 与 continue
来源：http://ch.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qr.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oj.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ap.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oe.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cf.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rd.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uq.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rg.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://ni.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sg.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ky.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sb.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ck.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ck.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yh.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wn.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ii.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://bi.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://cf.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://ce.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bb.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qp.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cn.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wa.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://bg.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rk.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://et.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hf.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://at.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sm.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lu.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ju.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ac.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://je.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ky.shxzukj.cn

[B13] 判断是否为数字
来源：http://yu.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://jp.panjiajie.cn

PHP:  is_numeric($x)
来源：http://do.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sb.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rj.haigaiapp.cn

Java: x instanceof Number
来源：http://mn.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rz.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://zc.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://qb.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://hv.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ra.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sp.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://tm.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://vr.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ay.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pu.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ie.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tl.hahajie.cn

[B15] 布尔运算与取反
来源：http://qk.huanxung.cn

Py:   a and b or not c
来源：http://ar.521024.cn

PHP:  $a && $b || !$c
来源：http://fg.bookmarksfly.cn

JS:   a && b || !c
来源：http://jk.newstarts.cn

TS:   a && b || !c
来源：http://tz.wgjwhj.cn

Java: a && b || !c
来源：http://mq.asd995.cn

Go:   a && b || !c
来源：http://nt.hnjuh.cn

Ruby: a && b || !c
来源：http://aa.gzmigu.cn

C#:   a && b || !c
来源：http://sn.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sr.shxzukj.cn

Py:   if not data: return
来源：http://uy.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://cc.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://xb.szxytkj.cn

TS:   if (!data) return;
来源：http://bh.bjjhwx.cn

Java: if (data == null) return;
来源：http://be.asd995.cn

Go:   if data == nil { return }
来源：http://mz.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://mr.9csxet.cn

C#:   if (data == null) return;
来源：http://sp.haigaiapp.cn

================================================================================
来源：http://ft.hnjuh.cn

C. 函数与作用域
来源：http://rw.wgjwhj.cn

================================================================================
来源：http://hc.nszjky.cn

[C01] 定义函数
来源：http://io.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://um.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cp.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://vu.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fg.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wm.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ht.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://gd.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zq.haigaiapp.cn

[C02] 默认参数
来源：http://ej.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://qd.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bi.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://br.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vq.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dy.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wf.521024.cn

Ruby: def greet(name = "World") = name
来源：http://rd.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://xh.shxzskj.cn

[C03] 可变参数
来源：http://ct.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://ag.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ha.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iz.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zy.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tl.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yz.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yo.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iv.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://wa.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oo.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hx.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rz.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wu.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://hg.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://qb.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://mj.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://qt.shxzukj.cn

[C05] 返回多个值
来源：http://za.nszjky.cn

Py:   return a, b
来源：http://tu.asd995.cn

PHP:  return [$a, $b];
来源：http://kr.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://os.newstarts.cn

TS:   return { a, b };
来源：http://vt.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rw.bookmarksfly.cn

Go:   return a, b
来源：http://hk.jctech888.com.cn

Ruby: return a, b
来源：http://vp.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://wl.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://mk.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://en.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zt.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://hn.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://sx.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nq.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fv.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://dj.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gx.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://im.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ip.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xo.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tg.lnxyls.cn

TS:   arr.map(String)
来源：http://kd.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cc.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bp.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://jw.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zb.yuexingan06.cn

[C08] 闭包
来源：http://jw.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ot.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://np.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cq.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vz.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wn.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://og.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lt.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zj.newstarts.cn

[C09] 递归
来源：http://qk.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://um.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zh.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ci.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gq.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pb.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sr.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tk.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bs.nszjky.cn

[C10] 变量作用域
来源：http://mf.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nk.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kw.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vh.szsharing.cn

TS:   同 JS
来源：http://df.szxytkj.cn

Java: 方法内为块级作用域
来源：http://ic.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://du.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bn.jctech888.com.cn

C#:   块级作用域
来源：http://hs.huanxung.cn

[C11] 模块导入与导出
来源：http://qv.colortex.cn

Py:   from module import func
来源：http://sb.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uy.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uc.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ot.nicolike.cn

Java: import java.util.List;
来源：http://cq.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vf.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://vw.yuntaijiaju.cn

C#:   using System.Text;
来源：http://se.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://bj.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://dn.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://nh.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://qn.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://jw.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gp.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://xc.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://zb.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jr.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://bn.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bw.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dk.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://be.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://in.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ug.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://pe.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://te.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rn.hahajie.cn

[C14] 泛型函数
来源：http://ii.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xx.9csxet.cn

PHP:  // 无泛型
来源：http://vv.muxihuayi.cn

JS:   // 无泛型
来源：http://px.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dg.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gs.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nl.shxzukj.cn

Ruby: # 无泛型
来源：http://tn.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://df.nszjky.cn

[C15] 解构 / 展开参数
来源：http://uj.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sx.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://tw.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nn.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ux.panjiajie.cn

Java: // 无解构
来源：http://sz.gzmigu.cn

Go:   // 无解构
来源：http://ir.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://hg.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://fk.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://zv.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xf.yuntaijiaju.cn

PHP:  // 无重载
来源：http://xe.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jh.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://kz.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ev.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://mw.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://lr.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mt.huixiangedu.cn

================================================================================
来源：http://ie.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://sz.asd995.cn

================================================================================
来源：http://at.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://yu.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jn.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ar.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xw.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qk.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jz.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://ks.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://xc.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yn.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://cn.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://py.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uw.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://zd.hahajie.cn

TS:   arr.push(4);
来源：http://vn.yuntaijiaju.cn

Java: list.add(4);
来源：http://vi.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://na.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://fx.wgjwhj.cn

C#:   list.Add(4);
来源：http://md.hahajie.cn

[D03] 在指定位置插入元素
来源：http://ms.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://tq.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hx.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bp.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://gd.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://er.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lo.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://th.colortex.cn

C#:   list.Insert(0, 0);
来源：http://ei.asd995.cn

[D04] 删除元素
来源：http://mg.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mf.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fi.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tn.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://no.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yp.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ld.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ui.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nf.colortex.cn

[D05] 访问与修改元素
来源：http://zq.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://we.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gh.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nd.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://ct.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://pd.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://wo.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kf.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tn.huanxung.cn

[D06] 数组长度
来源：http://zs.colortex.cn

Py:   len(arr)
来源：http://sp.hnjuh.cn

PHP:  count($arr);
来源：http://kl.huixiangedu.cn

JS:   arr.length
来源：http://da.panjiajie.cn

TS:   arr.length
来源：http://wv.521024.cn

Java: list.size();
来源：http://qb.muxihuayi.cn

Go:   len(arr)
来源：http://pb.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://ch.nicolike.cn

C#:   list.Count;
来源：http://cb.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://dt.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sc.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gw.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://gb.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://hb.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://bg.nicolike.cn

Go:   arr[1:4]
来源：http://zn.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://ax.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://mt.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://ta.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://ts.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://bu.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vb.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ts.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://np.bjjhwx.cn

Go:   append(a, b...)
来源：http://mj.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://ot.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://ej.shxzukj.cn

[D09] 排序（升序）
来源：http://bx.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://qk.szxytkj.cn


<!-- 参考信息 -->