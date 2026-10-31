代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jp.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://ew.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jx.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hd.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zz.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tt.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rr.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://du.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://di.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qe.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://wy.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://qy.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://yb.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://js.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vj.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qx.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mx.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://ml.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ud.yuexingan06.cn

[B12] 跳出多层循环
来源：http://yq.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ws.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wu.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bg.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kw.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cc.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kb.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hq.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vc.shxzukj.cn

[B13] 判断是否为数字
来源：http://ey.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://sm.nszjky.cn

PHP:  is_numeric($x)
来源：http://hx.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zh.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lg.nicolike.cn

Java: x instanceof Number
来源：http://xg.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ng.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://cm.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://lv.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://gk.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zh.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tx.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://kn.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://yu.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sh.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ds.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fk.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qs.shxzskj.cn

[B15] 布尔运算与取反
来源：http://dk.szsharing.cn

Py:   a and b or not c
来源：http://fk.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://vl.jctech888.com.cn

JS:   a && b || !c
来源：http://gb.gzmigu.cn

TS:   a && b || !c
来源：http://xe.nicolike.cn

Java: a && b || !c
来源：http://yh.521024.cn

Go:   a && b || !c
来源：http://zq.gzmigu.cn

Ruby: a && b || !c
来源：http://hm.panjiajie.cn

C#:   a && b || !c
来源：http://xa.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dt.521024.cn

Py:   if not data: return
来源：http://oa.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://lq.nszjky.cn

JS:   if (!data) return;
来源：http://of.bjjhwx.cn

TS:   if (!data) return;
来源：http://gz.shxzskj.cn

Java: if (data == null) return;
来源：http://rq.nicolike.cn

Go:   if data == nil { return }
来源：http://mt.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://ci.haigaiapp.cn

C#:   if (data == null) return;
来源：http://zr.yuexingan06.cn

================================================================================
来源：http://xp.chemitech.net.cn

C. 函数与作用域
来源：http://kq.muxihuayi.cn

================================================================================
来源：http://km.huixiangedu.cn

[C01] 定义函数
来源：http://dw.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://rn.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nt.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://cg.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ml.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vy.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jr.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://yt.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kf.hnjuh.cn

[C02] 默认参数
来源：http://yx.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://ep.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lc.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://ty.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fs.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qt.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rf.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://le.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://ju.shxzukj.cn

[C03] 可变参数
来源：http://be.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://rq.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://au.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ro.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://km.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zh.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nj.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dy.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://os.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://lm.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mv.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qy.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ex.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ke.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://xv.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://rc.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://nq.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://wy.szsharing.cn

[C05] 返回多个值
来源：http://sx.bjjhwx.cn

Py:   return a, b
来源：http://wd.lnxyls.cn

PHP:  return [$a, $b];
来源：http://wt.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vb.jianghongdianzi.cn

TS:   return { a, b };
来源：http://ec.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ji.huixiangedu.cn

Go:   return a, b
来源：http://ji.shxzukj.cn

Ruby: return a, b
来源：http://gy.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://tx.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://um.521024.cn

Py:   square = lambda x: x * x
来源：http://oe.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vg.521024.cn

JS:   const square = x => x * x;
来源：http://hf.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://xd.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zv.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sg.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://xl.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zy.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://vk.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qm.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vl.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sj.bjjhwx.cn

TS:   arr.map(String)
来源：http://vy.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iw.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yd.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://bk.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pq.haigaiapp.cn

[C08] 闭包
来源：http://bh.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rg.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lv.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rv.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nh.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pl.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nv.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ku.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://am.asd995.cn

[C09] 递归
来源：http://xa.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zh.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pr.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vw.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://la.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qp.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mu.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://le.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kf.yuntaijiaju.cn

[C10] 变量作用域
来源：http://ol.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nm.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fc.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gn.asd995.cn

TS:   同 JS
来源：http://wa.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://pl.chemitech.net.cn

Go:   花括号块级作用域
来源：http://gs.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://es.bjjhwx.cn

C#:   块级作用域
来源：http://mk.colortex.cn

[C11] 模块导入与导出
来源：http://dj.jctech888.com.cn

Py:   from module import func
来源：http://oo.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://en.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ux.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pp.yuexingan06.cn

Java: import java.util.List;
来源：http://wm.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dp.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://lk.shxzskj.cn

C#:   using System.Text;
来源：http://nh.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://ex.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://bq.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://ew.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://pu.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ib.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ej.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://md.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://ob.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://am.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://jy.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://od.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pa.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kj.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sn.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wo.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://sa.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jt.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gk.9csxet.cn

[C14] 泛型函数
来源：http://yu.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fn.huixiangedu.cn

PHP:  // 无泛型
来源：http://rn.nicolike.cn

JS:   // 无泛型
来源：http://tl.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tc.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wy.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://en.newstarts.cn

Ruby: # 无泛型
来源：http://no.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sn.newstarts.cn

[C15] 解构 / 展开参数
来源：http://ov.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tc.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://al.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yo.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pq.bookmarksfly.cn

Java: // 无解构
来源：http://wl.shxzskj.cn

Go:   // 无解构
来源：http://it.wgjwhj.cn

Ruby: a, b = pair
来源：http://sb.9csxet.cn

C#:   var (a, b) = pair;
来源：http://zb.9csxet.cn

[C16] 函数 / 方法重载
来源：http://sj.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ar.bookmarksfly.cn

PHP:  // 无重载
来源：http://zi.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eq.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://vw.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cm.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://re.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://fs.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aj.colortex.cn

================================================================================
来源：http://xy.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://fl.lnxyls.cn

================================================================================
来源：http://eu.9csxet.cn

[D01] 创建数组 / 列表
来源：http://kb.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://in.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pe.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ug.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cm.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nv.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://ks.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://se.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wa.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://id.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://id.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zm.muxihuayi.cn

JS:   arr.push(4);
来源：http://er.asd995.cn

TS:   arr.push(4);
来源：http://ch.jctech888.com.cn

Java: list.add(4);
来源：http://xn.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://aw.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://wt.asd995.cn

C#:   list.Add(4);
来源：http://zq.nszjky.cn

[D03] 在指定位置插入元素
来源：http://fb.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://zr.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jt.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dk.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://za.panjiajie.cn

Java: list.add(0, 0);
来源：http://by.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vo.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kv.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://fz.hnjuh.cn

[D04] 删除元素
来源：http://sl.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mx.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nm.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oh.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://qz.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rg.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sp.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cj.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xz.nicolike.cn

[D05] 访问与修改元素
来源：http://so.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sw.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vn.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vv.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://ho.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://ww.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://dr.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://am.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xz.huixinmuqiang.cn

[D06] 数组长度
来源：http://rb.shxzskj.cn

Py:   len(arr)
来源：http://et.shxzukj.cn

PHP:  count($arr);
来源：http://ht.chemitech.net.cn

JS:   arr.length
来源：http://po.shtwfgs.cn

TS:   arr.length
来源：http://bb.huanxung.cn

Java: list.size();
来源：http://vh.shxzukj.cn

Go:   len(arr)
来源：http://bx.9csxet.cn

Ruby: arr.length; arr.size
来源：http://rc.lnxyls.cn

C#:   list.Count;
来源：http://no.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://th.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ly.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jq.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://sh.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://hh.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://dv.asd995.cn

Go:   arr[1:4]
来源：http://ec.colortex.cn

Ruby: arr[1, 3]
来源：http://yf.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://fb.nszjky.cn

[D08] 合并两个数组
来源：http://qs.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://dt.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://wl.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mv.chemitech.net.cn

TS:   [...a, ...b];
来源：http://ff.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kp.bjjhwx.cn

Go:   append(a, b...)
来源：http://iv.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://xe.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://lk.gzmigu.cn

[D09] 排序（升序）
来源：http://ni.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://hz.nszjky.cn

PHP:  sort($arr);
来源：http://uq.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ye.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jy.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cl.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wx.chemitech.net.cn

Ruby: arr.sort
来源：http://jt.huanxung.cn

C#:   list.Sort();
来源：http://hg.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mu.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hs.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vk.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ow.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dm.nicolike.cn


<!-- 参考信息 -->