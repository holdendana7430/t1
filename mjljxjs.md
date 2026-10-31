代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oy.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://kk.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wn.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dj.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rz.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ci.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fj.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xp.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dx.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tb.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://tv.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://uk.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://ks.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gh.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xf.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nu.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fu.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://ng.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fr.521024.cn

[B12] 跳出多层循环
来源：http://vw.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dq.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bx.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ug.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rs.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://df.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qb.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ee.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ow.nicolike.cn

[B13] 判断是否为数字
来源：http://ao.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://lu.panjiajie.cn

PHP:  is_numeric($x)
来源：http://so.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jo.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xg.lnxyls.cn

Java: x instanceof Number
来源：http://ez.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dc.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://rb.lnxyls.cn

C#:   x is int or double or decimal
来源：http://wl.nicolike.cn

[B14] 判断值是否在集合内
来源：http://se.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pj.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ci.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://dg.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://po.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yi.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hw.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gf.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kr.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://vt.jianghongdianzi.cn

Py:   a and b or not c
来源：http://gq.newstarts.cn

PHP:  $a && $b || !$c
来源：http://fk.yuexingan06.cn

JS:   a && b || !c
来源：http://yo.muxihuayi.cn

TS:   a && b || !c
来源：http://ki.wgjwhj.cn

Java: a && b || !c
来源：http://br.hnjuh.cn

Go:   a && b || !c
来源：http://dk.gzmigu.cn

Ruby: a && b || !c
来源：http://eo.panjiajie.cn

C#:   a && b || !c
来源：http://ua.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cu.yuntaijiaju.cn

Py:   if not data: return
来源：http://fi.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://jk.szxytkj.cn

JS:   if (!data) return;
来源：http://wm.asd995.cn

TS:   if (!data) return;
来源：http://gc.muxihuayi.cn

Java: if (data == null) return;
来源：http://sf.nszjky.cn

Go:   if data == nil { return }
来源：http://pn.9csxet.cn

Ruby: return if data.nil?
来源：http://jt.jctech888.com.cn

C#:   if (data == null) return;
来源：http://ff.bookmarksfly.cn

================================================================================
来源：http://sp.huanxung.cn

C. 函数与作用域
来源：http://av.hnjuh.cn

================================================================================
来源：http://ie.bjjhwx.cn

[C01] 定义函数
来源：http://fp.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://vn.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ml.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://yv.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zk.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zk.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://on.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://lg.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xk.shtwfgs.cn

[C02] 默认参数
来源：http://ru.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://gq.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jy.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://ly.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gs.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pq.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zw.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://kr.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://pw.colortex.cn

[C03] 可变参数
来源：http://cf.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://tg.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jc.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gq.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sf.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wf.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zy.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qx.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jt.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://rq.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lc.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tu.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kc.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yu.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://nu.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://oa.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://wa.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://zs.huanxung.cn

[C05] 返回多个值
来源：http://jv.newstarts.cn

Py:   return a, b
来源：http://ll.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://qd.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ii.nszjky.cn

TS:   return { a, b };
来源：http://sz.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vd.panjiajie.cn

Go:   return a, b
来源：http://mc.yuntaijiaju.cn

Ruby: return a, b
来源：http://lt.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://mo.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://yo.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://fj.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xu.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://nq.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://tw.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lg.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://so.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://zg.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wn.521024.cn

[C07] 把函数作为参数传入
来源：http://oi.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://af.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ok.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uz.nszjky.cn

TS:   arr.map(String)
来源：http://yp.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xn.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uk.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://os.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fb.nszjky.cn

[C08] 闭包
来源：http://gt.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xc.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gz.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fi.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nj.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iv.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lu.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qx.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ok.hahajie.cn

[C09] 递归
来源：http://bs.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bp.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rb.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fz.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mo.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yj.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jt.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xu.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mv.nicolike.cn

[C10] 变量作用域
来源：http://lw.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pv.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ss.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ob.szsharing.cn

TS:   同 JS
来源：http://tf.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://ry.colortex.cn

Go:   花括号块级作用域
来源：http://dp.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fs.szsharing.cn

C#:   块级作用域
来源：http://mw.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://ti.szsharing.cn

Py:   from module import func
来源：http://lc.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hl.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jn.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cw.nszjky.cn

Java: import java.util.List;
来源：http://xl.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://to.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://yq.gzmigu.cn

C#:   using System.Text;
来源：http://dd.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://sh.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://lz.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://ek.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://vh.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://aj.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://je.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://bu.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://eh.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://an.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://nj.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tz.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kl.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kq.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cy.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vu.9csxet.cn

Go:   func add(a, b int) int
来源：http://xt.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pk.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ur.bjjhwx.cn

[C14] 泛型函数
来源：http://uw.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yn.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://bv.huixinmuqiang.cn

JS:   // 无泛型
来源：http://pf.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gu.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fh.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ua.hnjuh.cn

Ruby: # 无泛型
来源：http://bn.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xp.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://ch.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ss.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://wt.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ts.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ym.szxytkj.cn

Java: // 无解构
来源：http://vl.gzmigu.cn

Go:   // 无解构
来源：http://nf.gzmigu.cn

Ruby: a, b = pair
来源：http://ki.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://wj.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://kl.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://po.shtwfgs.cn

PHP:  // 无重载
来源：http://ar.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ng.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://go.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bm.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://gt.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://rx.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ek.szxytkj.cn

================================================================================
来源：http://co.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://id.huixinmuqiang.cn

================================================================================
来源：http://af.nszjky.cn

[D01] 创建数组 / 列表
来源：http://at.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fx.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://es.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vh.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://es.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bu.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://er.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://aw.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jd.szxytkj.cn

[D02] 追加元素到末尾
来源：http://rn.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://og.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wc.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://el.shxzukj.cn

TS:   arr.push(4);
来源：http://eb.newstarts.cn

Java: list.add(4);
来源：http://lr.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://qp.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://xo.9csxet.cn

C#:   list.Add(4);
来源：http://rv.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://nb.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://ol.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qx.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://na.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://cz.bjjhwx.cn

Java: list.add(0, 0);
来源：http://zv.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ul.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cf.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://pw.huixiangedu.cn

[D04] 删除元素
来源：http://ky.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qd.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sq.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zr.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://ya.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ur.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://we.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://st.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ej.wgjwhj.cn

[D05] 访问与修改元素
来源：http://dk.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ew.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fa.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xr.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://if.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://zx.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://wh.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gi.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://so.huixiangedu.cn

[D06] 数组长度
来源：http://zd.gzmigu.cn

Py:   len(arr)
来源：http://wj.asd995.cn

PHP:  count($arr);
来源：http://iz.panjiajie.cn

JS:   arr.length
来源：http://gx.hnjuh.cn

TS:   arr.length
来源：http://lo.yuntaijiaju.cn

Java: list.size();
来源：http://nx.gzmigu.cn

Go:   len(arr)
来源：http://xd.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://hc.bjjhwx.cn

C#:   list.Count;
来源：http://se.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://jh.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oy.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://te.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://om.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://kw.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://dg.shxzukj.cn

Go:   arr[1:4]
来源：http://dz.hnjuh.cn

Ruby: arr[1, 3]
来源：http://xv.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://as.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://xc.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://pb.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://xa.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xd.hahajie.cn

TS:   [...a, ...b];
来源：http://es.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://os.shtwfgs.cn

Go:   append(a, b...)
来源：http://kw.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://xy.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://jm.lnxyls.cn

[D09] 排序（升序）
来源：http://eo.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://ts.szsharing.cn

PHP:  sort($arr);
来源：http://fl.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://df.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wv.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qi.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ob.shxzskj.cn

Ruby: arr.sort
来源：http://ag.bjjhwx.cn

C#:   list.Sort();
来源：http://fq.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pm.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ty.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hf.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ax.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ep.haigaiapp.cn


<!-- 参考信息 -->