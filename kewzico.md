代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wi.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://au.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dw.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jf.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jv.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yz.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://eu.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://zn.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://dy.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://av.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nn.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://on.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tp.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://cf.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pl.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://md.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sd.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sa.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mh.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nh.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gc.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vp.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wd.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kr.haigaiapp.cn

[B13] 判断是否为数字
来源：http://dg.521024.cn

Py:   isinstance(x, (int, float))
来源：http://co.hnjuh.cn

PHP:  is_numeric($x)
来源：http://mn.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ad.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wd.gzmigu.cn

Java: x instanceof Number
来源：http://xt.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vy.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://qy.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://ie.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://pc.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xn.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iy.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://fv.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://zb.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sv.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vj.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ec.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ma.shxzskj.cn

[B15] 布尔运算与取反
来源：http://wl.asd995.cn

Py:   a and b or not c
来源：http://tf.newstarts.cn

PHP:  $a && $b || !$c
来源：http://cr.9csxet.cn

JS:   a && b || !c
来源：http://eh.szxytkj.cn

TS:   a && b || !c
来源：http://dn.asd995.cn

Java: a && b || !c
来源：http://qg.yuntaijiaju.cn

Go:   a && b || !c
来源：http://hi.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://yb.huixinmuqiang.cn

C#:   a && b || !c
来源：http://fc.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://je.huixinmuqiang.cn

Py:   if not data: return
来源：http://du.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://hs.shxzukj.cn

JS:   if (!data) return;
来源：http://hg.muxihuayi.cn

TS:   if (!data) return;
来源：http://hz.haigaiapp.cn

Java: if (data == null) return;
来源：http://yx.huanxung.cn

Go:   if data == nil { return }
来源：http://lo.huanxung.cn

Ruby: return if data.nil?
来源：http://dk.szxytkj.cn

C#:   if (data == null) return;
来源：http://mb.shxzskj.cn

================================================================================
来源：http://os.haigaiapp.cn

C. 函数与作用域
来源：http://za.shxzskj.cn

================================================================================
来源：http://ze.jianghongdianzi.cn

[C01] 定义函数
来源：http://va.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://su.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iq.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://re.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zj.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hk.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zy.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://ij.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cw.szxytkj.cn

[C02] 默认参数
来源：http://zx.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://xp.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sy.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://sg.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uq.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nb.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nn.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ti.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://ic.newstarts.cn

[C03] 可变参数
来源：http://or.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://ha.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pq.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wg.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mr.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ur.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sx.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vd.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cs.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://nj.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vw.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zg.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yd.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rs.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://uo.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://yn.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://xf.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://jw.chemitech.net.cn

[C05] 返回多个值
来源：http://xr.shxzukj.cn

Py:   return a, b
来源：http://sj.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://ag.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lp.shxzukj.cn

TS:   return { a, b };
来源：http://oi.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://la.bjjhwx.cn

Go:   return a, b
来源：http://na.521024.cn

Ruby: return a, b
来源：http://ak.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ty.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://si.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://tc.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lc.nicolike.cn

JS:   const square = x => x * x;
来源：http://dr.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://aa.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hu.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://od.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://yt.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xo.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://rl.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sk.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wv.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fs.shxzskj.cn

TS:   arr.map(String)
来源：http://op.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://le.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wr.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://dn.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ob.newstarts.cn

[C08] 闭包
来源：http://ww.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jn.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://re.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://te.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kk.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hg.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rc.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://em.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jq.colortex.cn

[C09] 递归
来源：http://bi.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ra.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xw.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fb.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zp.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pa.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hw.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ou.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rl.lnxyls.cn

[C10] 变量作用域
来源：http://yp.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sw.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sp.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uo.nszjky.cn

TS:   同 JS
来源：http://if.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://uc.jctech888.com.cn

Go:   花括号块级作用域
来源：http://mt.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kl.haigaiapp.cn

C#:   块级作用域
来源：http://ra.yuexingan06.cn

[C11] 模块导入与导出
来源：http://wa.haigaiapp.cn

Py:   from module import func
来源：http://ek.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ug.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xy.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fl.nszjky.cn

Java: import java.util.List;
来源：http://cs.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hc.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://yv.newstarts.cn

C#:   using System.Text;
来源：http://il.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://go.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://vx.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://zo.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://cc.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://hu.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pl.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://iw.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://lb.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pl.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://xr.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gf.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zr.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ld.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gy.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xd.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://tw.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://au.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nw.colortex.cn

[C14] 泛型函数
来源：http://ej.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zy.wgjwhj.cn

PHP:  // 无泛型
来源：http://ec.bjjhwx.cn

JS:   // 无泛型
来源：http://hm.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wz.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mb.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bg.gzmigu.cn

Ruby: # 无泛型
来源：http://up.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fk.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://tq.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lx.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://yh.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yf.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lc.yuexingan06.cn

Java: // 无解构
来源：http://um.shxzukj.cn

Go:   // 无解构
来源：http://vo.asd995.cn

Ruby: a, b = pair
来源：http://ms.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://pi.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://uh.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pc.haigaiapp.cn

PHP:  // 无重载
来源：http://uk.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ku.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://om.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sk.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://rb.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://xo.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ja.521024.cn

================================================================================
来源：http://cx.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://km.hahajie.cn

================================================================================
来源：http://ks.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://zw.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nv.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ek.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rk.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gb.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://je.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://fp.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://zu.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fd.521024.cn

[D02] 追加元素到末尾
来源：http://wh.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ey.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rj.colortex.cn

JS:   arr.push(4);
来源：http://pv.haigaiapp.cn

TS:   arr.push(4);
来源：http://sd.wgjwhj.cn

Java: list.add(4);
来源：http://jp.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://ar.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://vd.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://ov.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://ey.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://tz.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bp.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pl.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ju.lnxyls.cn

Java: list.add(0, 0);
来源：http://qk.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cn.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ca.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://ev.colortex.cn

[D04] 删除元素
来源：http://qe.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qj.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jy.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://id.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://ss.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nv.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tr.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jt.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cq.nszjky.cn

[D05] 访问与修改元素
来源：http://xg.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cs.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ar.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ra.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://vu.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ul.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://uy.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lx.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dk.9csxet.cn

[D06] 数组长度
来源：http://hq.bookmarksfly.cn

Py:   len(arr)
来源：http://wj.9csxet.cn

PHP:  count($arr);
来源：http://ao.nszjky.cn

JS:   arr.length
来源：http://wz.hahajie.cn

TS:   arr.length
来源：http://ua.nszjky.cn

Java: list.size();
来源：http://ei.muxihuayi.cn

Go:   len(arr)
来源：http://ni.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://ji.9csxet.cn

C#:   list.Count;
来源：http://nf.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://ud.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jy.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ev.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://aj.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://kg.asd995.cn

Java: list.subList(1, 4);
来源：http://qq.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://rr.szsharing.cn

Ruby: arr[1, 3]
来源：http://yn.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://bb.hahajie.cn

[D08] 合并两个数组
来源：http://zu.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://ty.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://tq.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ul.muxihuayi.cn

TS:   [...a, ...b];
来源：http://pk.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wd.shxzukj.cn

Go:   append(a, b...)
来源：http://ns.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://mi.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://iz.bookmarksfly.cn

[D09] 排序（升序）
来源：http://lv.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ms.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://zf.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bc.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lc.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zu.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zr.hahajie.cn

Ruby: arr.sort
来源：http://bh.gzmigu.cn

C#:   list.Sort();
来源：http://ii.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://za.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://do.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ig.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vw.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://px.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xa.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sq.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kw.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ho.chemitech.net.cn


<!-- 参考信息 -->