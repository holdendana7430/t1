代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bh.newstarts.cn

Java: x instanceof Number
来源：http://ab.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wl.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://qa.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://oc.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://cz.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kj.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lz.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ro.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://cg.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fu.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zt.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://du.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ca.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://yt.haigaiapp.cn

Py:   a and b or not c
来源：http://jl.newstarts.cn

PHP:  $a && $b || !$c
来源：http://xq.huixiangedu.cn

JS:   a && b || !c
来源：http://kp.colortex.cn

TS:   a && b || !c
来源：http://qk.huixinmuqiang.cn

Java: a && b || !c
来源：http://vi.hahajie.cn

Go:   a && b || !c
来源：http://yg.szsharing.cn

Ruby: a && b || !c
来源：http://fh.panjiajie.cn

C#:   a && b || !c
来源：http://qw.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hs.nszjky.cn

Py:   if not data: return
来源：http://wh.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://zm.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://bo.huanxung.cn

TS:   if (!data) return;
来源：http://uo.szsharing.cn

Java: if (data == null) return;
来源：http://iq.jctech888.com.cn

Go:   if data == nil { return }
来源：http://ta.jctech888.com.cn

Ruby: return if data.nil?
来源：http://gd.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://kg.nszjky.cn

================================================================================
来源：http://vw.huixiangedu.cn

C. 函数与作用域
来源：http://wc.lnxyls.cn

================================================================================
来源：http://bw.yuexingan06.cn

[C01] 定义函数
来源：http://tb.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://je.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pn.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://ys.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ub.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://re.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://me.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://hg.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mo.chemitech.net.cn

[C02] 默认参数
来源：http://xi.asd995.cn

Py:   def greet(name="World"): return name
来源：http://du.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vb.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://pi.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ct.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ab.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sg.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://me.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://vp.jctech888.com.cn

[C03] 可变参数
来源：http://qb.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://wl.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hs.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vt.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hw.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yq.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pb.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jv.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iv.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://bz.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qx.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xj.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lx.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://lk.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://pn.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://gp.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://rp.huixiangedu.cn

[C05] 返回多个值
来源：http://qw.szxytkj.cn

Py:   return a, b
来源：http://tn.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://lc.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dm.jianghongdianzi.cn

TS:   return { a, b };
来源：http://nd.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xc.szxytkj.cn

Go:   return a, b
来源：http://el.yuexingan06.cn

Ruby: return a, b
来源：http://er.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://pi.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://jz.nszjky.cn

Py:   square = lambda x: x * x
来源：http://vq.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rp.newstarts.cn

JS:   const square = x => x * x;
来源：http://uw.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://wc.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://as.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dm.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://nl.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ul.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://qz.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ue.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yf.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uy.asd995.cn

TS:   arr.map(String)
来源：http://tu.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ca.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://od.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://lp.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rz.nicolike.cn

[C08] 闭包
来源：http://ks.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cr.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qv.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rd.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cp.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qc.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tt.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sy.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://es.jianghongdianzi.cn

[C09] 递归
来源：http://cq.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eb.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gz.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://om.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vh.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ea.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ip.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wm.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nn.shtwfgs.cn

[C10] 变量作用域
来源：http://kf.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bo.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wy.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ih.521024.cn

TS:   同 JS
来源：http://re.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://fi.muxihuayi.cn

Go:   花括号块级作用域
来源：http://kz.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://so.wgjwhj.cn

C#:   块级作用域
来源：http://xe.shxzskj.cn

[C11] 模块导入与导出
来源：http://gy.gzmigu.cn

Py:   from module import func
来源：http://tc.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ze.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yr.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dv.newstarts.cn

Java: import java.util.List;
来源：http://tp.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ws.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://qj.huixinmuqiang.cn

C#:   using System.Text;
来源：http://dy.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://tf.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://lu.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://fm.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://ve.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://qj.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eg.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://qt.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://qh.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nu.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://vi.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fb.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zh.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tb.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yu.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aq.asd995.cn

Go:   func add(a, b int) int
来源：http://zt.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hs.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rg.colortex.cn

[C14] 泛型函数
来源：http://uj.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dm.panjiajie.cn

PHP:  // 无泛型
来源：http://wh.hahajie.cn

JS:   // 无泛型
来源：http://qo.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rx.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mn.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oh.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://oe.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mp.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://rh.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ze.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://ec.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ql.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lz.shtwfgs.cn

Java: // 无解构
来源：http://nh.521024.cn

Go:   // 无解构
来源：http://sv.newstarts.cn

Ruby: a, b = pair
来源：http://ke.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://lq.hahajie.cn

[C16] 函数 / 方法重载
来源：http://tb.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ba.haigaiapp.cn

PHP:  // 无重载
来源：http://kh.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bm.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ym.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ux.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://be.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://qx.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rp.jianghongdianzi.cn

================================================================================
来源：http://ws.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://ua.shxzukj.cn

================================================================================
来源：http://yt.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://gk.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rs.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wd.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vo.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wm.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qm.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://hy.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://ug.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://az.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://mt.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zx.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xc.nszjky.cn

JS:   arr.push(4);
来源：http://lb.shxzukj.cn

TS:   arr.push(4);
来源：http://vs.jianghongdianzi.cn

Java: list.add(4);
来源：http://cy.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://ze.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://eb.nszjky.cn

C#:   list.Add(4);
来源：http://rs.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://eo.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://wa.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cn.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yq.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://by.newstarts.cn

Java: list.add(0, 0);
来源：http://wq.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ih.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cd.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://bh.lnxyls.cn

[D04] 删除元素
来源：http://me.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jh.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vi.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xs.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://pr.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dl.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fz.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://em.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pb.panjiajie.cn

[D05] 访问与修改元素
来源：http://uw.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kf.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qw.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hd.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://ik.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://dk.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://dg.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nt.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qu.9csxet.cn

[D06] 数组长度
来源：http://rd.yuntaijiaju.cn

Py:   len(arr)
来源：http://jw.yuexingan06.cn

PHP:  count($arr);
来源：http://yv.gzmigu.cn

JS:   arr.length
来源：http://ga.shxzskj.cn

TS:   arr.length
来源：http://tf.huixinmuqiang.cn

Java: list.size();
来源：http://io.jctech888.com.cn

Go:   len(arr)
来源：http://il.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://qw.haigaiapp.cn

C#:   list.Count;
来源：http://gx.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://zc.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uo.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ou.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://ng.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ch.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://wk.521024.cn

Go:   arr[1:4]
来源：http://kg.gzmigu.cn

Ruby: arr[1, 3]
来源：http://lt.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://rk.bjjhwx.cn

[D08] 合并两个数组
来源：http://nj.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://yn.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://ur.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://af.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://ey.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dw.wgjwhj.cn

Go:   append(a, b...)
来源：http://ft.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://ib.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://fc.9csxet.cn

[D09] 排序（升序）
来源：http://yd.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ay.colortex.cn

PHP:  sort($arr);
来源：http://dy.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qz.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://za.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cd.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wv.9csxet.cn

Ruby: arr.sort
来源：http://it.huixinmuqiang.cn

C#:   list.Sort();
来源：http://ph.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jo.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kk.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gp.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ic.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gl.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ce.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aj.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wv.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sd.wgjwhj.cn

[D11] 反转数组
来源：http://oh.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eg.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://mw.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mm.9csxet.cn

TS:   [...arr].reverse();
来源：http://pc.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://vr.colortex.cn

Go:   slices.Reverse(arr)
来源：http://as.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://oz.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://tn.shxzskj.cn

[D12] 查找元素下标
来源：http://hc.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://fy.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hr.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yu.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cy.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://up.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://se.hahajie.cn

Ruby: arr.index(x)
来源：http://lu.huanxung.cn

C#:   list.IndexOf(x);
来源：http://ln.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://cu.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yd.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ip.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://ni.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://is.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lv.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vv.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://it.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dl.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://qm.shxzukj.cn


<!-- 参考信息 -->