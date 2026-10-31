代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kr.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://js.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hl.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ho.nszjky.cn

[B10] 遍历同时拿索引
来源：http://rl.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pz.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gr.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://om.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zz.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tp.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pl.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ep.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cu.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://fw.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ou.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://si.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://go.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hs.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rh.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://si.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://dl.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bf.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://ig.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xc.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zb.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qh.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ff.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iv.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ya.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://id.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rb.shxzukj.cn

[B13] 判断是否为数字
来源：http://bn.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://aj.lnxyls.cn

PHP:  is_numeric($x)
来源：http://jp.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oy.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ps.wgjwhj.cn

Java: x instanceof Number
来源：http://dm.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rf.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://ov.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://gp.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://dt.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fx.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tr.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://bw.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://ik.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ma.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xq.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ih.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pc.asd995.cn

[B15] 布尔运算与取反
来源：http://go.bjjhwx.cn

Py:   a and b or not c
来源：http://jm.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://rr.chemitech.net.cn

JS:   a && b || !c
来源：http://sc.asd995.cn

TS:   a && b || !c
来源：http://aq.jctech888.com.cn

Java: a && b || !c
来源：http://ya.9csxet.cn

Go:   a && b || !c
来源：http://ji.jctech888.com.cn

Ruby: a && b || !c
来源：http://kk.szsharing.cn

C#:   a && b || !c
来源：http://rn.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vs.shxzukj.cn

Py:   if not data: return
来源：http://rq.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://pn.muxihuayi.cn

JS:   if (!data) return;
来源：http://oj.hnjuh.cn

TS:   if (!data) return;
来源：http://sy.shxzskj.cn

Java: if (data == null) return;
来源：http://pc.huixiangedu.cn

Go:   if data == nil { return }
来源：http://wf.9csxet.cn

Ruby: return if data.nil?
来源：http://un.nicolike.cn

C#:   if (data == null) return;
来源：http://hy.muxihuayi.cn

================================================================================
来源：http://lx.hahajie.cn

C. 函数与作用域
来源：http://nm.wgjwhj.cn

================================================================================
来源：http://vt.521024.cn

[C01] 定义函数
来源：http://qn.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://sk.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nt.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://vr.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wj.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nx.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nf.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://gi.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mc.szsharing.cn

[C02] 默认参数
来源：http://mu.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://tu.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xa.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://nl.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lh.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ds.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oz.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://yh.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://cr.jianghongdianzi.cn

[C03] 可变参数
来源：http://rn.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://gz.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pv.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ji.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ee.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wl.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yy.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://je.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ci.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://lb.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hr.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yx.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gj.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ao.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://kv.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://by.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://ni.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://kb.huixiangedu.cn

[C05] 返回多个值
来源：http://xb.colortex.cn

Py:   return a, b
来源：http://qb.521024.cn

PHP:  return [$a, $b];
来源：http://cd.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://db.wgjwhj.cn

TS:   return { a, b };
来源：http://nf.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ke.nszjky.cn

Go:   return a, b
来源：http://ew.wgjwhj.cn

Ruby: return a, b
来源：http://mq.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://il.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://wi.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://ej.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kh.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://oz.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://gf.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yb.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kn.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://am.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ds.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://vz.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://re.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gl.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://op.nicolike.cn

TS:   arr.map(String)
来源：http://jc.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cg.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ve.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://ul.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sm.jianghongdianzi.cn

[C08] 闭包
来源：http://yr.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fc.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fl.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yk.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lq.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cq.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tc.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qt.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yz.colortex.cn

[C09] 递归
来源：http://lv.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bm.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vx.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kr.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qw.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://og.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mg.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jf.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dl.shxzukj.cn

[C10] 变量作用域
来源：http://ju.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ra.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ca.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rl.wgjwhj.cn

TS:   同 JS
来源：http://jn.newstarts.cn

Java: 方法内为块级作用域
来源：http://ty.hnjuh.cn

Go:   花括号块级作用域
来源：http://lu.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ln.panjiajie.cn

C#:   块级作用域
来源：http://dh.szsharing.cn

[C11] 模块导入与导出
来源：http://ek.nszjky.cn

Py:   from module import func
来源：http://pb.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rz.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ck.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zm.bookmarksfly.cn

Java: import java.util.List;
来源：http://xr.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kx.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://ix.asd995.cn

C#:   using System.Text;
来源：http://rt.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://ob.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://dh.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://bj.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://tf.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ns.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xc.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://ae.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://bu.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://js.521024.cn

[C13] 类型声明 / 类型注解
来源：http://or.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vu.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uo.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jh.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kb.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gb.shxzukj.cn

Go:   func add(a, b int) int
来源：http://cz.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nf.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ja.bookmarksfly.cn

[C14] 泛型函数
来源：http://io.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wt.hnjuh.cn

PHP:  // 无泛型
来源：http://fw.9csxet.cn

JS:   // 无泛型
来源：http://xf.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://or.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kn.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tb.jctech888.com.cn

Ruby: # 无泛型
来源：http://kd.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tl.colortex.cn

[C15] 解构 / 展开参数
来源：http://qu.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tr.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://cc.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eu.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gw.asd995.cn

Java: // 无解构
来源：http://fh.bookmarksfly.cn

Go:   // 无解构
来源：http://uf.9csxet.cn

Ruby: a, b = pair
来源：http://de.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://af.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://wj.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ls.hahajie.cn

PHP:  // 无重载
来源：http://ys.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cf.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://cl.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pr.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://cn.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://dp.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rm.521024.cn

================================================================================
来源：http://wk.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://lx.huixinmuqiang.cn

================================================================================
来源：http://ra.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://vo.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://km.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ug.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lp.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lz.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pi.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://wb.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://ue.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mb.newstarts.cn

[D02] 追加元素到末尾
来源：http://fw.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gp.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hv.newstarts.cn

JS:   arr.push(4);
来源：http://mt.bookmarksfly.cn

TS:   arr.push(4);
来源：http://zz.szxytkj.cn

Java: list.add(4);
来源：http://hj.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://ti.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://lr.szxytkj.cn

C#:   list.Add(4);
来源：http://zj.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://xb.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://nh.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lr.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qc.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://zz.asd995.cn

Java: list.add(0, 0);
来源：http://zx.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vh.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ov.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://rg.9csxet.cn

[D04] 删除元素
来源：http://gj.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sj.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ww.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://if.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://np.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ke.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vw.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uc.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ox.gzmigu.cn

[D05] 访问与修改元素
来源：http://oj.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uh.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ox.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cn.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://um.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://qi.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://gs.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dg.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bi.bookmarksfly.cn

[D06] 数组长度
来源：http://cn.asd995.cn

Py:   len(arr)
来源：http://gx.szxytkj.cn

PHP:  count($arr);
来源：http://gl.asd995.cn

JS:   arr.length
来源：http://ja.panjiajie.cn

TS:   arr.length
来源：http://sd.colortex.cn

Java: list.size();
来源：http://cy.bjjhwx.cn

Go:   len(arr)
来源：http://is.9csxet.cn

Ruby: arr.length; arr.size
来源：http://ir.chemitech.net.cn

C#:   list.Count;
来源：http://jt.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://nt.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cm.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://il.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://sr.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://ig.hnjuh.cn

Java: list.subList(1, 4);
来源：http://rg.shxzukj.cn

Go:   arr[1:4]
来源：http://yb.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://mt.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://me.521024.cn

[D08] 合并两个数组
来源：http://ax.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://xm.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://lx.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nf.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://me.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wb.521024.cn

Go:   append(a, b...)
来源：http://az.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://oz.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://hn.lnxyls.cn

[D09] 排序（升序）
来源：http://ll.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://kf.shxzskj.cn

PHP:  sort($arr);
来源：http://et.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rf.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qe.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://or.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yu.bookmarksfly.cn

Ruby: arr.sort
来源：http://kh.hnjuh.cn

C#:   list.Sort();
来源：http://xj.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://od.jianghongdianzi.cn


<!-- 参考信息 -->