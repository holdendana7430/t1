代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rx.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zq.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://iw.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://sc.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://qq.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kw.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gk.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dx.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tn.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://xr.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mu.lnxyls.cn

[B12] 跳出多层循环
来源：http://ab.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yj.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qm.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://is.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tu.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cl.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qo.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lv.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fc.jctech888.com.cn

[B13] 判断是否为数字
来源：http://tw.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://uk.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://bn.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pl.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ni.hnjuh.cn

Java: x instanceof Number
来源：http://ns.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tj.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://vn.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://jc.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://lc.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ah.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uc.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://ur.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://wq.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dd.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sc.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yl.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dz.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://pz.panjiajie.cn

Py:   a and b or not c
来源：http://ap.hahajie.cn

PHP:  $a && $b || !$c
来源：http://gg.wgjwhj.cn

JS:   a && b || !c
来源：http://qw.hnjuh.cn

TS:   a && b || !c
来源：http://cl.521024.cn

Java: a && b || !c
来源：http://ex.haigaiapp.cn

Go:   a && b || !c
来源：http://ee.nicolike.cn

Ruby: a && b || !c
来源：http://ru.szsharing.cn

C#:   a && b || !c
来源：http://ic.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://za.jctech888.com.cn

Py:   if not data: return
来源：http://ph.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://tf.hnjuh.cn

JS:   if (!data) return;
来源：http://na.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://tu.chemitech.net.cn

Java: if (data == null) return;
来源：http://rt.lnxyls.cn

Go:   if data == nil { return }
来源：http://gd.colortex.cn

Ruby: return if data.nil?
来源：http://ob.shxzskj.cn

C#:   if (data == null) return;
来源：http://xd.shxzskj.cn

================================================================================
来源：http://mx.shxzskj.cn

C. 函数与作用域
来源：http://ud.huixinmuqiang.cn

================================================================================
来源：http://nl.bjjhwx.cn

[C01] 定义函数
来源：http://tc.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://ln.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zi.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://zw.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sb.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ro.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xp.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://do.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ra.muxihuayi.cn

[C02] 默认参数
来源：http://ie.asd995.cn

Py:   def greet(name="World"): return name
来源：http://un.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ax.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://ym.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hl.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dq.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oj.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://xh.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://sl.newstarts.cn

[C03] 可变参数
来源：http://ty.521024.cn

Py:   def total(*args): return sum(args)
来源：http://ql.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uc.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wr.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qg.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ft.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zs.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pw.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rl.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://je.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wm.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yk.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zv.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ih.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://xs.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://ju.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://ny.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://bz.9csxet.cn

[C05] 返回多个值
来源：http://go.chemitech.net.cn

Py:   return a, b
来源：http://mg.gzmigu.cn

PHP:  return [$a, $b];
来源：http://jq.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oi.huixinmuqiang.cn

TS:   return { a, b };
来源：http://em.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zg.szxytkj.cn

Go:   return a, b
来源：http://zo.szxytkj.cn

Ruby: return a, b
来源：http://dh.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://yj.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://ld.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://rh.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dj.nszjky.cn

JS:   const square = x => x * x;
来源：http://ai.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://be.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://za.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hy.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://wf.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ag.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://ev.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aa.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wj.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kn.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://du.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kw.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ol.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://jk.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hr.haigaiapp.cn

[C08] 闭包
来源：http://qi.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://si.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yk.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nw.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qg.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bs.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zg.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bf.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vw.jianghongdianzi.cn

[C09] 递归
来源：http://tq.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://so.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://do.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://da.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hy.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wg.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hk.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://go.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qj.9csxet.cn

[C10] 变量作用域
来源：http://wc.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hy.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xw.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ch.chemitech.net.cn

TS:   同 JS
来源：http://lw.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://zn.9csxet.cn

Go:   花括号块级作用域
来源：http://mc.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kl.nicolike.cn

C#:   块级作用域
来源：http://vg.nszjky.cn

[C11] 模块导入与导出
来源：http://yq.hahajie.cn

Py:   from module import func
来源：http://wp.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zn.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vb.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bt.haigaiapp.cn

Java: import java.util.List;
来源：http://zl.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cc.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://ob.szsharing.cn

C#:   using System.Text;
来源：http://if.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://ct.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://hf.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://yq.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://th.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://jv.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yu.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://ag.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://kp.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wy.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://gn.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bv.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://we.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zm.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bt.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dw.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://rh.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tn.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sl.hahajie.cn

[C14] 泛型函数
来源：http://se.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mh.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://nt.yuntaijiaju.cn

JS:   // 无泛型
来源：http://ie.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sb.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xx.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ho.szxytkj.cn

Ruby: # 无泛型
来源：http://go.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ok.hahajie.cn

[C15] 解构 / 展开参数
来源：http://hb.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xa.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://tl.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zi.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uh.nszjky.cn

Java: // 无解构
来源：http://ns.lnxyls.cn

Go:   // 无解构
来源：http://zi.shxzukj.cn

Ruby: a, b = pair
来源：http://xe.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://ck.hahajie.cn

[C16] 函数 / 方法重载
来源：http://fz.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cq.bookmarksfly.cn

PHP:  // 无重载
来源：http://np.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fu.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://mm.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wo.521024.cn

Go:   // 无重载：用不同函数名
来源：http://vp.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://bb.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tu.asd995.cn

================================================================================
来源：http://ih.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://dn.muxihuayi.cn

================================================================================
来源：http://uq.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://ez.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mq.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cs.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zf.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nw.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://df.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://pf.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://gk.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://us.shxzskj.cn

[D02] 追加元素到末尾
来源：http://ae.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dp.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dc.shxzskj.cn

JS:   arr.push(4);
来源：http://ms.muxihuayi.cn

TS:   arr.push(4);
来源：http://yi.jianghongdianzi.cn

Java: list.add(4);
来源：http://sz.521024.cn

Go:   arr = append(arr, 4)
来源：http://fi.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ip.newstarts.cn

C#:   list.Add(4);
来源：http://zm.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://ng.asd995.cn

Py:   arr.insert(0, 0)
来源：http://gz.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rk.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nf.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://mw.shtwfgs.cn

Java: list.add(0, 0);
来源：http://ex.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zu.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lo.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://el.newstarts.cn

[D04] 删除元素
来源：http://sh.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jf.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mv.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mv.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://kv.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ud.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mj.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jb.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gj.colortex.cn

[D05] 访问与修改元素
来源：http://qz.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uv.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xj.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ot.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://jf.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://wr.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://de.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ei.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vn.jianghongdianzi.cn

[D06] 数组长度
来源：http://ww.huixinmuqiang.cn

Py:   len(arr)
来源：http://vf.haigaiapp.cn

PHP:  count($arr);
来源：http://xs.hahajie.cn

JS:   arr.length
来源：http://wq.nszjky.cn

TS:   arr.length
来源：http://vd.jianghongdianzi.cn

Java: list.size();
来源：http://qg.jctech888.com.cn

Go:   len(arr)
来源：http://gr.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://mx.asd995.cn

C#:   list.Count;
来源：http://ux.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://yk.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://un.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qc.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://jf.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://nr.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://dc.huixiangedu.cn

Go:   arr[1:4]
来源：http://uf.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://cv.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://io.chemitech.net.cn

[D08] 合并两个数组
来源：http://ws.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://em.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://ye.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ty.muxihuayi.cn

TS:   [...a, ...b];
来源：http://vs.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vv.hahajie.cn

Go:   append(a, b...)
来源：http://fb.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://da.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://la.haigaiapp.cn

[D09] 排序（升序）
来源：http://na.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://zh.hahajie.cn

PHP:  sort($arr);
来源：http://mp.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://im.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://of.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ed.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zv.chemitech.net.cn

Ruby: arr.sort
来源：http://ns.muxihuayi.cn

C#:   list.Sort();
来源：http://qa.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qg.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mo.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qn.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qt.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hg.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://az.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kv.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ka.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cq.jctech888.com.cn

[D11] 反转数组
来源：http://iw.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rp.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://ct.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eu.huanxung.cn


<!-- 参考信息 -->