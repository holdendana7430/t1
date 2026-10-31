代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pi.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vm.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yw.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pe.asd995.cn

[B10] 遍历同时拿索引
来源：http://he.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ks.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://no.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jc.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jo.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pl.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uk.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ma.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pg.521024.cn

[B11] 生成数字序列 / 区间
来源：http://xm.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://hl.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://ed.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://td.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ow.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uw.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://me.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://de.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ox.huanxung.cn

[B12] 跳出多层循环
来源：http://bc.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://py.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wg.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vt.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qk.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ei.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wq.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hb.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ys.shxzskj.cn

[B13] 判断是否为数字
来源：http://bj.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://zk.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://xm.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jw.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vz.muxihuayi.cn

Java: x instanceof Number
来源：http://ug.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tq.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://hr.asd995.cn

C#:   x is int or double or decimal
来源：http://mz.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://uh.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ji.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fd.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://pd.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://om.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vm.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://un.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ma.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xg.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://je.asd995.cn

Py:   a and b or not c
来源：http://ci.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://py.huixinmuqiang.cn

JS:   a && b || !c
来源：http://zt.bookmarksfly.cn

TS:   a && b || !c
来源：http://qo.colortex.cn

Java: a && b || !c
来源：http://wt.shxzskj.cn

Go:   a && b || !c
来源：http://ux.asd995.cn

Ruby: a && b || !c
来源：http://mr.jctech888.com.cn

C#:   a && b || !c
来源：http://vt.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yj.colortex.cn

Py:   if not data: return
来源：http://vx.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://gn.yuexingan06.cn

JS:   if (!data) return;
来源：http://zi.hahajie.cn

TS:   if (!data) return;
来源：http://mm.shtwfgs.cn

Java: if (data == null) return;
来源：http://tp.chemitech.net.cn

Go:   if data == nil { return }
来源：http://qc.huixiangedu.cn

Ruby: return if data.nil?
来源：http://kl.hahajie.cn

C#:   if (data == null) return;
来源：http://pw.gzmigu.cn

================================================================================
来源：http://pi.hnjuh.cn

C. 函数与作用域
来源：http://is.yuexingan06.cn

================================================================================
来源：http://jt.muxihuayi.cn

[C01] 定义函数
来源：http://yg.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://sw.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jx.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://pp.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bs.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xu.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ef.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://jl.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xj.huixinmuqiang.cn

[C02] 默认参数
来源：http://xy.colortex.cn

Py:   def greet(name="World"): return name
来源：http://wn.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vm.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://tc.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ew.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kf.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://om.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://tp.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ro.bookmarksfly.cn

[C03] 可变参数
来源：http://vw.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://ok.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tg.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tg.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ke.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rf.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jy.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cc.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gu.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://bf.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zc.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fl.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://op.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ek.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://fw.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://ep.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://cc.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://vm.521024.cn

[C05] 返回多个值
来源：http://th.szxytkj.cn

Py:   return a, b
来源：http://jl.gzmigu.cn

PHP:  return [$a, $b];
来源：http://nb.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ke.haigaiapp.cn

TS:   return { a, b };
来源：http://yi.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://of.shxzukj.cn

Go:   return a, b
来源：http://bu.bjjhwx.cn

Ruby: return a, b
来源：http://be.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://ae.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://ze.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://wu.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://su.shxzskj.cn

JS:   const square = x => x * x;
来源：http://jj.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://rc.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sf.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vh.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://oh.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hb.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://im.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bu.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eh.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fx.bookmarksfly.cn

TS:   arr.map(String)
来源：http://oq.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qw.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://im.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://kb.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zh.newstarts.cn

[C08] 闭包
来源：http://bz.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yg.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lt.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ux.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zy.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://go.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bc.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hu.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uc.huanxung.cn

[C09] 递归
来源：http://bm.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://li.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ng.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://if.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qf.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pf.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dx.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ij.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lc.muxihuayi.cn

[C10] 变量作用域
来源：http://ds.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vh.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yt.panjiajie.cn

TS:   同 JS
来源：http://hl.521024.cn

Java: 方法内为块级作用域
来源：http://qz.jctech888.com.cn

Go:   花括号块级作用域
来源：http://eo.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ss.shxzskj.cn

C#:   块级作用域
来源：http://jw.huixiangedu.cn

[C11] 模块导入与导出
来源：http://pp.521024.cn

Py:   from module import func
来源：http://ux.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nt.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qu.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vi.huixiangedu.cn

Java: import java.util.List;
来源：http://ev.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ax.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://zb.gzmigu.cn

C#:   using System.Text;
来源：http://qp.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://mu.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://yp.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://ud.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://te.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://qi.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uf.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://hq.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://ko.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://da.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://rn.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yi.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gs.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fp.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qm.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zu.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://ap.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ec.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yr.muxihuayi.cn

[C14] 泛型函数
来源：http://ah.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://md.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://uc.hahajie.cn

JS:   // 无泛型
来源：http://sr.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bs.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pi.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rv.huixiangedu.cn

Ruby: # 无泛型
来源：http://xh.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dv.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://wo.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nt.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://st.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lj.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://se.newstarts.cn

Java: // 无解构
来源：http://mm.jctech888.com.cn

Go:   // 无解构
来源：http://ix.szsharing.cn

Ruby: a, b = pair
来源：http://xs.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://aw.521024.cn

[C16] 函数 / 方法重载
来源：http://fu.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oj.shxzukj.cn

PHP:  // 无重载
来源：http://th.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gz.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://yy.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qc.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://pk.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://on.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://de.huanxung.cn

================================================================================
来源：http://lz.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://jo.yuexingan06.cn

================================================================================
来源：http://mh.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://gb.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ea.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ca.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ct.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fq.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://se.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://li.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://ah.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://im.lnxyls.cn

[D02] 追加元素到末尾
来源：http://jf.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ua.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ht.panjiajie.cn

JS:   arr.push(4);
来源：http://ew.asd995.cn

TS:   arr.push(4);
来源：http://ic.bookmarksfly.cn

Java: list.add(4);
来源：http://zw.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://wm.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://qw.newstarts.cn

C#:   list.Add(4);
来源：http://cu.521024.cn

[D03] 在指定位置插入元素
来源：http://xh.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://fe.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xp.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ra.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://hr.9csxet.cn

Java: list.add(0, 0);
来源：http://bu.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ny.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rk.colortex.cn

C#:   list.Insert(0, 0);
来源：http://ua.shxzskj.cn

[D04] 删除元素
来源：http://pb.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pk.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gq.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sf.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://jf.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gl.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ro.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fx.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://po.nicolike.cn

[D05] 访问与修改元素
来源：http://ij.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rw.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qd.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qr.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://ie.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://am.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ow.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cu.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cu.szsharing.cn

[D06] 数组长度
来源：http://in.newstarts.cn

Py:   len(arr)
来源：http://lf.muxihuayi.cn

PHP:  count($arr);
来源：http://ug.szxytkj.cn

JS:   arr.length
来源：http://wx.haigaiapp.cn

TS:   arr.length
来源：http://sg.shxzukj.cn

Java: list.size();
来源：http://og.nszjky.cn

Go:   len(arr)
来源：http://kv.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://ub.shtwfgs.cn

C#:   list.Count;
来源：http://pc.szsharing.cn

[D07] 切片 / 取子数组
来源：http://re.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ux.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pr.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://hn.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://qp.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://iv.lnxyls.cn

Go:   arr[1:4]
来源：http://mx.asd995.cn

Ruby: arr[1, 3]
来源：http://gc.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://qw.shxzskj.cn

[D08] 合并两个数组
来源：http://ng.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://ss.colortex.cn

PHP:  array_merge($a, $b);
来源：http://ys.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ws.haigaiapp.cn

TS:   [...a, ...b];
来源：http://vm.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bp.bjjhwx.cn

Go:   append(a, b...)
来源：http://ud.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://yf.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://jd.gzmigu.cn

[D09] 排序（升序）
来源：http://cw.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://om.panjiajie.cn

PHP:  sort($arr);
来源：http://ru.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hm.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ow.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bq.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yr.yuexingan06.cn

Ruby: arr.sort
来源：http://cf.hahajie.cn

C#:   list.Sort();
来源：http://nj.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pj.huixiangedu.cn


<!-- 参考信息 -->