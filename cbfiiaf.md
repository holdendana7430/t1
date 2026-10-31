代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rx.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ov.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gm.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hm.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iq.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tq.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://hl.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://fc.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://tk.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gh.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iy.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ga.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://vx.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wl.hnjuh.cn

[B12] 跳出多层循环
来源：http://fz.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ck.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uf.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://db.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bs.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lq.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oj.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bt.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://um.bjjhwx.cn

[B13] 判断是否为数字
来源：http://wt.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://me.nicolike.cn

PHP:  is_numeric($x)
来源：http://lc.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ks.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gk.newstarts.cn

Java: x instanceof Number
来源：http://sw.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eq.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://sl.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://jw.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://if.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ev.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iv.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ak.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://xs.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ty.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kq.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gd.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sq.nszjky.cn

[B15] 布尔运算与取反
来源：http://fc.nicolike.cn

Py:   a and b or not c
来源：http://pn.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://gx.chemitech.net.cn

JS:   a && b || !c
来源：http://kv.muxihuayi.cn

TS:   a && b || !c
来源：http://zo.521024.cn

Java: a && b || !c
来源：http://kp.shxzukj.cn

Go:   a && b || !c
来源：http://xj.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://hp.9csxet.cn

C#:   a && b || !c
来源：http://vv.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gh.nszjky.cn

Py:   if not data: return
来源：http://ge.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://pc.nszjky.cn

JS:   if (!data) return;
来源：http://qd.jctech888.com.cn

TS:   if (!data) return;
来源：http://xn.colortex.cn

Java: if (data == null) return;
来源：http://hy.hnjuh.cn

Go:   if data == nil { return }
来源：http://jy.wgjwhj.cn

Ruby: return if data.nil?
来源：http://mh.colortex.cn

C#:   if (data == null) return;
来源：http://zx.nszjky.cn

================================================================================
来源：http://to.yuntaijiaju.cn

C. 函数与作用域
来源：http://ox.bjjhwx.cn

================================================================================
来源：http://ls.9csxet.cn

[C01] 定义函数
来源：http://ae.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://vo.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yw.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://ck.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nq.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://va.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nk.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://td.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ig.hnjuh.cn

[C02] 默认参数
来源：http://pq.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://ri.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yg.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://fk.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jn.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sk.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://di.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://wp.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ha.hnjuh.cn

[C03] 可变参数
来源：http://nq.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://ll.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kf.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bq.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ra.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dk.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fm.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wf.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rq.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://qt.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ui.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xn.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ut.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zf.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://pt.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://ey.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://lw.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://zz.9csxet.cn

[C05] 返回多个值
来源：http://fa.lnxyls.cn

Py:   return a, b
来源：http://hj.asd995.cn

PHP:  return [$a, $b];
来源：http://lv.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yy.jianghongdianzi.cn

TS:   return { a, b };
来源：http://ve.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xx.chemitech.net.cn

Go:   return a, b
来源：http://cy.newstarts.cn

Ruby: return a, b
来源：http://rd.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://jr.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://rv.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://hz.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://at.nicolike.cn

JS:   const square = x => x * x;
来源：http://fk.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://cl.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ut.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://go.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://mf.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jo.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://hs.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sv.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yu.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xo.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://kn.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ui.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dq.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://aj.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://om.huanxung.cn

[C08] 闭包
来源：http://cs.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tc.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wr.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gt.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yy.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dc.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pb.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bu.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://es.jianghongdianzi.cn

[C09] 递归
来源：http://dn.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qr.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ls.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bo.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mh.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pr.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yw.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ty.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://in.haigaiapp.cn

[C10] 变量作用域
来源：http://wo.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ef.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pb.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qd.wgjwhj.cn

TS:   同 JS
来源：http://xb.szsharing.cn

Java: 方法内为块级作用域
来源：http://hq.jctech888.com.cn

Go:   花括号块级作用域
来源：http://fl.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wl.shxzukj.cn

C#:   块级作用域
来源：http://je.hnjuh.cn

[C11] 模块导入与导出
来源：http://db.huixiangedu.cn

Py:   from module import func
来源：http://sv.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pw.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ec.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nk.huanxung.cn

Java: import java.util.List;
来源：http://lk.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vn.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://df.hnjuh.cn

C#:   using System.Text;
来源：http://qx.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://gi.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://cm.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://xe.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://xc.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://ht.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oh.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://gp.521024.cn

Ruby: -> { puts "run" }.call
来源：http://sd.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dn.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://qn.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nr.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lb.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yv.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ar.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ds.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://sn.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lr.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tt.bjjhwx.cn

[C14] 泛型函数
来源：http://ef.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zp.9csxet.cn

PHP:  // 无泛型
来源：http://dp.muxihuayi.cn

JS:   // 无泛型
来源：http://ze.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ix.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vo.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gr.9csxet.cn

Ruby: # 无泛型
来源：http://wa.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iy.asd995.cn

[C15] 解构 / 展开参数
来源：http://zi.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ct.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://ko.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oa.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mt.szxytkj.cn

Java: // 无解构
来源：http://pn.bjjhwx.cn

Go:   // 无解构
来源：http://fn.9csxet.cn

Ruby: a, b = pair
来源：http://xo.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://yc.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://mg.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dy.yuexingan06.cn

PHP:  // 无重载
来源：http://aq.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://na.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://gg.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ms.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://bt.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://ck.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ul.9csxet.cn

================================================================================
来源：http://mq.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://ns.nszjky.cn

================================================================================
来源：http://ez.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://nr.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ig.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ab.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bl.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tp.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://os.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ly.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://lc.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cw.gzmigu.cn

[D02] 追加元素到末尾
来源：http://ti.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lf.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nu.lnxyls.cn

JS:   arr.push(4);
来源：http://io.huixiangedu.cn

TS:   arr.push(4);
来源：http://lw.szxytkj.cn

Java: list.add(4);
来源：http://dj.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://ks.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://uh.szsharing.cn

C#:   list.Add(4);
来源：http://wi.asd995.cn

[D03] 在指定位置插入元素
来源：http://zy.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://mm.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gv.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ut.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://nv.gzmigu.cn

Java: list.add(0, 0);
来源：http://dy.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nh.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://je.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://xu.huanxung.cn

[D04] 删除元素
来源：http://ng.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tk.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kd.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lg.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://sd.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xr.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ya.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://un.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uq.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://yr.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://is.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vw.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qc.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://yj.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://yx.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://yw.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dx.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kz.huixinmuqiang.cn

[D06] 数组长度
来源：http://wu.huanxung.cn

Py:   len(arr)
来源：http://gt.huixiangedu.cn

PHP:  count($arr);
来源：http://pu.bookmarksfly.cn

JS:   arr.length
来源：http://xq.hnjuh.cn

TS:   arr.length
来源：http://ej.huixiangedu.cn

Java: list.size();
来源：http://kh.colortex.cn

Go:   len(arr)
来源：http://jn.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://cz.shxzukj.cn

C#:   list.Count;
来源：http://gh.asd995.cn

[D07] 切片 / 取子数组
来源：http://to.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mj.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ne.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://xt.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://qd.szsharing.cn

Java: list.subList(1, 4);
来源：http://vl.haigaiapp.cn

Go:   arr[1:4]
来源：http://vr.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://qc.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://qo.shxzskj.cn

[D08] 合并两个数组
来源：http://tl.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://sw.521024.cn

PHP:  array_merge($a, $b);
来源：http://vz.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dc.colortex.cn

TS:   [...a, ...b];
来源：http://xx.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uu.bjjhwx.cn

Go:   append(a, b...)
来源：http://nw.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://zp.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://bj.bookmarksfly.cn

[D09] 排序（升序）
来源：http://ub.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://lj.shxzukj.cn

PHP:  sort($arr);
来源：http://qh.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jo.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sb.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vg.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://du.colortex.cn

Ruby: arr.sort
来源：http://pb.jctech888.com.cn

C#:   list.Sort();
来源：http://wn.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://io.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sy.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zq.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ms.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lf.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ha.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://em.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xs.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pj.newstarts.cn


<!-- 参考信息 -->