代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://nb.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mp.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://xf.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://zw.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://bk.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hu.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ob.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://wn.lnxyls.cn

[B09] break 与 continue
来源：http://ub.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ap.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://id.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sn.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ql.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mv.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cm.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ie.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fb.521024.cn

[B10] 遍历同时拿索引
来源：http://cg.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ru.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yd.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mk.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jl.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xw.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kp.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dz.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pa.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://hh.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://yk.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://oe.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gb.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bn.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eo.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yh.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://pt.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://th.nicolike.cn

[B12] 跳出多层循环
来源：http://ab.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ra.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jv.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bp.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ru.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://me.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cw.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iy.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wr.nicolike.cn

[B13] 判断是否为数字
来源：http://sp.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://fc.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://vd.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ox.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ma.shxzskj.cn

Java: x instanceof Number
来源：http://bo.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://os.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://yf.huanxung.cn

C#:   x is int or double or decimal
来源：http://xd.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://bl.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qm.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sn.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://xs.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://xf.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zy.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://db.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vz.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bz.hnjuh.cn

[B15] 布尔运算与取反
来源：http://rr.chemitech.net.cn

Py:   a and b or not c
来源：http://sx.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://te.huixiangedu.cn

JS:   a && b || !c
来源：http://mh.huixinmuqiang.cn

TS:   a && b || !c
来源：http://zl.szsharing.cn

Java: a && b || !c
来源：http://hm.huanxung.cn

Go:   a && b || !c
来源：http://bh.newstarts.cn

Ruby: a && b || !c
来源：http://dg.shtwfgs.cn

C#:   a && b || !c
来源：http://wh.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mg.panjiajie.cn

Py:   if not data: return
来源：http://pi.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://vn.9csxet.cn

JS:   if (!data) return;
来源：http://jq.chemitech.net.cn

TS:   if (!data) return;
来源：http://zg.szxytkj.cn

Java: if (data == null) return;
来源：http://ut.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://cm.newstarts.cn

Ruby: return if data.nil?
来源：http://sj.hnjuh.cn

C#:   if (data == null) return;
来源：http://fb.asd995.cn

================================================================================
来源：http://hg.newstarts.cn

C. 函数与作用域
来源：http://rz.muxihuayi.cn

================================================================================
来源：http://tw.gzmigu.cn

[C01] 定义函数
来源：http://yp.asd995.cn

Py:   def add(a, b): return a + b
来源：http://rz.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://me.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://ke.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pc.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jo.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fz.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://zd.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iu.panjiajie.cn

[C02] 默认参数
来源：http://xo.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://ah.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gz.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://vi.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://db.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://df.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cq.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://cj.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://xl.wgjwhj.cn

[C03] 可变参数
来源：http://dy.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://di.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rn.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ly.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://en.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wr.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kt.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nf.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cy.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://lw.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fr.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qd.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rd.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nj.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://vk.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://yk.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://fh.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://kb.jianghongdianzi.cn

[C05] 返回多个值
来源：http://nw.bookmarksfly.cn

Py:   return a, b
来源：http://dg.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://bc.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cp.huixinmuqiang.cn

TS:   return { a, b };
来源：http://vv.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ka.521024.cn

Go:   return a, b
来源：http://fu.wgjwhj.cn

Ruby: return a, b
来源：http://za.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://eh.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://dr.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://go.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ws.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://ss.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://wq.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tc.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hq.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://cz.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lb.colortex.cn

[C07] 把函数作为参数传入
来源：http://fz.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tg.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jo.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kl.huanxung.cn

TS:   arr.map(String)
来源：http://mu.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://og.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hl.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://fi.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ub.huanxung.cn

[C08] 闭包
来源：http://ij.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ai.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://py.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pw.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ca.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tu.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cl.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ro.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yi.jianghongdianzi.cn

[C09] 递归
来源：http://wt.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hv.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ry.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rg.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://br.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ie.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vr.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://er.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sp.521024.cn

[C10] 变量作用域
来源：http://pl.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ey.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aa.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gt.panjiajie.cn

TS:   同 JS
来源：http://fs.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://av.newstarts.cn

Go:   花括号块级作用域
来源：http://kq.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kh.haigaiapp.cn

C#:   块级作用域
来源：http://wx.nicolike.cn

[C11] 模块导入与导出
来源：http://xe.colortex.cn

Py:   from module import func
来源：http://wa.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mi.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ce.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dt.lnxyls.cn

Java: import java.util.List;
来源：http://uq.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fi.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://cq.lnxyls.cn

C#:   using System.Text;
来源：http://mv.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://xy.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://dl.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://py.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://cd.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://yj.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zl.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://in.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://si.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qr.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://lg.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sx.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ds.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hl.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yj.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nx.panjiajie.cn

Go:   func add(a, b int) int
来源：http://iz.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fu.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dp.bjjhwx.cn

[C14] 泛型函数
来源：http://ha.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dm.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://kt.yuexingan06.cn

JS:   // 无泛型
来源：http://jb.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tp.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ns.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hx.shxzskj.cn

Ruby: # 无泛型
来源：http://pm.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pg.9csxet.cn

[C15] 解构 / 展开参数
来源：http://hh.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bw.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://eh.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yp.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vh.haigaiapp.cn

Java: // 无解构
来源：http://dp.wgjwhj.cn

Go:   // 无解构
来源：http://lj.lnxyls.cn

Ruby: a, b = pair
来源：http://zl.asd995.cn

C#:   var (a, b) = pair;
来源：http://iy.colortex.cn

[C16] 函数 / 方法重载
来源：http://xd.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vs.bjjhwx.cn

PHP:  // 无重载
来源：http://xd.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pz.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://bb.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jf.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://yc.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://do.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jq.muxihuayi.cn

================================================================================
来源：http://pb.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://gg.521024.cn

================================================================================
来源：http://nx.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://we.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ps.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cj.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zn.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nb.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nr.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://pd.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://nr.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dh.521024.cn

[D02] 追加元素到末尾
来源：http://mo.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ne.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://af.yuexingan06.cn

JS:   arr.push(4);
来源：http://ww.hahajie.cn

TS:   arr.push(4);
来源：http://hd.shtwfgs.cn

Java: list.add(4);
来源：http://jl.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://tz.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://vn.nszjky.cn

C#:   list.Add(4);
来源：http://zf.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://ux.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://eu.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zr.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rj.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://ap.szsharing.cn

Java: list.add(0, 0);
来源：http://mr.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hk.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ju.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://pk.newstarts.cn

[D04] 删除元素
来源：http://tt.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mk.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bi.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bu.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://pa.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oq.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vx.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yt.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cu.yuexingan06.cn

[D05] 访问与修改元素
来源：http://sp.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sl.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wt.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dv.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ca.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://ib.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://po.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qw.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jg.hnjuh.cn

[D06] 数组长度
来源：http://ou.panjiajie.cn

Py:   len(arr)
来源：http://ku.huanxung.cn

PHP:  count($arr);
来源：http://dy.huixinmuqiang.cn

JS:   arr.length
来源：http://mn.huanxung.cn

TS:   arr.length
来源：http://on.haigaiapp.cn

Java: list.size();
来源：http://eb.bookmarksfly.cn

Go:   len(arr)
来源：http://bv.9csxet.cn

Ruby: arr.length; arr.size
来源：http://hr.wgjwhj.cn

C#:   list.Count;
来源：http://gr.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://ua.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://on.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tv.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://sw.521024.cn

TS:   arr.slice(1, 4);
来源：http://aa.521024.cn

Java: list.subList(1, 4);
来源：http://yo.szxytkj.cn

Go:   arr[1:4]
来源：http://sx.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://fs.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://sk.shtwfgs.cn

[D08] 合并两个数组
来源：http://dm.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://fl.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://cs.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ey.chemitech.net.cn

TS:   [...a, ...b];
来源：http://sv.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qk.chemitech.net.cn

Go:   append(a, b...)
来源：http://fx.nszjky.cn


<!-- 参考信息 -->