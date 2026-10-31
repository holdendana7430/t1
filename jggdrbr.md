代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://en.9csxet.cn

[B10] 遍历同时拿索引
来源：http://vt.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tu.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kb.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rq.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jt.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gt.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hc.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gl.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ik.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://mx.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://jq.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://nd.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jr.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ec.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uf.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ia.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://xz.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zn.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://pp.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yo.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jp.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://io.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lz.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://af.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pd.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vy.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qe.shxzskj.cn

[B13] 判断是否为数字
来源：http://fi.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://nm.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://lp.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uf.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://no.chemitech.net.cn

Java: x instanceof Number
来源：http://gy.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ey.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://wc.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://vn.nicolike.cn

[B14] 判断值是否在集合内
来源：http://hg.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yn.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fm.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://kd.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://by.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://du.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jo.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://si.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fg.szsharing.cn

[B15] 布尔运算与取反
来源：http://fa.chemitech.net.cn

Py:   a and b or not c
来源：http://hl.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://aq.chemitech.net.cn

JS:   a && b || !c
来源：http://tb.panjiajie.cn

TS:   a && b || !c
来源：http://le.nszjky.cn

Java: a && b || !c
来源：http://iv.szsharing.cn

Go:   a && b || !c
来源：http://qu.hnjuh.cn

Ruby: a && b || !c
来源：http://hm.szsharing.cn

C#:   a && b || !c
来源：http://yv.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ww.lnxyls.cn

Py:   if not data: return
来源：http://ni.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://fs.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://ck.yuexingan06.cn

TS:   if (!data) return;
来源：http://ri.jctech888.com.cn

Java: if (data == null) return;
来源：http://mg.521024.cn

Go:   if data == nil { return }
来源：http://br.bjjhwx.cn

Ruby: return if data.nil?
来源：http://ft.asd995.cn

C#:   if (data == null) return;
来源：http://ez.bookmarksfly.cn

================================================================================
来源：http://zh.hnjuh.cn

C. 函数与作用域
来源：http://ur.colortex.cn

================================================================================
来源：http://ud.yuntaijiaju.cn

[C01] 定义函数
来源：http://lm.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://xn.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ou.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://kq.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ly.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sf.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://si.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://yo.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wh.hnjuh.cn

[C02] 默认参数
来源：http://cy.asd995.cn

Py:   def greet(name="World"): return name
来源：http://pk.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ft.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://aw.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ci.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mu.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bo.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://tw.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://lj.shxzskj.cn

[C03] 可变参数
来源：http://ly.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://hq.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://we.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ap.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vr.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qs.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qw.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nh.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ss.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://xd.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jr.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wc.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fx.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oh.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://mm.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://es.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://mq.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://mv.nicolike.cn

[C05] 返回多个值
来源：http://bv.lnxyls.cn

Py:   return a, b
来源：http://rj.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://me.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xj.jianghongdianzi.cn

TS:   return { a, b };
来源：http://ro.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lb.yuexingan06.cn

Go:   return a, b
来源：http://dn.bjjhwx.cn

Ruby: return a, b
来源：http://qy.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://hl.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://sm.newstarts.cn

Py:   square = lambda x: x * x
来源：http://et.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gi.lnxyls.cn

JS:   const square = x => x * x;
来源：http://wq.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://fw.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gl.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vl.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://ec.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jc.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://pc.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wb.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gf.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ge.shxzukj.cn

TS:   arr.map(String)
来源：http://bh.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ry.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gb.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://yp.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://le.huixiangedu.cn

[C08] 闭包
来源：http://xj.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rq.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ub.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bt.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eq.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ir.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tb.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zg.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sk.muxihuayi.cn

[C09] 递归
来源：http://fs.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://le.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xt.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uy.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hj.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vd.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bh.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bv.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sg.lnxyls.cn

[C10] 变量作用域
来源：http://ct.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ks.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wu.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dl.bjjhwx.cn

TS:   同 JS
来源：http://ne.hnjuh.cn

Java: 方法内为块级作用域
来源：http://cc.huanxung.cn

Go:   花括号块级作用域
来源：http://uv.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ej.lnxyls.cn

C#:   块级作用域
来源：http://yn.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://nh.jctech888.com.cn

Py:   from module import func
来源：http://hd.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hk.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sd.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vy.hnjuh.cn

Java: import java.util.List;
来源：http://dl.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oh.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://zn.haigaiapp.cn

C#:   using System.Text;
来源：http://yt.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://ek.colortex.cn

Py:   (lambda: print("run"))()
来源：http://nv.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://wx.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://tr.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://ns.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wd.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://ym.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://iw.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qi.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://ie.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uo.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vt.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ht.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fj.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sz.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://qc.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oh.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://he.bookmarksfly.cn

[C14] 泛型函数
来源：http://it.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mc.hnjuh.cn

PHP:  // 无泛型
来源：http://jg.huixinmuqiang.cn

JS:   // 无泛型
来源：http://jm.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rv.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dx.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ob.gzmigu.cn

Ruby: # 无泛型
来源：http://ru.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zx.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://yj.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cc.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://gc.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xv.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ug.bjjhwx.cn

Java: // 无解构
来源：http://lk.nicolike.cn

Go:   // 无解构
来源：http://ph.521024.cn

Ruby: a, b = pair
来源：http://nd.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://hk.newstarts.cn

[C16] 函数 / 方法重载
来源：http://tb.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ep.nicolike.cn

PHP:  // 无重载
来源：http://ee.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jw.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://yo.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vh.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://nn.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://au.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ua.chemitech.net.cn

================================================================================
来源：http://te.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://yr.newstarts.cn

================================================================================
来源：http://ow.huanxung.cn

[D01] 创建数组 / 列表
来源：http://rb.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fm.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fq.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zj.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://va.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zc.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://ib.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://cl.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ti.hahajie.cn

[D02] 追加元素到末尾
来源：http://is.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://az.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qo.huanxung.cn

JS:   arr.push(4);
来源：http://fe.asd995.cn

TS:   arr.push(4);
来源：http://tm.panjiajie.cn

Java: list.add(4);
来源：http://fh.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://sq.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://cd.gzmigu.cn

C#:   list.Add(4);
来源：http://fd.nicolike.cn

[D03] 在指定位置插入元素
来源：http://aj.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://su.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mu.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://du.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://jh.panjiajie.cn

Java: list.add(0, 0);
来源：http://sq.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://py.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jh.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://xx.yuntaijiaju.cn

[D04] 删除元素
来源：http://gu.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ah.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mf.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sy.colortex.cn

TS:   arr.splice(0, 1);
来源：http://wc.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yn.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hp.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fe.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ln.shxzskj.cn

[D05] 访问与修改元素
来源：http://gz.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bl.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ay.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tk.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://kj.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://hz.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://iq.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://md.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vw.haigaiapp.cn

[D06] 数组长度
来源：http://md.lnxyls.cn

Py:   len(arr)
来源：http://lh.bookmarksfly.cn

PHP:  count($arr);
来源：http://kh.lnxyls.cn

JS:   arr.length
来源：http://oj.huanxung.cn

TS:   arr.length
来源：http://av.wgjwhj.cn

Java: list.size();
来源：http://we.bookmarksfly.cn

Go:   len(arr)
来源：http://mw.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://dr.shxzukj.cn

C#:   list.Count;
来源：http://aq.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://tl.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gm.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yt.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://if.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://lg.521024.cn

Java: list.subList(1, 4);
来源：http://gy.9csxet.cn

Go:   arr[1:4]
来源：http://ii.shxzskj.cn

Ruby: arr[1, 3]
来源：http://ww.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://zn.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://kv.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://th.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://tc.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gn.jctech888.com.cn

TS:   [...a, ...b];
来源：http://js.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ld.szxytkj.cn

Go:   append(a, b...)
来源：http://tc.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://ny.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://lz.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://bl.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://av.muxihuayi.cn

PHP:  sort($arr);
来源：http://ur.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xu.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ip.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zu.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fn.hnjuh.cn

Ruby: arr.sort
来源：http://cz.521024.cn

C#:   list.Sort();
来源：http://kk.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ik.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ko.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mi.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sj.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ud.colortex.cn


<!-- 参考信息 -->