代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ky.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ry.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rb.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uz.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ba.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://id.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://em.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pz.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pb.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ks.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ph.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ee.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vu.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yb.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://rd.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://kx.colortex.cn

PHP:  range(0, 10, 2);
来源：http://ui.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zy.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ji.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hr.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jj.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://kw.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tl.szxytkj.cn

[B12] 跳出多层循环
来源：http://ec.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hr.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zb.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rp.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://el.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rv.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cp.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gx.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yr.hahajie.cn

[B13] 判断是否为数字
来源：http://uw.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://ce.newstarts.cn

PHP:  is_numeric($x)
来源：http://uu.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://um.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kg.shxzukj.cn

Java: x instanceof Number
来源：http://ky.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mz.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://ni.panjiajie.cn

C#:   x is int or double or decimal
来源：http://se.huanxung.cn

[B14] 判断值是否在集合内
来源：http://jz.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bq.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ca.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://dl.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ur.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tx.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zm.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ns.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ur.asd995.cn

[B15] 布尔运算与取反
来源：http://ph.huanxung.cn

Py:   a and b or not c
来源：http://sy.colortex.cn

PHP:  $a && $b || !$c
来源：http://iz.shtwfgs.cn

JS:   a && b || !c
来源：http://so.9csxet.cn

TS:   a && b || !c
来源：http://nn.huanxung.cn

Java: a && b || !c
来源：http://ge.muxihuayi.cn

Go:   a && b || !c
来源：http://oa.yuexingan06.cn

Ruby: a && b || !c
来源：http://sq.szsharing.cn

C#:   a && b || !c
来源：http://jv.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://at.521024.cn

Py:   if not data: return
来源：http://uo.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://nz.lnxyls.cn

JS:   if (!data) return;
来源：http://ph.huanxung.cn

TS:   if (!data) return;
来源：http://ba.hnjuh.cn

Java: if (data == null) return;
来源：http://fy.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://zv.lnxyls.cn

Ruby: return if data.nil?
来源：http://rk.wgjwhj.cn

C#:   if (data == null) return;
来源：http://xr.asd995.cn

================================================================================
来源：http://fj.nicolike.cn

C. 函数与作用域
来源：http://jw.asd995.cn

================================================================================
来源：http://wa.yuexingan06.cn

[C01] 定义函数
来源：http://ao.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://qv.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ev.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://na.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cl.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cv.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ov.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://qp.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lg.asd995.cn

[C02] 默认参数
来源：http://vk.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://ip.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tw.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://to.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kl.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jl.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nk.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://lh.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ci.nicolike.cn

[C03] 可变参数
来源：http://xd.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://cb.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://by.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fs.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ss.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qm.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jb.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hd.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ug.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://fs.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fl.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xz.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yz.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vz.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://aw.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://ze.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://we.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://hq.shxzukj.cn

[C05] 返回多个值
来源：http://di.muxihuayi.cn

Py:   return a, b
来源：http://ng.lnxyls.cn

PHP:  return [$a, $b];
来源：http://kk.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zn.jctech888.com.cn

TS:   return { a, b };
来源：http://gq.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ap.bookmarksfly.cn

Go:   return a, b
来源：http://om.newstarts.cn

Ruby: return a, b
来源：http://cs.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://zk.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://ih.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://hb.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://il.gzmigu.cn

JS:   const square = x => x * x;
来源：http://lr.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://hh.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jb.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://id.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://yt.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://av.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://es.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bl.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gc.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qo.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://hb.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://np.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ze.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://qq.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qk.9csxet.cn

[C08] 闭包
来源：http://qs.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vd.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yu.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mf.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ub.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://by.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ao.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nt.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xz.shtwfgs.cn

[C09] 递归
来源：http://og.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ea.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uu.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://te.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bt.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ru.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fa.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zv.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rn.wgjwhj.cn

[C10] 变量作用域
来源：http://yw.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pc.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pv.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nc.haigaiapp.cn

TS:   同 JS
来源：http://ol.lnxyls.cn

Java: 方法内为块级作用域
来源：http://eq.huixiangedu.cn

Go:   花括号块级作用域
来源：http://iv.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lf.hahajie.cn

C#:   块级作用域
来源：http://ou.nicolike.cn

[C11] 模块导入与导出
来源：http://cv.hahajie.cn

Py:   from module import func
来源：http://lw.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zv.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ok.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tt.hnjuh.cn

Java: import java.util.List;
来源：http://tf.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://px.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://fz.chemitech.net.cn

C#:   using System.Text;
来源：http://gi.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://qo.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://nd.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://fj.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://im.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://pd.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hm.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://lh.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://tg.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ux.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://ch.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gj.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ky.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tm.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yx.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ag.newstarts.cn

Go:   func add(a, b int) int
来源：http://zx.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fm.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ym.newstarts.cn

[C14] 泛型函数
来源：http://ot.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tc.wgjwhj.cn

PHP:  // 无泛型
来源：http://iy.hnjuh.cn

JS:   // 无泛型
来源：http://dc.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://os.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jb.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tv.shxzukj.cn

Ruby: # 无泛型
来源：http://ad.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yv.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://fp.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zp.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://sl.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hj.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bl.panjiajie.cn

Java: // 无解构
来源：http://gt.jianghongdianzi.cn

Go:   // 无解构
来源：http://wo.hahajie.cn

Ruby: a, b = pair
来源：http://ev.nszjky.cn

C#:   var (a, b) = pair;
来源：http://ak.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://fh.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://so.huixinmuqiang.cn

PHP:  // 无重载
来源：http://cv.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ei.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://xi.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ds.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://ap.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://hz.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xw.panjiajie.cn

================================================================================
来源：http://zr.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://uy.bookmarksfly.cn

================================================================================
来源：http://nw.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://of.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://la.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pa.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fq.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kt.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zk.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://oc.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://sc.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ga.szsharing.cn

[D02] 追加元素到末尾
来源：http://qf.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ct.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ad.haigaiapp.cn

JS:   arr.push(4);
来源：http://bl.521024.cn

TS:   arr.push(4);
来源：http://ty.panjiajie.cn

Java: list.add(4);
来源：http://ti.521024.cn

Go:   arr = append(arr, 4)
来源：http://yq.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://gu.nszjky.cn

C#:   list.Add(4);
来源：http://bw.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://bz.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://cl.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xf.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dm.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ni.shxzskj.cn

Java: list.add(0, 0);
来源：http://nr.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lz.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kr.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://mo.wgjwhj.cn

[D04] 删除元素
来源：http://jq.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cg.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ib.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zm.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://om.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pt.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://te.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mw.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qv.jctech888.com.cn

[D05] 访问与修改元素
来源：http://ni.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dl.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lg.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hb.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://mu.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://up.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://na.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fc.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vf.newstarts.cn

[D06] 数组长度
来源：http://pv.yuexingan06.cn

Py:   len(arr)
来源：http://yt.huixinmuqiang.cn

PHP:  count($arr);
来源：http://zr.bjjhwx.cn

JS:   arr.length
来源：http://hj.gzmigu.cn

TS:   arr.length
来源：http://sz.haigaiapp.cn

Java: list.size();
来源：http://tk.huixinmuqiang.cn

Go:   len(arr)
来源：http://ui.hahajie.cn

Ruby: arr.length; arr.size
来源：http://he.haigaiapp.cn

C#:   list.Count;
来源：http://kg.newstarts.cn

[D07] 切片 / 取子数组
来源：http://mx.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ez.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dp.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://hg.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://yp.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://py.newstarts.cn

Go:   arr[1:4]
来源：http://uj.panjiajie.cn

Ruby: arr[1, 3]
来源：http://hq.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://hm.9csxet.cn

[D08] 合并两个数组
来源：http://cu.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://ay.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://ec.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fr.jctech888.com.cn

TS:   [...a, ...b];
来源：http://yb.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fn.panjiajie.cn

Go:   append(a, b...)
来源：http://nm.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://bj.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://nd.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://uk.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://mm.newstarts.cn

PHP:  sort($arr);
来源：http://tj.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dn.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cg.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rw.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ue.huanxung.cn

Ruby: arr.sort
来源：http://vv.shtwfgs.cn

C#:   list.Sort();
来源：http://ti.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oy.szsharing.cn


<!-- 参考信息 -->