代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uq.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://ci.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://df.9csxet.cn

[B12] 跳出多层循环
来源：http://lb.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://az.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sv.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fl.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ew.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ea.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uv.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vv.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yu.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://fm.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://al.colortex.cn

PHP:  is_numeric($x)
来源：http://pq.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cp.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ba.jianghongdianzi.cn

Java: x instanceof Number
来源：http://vl.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kb.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://sc.hahajie.cn

C#:   x is int or double or decimal
来源：http://zb.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://xf.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pf.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fz.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://of.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://lz.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fz.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cb.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://th.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mo.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://ao.newstarts.cn

Py:   a and b or not c
来源：http://fu.szsharing.cn

PHP:  $a && $b || !$c
来源：http://ht.yuntaijiaju.cn

JS:   a && b || !c
来源：http://pq.shxzukj.cn

TS:   a && b || !c
来源：http://zj.shxzukj.cn

Java: a && b || !c
来源：http://uc.muxihuayi.cn

Go:   a && b || !c
来源：http://fg.huanxung.cn

Ruby: a && b || !c
来源：http://ao.9csxet.cn

C#:   a && b || !c
来源：http://du.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xv.hahajie.cn

Py:   if not data: return
来源：http://ge.521024.cn

PHP:  if (!$data) { return; }
来源：http://zi.lnxyls.cn

JS:   if (!data) return;
来源：http://yp.shtwfgs.cn

TS:   if (!data) return;
来源：http://nu.nszjky.cn

Java: if (data == null) return;
来源：http://kh.szxytkj.cn

Go:   if data == nil { return }
来源：http://rz.huanxung.cn

Ruby: return if data.nil?
来源：http://ph.newstarts.cn

C#:   if (data == null) return;
来源：http://mp.haigaiapp.cn

================================================================================
来源：http://xf.szxytkj.cn

C. 函数与作用域
来源：http://fj.wgjwhj.cn

================================================================================
来源：http://wm.hahajie.cn

[C01] 定义函数
来源：http://kc.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://vg.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vl.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://gv.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cl.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mq.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cz.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://xf.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yz.shtwfgs.cn

[C02] 默认参数
来源：http://tm.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://tr.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kx.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://md.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ml.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fr.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ip.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://no.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://co.nszjky.cn

[C03] 可变参数
来源：http://pz.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://ea.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xd.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qo.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sf.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ou.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vw.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pw.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rj.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://bj.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qy.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sf.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yl.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pr.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://ix.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://to.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://pn.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://kr.szsharing.cn

[C05] 返回多个值
来源：http://gr.huanxung.cn

Py:   return a, b
来源：http://kt.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://pr.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ir.huixinmuqiang.cn

TS:   return { a, b };
来源：http://ym.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mw.hnjuh.cn

Go:   return a, b
来源：http://ra.gzmigu.cn

Ruby: return a, b
来源：http://gn.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://hg.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://px.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://bm.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hg.szxytkj.cn

JS:   const square = x => x * x;
来源：http://vt.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://mh.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mj.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ts.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://vs.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qj.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://ak.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ny.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gq.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mm.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://xl.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ie.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ns.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://cg.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zs.lnxyls.cn

[C08] 闭包
来源：http://xh.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qy.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yj.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://we.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ab.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dk.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dp.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qc.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mq.jianghongdianzi.cn

[C09] 递归
来源：http://ix.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ex.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tc.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://re.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ss.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vu.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://my.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zr.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://og.nszjky.cn

[C10] 变量作用域
来源：http://gh.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tc.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://og.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hs.jianghongdianzi.cn

TS:   同 JS
来源：http://uu.521024.cn

Java: 方法内为块级作用域
来源：http://cm.colortex.cn

Go:   花括号块级作用域
来源：http://yg.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iv.jianghongdianzi.cn

C#:   块级作用域
来源：http://mt.nicolike.cn

[C11] 模块导入与导出
来源：http://fe.gzmigu.cn

Py:   from module import func
来源：http://yo.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mx.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://js.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lx.bookmarksfly.cn

Java: import java.util.List;
来源：http://bd.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qv.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://vl.jianghongdianzi.cn

C#:   using System.Text;
来源：http://lg.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://ca.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://as.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://hf.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://np.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://wd.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ru.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://hg.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://pq.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ub.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://jy.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uf.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jj.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ns.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tf.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vv.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://uu.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gv.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ih.bjjhwx.cn

[C14] 泛型函数
来源：http://ql.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://is.gzmigu.cn

PHP:  // 无泛型
来源：http://ed.shxzskj.cn

JS:   // 无泛型
来源：http://dx.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gw.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cn.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qz.gzmigu.cn

Ruby: # 无泛型
来源：http://yr.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yl.huanxung.cn

[C15] 解构 / 展开参数
来源：http://eg.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zb.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://rx.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://du.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pa.9csxet.cn

Java: // 无解构
来源：http://dy.haigaiapp.cn

Go:   // 无解构
来源：http://qr.hnjuh.cn

Ruby: a, b = pair
来源：http://xi.colortex.cn

C#:   var (a, b) = pair;
来源：http://po.9csxet.cn

[C16] 函数 / 方法重载
来源：http://jb.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eg.huixiangedu.cn

PHP:  // 无重载
来源：http://an.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zm.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://my.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yb.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://fe.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://ix.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ep.szxytkj.cn

================================================================================
来源：http://ud.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://un.jianghongdianzi.cn

================================================================================
来源：http://as.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://lf.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://su.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bw.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sp.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ln.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ks.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://tg.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://au.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hb.szxytkj.cn

[D02] 追加元素到末尾
来源：http://ve.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aj.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ky.szxytkj.cn

JS:   arr.push(4);
来源：http://km.bookmarksfly.cn

TS:   arr.push(4);
来源：http://kc.bookmarksfly.cn

Java: list.add(4);
来源：http://zn.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://is.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://el.jctech888.com.cn

C#:   list.Add(4);
来源：http://nf.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://lj.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://fj.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lo.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nh.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://hz.jctech888.com.cn

Java: list.add(0, 0);
来源：http://wf.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cw.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ch.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://yb.nszjky.cn

[D04] 删除元素
来源：http://dq.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hc.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hg.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cj.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://in.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ni.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://is.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ts.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lz.chemitech.net.cn

[D05] 访问与修改元素
来源：http://jm.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gc.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hm.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lb.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://sg.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://bk.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://nf.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ho.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://il.newstarts.cn

[D06] 数组长度
来源：http://he.szsharing.cn

Py:   len(arr)
来源：http://es.wgjwhj.cn

PHP:  count($arr);
来源：http://dj.huanxung.cn

JS:   arr.length
来源：http://do.hahajie.cn

TS:   arr.length
来源：http://lg.asd995.cn

Java: list.size();
来源：http://bv.panjiajie.cn

Go:   len(arr)
来源：http://rv.hahajie.cn

Ruby: arr.length; arr.size
来源：http://ie.szsharing.cn

C#:   list.Count;
来源：http://uu.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://kj.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yb.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jj.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://ft.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://qz.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://gx.jctech888.com.cn

Go:   arr[1:4]
来源：http://qk.gzmigu.cn

Ruby: arr[1, 3]
来源：http://as.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://dv.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://kh.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://af.asd995.cn

PHP:  array_merge($a, $b);
来源：http://zt.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fl.chemitech.net.cn

TS:   [...a, ...b];
来源：http://ny.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vh.chemitech.net.cn

Go:   append(a, b...)
来源：http://tl.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://qs.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://yg.nszjky.cn

[D09] 排序（升序）
来源：http://zd.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://mv.szxytkj.cn

PHP:  sort($arr);
来源：http://la.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lc.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pd.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zn.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tk.hahajie.cn

Ruby: arr.sort
来源：http://fs.bjjhwx.cn

C#:   list.Sort();
来源：http://fg.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iz.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ew.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jd.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yl.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yp.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sz.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tv.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xv.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hp.hnjuh.cn

[D11] 反转数组
来源：http://pj.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rz.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://vm.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://se.szxytkj.cn

TS:   [...arr].reverse();
来源：http://ue.gzmigu.cn

Java: Collections.reverse(list);
来源：http://vc.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://xq.muxihuayi.cn

Ruby: arr.reverse
来源：http://nv.huanxung.cn

C#:   list.Reverse();
来源：http://ak.lnxyls.cn

[D12] 查找元素下标
来源：http://yz.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://eh.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oz.colortex.cn


<!-- 参考信息 -->