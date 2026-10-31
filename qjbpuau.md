代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ur.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xd.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://ci.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://mp.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://ro.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ea.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://po.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://se.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jq.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://wd.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yi.szsharing.cn

[B12] 跳出多层循环
来源：http://gr.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rj.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ee.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://te.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ca.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xt.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wb.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zm.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jk.hahajie.cn

[B13] 判断是否为数字
来源：http://ji.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://bg.szsharing.cn

PHP:  is_numeric($x)
来源：http://nv.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ov.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fy.huixiangedu.cn

Java: x instanceof Number
来源：http://sc.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bh.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://na.panjiajie.cn

C#:   x is int or double or decimal
来源：http://fz.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://ek.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://th.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://in.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://de.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://wy.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ml.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ly.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iz.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tx.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://fn.shxzskj.cn

Py:   a and b or not c
来源：http://iy.521024.cn

PHP:  $a && $b || !$c
来源：http://qm.shtwfgs.cn

JS:   a && b || !c
来源：http://ls.asd995.cn

TS:   a && b || !c
来源：http://ow.asd995.cn

Java: a && b || !c
来源：http://iy.hahajie.cn

Go:   a && b || !c
来源：http://xt.shtwfgs.cn

Ruby: a && b || !c
来源：http://ko.bjjhwx.cn

C#:   a && b || !c
来源：http://az.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://du.nicolike.cn

Py:   if not data: return
来源：http://xl.asd995.cn

PHP:  if (!$data) { return; }
来源：http://xr.wgjwhj.cn

JS:   if (!data) return;
来源：http://rw.shxzukj.cn

TS:   if (!data) return;
来源：http://kl.nicolike.cn

Java: if (data == null) return;
来源：http://hj.huanxung.cn

Go:   if data == nil { return }
来源：http://ph.9csxet.cn

Ruby: return if data.nil?
来源：http://bf.asd995.cn

C#:   if (data == null) return;
来源：http://gs.9csxet.cn

================================================================================
来源：http://xy.shtwfgs.cn

C. 函数与作用域
来源：http://js.chemitech.net.cn

================================================================================
来源：http://eu.gzmigu.cn

[C01] 定义函数
来源：http://nv.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://xq.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mj.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ls.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zc.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gn.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rn.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://un.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://be.bjjhwx.cn

[C02] 默认参数
来源：http://bo.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://cl.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yh.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://ar.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dh.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mp.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://es.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://pn.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://bk.szxytkj.cn

[C03] 可变参数
来源：http://ze.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://xg.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uz.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hi.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gr.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nu.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ok.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yu.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cb.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://rt.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ao.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uv.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ha.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xt.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://gn.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://bp.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://no.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://dy.lnxyls.cn

[C05] 返回多个值
来源：http://ua.newstarts.cn

Py:   return a, b
来源：http://oo.gzmigu.cn

PHP:  return [$a, $b];
来源：http://ta.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uf.huixiangedu.cn

TS:   return { a, b };
来源：http://cv.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cn.9csxet.cn

Go:   return a, b
来源：http://hs.521024.cn

Ruby: return a, b
来源：http://cv.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://yd.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://ik.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://xp.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yl.521024.cn

JS:   const square = x => x * x;
来源：http://dg.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://ac.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cu.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rw.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://lr.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vb.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://cq.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gv.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zr.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yz.szsharing.cn

TS:   arr.map(String)
来源：http://cg.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dq.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tz.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://ps.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nh.521024.cn

[C08] 闭包
来源：http://oi.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://co.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ew.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zm.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rk.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://en.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gm.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ld.jctech888.com.cn

[C09] 递归
来源：http://oc.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tb.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pc.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pn.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dh.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fv.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://be.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fz.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yq.yuntaijiaju.cn

[C10] 变量作用域
来源：http://ym.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dv.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tp.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mo.shtwfgs.cn

TS:   同 JS
来源：http://vw.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://ht.szxytkj.cn

Go:   花括号块级作用域
来源：http://xu.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ry.hahajie.cn

C#:   块级作用域
来源：http://kf.panjiajie.cn

[C11] 模块导入与导出
来源：http://rr.gzmigu.cn

Py:   from module import func
来源：http://im.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gr.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dz.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kc.szsharing.cn

Java: import java.util.List;
来源：http://lw.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zv.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://fb.huanxung.cn

C#:   using System.Text;
来源：http://fl.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://ex.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://vc.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://jn.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://pq.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://xm.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oz.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://do.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://ii.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fc.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://qx.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xx.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jo.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wg.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yo.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tk.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://gi.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://md.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mc.yuexingan06.cn

[C14] 泛型函数
来源：http://ei.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ym.szsharing.cn

PHP:  // 无泛型
来源：http://wd.huanxung.cn

JS:   // 无泛型
来源：http://pg.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vz.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ha.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hn.hnjuh.cn

Ruby: # 无泛型
来源：http://nd.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gw.huanxung.cn

[C15] 解构 / 展开参数
来源：http://hf.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fw.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://jb.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rh.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hm.bjjhwx.cn

Java: // 无解构
来源：http://we.yuntaijiaju.cn

Go:   // 无解构
来源：http://dw.nszjky.cn

Ruby: a, b = pair
来源：http://ni.9csxet.cn

C#:   var (a, b) = pair;
来源：http://gm.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://vl.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ig.bookmarksfly.cn

PHP:  // 无重载
来源：http://hb.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://av.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://ux.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nb.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://ll.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://ln.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xr.haigaiapp.cn

================================================================================
来源：http://zm.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://qf.yuexingan06.cn

================================================================================
来源：http://vz.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://lp.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bh.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jc.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hb.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wy.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zi.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://hw.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ea.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sd.newstarts.cn

[D02] 追加元素到末尾
来源：http://pj.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ak.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lf.huixiangedu.cn

JS:   arr.push(4);
来源：http://pa.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://wt.chemitech.net.cn

Java: list.add(4);
来源：http://vq.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://qq.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://di.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://tj.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://cb.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://dq.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://re.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qs.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://km.szsharing.cn

Java: list.add(0, 0);
来源：http://dn.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lb.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://co.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://qi.huixinmuqiang.cn

[D04] 删除元素
来源：http://uu.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dv.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nh.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yc.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://rr.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ef.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sp.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ot.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xl.haigaiapp.cn

[D05] 访问与修改元素
来源：http://lx.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://os.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vf.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mi.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://cf.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://ds.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://yt.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ex.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tk.bookmarksfly.cn

[D06] 数组长度
来源：http://zl.jctech888.com.cn

Py:   len(arr)
来源：http://ih.chemitech.net.cn

PHP:  count($arr);
来源：http://rn.huanxung.cn

JS:   arr.length
来源：http://jm.nszjky.cn

TS:   arr.length
来源：http://og.haigaiapp.cn

Java: list.size();
来源：http://fq.hahajie.cn

Go:   len(arr)
来源：http://ig.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://ne.shxzskj.cn

C#:   list.Count;
来源：http://dr.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://du.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://al.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ro.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://zl.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://qp.panjiajie.cn

Java: list.subList(1, 4);
来源：http://xb.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://qk.colortex.cn

Ruby: arr[1, 3]
来源：http://ct.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://tk.nszjky.cn

[D08] 合并两个数组
来源：http://dy.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://bb.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://rw.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fy.nszjky.cn

TS:   [...a, ...b];
来源：http://gy.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fz.wgjwhj.cn

Go:   append(a, b...)
来源：http://zf.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://xk.521024.cn

C#:   a.Concat(b).ToList()
来源：http://vn.asd995.cn

[D09] 排序（升序）
来源：http://fg.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://xk.colortex.cn

PHP:  sort($arr);
来源：http://gh.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://id.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wl.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mq.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hg.szxytkj.cn

Ruby: arr.sort
来源：http://lv.yuexingan06.cn

C#:   list.Sort();
来源：http://la.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bp.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://km.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jz.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oj.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kf.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ec.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://in.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ea.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gx.nicolike.cn

[D11] 反转数组
来源：http://nq.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fx.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://zs.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lq.colortex.cn


<!-- 参考信息 -->