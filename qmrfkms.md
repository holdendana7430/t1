代发 wailian999

[B09] break 与 continue
来源：http://wj.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://la.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rk.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vl.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://db.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qu.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sp.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oq.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://so.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://jp.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ko.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nt.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zc.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xy.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yi.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wa.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wz.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xq.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://oj.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://gw.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://hl.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kn.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bt.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wd.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zt.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://so.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ub.colortex.cn

[B12] 跳出多层循环
来源：http://jw.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ye.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://er.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rn.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ct.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iv.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tj.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ur.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kr.hahajie.cn

[B13] 判断是否为数字
来源：http://wq.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://bq.521024.cn

PHP:  is_numeric($x)
来源：http://st.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ho.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ko.szxytkj.cn

Java: x instanceof Number
来源：http://lx.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://as.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://wt.nicolike.cn

C#:   x is int or double or decimal
来源：http://ua.521024.cn

[B14] 判断值是否在集合内
来源：http://tx.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ry.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xv.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://jc.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://lq.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qk.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oz.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lw.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sy.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://ix.yuntaijiaju.cn

Py:   a and b or not c
来源：http://lu.asd995.cn

PHP:  $a && $b || !$c
来源：http://iy.521024.cn

JS:   a && b || !c
来源：http://vo.nicolike.cn

TS:   a && b || !c
来源：http://pz.huanxung.cn

Java: a && b || !c
来源：http://lw.yuexingan06.cn

Go:   a && b || !c
来源：http://lj.bjjhwx.cn

Ruby: a && b || !c
来源：http://lt.9csxet.cn

C#:   a && b || !c
来源：http://ri.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yd.newstarts.cn

Py:   if not data: return
来源：http://ex.asd995.cn

PHP:  if (!$data) { return; }
来源：http://sd.haigaiapp.cn

JS:   if (!data) return;
来源：http://gv.jctech888.com.cn

TS:   if (!data) return;
来源：http://hp.lnxyls.cn

Java: if (data == null) return;
来源：http://qz.wgjwhj.cn

Go:   if data == nil { return }
来源：http://bj.haigaiapp.cn

Ruby: return if data.nil?
来源：http://yk.chemitech.net.cn

C#:   if (data == null) return;
来源：http://yb.bookmarksfly.cn

================================================================================
来源：http://kf.bjjhwx.cn

C. 函数与作用域
来源：http://qz.bookmarksfly.cn

================================================================================
来源：http://mh.huanxung.cn

[C01] 定义函数
来源：http://cs.521024.cn

Py:   def add(a, b): return a + b
来源：http://nh.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ec.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ki.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ut.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ml.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rf.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://om.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yw.bookmarksfly.cn

[C02] 默认参数
来源：http://qh.521024.cn

Py:   def greet(name="World"): return name
来源：http://ma.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qq.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://fk.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://op.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kx.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ge.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://dh.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://db.asd995.cn

[C03] 可变参数
来源：http://su.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://eo.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://py.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yw.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uq.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rn.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pg.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cy.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gn.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://yq.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dr.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rh.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rx.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yp.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://fq.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://fr.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://qo.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://dj.shxzukj.cn

[C05] 返回多个值
来源：http://yi.newstarts.cn

Py:   return a, b
来源：http://su.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://iu.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fh.huanxung.cn

TS:   return { a, b };
来源：http://fb.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xa.asd995.cn

Go:   return a, b
来源：http://vc.panjiajie.cn

Ruby: return a, b
来源：http://zf.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://un.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://yp.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://ge.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nt.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://je.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://yu.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kw.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wx.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://mp.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ww.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://iy.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iy.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pe.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cp.huixiangedu.cn

TS:   arr.map(String)
来源：http://af.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dj.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lz.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://zq.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cz.yuexingan06.cn

[C08] 闭包
来源：http://uu.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iz.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vr.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ch.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uj.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jl.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ox.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ox.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ot.wgjwhj.cn

[C09] 递归
来源：http://vk.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zr.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yr.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nl.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hw.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qs.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eg.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hb.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ob.panjiajie.cn

[C10] 变量作用域
来源：http://ni.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ro.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jj.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ml.chemitech.net.cn

TS:   同 JS
来源：http://hf.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://zu.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://nv.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dj.huixiangedu.cn

C#:   块级作用域
来源：http://gw.szsharing.cn

[C11] 模块导入与导出
来源：http://gm.colortex.cn

Py:   from module import func
来源：http://ex.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kx.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sm.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gh.szsharing.cn

Java: import java.util.List;
来源：http://fv.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://so.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://ye.muxihuayi.cn

C#:   using System.Text;
来源：http://ut.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://gy.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://ao.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://xe.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://pq.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://cu.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sp.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://vq.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://en.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ac.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://hn.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xb.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vu.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cq.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sh.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zh.nicolike.cn

Go:   func add(a, b int) int
来源：http://vn.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ms.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sf.muxihuayi.cn

[C14] 泛型函数
来源：http://ju.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wj.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://ip.521024.cn

JS:   // 无泛型
来源：http://ct.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://if.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bg.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zy.gzmigu.cn

Ruby: # 无泛型
来源：http://zy.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bj.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://db.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tm.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://wz.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bo.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ro.huixinmuqiang.cn

Java: // 无解构
来源：http://au.szxytkj.cn

Go:   // 无解构
来源：http://yg.hnjuh.cn

Ruby: a, b = pair
来源：http://gc.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://vq.asd995.cn

[C16] 函数 / 方法重载
来源：http://ef.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kd.hahajie.cn

PHP:  // 无重载
来源：http://cg.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nr.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ky.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mo.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://vl.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://vc.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gk.muxihuayi.cn

================================================================================
来源：http://ky.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://om.shxzskj.cn

================================================================================
来源：http://cc.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://rz.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://it.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rg.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rx.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uz.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ru.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://hk.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://mt.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ja.shxzukj.cn

[D02] 追加元素到末尾
来源：http://za.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sr.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lg.lnxyls.cn

JS:   arr.push(4);
来源：http://jx.gzmigu.cn

TS:   arr.push(4);
来源：http://pc.jianghongdianzi.cn

Java: list.add(4);
来源：http://ln.colortex.cn

Go:   arr = append(arr, 4)
来源：http://ap.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://uo.newstarts.cn

C#:   list.Add(4);
来源：http://my.asd995.cn

[D03] 在指定位置插入元素
来源：http://wa.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://pj.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jv.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ky.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://il.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://og.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vq.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ae.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://mg.hahajie.cn

[D04] 删除元素
来源：http://fh.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ku.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://be.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jn.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://sg.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pu.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lc.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jt.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nr.shtwfgs.cn

[D05] 访问与修改元素
来源：http://vy.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://td.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nm.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ob.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://cb.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://cf.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://dw.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lr.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ki.newstarts.cn

[D06] 数组长度
来源：http://cc.asd995.cn

Py:   len(arr)
来源：http://lc.bjjhwx.cn

PHP:  count($arr);
来源：http://ky.shxzukj.cn

JS:   arr.length
来源：http://vh.hnjuh.cn

TS:   arr.length
来源：http://ho.panjiajie.cn

Java: list.size();
来源：http://ci.bookmarksfly.cn

Go:   len(arr)
来源：http://fj.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://zx.hahajie.cn

C#:   list.Count;
来源：http://ax.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://zx.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ni.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xi.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://ac.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://ty.szsharing.cn

Java: list.subList(1, 4);
来源：http://ga.nicolike.cn

Go:   arr[1:4]
来源：http://it.9csxet.cn

Ruby: arr[1, 3]
来源：http://bc.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://vx.shxzukj.cn

[D08] 合并两个数组
来源：http://ni.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://tf.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://kx.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lo.yuexingan06.cn

TS:   [...a, ...b];
来源：http://ul.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://af.szsharing.cn

Go:   append(a, b...)
来源：http://dl.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://nu.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://hl.huixiangedu.cn

[D09] 排序（升序）
来源：http://zs.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://uh.nszjky.cn

PHP:  sort($arr);
来源：http://om.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ge.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oz.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ro.bjjhwx.cn


<!-- 参考信息 -->