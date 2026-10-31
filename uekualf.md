代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://on.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kd.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ca.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ty.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ug.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://fs.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qr.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ua.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://af.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ea.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ex.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lh.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ms.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tt.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://za.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://zw.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://at.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fj.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sc.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://el.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xi.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://mb.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hf.nszjky.cn

[B12] 跳出多层循环
来源：http://ny.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tc.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ht.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iw.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://se.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ih.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ly.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ey.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jh.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://rr.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://ek.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://bs.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ig.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zh.asd995.cn

Java: x instanceof Number
来源：http://rr.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jk.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://xm.shxzukj.cn

C#:   x is int or double or decimal
来源：http://is.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://gs.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nv.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ms.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://xt.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://dz.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iz.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sn.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xw.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://do.panjiajie.cn

[B15] 布尔运算与取反
来源：http://pr.haigaiapp.cn

Py:   a and b or not c
来源：http://pa.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://tf.huanxung.cn

JS:   a && b || !c
来源：http://zt.wgjwhj.cn

TS:   a && b || !c
来源：http://no.hnjuh.cn

Java: a && b || !c
来源：http://ow.yuntaijiaju.cn

Go:   a && b || !c
来源：http://ed.hahajie.cn

Ruby: a && b || !c
来源：http://hz.yuntaijiaju.cn

C#:   a && b || !c
来源：http://gp.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kc.huixinmuqiang.cn

Py:   if not data: return
来源：http://rs.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://os.lnxyls.cn

JS:   if (!data) return;
来源：http://gc.nicolike.cn

TS:   if (!data) return;
来源：http://vq.szsharing.cn

Java: if (data == null) return;
来源：http://sm.gzmigu.cn

Go:   if data == nil { return }
来源：http://qm.wgjwhj.cn

Ruby: return if data.nil?
来源：http://sc.huanxung.cn

C#:   if (data == null) return;
来源：http://nv.jctech888.com.cn

================================================================================
来源：http://qk.bookmarksfly.cn

C. 函数与作用域
来源：http://vr.bookmarksfly.cn

================================================================================
来源：http://qq.panjiajie.cn

[C01] 定义函数
来源：http://jf.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://ml.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ps.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://xe.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fp.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yi.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sb.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://gs.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yv.muxihuayi.cn

[C02] 默认参数
来源：http://aw.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://pb.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gq.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://ex.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nh.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ga.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vr.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://iq.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://oo.nicolike.cn

[C03] 可变参数
来源：http://ae.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://yg.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tm.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ty.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mi.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ea.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zs.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lj.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ib.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://pu.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://im.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aw.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jv.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tg.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://sd.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://uz.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://aj.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://ez.521024.cn

[C05] 返回多个值
来源：http://zy.hnjuh.cn

Py:   return a, b
来源：http://dq.nszjky.cn

PHP:  return [$a, $b];
来源：http://sg.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tu.szxytkj.cn

TS:   return { a, b };
来源：http://uu.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oo.colortex.cn

Go:   return a, b
来源：http://rq.yuexingan06.cn

Ruby: return a, b
来源：http://an.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://nx.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://ki.colortex.cn

Py:   square = lambda x: x * x
来源：http://su.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rs.nicolike.cn

JS:   const square = x => x * x;
来源：http://bs.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://cf.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lk.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fx.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://jf.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://io.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://rk.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qi.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ea.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bb.szsharing.cn

TS:   arr.map(String)
来源：http://wg.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hp.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nt.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://ui.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lt.nicolike.cn

[C08] 闭包
来源：http://kc.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dk.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zn.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ej.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fm.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qq.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xi.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gb.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://py.gzmigu.cn

[C09] 递归
来源：http://vl.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://me.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pq.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uq.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fn.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ig.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sq.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ls.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fl.shtwfgs.cn

[C10] 变量作用域
来源：http://nn.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vn.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hl.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oe.lnxyls.cn

TS:   同 JS
来源：http://kj.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://fc.szxytkj.cn

Go:   花括号块级作用域
来源：http://zi.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ei.huixiangedu.cn

C#:   块级作用域
来源：http://qp.521024.cn

[C11] 模块导入与导出
来源：http://ju.9csxet.cn

Py:   from module import func
来源：http://yn.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://co.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ej.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pp.szxytkj.cn

Java: import java.util.List;
来源：http://zm.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mf.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://wg.panjiajie.cn

C#:   using System.Text;
来源：http://gf.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://ak.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://aj.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://gc.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://wb.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://jr.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lu.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://yq.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://na.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ct.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://wz.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sl.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gi.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oq.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nz.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wp.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://py.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://it.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kz.haigaiapp.cn

[C14] 泛型函数
来源：http://mn.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tq.bjjhwx.cn

PHP:  // 无泛型
来源：http://us.lnxyls.cn

JS:   // 无泛型
来源：http://gt.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ky.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ee.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iu.jctech888.com.cn

Ruby: # 无泛型
来源：http://sv.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ch.asd995.cn

[C15] 解构 / 展开参数
来源：http://fy.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lz.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://vi.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ra.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://er.panjiajie.cn

Java: // 无解构
来源：http://cu.huanxung.cn

Go:   // 无解构
来源：http://re.huanxung.cn

Ruby: a, b = pair
来源：http://yl.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://ox.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://su.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vo.huanxung.cn

PHP:  // 无重载
来源：http://rn.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xs.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://fk.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qv.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://zd.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://sf.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dm.huixinmuqiang.cn

================================================================================
来源：http://gm.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://si.yuntaijiaju.cn

================================================================================
来源：http://ky.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://vb.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jg.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dk.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bb.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://um.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ev.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://yq.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://uj.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ji.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://qe.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zm.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vc.jctech888.com.cn

JS:   arr.push(4);
来源：http://kz.muxihuayi.cn

TS:   arr.push(4);
来源：http://ya.yuntaijiaju.cn

Java: list.add(4);
来源：http://qf.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://ai.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://sf.hnjuh.cn

C#:   list.Add(4);
来源：http://ms.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://rk.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://yg.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wc.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ss.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://wv.nszjky.cn

Java: list.add(0, 0);
来源：http://nr.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://px.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nv.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://dg.asd995.cn

[D04] 删除元素
来源：http://bp.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://du.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uh.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ue.colortex.cn

TS:   arr.splice(0, 1);
来源：http://wu.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fo.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://od.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ce.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sn.haigaiapp.cn

[D05] 访问与修改元素
来源：http://mf.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pl.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zo.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uz.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://jb.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://ad.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://xt.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qe.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jp.9csxet.cn

[D06] 数组长度
来源：http://wl.yuexingan06.cn

Py:   len(arr)
来源：http://rs.colortex.cn

PHP:  count($arr);
来源：http://iy.gzmigu.cn

JS:   arr.length
来源：http://vn.jctech888.com.cn

TS:   arr.length
来源：http://ih.panjiajie.cn

Java: list.size();
来源：http://yn.shxzukj.cn

Go:   len(arr)
来源：http://ki.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://mp.szsharing.cn

C#:   list.Count;
来源：http://db.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://gq.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tq.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tj.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://jz.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://nh.newstarts.cn

Java: list.subList(1, 4);
来源：http://rr.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://fh.nicolike.cn

Ruby: arr[1, 3]
来源：http://mz.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://ow.muxihuayi.cn

[D08] 合并两个数组
来源：http://qd.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://an.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://ja.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nv.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://fe.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wi.shtwfgs.cn

Go:   append(a, b...)
来源：http://sn.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://hg.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://fj.hnjuh.cn

[D09] 排序（升序）
来源：http://nw.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://aw.lnxyls.cn

PHP:  sort($arr);
来源：http://ex.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xo.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ib.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pz.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sn.nicolike.cn

Ruby: arr.sort
来源：http://ov.gzmigu.cn

C#:   list.Sort();
来源：http://pm.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hr.szsharing.cn


<!-- 参考信息 -->