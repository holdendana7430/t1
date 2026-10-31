代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://rk.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://uz.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gr.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kp.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bc.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oo.nicolike.cn

[B15] 布尔运算与取反
来源：http://oh.nicolike.cn

Py:   a and b or not c
来源：http://dv.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://dq.chemitech.net.cn

JS:   a && b || !c
来源：http://dh.shxzukj.cn

TS:   a && b || !c
来源：http://sv.shxzskj.cn

Java: a && b || !c
来源：http://ti.shxzukj.cn

Go:   a && b || !c
来源：http://fu.newstarts.cn

Ruby: a && b || !c
来源：http://ju.521024.cn

C#:   a && b || !c
来源：http://gf.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ej.gzmigu.cn

Py:   if not data: return
来源：http://cb.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://cw.bookmarksfly.cn

JS:   if (!data) return;
来源：http://ki.hnjuh.cn

TS:   if (!data) return;
来源：http://ij.lnxyls.cn

Java: if (data == null) return;
来源：http://du.shtwfgs.cn

Go:   if data == nil { return }
来源：http://fv.haigaiapp.cn

Ruby: return if data.nil?
来源：http://vb.hnjuh.cn

C#:   if (data == null) return;
来源：http://jr.shxzukj.cn

================================================================================
来源：http://sr.chemitech.net.cn

C. 函数与作用域
来源：http://jm.gzmigu.cn

================================================================================
来源：http://ch.bookmarksfly.cn

[C01] 定义函数
来源：http://dh.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://eq.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://et.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://if.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hd.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qv.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yx.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://ez.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ze.jianghongdianzi.cn

[C02] 默认参数
来源：http://yy.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://cv.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vz.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://ke.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://if.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://in.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ya.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://dt.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://hk.hnjuh.cn

[C03] 可变参数
来源：http://mt.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://ef.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pr.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ni.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ga.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uj.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cn.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://es.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ir.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://kw.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://un.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zt.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cx.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vh.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://cw.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://ro.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://pk.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://um.szxytkj.cn

[C05] 返回多个值
来源：http://ii.shxzskj.cn

Py:   return a, b
来源：http://ax.nszjky.cn

PHP:  return [$a, $b];
来源：http://vf.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yx.shxzskj.cn

TS:   return { a, b };
来源：http://rf.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dv.panjiajie.cn

Go:   return a, b
来源：http://yg.huanxung.cn

Ruby: return a, b
来源：http://ai.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://zq.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://ew.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://lu.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mf.9csxet.cn

JS:   const square = x => x * x;
来源：http://ua.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://nb.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bj.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cz.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://zo.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lj.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://ng.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://er.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pr.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ml.huixiangedu.cn

TS:   arr.map(String)
来源：http://pi.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rv.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gw.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://yc.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ea.muxihuayi.cn

[C08] 闭包
来源：http://yx.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hf.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pv.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mh.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dj.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nz.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yu.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mo.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hl.chemitech.net.cn

[C09] 递归
来源：http://ky.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wa.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://by.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qj.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gs.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pf.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gn.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xe.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uw.bjjhwx.cn

[C10] 变量作用域
来源：http://ky.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kk.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dk.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dv.gzmigu.cn

TS:   同 JS
来源：http://ho.9csxet.cn

Java: 方法内为块级作用域
来源：http://pj.haigaiapp.cn

Go:   花括号块级作用域
来源：http://wn.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wu.shtwfgs.cn

C#:   块级作用域
来源：http://mx.newstarts.cn

[C11] 模块导入与导出
来源：http://sz.huanxung.cn

Py:   from module import func
来源：http://qv.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xj.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sg.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tf.jianghongdianzi.cn

Java: import java.util.List;
来源：http://fo.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sg.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://ty.nicolike.cn

C#:   using System.Text;
来源：http://ao.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://gd.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://by.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://rz.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://qq.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://hl.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qm.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://pi.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://yp.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ra.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://ji.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bd.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ky.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ln.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zl.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ny.hnjuh.cn

Go:   func add(a, b int) int
来源：http://bq.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hv.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mr.szsharing.cn

[C14] 泛型函数
来源：http://wo.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zx.colortex.cn

PHP:  // 无泛型
来源：http://fp.yuexingan06.cn

JS:   // 无泛型
来源：http://cc.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://je.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tu.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ib.colortex.cn

Ruby: # 无泛型
来源：http://rc.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ya.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://lw.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lt.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://rz.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sc.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ky.yuexingan06.cn

Java: // 无解构
来源：http://ep.huanxung.cn

Go:   // 无解构
来源：http://by.szxytkj.cn

Ruby: a, b = pair
来源：http://hx.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://iq.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://ug.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wq.muxihuayi.cn

PHP:  // 无重载
来源：http://yz.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fu.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://qs.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hh.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://rx.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://io.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://op.huixiangedu.cn

================================================================================
来源：http://zm.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://lr.bookmarksfly.cn

================================================================================
来源：http://kh.521024.cn

[D01] 创建数组 / 列表
来源：http://yp.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://py.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mm.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dm.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uc.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nx.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://zf.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://hj.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ok.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://lx.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wl.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://re.szxytkj.cn

JS:   arr.push(4);
来源：http://fc.bjjhwx.cn

TS:   arr.push(4);
来源：http://ql.szsharing.cn

Java: list.add(4);
来源：http://pc.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://aq.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://mr.haigaiapp.cn

C#:   list.Add(4);
来源：http://ar.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://sf.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://mr.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ot.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ov.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://tp.huanxung.cn

Java: list.add(0, 0);
来源：http://st.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ch.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://td.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://lu.shtwfgs.cn

[D04] 删除元素
来源：http://pb.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fy.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pr.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://db.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://fk.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bd.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ep.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fi.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lu.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://ic.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oi.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iy.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bn.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://cl.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ss.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://bi.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cs.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rt.haigaiapp.cn

[D06] 数组长度
来源：http://qy.nicolike.cn

Py:   len(arr)
来源：http://cu.shtwfgs.cn

PHP:  count($arr);
来源：http://pf.yuexingan06.cn

JS:   arr.length
来源：http://fx.shxzukj.cn

TS:   arr.length
来源：http://fn.huixinmuqiang.cn

Java: list.size();
来源：http://rk.haigaiapp.cn

Go:   len(arr)
来源：http://wf.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://ay.colortex.cn

C#:   list.Count;
来源：http://qc.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://kh.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qq.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wa.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://uc.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://np.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://wx.9csxet.cn

Go:   arr[1:4]
来源：http://fp.szxytkj.cn

Ruby: arr[1, 3]
来源：http://su.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://wn.szsharing.cn

[D08] 合并两个数组
来源：http://ew.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://tw.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://od.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xm.lnxyls.cn

TS:   [...a, ...b];
来源：http://mr.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nx.jctech888.com.cn

Go:   append(a, b...)
来源：http://ou.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://dx.521024.cn

C#:   a.Concat(b).ToList()
来源：http://xu.wgjwhj.cn

[D09] 排序（升序）
来源：http://ta.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://ah.shxzukj.cn

PHP:  sort($arr);
来源：http://mt.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fx.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kh.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fo.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://na.yuntaijiaju.cn

Ruby: arr.sort
来源：http://zo.shxzukj.cn

C#:   list.Sort();
来源：http://ep.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ma.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://li.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ni.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ft.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ux.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pw.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eg.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qk.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tc.muxihuayi.cn

[D11] 反转数组
来源：http://ay.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xq.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://gy.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://do.huanxung.cn

TS:   [...arr].reverse();
来源：http://nk.newstarts.cn

Java: Collections.reverse(list);
来源：http://bj.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://ps.szsharing.cn

Ruby: arr.reverse
来源：http://gt.hnjuh.cn

C#:   list.Reverse();
来源：http://ob.521024.cn

[D12] 查找元素下标
来源：http://ir.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://hi.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pk.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dn.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://am.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kn.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://ui.shxzskj.cn

Ruby: arr.index(x)
来源：http://gh.521024.cn

C#:   list.IndexOf(x);
来源：http://nb.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://jy.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fi.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://or.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://ml.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://na.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bx.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jq.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jk.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tl.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://qe.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oa.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zf.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://bq.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://wj.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tv.huanxung.cn

Go:   // 手写循环
来源：http://et.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yh.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sx.jctech888.com.cn


<!-- 参考信息 -->