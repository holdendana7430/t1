代发 wailian999

[B09] break 与 continue
来源：http://ir.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hl.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ww.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sc.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xs.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://np.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ho.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ys.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://on.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://pg.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uh.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qc.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wp.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ly.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cf.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nd.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ay.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sl.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://jj.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://tw.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://xf.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vr.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rc.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tg.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xt.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://vo.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pp.yuexingan06.cn

[B12] 跳出多层循环
来源：http://cf.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fd.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wi.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bx.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ks.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ka.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ls.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fd.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gr.jctech888.com.cn

[B13] 判断是否为数字
来源：http://jo.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://wr.nszjky.cn

PHP:  is_numeric($x)
来源：http://fd.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hr.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lx.yuexingan06.cn

Java: x instanceof Number
来源：http://qe.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ob.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://bs.szsharing.cn

C#:   x is int or double or decimal
来源：http://fc.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://ah.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yc.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gj.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://iu.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://wq.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yt.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wh.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pr.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vk.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://yk.muxihuayi.cn

Py:   a and b or not c
来源：http://cv.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://ew.lnxyls.cn

JS:   a && b || !c
来源：http://bs.jianghongdianzi.cn

TS:   a && b || !c
来源：http://fo.hahajie.cn

Java: a && b || !c
来源：http://jj.szxytkj.cn

Go:   a && b || !c
来源：http://ht.lnxyls.cn

Ruby: a && b || !c
来源：http://pl.bjjhwx.cn

C#:   a && b || !c
来源：http://hm.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lq.huixiangedu.cn

Py:   if not data: return
来源：http://lu.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://cu.haigaiapp.cn

JS:   if (!data) return;
来源：http://ns.yuexingan06.cn

TS:   if (!data) return;
来源：http://wy.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://ck.wgjwhj.cn

Go:   if data == nil { return }
来源：http://bp.huixiangedu.cn

Ruby: return if data.nil?
来源：http://wl.shxzukj.cn

C#:   if (data == null) return;
来源：http://ts.hahajie.cn

================================================================================
来源：http://bb.muxihuayi.cn

C. 函数与作用域
来源：http://tw.huixiangedu.cn

================================================================================
来源：http://bn.newstarts.cn

[C01] 定义函数
来源：http://ta.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://xz.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qv.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://es.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mh.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ob.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mg.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://tm.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yy.huanxung.cn

[C02] 默认参数
来源：http://lm.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://ei.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://or.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://pd.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://da.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ji.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gz.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://xs.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://ki.hahajie.cn

[C03] 可变参数
来源：http://vs.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://id.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oj.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dx.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ty.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ja.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lm.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ko.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tj.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://xx.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hc.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ww.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jj.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yu.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://rw.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://ci.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://wu.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://et.yuexingan06.cn

[C05] 返回多个值
来源：http://ad.panjiajie.cn

Py:   return a, b
来源：http://fp.9csxet.cn

PHP:  return [$a, $b];
来源：http://bz.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ug.shtwfgs.cn

TS:   return { a, b };
来源：http://gz.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ve.shtwfgs.cn

Go:   return a, b
来源：http://yf.bookmarksfly.cn

Ruby: return a, b
来源：http://hn.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://sz.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://cx.colortex.cn

Py:   square = lambda x: x * x
来源：http://nn.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://td.huanxung.cn

JS:   const square = x => x * x;
来源：http://qc.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://kx.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://id.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xl.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://es.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lr.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://wb.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ho.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kn.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ut.chemitech.net.cn

TS:   arr.map(String)
来源：http://gq.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tb.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://op.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://ec.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ex.yuexingan06.cn

[C08] 闭包
来源：http://xf.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bd.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://js.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hi.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://am.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xb.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ky.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cb.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lg.shtwfgs.cn

[C09] 递归
来源：http://eu.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ec.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zc.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hs.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mi.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ho.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lz.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ik.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bl.bjjhwx.cn

[C10] 变量作用域
来源：http://vl.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lo.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hl.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://li.nicolike.cn

TS:   同 JS
来源：http://ni.9csxet.cn

Java: 方法内为块级作用域
来源：http://xz.9csxet.cn

Go:   花括号块级作用域
来源：http://ch.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ss.jianghongdianzi.cn

C#:   块级作用域
来源：http://do.asd995.cn

[C11] 模块导入与导出
来源：http://ui.nicolike.cn

Py:   from module import func
来源：http://ck.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kf.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://di.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zq.asd995.cn

Java: import java.util.List;
来源：http://zx.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ey.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://dm.yuexingan06.cn

C#:   using System.Text;
来源：http://fh.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://rj.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://sb.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://vx.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://or.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://kj.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ez.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ef.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://us.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ns.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://vl.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fl.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gj.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cp.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kh.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://si.521024.cn

Go:   func add(a, b int) int
来源：http://do.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pj.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rj.szxytkj.cn

[C14] 泛型函数
来源：http://bi.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gx.nicolike.cn

PHP:  // 无泛型
来源：http://om.chemitech.net.cn

JS:   // 无泛型
来源：http://bj.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qb.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pk.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bg.shtwfgs.cn

Ruby: # 无泛型
来源：http://ni.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sw.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://yt.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wj.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://rj.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xx.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kv.yuexingan06.cn

Java: // 无解构
来源：http://wk.colortex.cn

Go:   // 无解构
来源：http://ff.nszjky.cn

Ruby: a, b = pair
来源：http://dj.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://oo.huanxung.cn

[C16] 函数 / 方法重载
来源：http://sz.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hn.521024.cn

PHP:  // 无重载
来源：http://ql.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oe.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://dz.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yg.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://ur.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://ih.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pa.asd995.cn

================================================================================
来源：http://sf.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://zq.shxzukj.cn

================================================================================
来源：http://ap.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://zt.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ur.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rr.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ll.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xf.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dp.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://qa.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://wy.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wp.asd995.cn

[D02] 追加元素到末尾
来源：http://wb.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pq.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qg.hnjuh.cn

JS:   arr.push(4);
来源：http://hr.bookmarksfly.cn

TS:   arr.push(4);
来源：http://qx.huixiangedu.cn

Java: list.add(4);
来源：http://ac.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://ey.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://if.muxihuayi.cn

C#:   list.Add(4);
来源：http://yf.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://hf.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://dx.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kf.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nt.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://by.shtwfgs.cn

Java: list.add(0, 0);
来源：http://eu.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vq.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wo.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://sa.hnjuh.cn

[D04] 删除元素
来源：http://pl.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ep.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sz.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wt.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://yi.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://on.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://to.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bj.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dg.521024.cn

[D05] 访问与修改元素
来源：http://vc.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xo.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://et.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ou.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://dd.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://vb.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://sq.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jw.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zm.hahajie.cn

[D06] 数组长度
来源：http://jg.colortex.cn

Py:   len(arr)
来源：http://mv.521024.cn

PHP:  count($arr);
来源：http://fj.huixinmuqiang.cn

JS:   arr.length
来源：http://oy.shtwfgs.cn

TS:   arr.length
来源：http://zu.asd995.cn

Java: list.size();
来源：http://os.asd995.cn

Go:   len(arr)
来源：http://kg.szsharing.cn

Ruby: arr.length; arr.size
来源：http://fd.gzmigu.cn

C#:   list.Count;
来源：http://ys.newstarts.cn

[D07] 切片 / 取子数组
来源：http://uv.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nh.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pk.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://xj.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://qr.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://bg.szsharing.cn

Go:   arr[1:4]
来源：http://cj.lnxyls.cn

Ruby: arr[1, 3]
来源：http://vo.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://dl.panjiajie.cn

[D08] 合并两个数组
来源：http://tl.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://te.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://hg.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hb.521024.cn

TS:   [...a, ...b];
来源：http://bk.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wl.521024.cn

Go:   append(a, b...)
来源：http://rj.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://iu.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://ew.panjiajie.cn

[D09] 排序（升序）
来源：http://fk.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://el.asd995.cn

PHP:  sort($arr);
来源：http://xy.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vl.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rx.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://to.jctech888.com.cn


<!-- 参考信息 -->