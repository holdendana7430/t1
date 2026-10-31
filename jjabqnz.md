代发 wailian999

C#:   x is int or double or decimal
来源：http://dr.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://rc.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qj.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://we.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://xw.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://ao.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zf.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tq.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kl.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vi.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://ou.huanxung.cn

Py:   a and b or not c
来源：http://xj.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://by.9csxet.cn

JS:   a && b || !c
来源：http://mc.asd995.cn

TS:   a && b || !c
来源：http://af.jctech888.com.cn

Java: a && b || !c
来源：http://sn.bjjhwx.cn

Go:   a && b || !c
来源：http://qc.521024.cn

Ruby: a && b || !c
来源：http://xr.asd995.cn

C#:   a && b || !c
来源：http://im.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kf.huixinmuqiang.cn

Py:   if not data: return
来源：http://az.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://ef.colortex.cn

JS:   if (!data) return;
来源：http://pp.newstarts.cn

TS:   if (!data) return;
来源：http://jl.huanxung.cn

Java: if (data == null) return;
来源：http://pv.9csxet.cn

Go:   if data == nil { return }
来源：http://sf.colortex.cn

Ruby: return if data.nil?
来源：http://iy.521024.cn

C#:   if (data == null) return;
来源：http://wc.szsharing.cn

================================================================================
来源：http://mg.huanxung.cn

C. 函数与作用域
来源：http://wb.nicolike.cn

================================================================================
来源：http://uq.chemitech.net.cn

[C01] 定义函数
来源：http://bk.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://cx.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ke.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://pq.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nm.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xn.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bl.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://bm.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://so.nicolike.cn

[C02] 默认参数
来源：http://uq.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://di.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://do.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ex.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fw.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nk.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rr.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://dd.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://zu.lnxyls.cn

[C03] 可变参数
来源：http://ds.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://ub.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ej.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ly.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qd.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kb.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gz.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bf.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ur.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://wj.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vs.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vb.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://do.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ru.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://in.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://sr.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://nm.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://cw.nicolike.cn

[C05] 返回多个值
来源：http://nc.bookmarksfly.cn

Py:   return a, b
来源：http://wn.huanxung.cn

PHP:  return [$a, $b];
来源：http://tu.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ay.haigaiapp.cn

TS:   return { a, b };
来源：http://zx.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wm.asd995.cn

Go:   return a, b
来源：http://hi.huixinmuqiang.cn

Ruby: return a, b
来源：http://is.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://jd.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://tv.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://zg.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qg.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://bv.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://ej.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ew.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oq.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://pk.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ud.asd995.cn

[C07] 把函数作为参数传入
来源：http://bq.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kf.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://he.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uv.wgjwhj.cn

TS:   arr.map(String)
来源：http://pw.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rc.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ay.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://kk.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tc.lnxyls.cn

[C08] 闭包
来源：http://jo.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zu.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rr.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://li.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xr.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wz.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qh.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sz.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ex.hahajie.cn

[C09] 递归
来源：http://xb.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rg.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ue.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://la.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zz.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://px.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lj.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bz.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tu.nszjky.cn

[C10] 变量作用域
来源：http://ea.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uz.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vq.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bo.hahajie.cn

TS:   同 JS
来源：http://cm.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://hz.shxzskj.cn

Go:   花括号块级作用域
来源：http://ke.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wz.huixinmuqiang.cn

C#:   块级作用域
来源：http://pt.jctech888.com.cn

[C11] 模块导入与导出
来源：http://dd.9csxet.cn

Py:   from module import func
来源：http://it.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oh.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://od.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nk.wgjwhj.cn

Java: import java.util.List;
来源：http://nr.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ea.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://bl.shxzskj.cn

C#:   using System.Text;
来源：http://vh.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://ya.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://mx.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://vx.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://bh.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://de.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ou.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://rh.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://qi.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vd.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://nx.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jy.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ho.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mg.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ic.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://ha.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://we.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ie.panjiajie.cn

[C14] 泛型函数
来源：http://ba.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ye.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://sd.szsharing.cn

JS:   // 无泛型
来源：http://zk.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ll.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://of.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wy.bjjhwx.cn

Ruby: # 无泛型
来源：http://qp.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zf.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://sr.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cw.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://re.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hj.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ml.panjiajie.cn

Java: // 无解构
来源：http://pk.muxihuayi.cn

Go:   // 无解构
来源：http://gz.jctech888.com.cn

Ruby: a, b = pair
来源：http://qd.asd995.cn

C#:   var (a, b) = pair;
来源：http://dm.szsharing.cn

[C16] 函数 / 方法重载
来源：http://zh.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ca.lnxyls.cn

PHP:  // 无重载
来源：http://yo.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rh.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://df.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uw.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://qr.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://ks.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cl.lnxyls.cn

================================================================================
来源：http://te.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://fc.yuexingan06.cn

================================================================================
来源：http://ix.hahajie.cn

[D01] 创建数组 / 列表
来源：http://io.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yu.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vo.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yj.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fv.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hf.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://qy.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://nx.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zv.huanxung.cn

[D02] 追加元素到末尾
来源：http://ye.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kc.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rl.lnxyls.cn

JS:   arr.push(4);
来源：http://mt.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://kd.jctech888.com.cn

Java: list.add(4);
来源：http://ji.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ij.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://bk.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://lj.huanxung.cn

[D03] 在指定位置插入元素
来源：http://bv.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://zs.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sd.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jf.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://vf.shtwfgs.cn

Java: list.add(0, 0);
来源：http://yn.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ob.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yh.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://ik.wgjwhj.cn

[D04] 删除元素
来源：http://xx.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bf.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ck.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ml.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://qo.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nk.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pn.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hm.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qk.hnjuh.cn

[D05] 访问与修改元素
来源：http://tq.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hk.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ax.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eg.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://ll.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://id.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://ns.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aw.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ut.shtwfgs.cn

[D06] 数组长度
来源：http://vp.gzmigu.cn

Py:   len(arr)
来源：http://by.szsharing.cn

PHP:  count($arr);
来源：http://qx.bjjhwx.cn

JS:   arr.length
来源：http://kd.jianghongdianzi.cn

TS:   arr.length
来源：http://hk.chemitech.net.cn

Java: list.size();
来源：http://kc.szsharing.cn

Go:   len(arr)
来源：http://sn.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://jm.jctech888.com.cn

C#:   list.Count;
来源：http://gk.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://ga.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bf.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xs.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://ln.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://jo.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://jr.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://hk.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://un.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://em.bookmarksfly.cn

[D08] 合并两个数组
来源：http://ef.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://fi.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://rg.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ip.shxzukj.cn

TS:   [...a, ...b];
来源：http://ow.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://la.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://xj.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://ue.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://jj.9csxet.cn

[D09] 排序（升序）
来源：http://ts.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://vt.bookmarksfly.cn

PHP:  sort($arr);
来源：http://hr.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kk.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vo.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sz.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mx.gzmigu.cn

Ruby: arr.sort
来源：http://rd.newstarts.cn

C#:   list.Sort();
来源：http://pu.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pk.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dp.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wz.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://px.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wv.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lq.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vp.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vm.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uq.chemitech.net.cn

[D11] 反转数组
来源：http://js.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ce.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://rs.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sn.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://vl.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://aq.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://qe.wgjwhj.cn

Ruby: arr.reverse
来源：http://db.521024.cn

C#:   list.Reverse();
来源：http://be.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://ub.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://aa.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gr.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pl.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gl.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ft.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://hn.chemitech.net.cn

Ruby: arr.index(x)
来源：http://ar.nszjky.cn

C#:   list.IndexOf(x);
来源：http://jp.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://vs.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jm.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zc.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://ex.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://br.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yg.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ll.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://an.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uo.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://vr.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uf.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ij.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://nl.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://lk.szxytkj.cn


<!-- 参考信息 -->