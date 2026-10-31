代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://al.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://nr.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vw.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ye.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jm.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ys.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qp.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hl.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://de.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fd.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://tn.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://vi.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://qr.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qx.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ky.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xj.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sv.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://bu.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tl.panjiajie.cn

[B12] 跳出多层循环
来源：http://bi.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nr.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pa.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fv.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sz.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pv.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gl.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://li.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fr.huanxung.cn

[B13] 判断是否为数字
来源：http://eb.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://mv.9csxet.cn

PHP:  is_numeric($x)
来源：http://yg.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jj.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xq.lnxyls.cn

Java: x instanceof Number
来源：http://bs.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uc.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://wa.9csxet.cn

C#:   x is int or double or decimal
来源：http://lh.nszjky.cn

[B14] 判断值是否在集合内
来源：http://bw.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rx.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mx.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://jm.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://ux.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://us.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cx.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wd.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wr.szsharing.cn

[B15] 布尔运算与取反
来源：http://ly.huixinmuqiang.cn

Py:   a and b or not c
来源：http://fg.newstarts.cn

PHP:  $a && $b || !$c
来源：http://kw.asd995.cn

JS:   a && b || !c
来源：http://ls.szsharing.cn

TS:   a && b || !c
来源：http://dd.yuntaijiaju.cn

Java: a && b || !c
来源：http://sm.huanxung.cn

Go:   a && b || !c
来源：http://ae.huanxung.cn

Ruby: a && b || !c
来源：http://zq.521024.cn

C#:   a && b || !c
来源：http://tx.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vf.asd995.cn

Py:   if not data: return
来源：http://js.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://dm.nszjky.cn

JS:   if (!data) return;
来源：http://zn.szxytkj.cn

TS:   if (!data) return;
来源：http://hy.panjiajie.cn

Java: if (data == null) return;
来源：http://lu.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://mh.hahajie.cn

Ruby: return if data.nil?
来源：http://si.gzmigu.cn

C#:   if (data == null) return;
来源：http://by.wgjwhj.cn

================================================================================
来源：http://wx.colortex.cn

C. 函数与作用域
来源：http://ck.szxytkj.cn

================================================================================
来源：http://re.jctech888.com.cn

[C01] 定义函数
来源：http://mz.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://pp.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ev.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ju.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ez.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zx.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://no.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://kt.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dx.lnxyls.cn

[C02] 默认参数
来源：http://vw.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://mz.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ei.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://bv.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fg.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://al.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ro.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://cu.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://go.yuexingan06.cn

[C03] 可变参数
来源：http://nb.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://vi.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://an.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bt.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cs.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wh.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vw.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rw.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ix.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://vk.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ch.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tb.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rw.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://su.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://cp.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://hl.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://na.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://pf.wgjwhj.cn

[C05] 返回多个值
来源：http://zm.szsharing.cn

Py:   return a, b
来源：http://kf.huanxung.cn

PHP:  return [$a, $b];
来源：http://rp.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pd.huixiangedu.cn

TS:   return { a, b };
来源：http://jt.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cd.bjjhwx.cn

Go:   return a, b
来源：http://kt.newstarts.cn

Ruby: return a, b
来源：http://fz.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://el.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://gy.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://ln.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wz.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://nu.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://yx.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kx.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://aq.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://kz.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://si.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://mv.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xh.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bo.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vg.haigaiapp.cn

TS:   arr.map(String)
来源：http://lt.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ox.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tk.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://nq.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kg.huanxung.cn

[C08] 闭包
来源：http://rg.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dr.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://az.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ew.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ih.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bc.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ox.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tw.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vw.chemitech.net.cn

[C09] 递归
来源：http://rq.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mb.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mz.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://th.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qh.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xp.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uq.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sf.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vu.hnjuh.cn

[C10] 变量作用域
来源：http://tl.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hv.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kl.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gw.huixinmuqiang.cn

TS:   同 JS
来源：http://fx.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://qb.huixiangedu.cn

Go:   花括号块级作用域
来源：http://un.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pn.shxzukj.cn

C#:   块级作用域
来源：http://te.bjjhwx.cn

[C11] 模块导入与导出
来源：http://dv.bjjhwx.cn

Py:   from module import func
来源：http://hv.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mh.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uk.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ia.nszjky.cn

Java: import java.util.List;
来源：http://gu.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nm.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://hl.jianghongdianzi.cn

C#:   using System.Text;
来源：http://yb.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://cp.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://az.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://gv.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://gj.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://lt.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nj.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://mx.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://nr.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sn.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://it.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xh.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vp.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pw.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gt.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sy.shxzukj.cn

Go:   func add(a, b int) int
来源：http://va.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yo.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ni.521024.cn

[C14] 泛型函数
来源：http://pf.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bj.jctech888.com.cn

PHP:  // 无泛型
来源：http://bz.lnxyls.cn

JS:   // 无泛型
来源：http://bz.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gr.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rr.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cf.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://dc.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vn.newstarts.cn

[C15] 解构 / 展开参数
来源：http://vm.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pb.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://qu.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mm.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zw.jctech888.com.cn

Java: // 无解构
来源：http://ab.asd995.cn

Go:   // 无解构
来源：http://zu.nicolike.cn

Ruby: a, b = pair
来源：http://yv.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://hj.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://ds.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vk.szxytkj.cn

PHP:  // 无重载
来源：http://uy.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rw.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://os.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sd.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://me.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://ga.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mg.nszjky.cn

================================================================================
来源：http://bt.521024.cn

D. 数组 / 列表 / 集合
来源：http://uo.bjjhwx.cn

================================================================================
来源：http://fi.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://nm.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://be.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tx.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zn.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ek.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vr.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://ez.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://nh.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gn.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://si.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gp.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://in.shtwfgs.cn

JS:   arr.push(4);
来源：http://wr.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://nr.chemitech.net.cn

Java: list.add(4);
来源：http://hw.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://ad.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://hi.hahajie.cn

C#:   list.Add(4);
来源：http://ur.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://pv.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://jq.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ly.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ru.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://gy.colortex.cn

Java: list.add(0, 0);
来源：http://bj.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ju.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://od.521024.cn

C#:   list.Insert(0, 0);
来源：http://xw.asd995.cn

[D04] 删除元素
来源：http://uk.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pg.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zv.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vc.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://an.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gp.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://if.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vz.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ax.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://ph.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ka.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mu.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ve.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://if.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://dj.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://eb.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://km.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ig.huanxung.cn

[D06] 数组长度
来源：http://jo.yuexingan06.cn

Py:   len(arr)
来源：http://yk.nicolike.cn

PHP:  count($arr);
来源：http://vg.bookmarksfly.cn

JS:   arr.length
来源：http://mc.bookmarksfly.cn

TS:   arr.length
来源：http://ba.9csxet.cn

Java: list.size();
来源：http://zj.nszjky.cn

Go:   len(arr)
来源：http://fj.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://wz.hnjuh.cn

C#:   list.Count;
来源：http://dl.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://kh.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tq.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rb.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://vm.521024.cn

TS:   arr.slice(1, 4);
来源：http://qw.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://mm.9csxet.cn

Go:   arr[1:4]
来源：http://oc.9csxet.cn

Ruby: arr[1, 3]
来源：http://sc.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://kq.nszjky.cn

[D08] 合并两个数组
来源：http://mk.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://nn.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://is.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bs.shxzukj.cn

TS:   [...a, ...b];
来源：http://jf.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ei.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://py.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://aj.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://xt.nicolike.cn

[D09] 排序（升序）
来源：http://po.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://fu.muxihuayi.cn

PHP:  sort($arr);
来源：http://fa.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zb.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yv.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qb.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ed.hnjuh.cn

Ruby: arr.sort
来源：http://ul.asd995.cn

C#:   list.Sort();
来源：http://ee.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dy.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://we.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ws.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gi.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rv.9csxet.cn


<!-- 参考信息 -->