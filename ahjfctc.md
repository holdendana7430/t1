代发 wailian999

C#:   x is int or double or decimal
来源：http://fu.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://co.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ng.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jf.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://jy.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://qh.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ov.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rx.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nl.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ul.nszjky.cn

[B15] 布尔运算与取反
来源：http://rm.huixinmuqiang.cn

Py:   a and b or not c
来源：http://dq.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://ed.nicolike.cn

JS:   a && b || !c
来源：http://xn.bjjhwx.cn

TS:   a && b || !c
来源：http://yb.bookmarksfly.cn

Java: a && b || !c
来源：http://qb.wgjwhj.cn

Go:   a && b || !c
来源：http://ea.szxytkj.cn

Ruby: a && b || !c
来源：http://uw.haigaiapp.cn

C#:   a && b || !c
来源：http://st.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jq.szxytkj.cn

Py:   if not data: return
来源：http://dh.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://bb.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://sd.szsharing.cn

TS:   if (!data) return;
来源：http://qs.bookmarksfly.cn

Java: if (data == null) return;
来源：http://fr.hnjuh.cn

Go:   if data == nil { return }
来源：http://ak.szxytkj.cn

Ruby: return if data.nil?
来源：http://en.asd995.cn

C#:   if (data == null) return;
来源：http://ey.yuntaijiaju.cn

================================================================================
来源：http://ku.bjjhwx.cn

C. 函数与作用域
来源：http://gq.bjjhwx.cn

================================================================================
来源：http://wj.huixinmuqiang.cn

[C01] 定义函数
来源：http://ng.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://wc.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ci.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://xd.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ww.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://et.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rz.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://cd.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vp.asd995.cn

[C02] 默认参数
来源：http://qs.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://wa.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://si.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://px.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tc.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zk.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ch.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://et.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://wg.yuntaijiaju.cn

[C03] 可变参数
来源：http://cl.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://gv.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sp.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eg.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xr.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qy.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nu.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uj.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lp.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://qx.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jc.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wj.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wh.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kh.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://un.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://xe.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://in.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://kt.huixinmuqiang.cn

[C05] 返回多个值
来源：http://dc.yuexingan06.cn

Py:   return a, b
来源：http://bw.nicolike.cn

PHP:  return [$a, $b];
来源：http://db.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ut.shxzukj.cn

TS:   return { a, b };
来源：http://uu.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cx.panjiajie.cn

Go:   return a, b
来源：http://dp.asd995.cn

Ruby: return a, b
来源：http://ui.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://hc.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://bo.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://bi.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ky.colortex.cn

JS:   const square = x => x * x;
来源：http://ge.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://xq.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yu.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tg.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://we.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://br.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://db.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ch.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wl.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ik.yuexingan06.cn

TS:   arr.map(String)
来源：http://mr.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ag.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mq.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://qt.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oa.muxihuayi.cn

[C08] 闭包
来源：http://ca.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qq.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gb.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hl.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lw.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://da.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oq.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://po.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mx.hahajie.cn

[C09] 递归
来源：http://js.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dp.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ns.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jq.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fy.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xf.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kf.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sm.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qx.hahajie.cn

[C10] 变量作用域
来源：http://bh.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://av.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ui.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dj.lnxyls.cn

TS:   同 JS
来源：http://ml.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ex.shxzukj.cn

Go:   花括号块级作用域
来源：http://rc.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qk.gzmigu.cn

C#:   块级作用域
来源：http://et.bjjhwx.cn

[C11] 模块导入与导出
来源：http://ps.szxytkj.cn

Py:   from module import func
来源：http://kn.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kv.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zo.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qs.hahajie.cn

Java: import java.util.List;
来源：http://pw.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rx.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://bd.gzmigu.cn

C#:   using System.Text;
来源：http://xu.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://vp.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://jz.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://fi.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://pc.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://hx.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qq.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://ez.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://mp.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ru.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://mg.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ry.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ky.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://le.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lk.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zu.521024.cn

Go:   func add(a, b int) int
来源：http://ju.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nl.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://no.asd995.cn

[C14] 泛型函数
来源：http://pl.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kn.newstarts.cn

PHP:  // 无泛型
来源：http://sw.nicolike.cn

JS:   // 无泛型
来源：http://xv.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yr.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ot.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dq.colortex.cn

Ruby: # 无泛型
来源：http://qp.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zg.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://ap.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pl.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://nx.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://he.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pf.newstarts.cn

Java: // 无解构
来源：http://mc.chemitech.net.cn

Go:   // 无解构
来源：http://px.wgjwhj.cn

Ruby: a, b = pair
来源：http://eg.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://nr.nszjky.cn

[C16] 函数 / 方法重载
来源：http://tm.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jt.bookmarksfly.cn

PHP:  // 无重载
来源：http://zh.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wm.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://rz.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yy.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://ev.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://dk.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yy.9csxet.cn

================================================================================
来源：http://mx.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://jl.chemitech.net.cn

================================================================================
来源：http://cg.9csxet.cn

[D01] 创建数组 / 列表
来源：http://mv.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wa.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sn.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qa.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://up.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bb.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://rp.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://st.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yd.gzmigu.cn

[D02] 追加元素到末尾
来源：http://eb.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gn.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ee.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://aa.asd995.cn

TS:   arr.push(4);
来源：http://bn.nicolike.cn

Java: list.add(4);
来源：http://ck.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://mb.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://kq.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://gy.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://ab.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://de.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ru.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fe.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://ej.nicolike.cn

Java: list.add(0, 0);
来源：http://ir.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pz.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hp.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://lp.haigaiapp.cn

[D04] 删除元素
来源：http://io.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://np.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qb.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pi.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://vi.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gb.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bs.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eh.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bn.shxzskj.cn

[D05] 访问与修改元素
来源：http://ib.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nt.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sc.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eq.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://pt.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://uz.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://rf.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ee.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sj.nszjky.cn

[D06] 数组长度
来源：http://nz.nszjky.cn

Py:   len(arr)
来源：http://vr.nszjky.cn

PHP:  count($arr);
来源：http://hi.yuexingan06.cn

JS:   arr.length
来源：http://kw.yuexingan06.cn

TS:   arr.length
来源：http://nf.muxihuayi.cn

Java: list.size();
来源：http://sh.chemitech.net.cn

Go:   len(arr)
来源：http://hu.nszjky.cn

Ruby: arr.length; arr.size
来源：http://eq.shxzskj.cn

C#:   list.Count;
来源：http://wh.9csxet.cn

[D07] 切片 / 取子数组
来源：http://cg.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hw.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bq.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://td.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://gx.asd995.cn

Java: list.subList(1, 4);
来源：http://tr.panjiajie.cn

Go:   arr[1:4]
来源：http://ul.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://vk.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://qg.yuexingan06.cn

[D08] 合并两个数组
来源：http://oe.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://bw.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://kt.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jc.nicolike.cn

TS:   [...a, ...b];
来源：http://pl.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jg.muxihuayi.cn

Go:   append(a, b...)
来源：http://al.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://nf.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://fy.muxihuayi.cn

[D09] 排序（升序）
来源：http://pc.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://dd.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://yq.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fk.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lp.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fr.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://og.jctech888.com.cn

Ruby: arr.sort
来源：http://cc.hnjuh.cn

C#:   list.Sort();
来源：http://cx.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hg.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qx.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lq.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dt.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jt.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bt.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bu.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mi.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lm.lnxyls.cn

[D11] 反转数组
来源：http://ia.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wa.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://an.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sw.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://uw.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://ex.asd995.cn

Go:   slices.Reverse(arr)
来源：http://po.shxzskj.cn

Ruby: arr.reverse
来源：http://pi.asd995.cn

C#:   list.Reverse();
来源：http://rt.shxzukj.cn

[D12] 查找元素下标
来源：http://zj.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://tn.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fs.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hs.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mn.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kz.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://nv.gzmigu.cn

Ruby: arr.index(x)
来源：http://pw.nszjky.cn

C#:   list.IndexOf(x);
来源：http://wo.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://lr.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zp.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://so.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://gw.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://vp.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hc.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bo.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wo.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dp.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://cr.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sw.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kh.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://up.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://qd.jianghongdianzi.cn


<!-- 参考信息 -->