代发 wailian999

[B09] break 与 continue
来源：http://pn.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rn.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tg.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://om.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://us.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ha.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cb.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lg.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qf.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://gp.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yw.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pf.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vi.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tc.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lk.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lj.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ze.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nv.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://ln.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://wk.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://ms.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nk.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ni.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wq.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sk.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://lh.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://us.521024.cn

[B12] 跳出多层循环
来源：http://rs.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yz.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sg.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kg.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zd.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cy.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mw.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lv.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lk.shxzukj.cn

[B13] 判断是否为数字
来源：http://jd.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://lj.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://lf.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dc.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://en.lnxyls.cn

Java: x instanceof Number
来源：http://ck.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kz.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://dq.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://lr.nszjky.cn

[B14] 判断值是否在集合内
来源：http://qc.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vq.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gy.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://kn.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://xt.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eh.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bf.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vm.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zf.9csxet.cn

[B15] 布尔运算与取反
来源：http://cz.hnjuh.cn

Py:   a and b or not c
来源：http://yl.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://zu.szxytkj.cn

JS:   a && b || !c
来源：http://dc.huanxung.cn

TS:   a && b || !c
来源：http://xa.yuntaijiaju.cn

Java: a && b || !c
来源：http://mf.newstarts.cn

Go:   a && b || !c
来源：http://fs.hnjuh.cn

Ruby: a && b || !c
来源：http://gg.shxzukj.cn

C#:   a && b || !c
来源：http://uf.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mb.shtwfgs.cn

Py:   if not data: return
来源：http://mq.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://kx.haigaiapp.cn

JS:   if (!data) return;
来源：http://hp.newstarts.cn

TS:   if (!data) return;
来源：http://pk.nicolike.cn

Java: if (data == null) return;
来源：http://hw.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://dt.szsharing.cn

Ruby: return if data.nil?
来源：http://pc.wgjwhj.cn

C#:   if (data == null) return;
来源：http://zd.newstarts.cn

================================================================================
来源：http://ih.521024.cn

C. 函数与作用域
来源：http://wx.lnxyls.cn

================================================================================
来源：http://ig.shxzskj.cn

[C01] 定义函数
来源：http://ts.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://rt.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gc.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://cc.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zq.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vb.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bi.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://gf.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bm.huixinmuqiang.cn

[C02] 默认参数
来源：http://vo.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://kt.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bh.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://wo.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vg.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pu.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uc.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://zn.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://lo.muxihuayi.cn

[C03] 可变参数
来源：http://gv.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://tv.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ty.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qf.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bk.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://de.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yo.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hv.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sw.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://du.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ta.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uz.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://av.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lb.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://tt.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://pn.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://ux.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://vt.nszjky.cn

[C05] 返回多个值
来源：http://vm.gzmigu.cn

Py:   return a, b
来源：http://ek.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://sc.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ns.lnxyls.cn

TS:   return { a, b };
来源：http://do.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wz.asd995.cn

Go:   return a, b
来源：http://xp.colortex.cn

Ruby: return a, b
来源：http://ya.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://hx.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://nd.colortex.cn

Py:   square = lambda x: x * x
来源：http://nm.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ii.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://ql.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://jm.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rt.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qr.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://iy.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bj.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://iq.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://or.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kz.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://om.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://si.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jb.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zh.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://fa.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iy.shxzukj.cn

[C08] 闭包
来源：http://tn.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ci.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ke.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dn.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ps.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ut.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zd.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ze.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ss.szxytkj.cn

[C09] 递归
来源：http://vx.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rz.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wo.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ij.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sg.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ac.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bu.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lo.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wv.asd995.cn

[C10] 变量作用域
来源：http://xp.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cm.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sl.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://so.gzmigu.cn

TS:   同 JS
来源：http://av.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://xg.yuexingan06.cn

Go:   花括号块级作用域
来源：http://xk.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tb.huanxung.cn

C#:   块级作用域
来源：http://jw.9csxet.cn

[C11] 模块导入与导出
来源：http://sp.asd995.cn

Py:   from module import func
来源：http://nh.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ak.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xf.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fp.gzmigu.cn

Java: import java.util.List;
来源：http://km.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sy.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://lm.jctech888.com.cn

C#:   using System.Text;
来源：http://to.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://nv.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://os.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://xq.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://mf.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://hm.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tf.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://vc.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://kn.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://we.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://ye.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jn.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qn.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bp.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wj.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cu.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://xg.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mj.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xs.bjjhwx.cn

[C14] 泛型函数
来源：http://rl.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fa.9csxet.cn

PHP:  // 无泛型
来源：http://ug.asd995.cn

JS:   // 无泛型
来源：http://zk.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mu.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ml.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vy.szxytkj.cn

Ruby: # 无泛型
来源：http://wq.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://de.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://ll.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gj.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://gb.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jp.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lk.hahajie.cn

Java: // 无解构
来源：http://iz.shtwfgs.cn

Go:   // 无解构
来源：http://sw.huanxung.cn

Ruby: a, b = pair
来源：http://yu.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://dd.newstarts.cn

[C16] 函数 / 方法重载
来源：http://ou.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mn.bookmarksfly.cn

PHP:  // 无重载
来源：http://ye.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mu.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://vz.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uq.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://yt.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://cv.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lt.haigaiapp.cn

================================================================================
来源：http://tb.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://xu.szxytkj.cn

================================================================================
来源：http://hk.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://cq.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rg.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sl.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rw.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pc.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ro.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://hw.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://jk.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vi.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://lv.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rf.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rr.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://ut.shxzskj.cn

TS:   arr.push(4);
来源：http://wg.asd995.cn

Java: list.add(4);
来源：http://uh.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://xv.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://nf.521024.cn

C#:   list.Add(4);
来源：http://zl.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://kl.colortex.cn

Py:   arr.insert(0, 0)
来源：http://cc.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mt.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ss.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://cw.asd995.cn

Java: list.add(0, 0);
来源：http://nm.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gr.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wv.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://kq.shxzukj.cn

[D04] 删除元素
来源：http://jd.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jw.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ft.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wy.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://rb.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wc.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ia.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qa.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tv.9csxet.cn

[D05] 访问与修改元素
来源：http://ml.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hp.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mw.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jd.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://az.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://zq.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://dm.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kv.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vo.yuntaijiaju.cn

[D06] 数组长度
来源：http://mt.yuntaijiaju.cn

Py:   len(arr)
来源：http://gz.panjiajie.cn

PHP:  count($arr);
来源：http://fl.shtwfgs.cn

JS:   arr.length
来源：http://fa.bjjhwx.cn

TS:   arr.length
来源：http://iw.huixinmuqiang.cn

Java: list.size();
来源：http://mv.huixinmuqiang.cn

Go:   len(arr)
来源：http://hm.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://wa.colortex.cn

C#:   list.Count;
来源：http://bk.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://lk.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fv.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qo.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://tb.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://sc.nszjky.cn

Java: list.subList(1, 4);
来源：http://cm.szxytkj.cn

Go:   arr[1:4]
来源：http://ds.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://yi.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://ka.huixiangedu.cn

[D08] 合并两个数组
来源：http://ql.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://sf.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://zh.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ts.lnxyls.cn

TS:   [...a, ...b];
来源：http://io.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qn.gzmigu.cn

Go:   append(a, b...)
来源：http://fm.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://sq.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://fx.521024.cn

[D09] 排序（升序）
来源：http://ol.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://wo.colortex.cn

PHP:  sort($arr);
来源：http://ug.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yx.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fl.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xv.shxzskj.cn


<!-- 参考信息 -->