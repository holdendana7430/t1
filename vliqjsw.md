代发 wailian999

PHP:  range(0, 10, 2);
来源：http://zm.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://of.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bu.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xh.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cl.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://fw.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vg.huanxung.cn

[B12] 跳出多层循环
来源：http://ib.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nm.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://di.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uu.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://go.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://be.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xs.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ci.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sr.yuexingan06.cn

[B13] 判断是否为数字
来源：http://kd.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://jp.shxzskj.cn

PHP:  is_numeric($x)
来源：http://es.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ra.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oc.shtwfgs.cn

Java: x instanceof Number
来源：http://rw.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://re.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://ep.hahajie.cn

C#:   x is int or double or decimal
来源：http://eo.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://fs.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ep.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ot.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://xr.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://xv.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sz.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bc.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tk.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://og.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://sj.hahajie.cn

Py:   a and b or not c
来源：http://ij.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://dl.colortex.cn

JS:   a && b || !c
来源：http://mg.9csxet.cn

TS:   a && b || !c
来源：http://pr.chemitech.net.cn

Java: a && b || !c
来源：http://nq.muxihuayi.cn

Go:   a && b || !c
来源：http://pq.asd995.cn

Ruby: a && b || !c
来源：http://vu.wgjwhj.cn

C#:   a && b || !c
来源：http://ey.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yv.wgjwhj.cn

Py:   if not data: return
来源：http://nv.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://xn.szxytkj.cn

JS:   if (!data) return;
来源：http://jp.9csxet.cn

TS:   if (!data) return;
来源：http://xq.wgjwhj.cn

Java: if (data == null) return;
来源：http://ck.huanxung.cn

Go:   if data == nil { return }
来源：http://kg.panjiajie.cn

Ruby: return if data.nil?
来源：http://im.huanxung.cn

C#:   if (data == null) return;
来源：http://ud.panjiajie.cn

================================================================================
来源：http://bc.9csxet.cn

C. 函数与作用域
来源：http://qj.shxzskj.cn

================================================================================
来源：http://pe.colortex.cn

[C01] 定义函数
来源：http://wd.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://dc.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cw.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://ux.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cy.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ar.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ph.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://pd.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://an.hnjuh.cn

[C02] 默认参数
来源：http://tl.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://yw.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bx.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://ef.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nm.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zo.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yy.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://sa.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://vu.szsharing.cn

[C03] 可变参数
来源：http://nt.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://ex.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jq.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wn.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ly.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ad.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hd.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mq.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ir.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://fv.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cg.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ig.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qg.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yz.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://iy.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://cn.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://zz.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://jk.bjjhwx.cn

[C05] 返回多个值
来源：http://cu.colortex.cn

Py:   return a, b
来源：http://ms.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://ns.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zj.huixinmuqiang.cn

TS:   return { a, b };
来源：http://vf.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qd.yuntaijiaju.cn

Go:   return a, b
来源：http://el.chemitech.net.cn

Ruby: return a, b
来源：http://pn.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://gj.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://rg.colortex.cn

Py:   square = lambda x: x * x
来源：http://tq.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jg.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://jd.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://bx.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://du.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hi.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://xy.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hp.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://cg.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sv.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://al.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bh.huixiangedu.cn

TS:   arr.map(String)
来源：http://wz.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sd.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vy.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://bo.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bq.szxytkj.cn

[C08] 闭包
来源：http://fk.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ta.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://an.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sm.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mm.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://es.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zw.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lo.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mj.521024.cn

[C09] 递归
来源：http://pz.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hw.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jt.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://od.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qj.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://na.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ge.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ze.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ap.yuexingan06.cn

[C10] 变量作用域
来源：http://eh.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://on.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kw.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ik.muxihuayi.cn

TS:   同 JS
来源：http://pd.521024.cn

Java: 方法内为块级作用域
来源：http://nl.shxzukj.cn

Go:   花括号块级作用域
来源：http://xu.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pl.szsharing.cn

C#:   块级作用域
来源：http://cp.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://jq.newstarts.cn

Py:   from module import func
来源：http://cd.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://je.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zw.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xc.huixiangedu.cn

Java: import java.util.List;
来源：http://gv.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vk.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://ea.colortex.cn

C#:   using System.Text;
来源：http://hs.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://ud.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://af.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://wn.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://my.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://te.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zs.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://vx.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://ph.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://np.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://xo.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lk.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cu.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://df.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xi.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pl.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://wh.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pr.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tq.szsharing.cn

[C14] 泛型函数
来源：http://oz.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vx.yuexingan06.cn

PHP:  // 无泛型
来源：http://hz.huanxung.cn

JS:   // 无泛型
来源：http://ks.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vq.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ss.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uk.shtwfgs.cn

Ruby: # 无泛型
来源：http://ph.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vn.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://sd.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://au.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://dn.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mp.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rh.lnxyls.cn

Java: // 无解构
来源：http://jg.shtwfgs.cn

Go:   // 无解构
来源：http://nc.huanxung.cn

Ruby: a, b = pair
来源：http://pw.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://yz.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://xl.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ul.hahajie.cn

PHP:  // 无重载
来源：http://zn.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sj.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://mc.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pe.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://mm.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://rz.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jh.nicolike.cn

================================================================================
来源：http://se.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://yo.muxihuayi.cn

================================================================================
来源：http://jq.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://kk.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mb.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ix.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bi.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gc.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ht.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ve.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://va.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://th.gzmigu.cn

[D02] 追加元素到末尾
来源：http://tq.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ye.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ul.newstarts.cn

JS:   arr.push(4);
来源：http://za.huixiangedu.cn

TS:   arr.push(4);
来源：http://gs.yuntaijiaju.cn

Java: list.add(4);
来源：http://kg.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://zz.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://ui.521024.cn

C#:   list.Add(4);
来源：http://qm.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://qm.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://hz.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nl.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ub.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://dn.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://em.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://td.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ux.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://qk.chemitech.net.cn

[D04] 删除元素
来源：http://vu.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bd.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tn.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pw.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://uw.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qn.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ks.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ei.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://le.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://re.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wo.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ch.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gj.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://bx.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://si.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://lb.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://if.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kj.nicolike.cn

[D06] 数组长度
来源：http://zm.bjjhwx.cn

Py:   len(arr)
来源：http://hp.lnxyls.cn

PHP:  count($arr);
来源：http://bq.bjjhwx.cn

JS:   arr.length
来源：http://pv.colortex.cn

TS:   arr.length
来源：http://qh.nicolike.cn

Java: list.size();
来源：http://xe.nszjky.cn

Go:   len(arr)
来源：http://eu.521024.cn

Ruby: arr.length; arr.size
来源：http://nl.huixinmuqiang.cn

C#:   list.Count;
来源：http://kk.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://pu.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yl.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ow.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://ah.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://zu.9csxet.cn

Java: list.subList(1, 4);
来源：http://yg.gzmigu.cn

Go:   arr[1:4]
来源：http://dd.lnxyls.cn

Ruby: arr[1, 3]
来源：http://ge.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://ax.muxihuayi.cn

[D08] 合并两个数组
来源：http://ek.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://jt.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://ms.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://he.nszjky.cn

TS:   [...a, ...b];
来源：http://uf.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sx.panjiajie.cn

Go:   append(a, b...)
来源：http://gl.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://ay.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://lz.gzmigu.cn

[D09] 排序（升序）
来源：http://wj.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ae.huixiangedu.cn

PHP:  sort($arr);
来源：http://ed.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fm.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kd.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hc.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zr.hnjuh.cn

Ruby: arr.sort
来源：http://ly.colortex.cn

C#:   list.Sort();
来源：http://qd.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ad.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rg.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qh.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oj.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hd.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rq.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dx.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cx.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fs.huixiangedu.cn

[D11] 反转数组
来源：http://uc.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ww.asd995.cn

PHP:  array_reverse($arr);
来源：http://bj.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://au.521024.cn

TS:   [...arr].reverse();
来源：http://gx.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://jv.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://dx.huanxung.cn

Ruby: arr.reverse
来源：http://hn.bjjhwx.cn


<!-- 参考信息 -->