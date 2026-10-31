代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://xc.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vg.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sv.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://sr.9csxet.cn

[B09] break 与 continue
来源：http://ws.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://se.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ti.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vt.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yp.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vs.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yd.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qa.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wm.521024.cn

[B10] 遍历同时拿索引
来源：http://jz.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xw.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mb.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pa.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ox.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hn.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rg.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sa.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://gi.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://xy.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://xe.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wd.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://im.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ft.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://id.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://ta.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gi.huanxung.cn

[B12] 跳出多层循环
来源：http://vn.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jo.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bd.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qx.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ue.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tl.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ro.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fo.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zi.gzmigu.cn

[B13] 判断是否为数字
来源：http://cn.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://qk.szxytkj.cn

PHP:  is_numeric($x)
来源：http://ll.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mj.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xo.muxihuayi.cn

Java: x instanceof Number
来源：http://wg.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yo.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://se.gzmigu.cn

C#:   x is int or double or decimal
来源：http://hd.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://hy.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cg.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fe.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://da.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://tg.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vv.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vr.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xd.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rj.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://wi.jctech888.com.cn

Py:   a and b or not c
来源：http://mq.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://bl.jctech888.com.cn

JS:   a && b || !c
来源：http://rp.nicolike.cn

TS:   a && b || !c
来源：http://yc.lnxyls.cn

Java: a && b || !c
来源：http://va.newstarts.cn

Go:   a && b || !c
来源：http://zy.haigaiapp.cn

Ruby: a && b || !c
来源：http://cd.yuexingan06.cn

C#:   a && b || !c
来源：http://qr.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hm.jianghongdianzi.cn

Py:   if not data: return
来源：http://yt.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://up.chemitech.net.cn

JS:   if (!data) return;
来源：http://af.nszjky.cn

TS:   if (!data) return;
来源：http://np.nszjky.cn

Java: if (data == null) return;
来源：http://ri.wgjwhj.cn

Go:   if data == nil { return }
来源：http://zh.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://qa.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://ln.nszjky.cn

================================================================================
来源：http://kn.shxzskj.cn

C. 函数与作用域
来源：http://ui.wgjwhj.cn

================================================================================
来源：http://pk.szxytkj.cn

[C01] 定义函数
来源：http://of.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://mt.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jk.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://ci.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ww.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zj.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://at.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://lm.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zr.panjiajie.cn

[C02] 默认参数
来源：http://ng.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://rw.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tx.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://gh.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jq.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://th.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ti.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://ri.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://mp.nszjky.cn

[C03] 可变参数
来源：http://dz.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://de.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lh.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ro.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lx.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xn.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ju.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sh.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vo.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://bw.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hg.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qt.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kn.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rx.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://sl.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://qc.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://sa.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://ut.yuntaijiaju.cn

[C05] 返回多个值
来源：http://ih.521024.cn

Py:   return a, b
来源：http://av.newstarts.cn

PHP:  return [$a, $b];
来源：http://ue.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://en.nicolike.cn

TS:   return { a, b };
来源：http://eb.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gg.lnxyls.cn

Go:   return a, b
来源：http://je.yuexingan06.cn

Ruby: return a, b
来源：http://xr.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://ar.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://bt.newstarts.cn

Py:   square = lambda x: x * x
来源：http://rf.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cd.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://gv.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://xw.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qx.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sb.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://mt.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dm.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://dz.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fa.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yg.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nz.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://we.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mn.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://le.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://gu.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wq.huixinmuqiang.cn

[C08] 闭包
来源：http://fx.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ff.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://js.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xp.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bu.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ly.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ld.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ii.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lx.bjjhwx.cn

[C09] 递归
来源：http://xi.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ni.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hn.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zu.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://el.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fk.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yv.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hu.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ww.huixiangedu.cn

[C10] 变量作用域
来源：http://un.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ac.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xs.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qg.bjjhwx.cn

TS:   同 JS
来源：http://dc.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://lu.yuexingan06.cn

Go:   花括号块级作用域
来源：http://oa.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ms.panjiajie.cn

C#:   块级作用域
来源：http://md.newstarts.cn

[C11] 模块导入与导出
来源：http://nr.lnxyls.cn

Py:   from module import func
来源：http://qj.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ip.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aw.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qo.muxihuayi.cn

Java: import java.util.List;
来源：http://rg.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qa.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://yo.nicolike.cn

C#:   using System.Text;
来源：http://vr.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://lo.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://iy.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://re.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://lu.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://ri.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zi.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://qx.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://uh.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lc.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://sw.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dd.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pz.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oh.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://es.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wk.hahajie.cn

Go:   func add(a, b int) int
来源：http://jk.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xf.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://br.jianghongdianzi.cn

[C14] 泛型函数
来源：http://cw.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cl.huixiangedu.cn

PHP:  // 无泛型
来源：http://vq.huixinmuqiang.cn

JS:   // 无泛型
来源：http://zz.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cn.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uu.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://um.huixiangedu.cn

Ruby: # 无泛型
来源：http://ap.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hf.nszjky.cn

[C15] 解构 / 展开参数
来源：http://mj.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pv.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://bx.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mu.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bx.szsharing.cn

Java: // 无解构
来源：http://gy.hnjuh.cn

Go:   // 无解构
来源：http://ef.shxzskj.cn

Ruby: a, b = pair
来源：http://sz.521024.cn

C#:   var (a, b) = pair;
来源：http://iw.newstarts.cn

[C16] 函数 / 方法重载
来源：http://oi.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://my.szsharing.cn

PHP:  // 无重载
来源：http://ws.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kp.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://bs.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://at.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://sh.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://jt.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gr.lnxyls.cn

================================================================================
来源：http://er.asd995.cn

D. 数组 / 列表 / 集合
来源：http://qh.wgjwhj.cn

================================================================================
来源：http://yq.huanxung.cn

[D01] 创建数组 / 列表
来源：http://zo.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hg.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sd.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ok.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ky.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uq.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://eq.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://ly.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://af.521024.cn

[D02] 追加元素到末尾
来源：http://db.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dw.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rp.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://sp.nicolike.cn

TS:   arr.push(4);
来源：http://lz.hnjuh.cn

Java: list.add(4);
来源：http://qj.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://hb.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://dh.shxzskj.cn

C#:   list.Add(4);
来源：http://et.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://qa.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://ro.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fy.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sx.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://lm.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://jw.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xh.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nk.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://bm.9csxet.cn

[D04] 删除元素
来源：http://sn.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vo.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wh.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ce.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://dd.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bv.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ke.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://as.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mu.haigaiapp.cn

[D05] 访问与修改元素
来源：http://eb.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ti.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hd.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yy.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://tm.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://vn.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://iw.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://br.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iw.lnxyls.cn

[D06] 数组长度
来源：http://ga.jctech888.com.cn

Py:   len(arr)
来源：http://yd.huixinmuqiang.cn

PHP:  count($arr);
来源：http://yx.jianghongdianzi.cn

JS:   arr.length
来源：http://ht.gzmigu.cn

TS:   arr.length
来源：http://ky.bookmarksfly.cn

Java: list.size();
来源：http://pa.lnxyls.cn

Go:   len(arr)
来源：http://sp.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://ys.nicolike.cn

C#:   list.Count;
来源：http://dd.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://to.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rc.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wj.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://zx.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://ck.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://to.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://ok.huanxung.cn

Ruby: arr[1, 3]
来源：http://hv.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://dq.jctech888.com.cn

[D08] 合并两个数组
来源：http://yd.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://es.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://xr.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rp.yuexingan06.cn

TS:   [...a, ...b];
来源：http://pi.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aw.nicolike.cn

Go:   append(a, b...)
来源：http://ti.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://ua.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://kq.nszjky.cn

[D09] 排序（升序）
来源：http://xx.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://pu.wgjwhj.cn


<!-- 参考信息 -->