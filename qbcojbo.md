代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qt.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vw.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ue.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rj.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hl.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vt.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://mv.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://xm.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://xu.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jn.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wm.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://no.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gg.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://ex.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gl.shtwfgs.cn

[B12] 跳出多层循环
来源：http://oa.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bu.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vf.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lj.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dn.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pj.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ms.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wj.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ds.szsharing.cn

[B13] 判断是否为数字
来源：http://zf.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://rt.szxytkj.cn

PHP:  is_numeric($x)
来源：http://nt.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tf.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zk.asd995.cn

Java: x instanceof Number
来源：http://ec.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wq.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ey.huanxung.cn

C#:   x is int or double or decimal
来源：http://py.521024.cn

[B14] 判断值是否在集合内
来源：http://xo.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gp.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ny.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ei.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://xb.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://st.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ko.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xs.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pg.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://bh.lnxyls.cn

Py:   a and b or not c
来源：http://ta.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://ac.bjjhwx.cn

JS:   a && b || !c
来源：http://yo.hnjuh.cn

TS:   a && b || !c
来源：http://pb.wgjwhj.cn

Java: a && b || !c
来源：http://ui.bookmarksfly.cn

Go:   a && b || !c
来源：http://jj.nszjky.cn

Ruby: a && b || !c
来源：http://kf.yuntaijiaju.cn

C#:   a && b || !c
来源：http://vt.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ra.hnjuh.cn

Py:   if not data: return
来源：http://om.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://kh.521024.cn

JS:   if (!data) return;
来源：http://kr.nicolike.cn

TS:   if (!data) return;
来源：http://lj.szxytkj.cn

Java: if (data == null) return;
来源：http://vs.wgjwhj.cn

Go:   if data == nil { return }
来源：http://sg.asd995.cn

Ruby: return if data.nil?
来源：http://fd.nicolike.cn

C#:   if (data == null) return;
来源：http://sr.yuexingan06.cn

================================================================================
来源：http://uf.hahajie.cn

C. 函数与作用域
来源：http://ga.nszjky.cn

================================================================================
来源：http://zo.nicolike.cn

[C01] 定义函数
来源：http://gp.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://ul.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xa.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://rq.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ks.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rf.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wq.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://pf.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://og.huixiangedu.cn

[C02] 默认参数
来源：http://tt.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://bf.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ta.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://tx.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qp.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pz.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zs.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://bj.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://sn.bjjhwx.cn

[C03] 可变参数
来源：http://bb.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://hh.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cc.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hs.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dq.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xy.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qq.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tq.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wt.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://uv.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sa.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://il.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nr.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cj.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ak.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://di.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://hv.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://ss.huanxung.cn

[C05] 返回多个值
来源：http://nz.muxihuayi.cn

Py:   return a, b
来源：http://cp.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://ty.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uz.szsharing.cn

TS:   return { a, b };
来源：http://md.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wr.panjiajie.cn

Go:   return a, b
来源：http://ou.lnxyls.cn

Ruby: return a, b
来源：http://hg.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://ip.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://zh.huanxung.cn

Py:   square = lambda x: x * x
来源：http://zy.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eg.huanxung.cn

JS:   const square = x => x * x;
来源：http://cl.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://dg.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jk.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ib.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://yn.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mj.hahajie.cn

[C07] 把函数作为参数传入
来源：http://fg.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gc.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fz.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sf.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://qy.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uf.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lj.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://lr.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bw.shxzskj.cn

[C08] 闭包
来源：http://uy.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://se.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yq.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yr.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://av.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ig.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://of.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tr.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tn.521024.cn

[C09] 递归
来源：http://mt.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lo.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uu.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pc.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://of.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wa.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ff.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xh.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lp.521024.cn

[C10] 变量作用域
来源：http://lz.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cc.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hl.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://am.chemitech.net.cn

TS:   同 JS
来源：http://vp.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://nj.wgjwhj.cn

Go:   花括号块级作用域
来源：http://xy.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gd.szsharing.cn

C#:   块级作用域
来源：http://oc.shxzukj.cn

[C11] 模块导入与导出
来源：http://pp.bookmarksfly.cn

Py:   from module import func
来源：http://cx.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zy.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lr.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pj.shtwfgs.cn

Java: import java.util.List;
来源：http://kn.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tt.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://py.muxihuayi.cn

C#:   using System.Text;
来源：http://iw.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://tr.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://na.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://xl.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://nf.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://zn.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mg.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://gm.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://fi.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bd.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://ov.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zz.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ob.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ln.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://go.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://eo.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://se.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ot.szsharing.cn

[C14] 泛型函数
来源：http://rs.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xc.shxzskj.cn

PHP:  // 无泛型
来源：http://rl.panjiajie.cn

JS:   // 无泛型
来源：http://of.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mh.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mu.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ks.shtwfgs.cn

Ruby: # 无泛型
来源：http://oc.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lk.huanxung.cn

[C15] 解构 / 展开参数
来源：http://xn.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ja.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://hy.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fl.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://go.yuntaijiaju.cn

Java: // 无解构
来源：http://ah.shtwfgs.cn

Go:   // 无解构
来源：http://xe.chemitech.net.cn

Ruby: a, b = pair
来源：http://ac.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://zn.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://ve.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ca.shtwfgs.cn

PHP:  // 无重载
来源：http://vt.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pt.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://fa.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dg.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://ho.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://kv.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ci.bjjhwx.cn

================================================================================
来源：http://bi.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://dq.newstarts.cn

================================================================================
来源：http://ad.szsharing.cn

[D01] 创建数组 / 列表
来源：http://zj.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wl.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fg.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mv.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eb.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qk.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://sk.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://st.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ak.huanxung.cn

[D02] 追加元素到末尾
来源：http://de.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nl.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ps.szxytkj.cn

JS:   arr.push(4);
来源：http://cn.shtwfgs.cn

TS:   arr.push(4);
来源：http://hc.huixiangedu.cn

Java: list.add(4);
来源：http://ff.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://lw.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://rr.bookmarksfly.cn

C#:   list.Add(4);
来源：http://gn.asd995.cn

[D03] 在指定位置插入元素
来源：http://fm.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://lz.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ra.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jp.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://yr.haigaiapp.cn

Java: list.add(0, 0);
来源：http://lw.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xc.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gn.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://cu.asd995.cn

[D04] 删除元素
来源：http://xs.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ia.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://py.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rn.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://xy.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://md.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vy.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://if.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wj.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://sr.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zd.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mx.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ac.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://qw.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://cm.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://et.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jb.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lc.wgjwhj.cn

[D06] 数组长度
来源：http://yi.newstarts.cn

Py:   len(arr)
来源：http://hj.huanxung.cn

PHP:  count($arr);
来源：http://ys.asd995.cn

JS:   arr.length
来源：http://lg.shtwfgs.cn

TS:   arr.length
来源：http://fe.huixiangedu.cn

Java: list.size();
来源：http://gz.huixiangedu.cn

Go:   len(arr)
来源：http://tt.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://qn.shxzskj.cn

C#:   list.Count;
来源：http://zj.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://ql.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ac.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pk.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://zh.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://gy.shxzskj.cn

Java: list.subList(1, 4);
来源：http://hq.haigaiapp.cn

Go:   arr[1:4]
来源：http://lo.hnjuh.cn

Ruby: arr[1, 3]
来源：http://vr.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://rm.shxzskj.cn

[D08] 合并两个数组
来源：http://rx.521024.cn

Py:   a + b;  a.extend(b)
来源：http://hj.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://em.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ra.muxihuayi.cn

TS:   [...a, ...b];
来源：http://dh.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kh.gzmigu.cn

Go:   append(a, b...)
来源：http://qx.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://qm.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://hi.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://kw.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://fq.hnjuh.cn

PHP:  sort($arr);
来源：http://jq.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wc.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uc.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://da.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://se.asd995.cn

Ruby: arr.sort
来源：http://wc.szsharing.cn

C#:   list.Sort();
来源：http://hp.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dw.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hd.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hq.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bt.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pj.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bn.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yy.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zf.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rh.panjiajie.cn


<!-- 参考信息 -->