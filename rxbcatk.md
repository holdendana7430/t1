代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://qy.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pt.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://od.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://ur.521024.cn

[B09] break 与 continue
来源：http://iq.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xz.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ht.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ye.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qs.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oi.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ss.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qs.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ur.nicolike.cn

[B10] 遍历同时拿索引
来源：http://cd.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sn.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ig.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hq.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ns.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ev.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xm.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ev.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ag.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://pa.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://dj.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://tb.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ag.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ri.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eh.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ou.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://oy.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dp.newstarts.cn

[B12] 跳出多层循环
来源：http://st.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lv.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zm.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tj.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dh.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://be.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vm.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cy.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mk.shtwfgs.cn

[B13] 判断是否为数字
来源：http://nc.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://fs.shxzukj.cn

PHP:  is_numeric($x)
来源：http://xg.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yu.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pi.gzmigu.cn

Java: x instanceof Number
来源：http://zh.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ly.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://qd.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://ik.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://dg.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lp.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wj.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://cv.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://rx.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bm.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://se.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wg.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hn.szxytkj.cn

[B15] 布尔运算与取反
来源：http://gg.haigaiapp.cn

Py:   a and b or not c
来源：http://gi.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://kd.9csxet.cn

JS:   a && b || !c
来源：http://nj.nicolike.cn

TS:   a && b || !c
来源：http://tb.yuexingan06.cn

Java: a && b || !c
来源：http://xe.521024.cn

Go:   a && b || !c
来源：http://li.nicolike.cn

Ruby: a && b || !c
来源：http://dr.521024.cn

C#:   a && b || !c
来源：http://nw.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lt.521024.cn

Py:   if not data: return
来源：http://vm.colortex.cn

PHP:  if (!$data) { return; }
来源：http://xy.9csxet.cn

JS:   if (!data) return;
来源：http://vl.bjjhwx.cn

TS:   if (!data) return;
来源：http://ks.szxytkj.cn

Java: if (data == null) return;
来源：http://rj.huanxung.cn

Go:   if data == nil { return }
来源：http://aa.hahajie.cn

Ruby: return if data.nil?
来源：http://rd.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://zh.yuexingan06.cn

================================================================================
来源：http://ki.panjiajie.cn

C. 函数与作用域
来源：http://by.gzmigu.cn

================================================================================
来源：http://cj.9csxet.cn

[C01] 定义函数
来源：http://jl.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://uh.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ao.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://vr.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iy.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sx.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sq.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://hz.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://br.szsharing.cn

[C02] 默认参数
来源：http://sr.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://xj.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sj.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://wd.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ca.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lw.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cb.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://ck.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://wz.nszjky.cn

[C03] 可变参数
来源：http://ku.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://fd.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fj.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://il.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ex.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lz.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://am.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://us.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ny.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://rk.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ru.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mo.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://od.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fw.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://pj.521024.cn

Go:   // 无：用配置结构体参数
来源：http://za.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://br.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://pu.szsharing.cn

[C05] 返回多个值
来源：http://sr.huixinmuqiang.cn

Py:   return a, b
来源：http://tx.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://sz.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hw.shxzukj.cn

TS:   return { a, b };
来源：http://yq.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vz.nszjky.cn

Go:   return a, b
来源：http://tv.yuntaijiaju.cn

Ruby: return a, b
来源：http://yr.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://pg.colortex.cn

[C06] 匿名函数 / lambda
来源：http://ov.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://dk.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xh.szsharing.cn

JS:   const square = x => x * x;
来源：http://as.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://gm.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xy.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xs.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://hf.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qm.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://wg.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ac.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qt.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cq.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://jq.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cc.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://la.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://il.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qt.shxzskj.cn

[C08] 闭包
来源：http://kg.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://db.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://on.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cj.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xp.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hb.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wr.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dl.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zi.lnxyls.cn

[C09] 递归
来源：http://wh.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nv.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://on.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://av.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sv.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://na.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fq.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qz.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://so.lnxyls.cn

[C10] 变量作用域
来源：http://vs.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pp.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hl.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://os.bookmarksfly.cn

TS:   同 JS
来源：http://bn.shxzukj.cn

Java: 方法内为块级作用域
来源：http://vu.szxytkj.cn

Go:   花括号块级作用域
来源：http://ug.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vs.shxzukj.cn

C#:   块级作用域
来源：http://bm.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://io.huixinmuqiang.cn

Py:   from module import func
来源：http://bx.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iu.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://js.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oi.szsharing.cn

Java: import java.util.List;
来源：http://da.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pz.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://hb.chemitech.net.cn

C#:   using System.Text;
来源：http://zy.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://ln.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://vy.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://jd.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://th.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://fe.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oe.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://wi.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ex.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sn.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://xk.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ez.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jh.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vy.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xy.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ya.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://ad.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yb.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qc.hahajie.cn

[C14] 泛型函数
来源：http://rm.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tg.jctech888.com.cn

PHP:  // 无泛型
来源：http://gv.shxzukj.cn

JS:   // 无泛型
来源：http://vc.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xc.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eo.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lo.521024.cn

Ruby: # 无泛型
来源：http://db.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ar.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://cn.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mt.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://gk.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cz.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qy.huixinmuqiang.cn

Java: // 无解构
来源：http://fs.gzmigu.cn

Go:   // 无解构
来源：http://dj.szxytkj.cn

Ruby: a, b = pair
来源：http://mw.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://vv.nicolike.cn

[C16] 函数 / 方法重载
来源：http://uf.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tc.szxytkj.cn

PHP:  // 无重载
来源：http://pi.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uf.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://wt.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://el.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://fp.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://xx.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://an.shxzskj.cn

================================================================================
来源：http://pd.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://qh.shtwfgs.cn

================================================================================
来源：http://cv.colortex.cn

[D01] 创建数组 / 列表
来源：http://vy.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uq.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uj.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gd.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bl.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eh.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://qb.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://fv.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xs.9csxet.cn

[D02] 追加元素到末尾
来源：http://qy.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zr.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tj.nicolike.cn

JS:   arr.push(4);
来源：http://bp.haigaiapp.cn

TS:   arr.push(4);
来源：http://qh.chemitech.net.cn

Java: list.add(4);
来源：http://hr.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://xi.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://ac.szsharing.cn

C#:   list.Add(4);
来源：http://bm.521024.cn

[D03] 在指定位置插入元素
来源：http://br.asd995.cn

Py:   arr.insert(0, 0)
来源：http://jy.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://la.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dm.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://ou.shxzskj.cn

Java: list.add(0, 0);
来源：http://ad.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jr.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qe.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://hm.gzmigu.cn

[D04] 删除元素
来源：http://an.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xj.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ed.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ph.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://mf.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dl.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rh.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cn.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wx.9csxet.cn

[D05] 访问与修改元素
来源：http://hi.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://on.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vy.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vp.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://ku.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://mo.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ci.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://od.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fv.szsharing.cn

[D06] 数组长度
来源：http://cg.wgjwhj.cn

Py:   len(arr)
来源：http://nk.shxzskj.cn

PHP:  count($arr);
来源：http://nf.521024.cn

JS:   arr.length
来源：http://qw.521024.cn

TS:   arr.length
来源：http://go.bookmarksfly.cn

Java: list.size();
来源：http://ka.muxihuayi.cn

Go:   len(arr)
来源：http://ms.newstarts.cn

Ruby: arr.length; arr.size
来源：http://ti.huixinmuqiang.cn

C#:   list.Count;
来源：http://sq.9csxet.cn

[D07] 切片 / 取子数组
来源：http://tm.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://li.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sx.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://ts.colortex.cn

TS:   arr.slice(1, 4);
来源：http://ar.nicolike.cn

Java: list.subList(1, 4);
来源：http://zr.9csxet.cn

Go:   arr[1:4]
来源：http://dk.9csxet.cn

Ruby: arr[1, 3]
来源：http://yn.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://ac.muxihuayi.cn

[D08] 合并两个数组
来源：http://qr.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://qa.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://rf.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tu.newstarts.cn

TS:   [...a, ...b];
来源：http://ob.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jg.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://fb.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://wc.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://cd.szxytkj.cn

[D09] 排序（升序）
来源：http://sn.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://oo.wgjwhj.cn


<!-- 参考信息 -->