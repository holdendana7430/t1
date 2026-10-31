代发 wailian999

[B09] break 与 continue
来源：http://bl.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ci.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hk.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iq.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ln.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gw.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yl.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ro.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rc.szsharing.cn

[B10] 遍历同时拿索引
来源：http://ha.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wd.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uu.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ue.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pn.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oi.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gb.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yc.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qb.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://vn.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://cv.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://jm.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tx.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iq.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fc.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fz.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://bs.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vr.gzmigu.cn

[B12] 跳出多层循环
来源：http://pu.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nl.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rd.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ri.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kr.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://um.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hy.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ua.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jh.shxzskj.cn

[B13] 判断是否为数字
来源：http://ot.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://ta.panjiajie.cn

PHP:  is_numeric($x)
来源：http://np.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ye.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yf.szsharing.cn

Java: x instanceof Number
来源：http://iw.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pi.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://zq.szsharing.cn

C#:   x is int or double or decimal
来源：http://pk.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://xf.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rz.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qv.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://cb.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://yc.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vp.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://te.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rr.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mu.asd995.cn

[B15] 布尔运算与取反
来源：http://rx.lnxyls.cn

Py:   a and b or not c
来源：http://xq.nicolike.cn

PHP:  $a && $b || !$c
来源：http://hd.colortex.cn

JS:   a && b || !c
来源：http://wo.bjjhwx.cn

TS:   a && b || !c
来源：http://xc.newstarts.cn

Java: a && b || !c
来源：http://qh.huanxung.cn

Go:   a && b || !c
来源：http://iz.panjiajie.cn

Ruby: a && b || !c
来源：http://xx.muxihuayi.cn

C#:   a && b || !c
来源：http://fy.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xh.huixiangedu.cn

Py:   if not data: return
来源：http://vf.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://gl.newstarts.cn

JS:   if (!data) return;
来源：http://db.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://se.nicolike.cn

Java: if (data == null) return;
来源：http://jv.hahajie.cn

Go:   if data == nil { return }
来源：http://bo.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://qn.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://us.huixiangedu.cn

================================================================================
来源：http://gr.lnxyls.cn

C. 函数与作用域
来源：http://le.szsharing.cn

================================================================================
来源：http://fr.jianghongdianzi.cn

[C01] 定义函数
来源：http://wq.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://ds.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oq.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://gj.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ij.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sp.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://on.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://iz.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ot.szsharing.cn

[C02] 默认参数
来源：http://sr.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://jz.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ml.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://zi.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yi.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gf.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yj.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://sp.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://ep.bookmarksfly.cn

[C03] 可变参数
来源：http://rr.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://hl.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oz.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ym.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dz.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ai.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rx.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ah.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://id.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://mh.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cv.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yi.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cw.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ft.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://os.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://to.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://du.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://nw.shxzskj.cn

[C05] 返回多个值
来源：http://vw.huixiangedu.cn

Py:   return a, b
来源：http://ay.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://yn.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rt.hahajie.cn

TS:   return { a, b };
来源：http://nv.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ps.szxytkj.cn

Go:   return a, b
来源：http://ao.huanxung.cn

Ruby: return a, b
来源：http://vz.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://jq.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://mw.nszjky.cn

Py:   square = lambda x: x * x
来源：http://ry.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uh.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://vo.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://iw.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ip.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://de.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://do.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nc.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://ku.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ng.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rf.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ku.muxihuayi.cn

TS:   arr.map(String)
来源：http://gf.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oc.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xf.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://wr.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://td.nicolike.cn

[C08] 闭包
来源：http://sn.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://an.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kh.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tv.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eu.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pi.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hs.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kb.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tc.shxzskj.cn

[C09] 递归
来源：http://ll.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qq.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ff.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dd.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wk.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pk.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pd.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qd.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lw.hahajie.cn

[C10] 变量作用域
来源：http://cf.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zn.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nk.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fd.hnjuh.cn

TS:   同 JS
来源：http://pt.nszjky.cn

Java: 方法内为块级作用域
来源：http://xz.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://au.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://to.jianghongdianzi.cn

C#:   块级作用域
来源：http://mi.bjjhwx.cn

[C11] 模块导入与导出
来源：http://vr.yuexingan06.cn

Py:   from module import func
来源：http://lo.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cq.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fe.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ou.asd995.cn

Java: import java.util.List;
来源：http://wv.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wa.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://an.shxzukj.cn

C#:   using System.Text;
来源：http://bn.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://jt.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://yj.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://uz.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ia.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://nj.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wa.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://ve.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://pp.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fr.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://no.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eq.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ig.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ct.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jy.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ut.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://gy.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fb.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mk.lnxyls.cn

[C14] 泛型函数
来源：http://xb.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hs.szsharing.cn

PHP:  // 无泛型
来源：http://dg.nszjky.cn

JS:   // 无泛型
来源：http://ao.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lb.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rq.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dk.nszjky.cn

Ruby: # 无泛型
来源：http://ry.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gl.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://ws.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dx.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://ti.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ru.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cs.shtwfgs.cn

Java: // 无解构
来源：http://hi.shxzskj.cn

Go:   // 无解构
来源：http://qu.haigaiapp.cn

Ruby: a, b = pair
来源：http://ll.nszjky.cn

C#:   var (a, b) = pair;
来源：http://ar.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://ug.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://di.szxytkj.cn

PHP:  // 无重载
来源：http://xt.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mk.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://ai.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gr.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://jo.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://pn.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jq.9csxet.cn

================================================================================
来源：http://xz.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://lu.asd995.cn

================================================================================
来源：http://hf.szsharing.cn

[D01] 创建数组 / 列表
来源：http://pm.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bq.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sk.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fq.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://me.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ij.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://qg.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://at.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hm.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://lg.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qj.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yv.gzmigu.cn

JS:   arr.push(4);
来源：http://dk.hahajie.cn

TS:   arr.push(4);
来源：http://ry.521024.cn

Java: list.add(4);
来源：http://mw.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://vu.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://fw.newstarts.cn

C#:   list.Add(4);
来源：http://nh.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://im.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://gv.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ug.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hu.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://sm.nicolike.cn

Java: list.add(0, 0);
来源：http://he.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pg.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ru.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://zi.jctech888.com.cn

[D04] 删除元素
来源：http://fu.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qi.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zn.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qn.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://dc.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bi.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lc.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fn.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iu.szxytkj.cn

[D05] 访问与修改元素
来源：http://pn.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rj.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://py.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cb.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://im.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://xq.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://sr.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cr.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://et.colortex.cn

[D06] 数组长度
来源：http://wx.shtwfgs.cn

Py:   len(arr)
来源：http://qj.muxihuayi.cn

PHP:  count($arr);
来源：http://lj.nicolike.cn

JS:   arr.length
来源：http://le.chemitech.net.cn

TS:   arr.length
来源：http://qz.hnjuh.cn

Java: list.size();
来源：http://vg.wgjwhj.cn

Go:   len(arr)
来源：http://eb.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://mz.szsharing.cn

C#:   list.Count;
来源：http://my.colortex.cn

[D07] 切片 / 取子数组
来源：http://vl.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ni.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bb.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://wb.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://at.nszjky.cn

Java: list.subList(1, 4);
来源：http://yt.chemitech.net.cn

Go:   arr[1:4]
来源：http://ck.nszjky.cn

Ruby: arr[1, 3]
来源：http://qn.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://ig.shtwfgs.cn

[D08] 合并两个数组
来源：http://ca.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://dt.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://yo.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://er.hnjuh.cn

TS:   [...a, ...b];
来源：http://ph.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ia.521024.cn

Go:   append(a, b...)
来源：http://yg.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://jh.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://cp.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://rx.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://pm.9csxet.cn

PHP:  sort($arr);
来源：http://in.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://no.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qq.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ld.jianghongdianzi.cn


<!-- 参考信息 -->