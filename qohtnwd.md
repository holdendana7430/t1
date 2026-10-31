代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fg.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://nz.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zk.gzmigu.cn

[B12] 跳出多层循环
来源：http://qn.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mn.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zu.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tt.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bv.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ky.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tf.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hp.jctech888.com.cn

[B13] 判断是否为数字
来源：http://qf.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://ev.shxzukj.cn

PHP:  is_numeric($x)
来源：http://ky.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://us.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xm.szsharing.cn

Java: x instanceof Number
来源：http://wh.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xb.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://zp.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://lm.521024.cn

[B14] 判断值是否在集合内
来源：http://ld.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wg.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ba.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ql.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ig.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gu.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ox.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vr.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vv.asd995.cn

[B15] 布尔运算与取反
来源：http://me.nicolike.cn

Py:   a and b or not c
来源：http://cx.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ak.colortex.cn

JS:   a && b || !c
来源：http://hq.9csxet.cn

TS:   a && b || !c
来源：http://dl.newstarts.cn

Java: a && b || !c
来源：http://ca.9csxet.cn

Go:   a && b || !c
来源：http://zs.gzmigu.cn

Ruby: a && b || !c
来源：http://pm.shxzukj.cn

C#:   a && b || !c
来源：http://mu.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vt.nszjky.cn

Py:   if not data: return
来源：http://xv.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://sf.hahajie.cn

JS:   if (!data) return;
来源：http://ux.shxzskj.cn

TS:   if (!data) return;
来源：http://pp.hahajie.cn

Java: if (data == null) return;
来源：http://ly.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://oa.huixiangedu.cn

Ruby: return if data.nil?
来源：http://yr.yuexingan06.cn

C#:   if (data == null) return;
来源：http://gq.yuntaijiaju.cn

================================================================================
来源：http://yp.bjjhwx.cn

C. 函数与作用域
来源：http://hq.hnjuh.cn

================================================================================
来源：http://jf.nicolike.cn

[C01] 定义函数
来源：http://zs.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://om.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bl.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://xu.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eu.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jh.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ys.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://ue.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ij.huixinmuqiang.cn

[C02] 默认参数
来源：http://lc.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://va.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oc.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://do.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ms.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fa.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pm.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://xl.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://ak.nicolike.cn

[C03] 可变参数
来源：http://gn.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://re.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ry.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xu.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://io.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nd.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cm.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kq.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hs.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://hd.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nz.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://up.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jr.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ze.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://fb.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://ai.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://rx.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://mj.jctech888.com.cn

[C05] 返回多个值
来源：http://wl.bookmarksfly.cn

Py:   return a, b
来源：http://ze.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://al.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cg.huixiangedu.cn

TS:   return { a, b };
来源：http://sh.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ov.shxzskj.cn

Go:   return a, b
来源：http://ov.nicolike.cn

Ruby: return a, b
来源：http://fn.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://rw.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://ne.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://gr.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ke.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://nc.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ed.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ir.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ro.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://hm.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ni.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://is.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tm.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ig.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vt.hnjuh.cn

TS:   arr.map(String)
来源：http://yf.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lb.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tb.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://rg.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bm.shxzskj.cn

[C08] 闭包
来源：http://ll.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gp.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eb.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nf.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://et.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tf.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://go.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ax.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xc.newstarts.cn

[C09] 递归
来源：http://qd.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ed.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ro.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hs.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bf.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bu.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ds.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nh.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gj.nicolike.cn

[C10] 变量作用域
来源：http://mr.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xl.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mb.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pu.asd995.cn

TS:   同 JS
来源：http://ji.newstarts.cn

Java: 方法内为块级作用域
来源：http://sz.lnxyls.cn

Go:   花括号块级作用域
来源：http://bd.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tf.shxzukj.cn

C#:   块级作用域
来源：http://jk.521024.cn

[C11] 模块导入与导出
来源：http://qh.szxytkj.cn

Py:   from module import func
来源：http://nd.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qq.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bu.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cp.muxihuayi.cn

Java: import java.util.List;
来源：http://ms.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ci.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://kg.yuexingan06.cn

C#:   using System.Text;
来源：http://au.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://fr.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://re.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://kj.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://ec.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://iv.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rk.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://ic.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://bu.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rw.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://fv.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nw.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ju.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tr.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hd.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tc.521024.cn

Go:   func add(a, b int) int
来源：http://ig.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dl.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xq.bjjhwx.cn

[C14] 泛型函数
来源：http://lr.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://by.newstarts.cn

PHP:  // 无泛型
来源：http://ih.nicolike.cn

JS:   // 无泛型
来源：http://fm.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iy.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tv.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pa.yuexingan06.cn

Ruby: # 无泛型
来源：http://yj.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://il.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://rr.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ck.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://he.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ts.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tj.szsharing.cn

Java: // 无解构
来源：http://np.yuexingan06.cn

Go:   // 无解构
来源：http://di.gzmigu.cn

Ruby: a, b = pair
来源：http://gw.9csxet.cn

C#:   var (a, b) = pair;
来源：http://lb.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://ju.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tl.shxzskj.cn

PHP:  // 无重载
来源：http://lp.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nt.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://lx.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tm.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://wt.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://ys.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wb.colortex.cn

================================================================================
来源：http://aw.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://zm.hahajie.cn

================================================================================
来源：http://wp.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://lj.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sy.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zl.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fn.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pk.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://de.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://ja.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://hq.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fc.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://eu.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qk.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tx.lnxyls.cn

JS:   arr.push(4);
来源：http://th.bjjhwx.cn

TS:   arr.push(4);
来源：http://va.yuntaijiaju.cn

Java: list.add(4);
来源：http://mh.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://aw.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://bb.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://da.huanxung.cn

[D03] 在指定位置插入元素
来源：http://jo.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://mf.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sh.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ul.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://pn.shxzskj.cn

Java: list.add(0, 0);
来源：http://pl.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ts.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dy.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://tj.asd995.cn

[D04] 删除元素
来源：http://sr.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xp.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uc.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nd.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://db.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oq.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qa.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fw.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kb.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://he.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://be.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oj.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rn.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://ev.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://pi.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://qr.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sd.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cx.colortex.cn

[D06] 数组长度
来源：http://af.nszjky.cn

Py:   len(arr)
来源：http://dp.szxytkj.cn

PHP:  count($arr);
来源：http://np.muxihuayi.cn

JS:   arr.length
来源：http://ba.jctech888.com.cn

TS:   arr.length
来源：http://gl.panjiajie.cn

Java: list.size();
来源：http://dc.yuntaijiaju.cn

Go:   len(arr)
来源：http://cd.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://wr.haigaiapp.cn

C#:   list.Count;
来源：http://pp.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://fb.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tu.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mx.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://bi.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://le.521024.cn

Java: list.subList(1, 4);
来源：http://rp.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://pv.gzmigu.cn

Ruby: arr[1, 3]
来源：http://em.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://np.yuexingan06.cn

[D08] 合并两个数组
来源：http://jj.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://ox.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://il.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ab.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://cu.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dg.521024.cn

Go:   append(a, b...)
来源：http://ez.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://gn.521024.cn

C#:   a.Concat(b).ToList()
来源：http://xy.gzmigu.cn

[D09] 排序（升序）
来源：http://jd.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://sm.chemitech.net.cn

PHP:  sort($arr);
来源：http://dz.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ug.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hh.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qn.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lj.nszjky.cn

Ruby: arr.sort
来源：http://hr.wgjwhj.cn

C#:   list.Sort();
来源：http://mc.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tp.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eq.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dt.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dh.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ej.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://km.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ap.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ql.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mw.9csxet.cn

[D11] 反转数组
来源：http://jt.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gc.szsharing.cn

PHP:  array_reverse($arr);
来源：http://sd.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kt.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://iw.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://za.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://fv.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://mb.colortex.cn

C#:   list.Reverse();
来源：http://gl.9csxet.cn

[D12] 查找元素下标
来源：http://zl.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://xg.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pp.chemitech.net.cn


<!-- 参考信息 -->