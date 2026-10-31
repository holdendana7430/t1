代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nl.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://be.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ak.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cx.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bf.newstarts.cn

[B10] 遍历同时拿索引
来源：http://yk.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fa.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qx.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qj.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xo.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oe.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://le.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zj.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qk.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://pa.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://mi.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://zi.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eh.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ee.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qk.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vv.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://gi.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gn.asd995.cn

[B12] 跳出多层循环
来源：http://sg.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yz.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://on.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mx.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uf.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hm.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jd.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kn.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ze.haigaiapp.cn

[B13] 判断是否为数字
来源：http://hp.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://oy.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://un.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zo.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pp.wgjwhj.cn

Java: x instanceof Number
来源：http://nu.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jk.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://jz.shxzskj.cn

C#:   x is int or double or decimal
来源：http://xh.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://as.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sy.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bb.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://af.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://cp.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://es.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pe.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kd.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zw.lnxyls.cn

[B15] 布尔运算与取反
来源：http://fs.yuntaijiaju.cn

Py:   a and b or not c
来源：http://zv.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://ih.hnjuh.cn

JS:   a && b || !c
来源：http://ri.hahajie.cn

TS:   a && b || !c
来源：http://mn.yuntaijiaju.cn

Java: a && b || !c
来源：http://cg.hahajie.cn

Go:   a && b || !c
来源：http://ak.bookmarksfly.cn

Ruby: a && b || !c
来源：http://ya.521024.cn

C#:   a && b || !c
来源：http://cm.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ak.bookmarksfly.cn

Py:   if not data: return
来源：http://fe.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://vz.gzmigu.cn

JS:   if (!data) return;
来源：http://fm.haigaiapp.cn

TS:   if (!data) return;
来源：http://ei.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://vf.muxihuayi.cn

Go:   if data == nil { return }
来源：http://ih.huixiangedu.cn

Ruby: return if data.nil?
来源：http://yp.bjjhwx.cn

C#:   if (data == null) return;
来源：http://pv.shxzskj.cn

================================================================================
来源：http://us.panjiajie.cn

C. 函数与作用域
来源：http://zz.yuexingan06.cn

================================================================================
来源：http://vy.newstarts.cn

[C01] 定义函数
来源：http://yp.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://ir.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lx.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://oh.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jz.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ir.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vi.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://hi.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fz.9csxet.cn

[C02] 默认参数
来源：http://vb.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://eg.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zv.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://fk.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ak.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jy.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vv.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ce.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://to.huixinmuqiang.cn

[C03] 可变参数
来源：http://ra.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://oy.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hq.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xs.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pu.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xp.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iq.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bl.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mc.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://ep.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ah.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hc.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ql.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gq.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://zu.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://xt.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://bo.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://yl.yuexingan06.cn

[C05] 返回多个值
来源：http://vy.huixiangedu.cn

Py:   return a, b
来源：http://ww.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://dq.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jh.hnjuh.cn

TS:   return { a, b };
来源：http://fg.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sm.nicolike.cn

Go:   return a, b
来源：http://tj.hnjuh.cn

Ruby: return a, b
来源：http://eb.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://kq.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://uu.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://vn.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://so.szsharing.cn

JS:   const square = x => x * x;
来源：http://fh.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://nj.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vt.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sq.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://fu.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://og.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://hq.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pu.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ko.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zf.panjiajie.cn

TS:   arr.map(String)
来源：http://hh.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nj.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://df.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://zh.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ze.wgjwhj.cn

[C08] 闭包
来源：http://eb.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xv.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oe.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ib.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fh.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jb.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oo.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xr.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tu.chemitech.net.cn

[C09] 递归
来源：http://lu.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uu.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cb.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hl.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ew.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mm.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xf.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tz.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ka.asd995.cn

[C10] 变量作用域
来源：http://eh.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ry.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vy.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bj.chemitech.net.cn

TS:   同 JS
来源：http://ri.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://fk.huixiangedu.cn

Go:   花括号块级作用域
来源：http://xu.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://an.hnjuh.cn

C#:   块级作用域
来源：http://bo.colortex.cn

[C11] 模块导入与导出
来源：http://hd.newstarts.cn

Py:   from module import func
来源：http://fz.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nd.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lh.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://at.chemitech.net.cn

Java: import java.util.List;
来源：http://ba.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zc.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://ti.yuexingan06.cn

C#:   using System.Text;
来源：http://fe.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://wr.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://rq.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://dk.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://rr.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://bh.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://it.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://si.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://ag.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mo.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://ap.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yv.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sr.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hd.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dj.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zn.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://kb.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jl.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wl.shtwfgs.cn

[C14] 泛型函数
来源：http://gb.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yc.asd995.cn

PHP:  // 无泛型
来源：http://ej.hnjuh.cn

JS:   // 无泛型
来源：http://sc.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nj.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xc.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tr.huixiangedu.cn

Ruby: # 无泛型
来源：http://lr.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ip.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://mb.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://el.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://cv.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://av.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ic.lnxyls.cn

Java: // 无解构
来源：http://zl.jianghongdianzi.cn

Go:   // 无解构
来源：http://an.wgjwhj.cn

Ruby: a, b = pair
来源：http://id.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://wf.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://lb.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ug.hahajie.cn

PHP:  // 无重载
来源：http://tg.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lp.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://au.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://af.521024.cn

Go:   // 无重载：用不同函数名
来源：http://cg.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://sw.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ni.wgjwhj.cn

================================================================================
来源：http://nc.521024.cn

D. 数组 / 列表 / 集合
来源：http://md.9csxet.cn

================================================================================
来源：http://xe.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://eb.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dw.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cm.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fi.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jm.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ou.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://ga.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://mg.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zs.hahajie.cn

[D02] 追加元素到末尾
来源：http://ro.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yj.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://od.szsharing.cn

JS:   arr.push(4);
来源：http://pj.shxzukj.cn

TS:   arr.push(4);
来源：http://nk.nszjky.cn

Java: list.add(4);
来源：http://yw.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://lt.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ok.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://ej.nicolike.cn

[D03] 在指定位置插入元素
来源：http://nc.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://xq.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ky.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ri.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://jq.gzmigu.cn

Java: list.add(0, 0);
来源：http://ht.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uq.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bc.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://zi.newstarts.cn

[D04] 删除元素
来源：http://zc.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://or.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zg.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pg.colortex.cn

TS:   arr.splice(0, 1);
来源：http://he.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cb.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ix.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gx.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ip.yuexingan06.cn

[D05] 访问与修改元素
来源：http://zx.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ek.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zu.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gp.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://yh.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://cd.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://qn.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ss.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://np.huixinmuqiang.cn

[D06] 数组长度
来源：http://kf.bookmarksfly.cn

Py:   len(arr)
来源：http://wm.lnxyls.cn

PHP:  count($arr);
来源：http://py.nszjky.cn

JS:   arr.length
来源：http://pv.gzmigu.cn

TS:   arr.length
来源：http://hw.521024.cn

Java: list.size();
来源：http://io.shtwfgs.cn

Go:   len(arr)
来源：http://dx.newstarts.cn

Ruby: arr.length; arr.size
来源：http://be.nszjky.cn

C#:   list.Count;
来源：http://of.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://ao.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://id.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://so.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://rg.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://ug.asd995.cn

Java: list.subList(1, 4);
来源：http://ho.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://hp.9csxet.cn

Ruby: arr[1, 3]
来源：http://cg.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://sj.huanxung.cn

[D08] 合并两个数组
来源：http://sq.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://ak.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://tx.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ns.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://cc.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://il.lnxyls.cn

Go:   append(a, b...)
来源：http://st.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://sf.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://nx.jctech888.com.cn

[D09] 排序（升序）
来源：http://dg.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://xj.nicolike.cn

PHP:  sort($arr);
来源：http://fj.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ws.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://un.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://my.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://af.huanxung.cn

Ruby: arr.sort
来源：http://id.shxzukj.cn

C#:   list.Sort();
来源：http://tb.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yq.haigaiapp.cn


<!-- 参考信息 -->