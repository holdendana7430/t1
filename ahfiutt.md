代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yf.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://nj.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yp.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gu.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aw.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gm.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iv.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jc.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vw.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fr.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://yu.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://xk.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://vh.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ol.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sx.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ec.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pp.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://ep.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fx.lnxyls.cn

[B12] 跳出多层循环
来源：http://fh.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sb.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kz.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zt.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ws.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lw.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gp.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ca.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ox.hnjuh.cn

[B13] 判断是否为数字
来源：http://ze.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://qe.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://gm.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ws.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vz.shxzukj.cn

Java: x instanceof Number
来源：http://xa.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bd.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://ja.521024.cn

C#:   x is int or double or decimal
来源：http://xp.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://gc.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cx.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sb.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://iz.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://ls.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zi.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eo.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ex.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ll.gzmigu.cn

[B15] 布尔运算与取反
来源：http://jz.shtwfgs.cn

Py:   a and b or not c
来源：http://pv.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://wh.colortex.cn

JS:   a && b || !c
来源：http://or.jctech888.com.cn

TS:   a && b || !c
来源：http://xh.hnjuh.cn

Java: a && b || !c
来源：http://nm.bookmarksfly.cn

Go:   a && b || !c
来源：http://ib.hnjuh.cn

Ruby: a && b || !c
来源：http://tl.huixiangedu.cn

C#:   a && b || !c
来源：http://tx.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tu.9csxet.cn

Py:   if not data: return
来源：http://yv.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://sc.hnjuh.cn

JS:   if (!data) return;
来源：http://st.szxytkj.cn

TS:   if (!data) return;
来源：http://wa.hnjuh.cn

Java: if (data == null) return;
来源：http://tg.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://zw.shxzukj.cn

Ruby: return if data.nil?
来源：http://gz.gzmigu.cn

C#:   if (data == null) return;
来源：http://gi.hnjuh.cn

================================================================================
来源：http://nq.szxytkj.cn

C. 函数与作用域
来源：http://kg.szsharing.cn

================================================================================
来源：http://wg.jctech888.com.cn

[C01] 定义函数
来源：http://xr.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://km.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ks.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://ro.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tk.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fu.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fn.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://ph.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ur.wgjwhj.cn

[C02] 默认参数
来源：http://xg.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://bz.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://km.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://be.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yb.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ur.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lj.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://pz.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://ty.huixinmuqiang.cn

[C03] 可变参数
来源：http://rb.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://go.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tx.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mn.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ac.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://np.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xj.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xk.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pi.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://rs.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kg.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nu.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zz.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ma.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://ao.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://ej.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://th.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://qe.yuntaijiaju.cn

[C05] 返回多个值
来源：http://fh.shtwfgs.cn

Py:   return a, b
来源：http://xh.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://gz.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oz.521024.cn

TS:   return { a, b };
来源：http://ak.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qs.huixinmuqiang.cn

Go:   return a, b
来源：http://pj.shxzukj.cn

Ruby: return a, b
来源：http://gy.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://vz.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://qk.colortex.cn

Py:   square = lambda x: x * x
来源：http://xi.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cq.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://pl.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://hc.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pa.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mo.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://wy.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://og.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://nb.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yc.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lu.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mu.jctech888.com.cn

TS:   arr.map(String)
来源：http://vl.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oa.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://da.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://bv.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qg.shtwfgs.cn

[C08] 闭包
来源：http://fd.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aw.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gm.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dd.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fz.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ny.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://br.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qh.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pu.yuexingan06.cn

[C09] 递归
来源：http://ii.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://am.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oa.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ph.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tr.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lh.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ra.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nh.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fi.jctech888.com.cn

[C10] 变量作用域
来源：http://ax.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sk.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zl.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kt.haigaiapp.cn

TS:   同 JS
来源：http://qc.shxzukj.cn

Java: 方法内为块级作用域
来源：http://yi.nszjky.cn

Go:   花括号块级作用域
来源：http://cz.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gb.jianghongdianzi.cn

C#:   块级作用域
来源：http://zt.hahajie.cn

[C11] 模块导入与导出
来源：http://zm.huixinmuqiang.cn

Py:   from module import func
来源：http://vr.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xj.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aw.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tn.huixiangedu.cn

Java: import java.util.List;
来源：http://xn.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rt.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://or.9csxet.cn

C#:   using System.Text;
来源：http://vu.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://ux.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://po.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://tb.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://hp.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://tw.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ud.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://gk.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://zq.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yl.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://rs.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://it.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://up.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zf.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ri.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dt.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://hg.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uo.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qv.colortex.cn

[C14] 泛型函数
来源：http://be.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wd.chemitech.net.cn

PHP:  // 无泛型
来源：http://ro.jianghongdianzi.cn

JS:   // 无泛型
来源：http://hw.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ir.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jn.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cz.huanxung.cn

Ruby: # 无泛型
来源：http://ot.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xh.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://tc.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pq.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ki.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jp.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://at.asd995.cn

Java: // 无解构
来源：http://wm.wgjwhj.cn

Go:   // 无解构
来源：http://eo.lnxyls.cn

Ruby: a, b = pair
来源：http://uh.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://nf.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://mg.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pv.asd995.cn

PHP:  // 无重载
来源：http://os.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vc.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://fw.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cn.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://ri.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://jg.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cn.521024.cn

================================================================================
来源：http://cm.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://xs.9csxet.cn

================================================================================
来源：http://vd.szsharing.cn

[D01] 创建数组 / 列表
来源：http://dy.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mf.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ub.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wv.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kl.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ge.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://jw.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://av.521024.cn

[D02] 追加元素到末尾
来源：http://zw.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ee.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zg.yuexingan06.cn

JS:   arr.push(4);
来源：http://oo.521024.cn

TS:   arr.push(4);
来源：http://ct.nicolike.cn

Java: list.add(4);
来源：http://ai.521024.cn

Go:   arr = append(arr, 4)
来源：http://dk.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://ft.gzmigu.cn

C#:   list.Add(4);
来源：http://ou.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://te.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://tk.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://to.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qp.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://cc.nszjky.cn

Java: list.add(0, 0);
来源：http://cb.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://za.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sn.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://sh.newstarts.cn

[D04] 删除元素
来源：http://fz.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wl.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vc.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bw.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://gg.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uc.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qt.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bn.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vi.nszjky.cn

[D05] 访问与修改元素
来源：http://vp.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bv.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zk.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wu.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://ns.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://yv.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://lm.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nc.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xh.hnjuh.cn

[D06] 数组长度
来源：http://uv.nszjky.cn

Py:   len(arr)
来源：http://wp.szxytkj.cn

PHP:  count($arr);
来源：http://vx.asd995.cn

JS:   arr.length
来源：http://ze.lnxyls.cn

TS:   arr.length
来源：http://lc.hahajie.cn

Java: list.size();
来源：http://xa.haigaiapp.cn

Go:   len(arr)
来源：http://nx.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://ie.hnjuh.cn

C#:   list.Count;
来源：http://cn.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://ig.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gw.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qe.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://ry.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://qn.shxzukj.cn

Java: list.subList(1, 4);
来源：http://cy.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://jr.newstarts.cn

Ruby: arr[1, 3]
来源：http://ch.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://gt.shxzukj.cn

[D08] 合并两个数组
来源：http://in.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://tp.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://ea.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zq.lnxyls.cn

TS:   [...a, ...b];
来源：http://ox.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ql.shtwfgs.cn

Go:   append(a, b...)
来源：http://xa.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://yu.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://vp.wgjwhj.cn

[D09] 排序（升序）
来源：http://to.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://jn.huanxung.cn

PHP:  sort($arr);
来源：http://os.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ef.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gi.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kj.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xp.nszjky.cn

Ruby: arr.sort
来源：http://xc.shtwfgs.cn

C#:   list.Sort();
来源：http://ec.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://it.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rt.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mm.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vr.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oz.nicolike.cn


<!-- 参考信息 -->