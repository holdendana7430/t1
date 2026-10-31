代发 wailian999

Java: if (data == null) return;
来源：http://wt.huanxung.cn

Go:   if data == nil { return }
来源：http://xv.yuexingan06.cn

Ruby: return if data.nil?
来源：http://rp.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://kp.hahajie.cn

================================================================================
来源：http://rp.9csxet.cn

C. 函数与作用域
来源：http://zh.bjjhwx.cn

================================================================================
来源：http://qu.9csxet.cn

[C01] 定义函数
来源：http://fi.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://vj.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gt.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://ri.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yz.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qs.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://et.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://zx.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jh.shxzskj.cn

[C02] 默认参数
来源：http://mi.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://he.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fi.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://hw.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dy.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hj.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nk.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://vu.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://dq.szsharing.cn

[C03] 可变参数
来源：http://qh.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://kp.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yf.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wm.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mu.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ap.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qj.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zi.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wc.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ru.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oy.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ok.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ad.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zw.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://od.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://od.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://qn.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://rz.huixinmuqiang.cn

[C05] 返回多个值
来源：http://gs.huanxung.cn

Py:   return a, b
来源：http://wi.gzmigu.cn

PHP:  return [$a, $b];
来源：http://tn.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dw.yuntaijiaju.cn

TS:   return { a, b };
来源：http://fb.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zj.asd995.cn

Go:   return a, b
来源：http://zk.521024.cn

Ruby: return a, b
来源：http://pc.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://xw.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://gk.hahajie.cn

Py:   square = lambda x: x * x
来源：http://yl.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pi.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://gy.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://is.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qh.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dx.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://al.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hw.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://ul.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ae.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mh.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tu.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://lf.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pu.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ed.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://ym.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://aw.huanxung.cn

[C08] 闭包
来源：http://gy.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rk.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vs.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mp.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ov.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xu.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fg.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gs.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mg.colortex.cn

[C09] 递归
来源：http://yr.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rz.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gj.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uo.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eb.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dx.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dc.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ro.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hc.newstarts.cn

[C10] 变量作用域
来源：http://lp.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ym.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nr.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nq.hnjuh.cn

TS:   同 JS
来源：http://oy.colortex.cn

Java: 方法内为块级作用域
来源：http://gb.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://cp.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nm.gzmigu.cn

C#:   块级作用域
来源：http://vw.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://wt.jctech888.com.cn

Py:   from module import func
来源：http://xh.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bo.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://so.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cj.nicolike.cn

Java: import java.util.List;
来源：http://wz.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xx.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://hz.huanxung.cn

C#:   using System.Text;
来源：http://fx.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://qa.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://nn.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://ml.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://td.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ts.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lq.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://ia.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://zd.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ga.521024.cn

[C13] 类型声明 / 类型注解
来源：http://rw.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jv.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pb.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fn.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wf.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qh.szxytkj.cn

Go:   func add(a, b int) int
来源：http://qf.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wy.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ho.bookmarksfly.cn

[C14] 泛型函数
来源：http://ud.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gz.521024.cn

PHP:  // 无泛型
来源：http://ip.9csxet.cn

JS:   // 无泛型
来源：http://br.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://no.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sl.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ly.hnjuh.cn

Ruby: # 无泛型
来源：http://cg.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bv.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://yw.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tq.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://qp.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xc.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gb.huixinmuqiang.cn

Java: // 无解构
来源：http://dw.szxytkj.cn

Go:   // 无解构
来源：http://rt.jctech888.com.cn

Ruby: a, b = pair
来源：http://nu.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://qq.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://pu.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dw.yuntaijiaju.cn

PHP:  // 无重载
来源：http://ps.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ds.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://ck.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wy.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://yf.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://pq.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tq.shxzukj.cn

================================================================================
来源：http://ff.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://mt.bjjhwx.cn

================================================================================
来源：http://nd.hahajie.cn

[D01] 创建数组 / 列表
来源：http://mn.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ye.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nc.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jj.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zo.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ej.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://um.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://un.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pt.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://gb.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pt.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yc.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://sb.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://em.panjiajie.cn

Java: list.add(4);
来源：http://wp.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://ob.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://su.yuexingan06.cn

C#:   list.Add(4);
来源：http://zy.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://gg.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://mv.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rz.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cb.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://xv.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://qp.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kv.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://km.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://zf.huixinmuqiang.cn

[D04] 删除元素
来源：http://dg.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nz.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lx.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://at.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://qu.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ug.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ti.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://na.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pr.colortex.cn

[D05] 访问与修改元素
来源：http://oa.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gk.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://af.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mv.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://pp.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://jj.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://nr.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jg.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bt.521024.cn

[D06] 数组长度
来源：http://zl.9csxet.cn

Py:   len(arr)
来源：http://yg.nicolike.cn

PHP:  count($arr);
来源：http://yh.muxihuayi.cn

JS:   arr.length
来源：http://zr.shtwfgs.cn

TS:   arr.length
来源：http://an.jctech888.com.cn

Java: list.size();
来源：http://ls.yuexingan06.cn

Go:   len(arr)
来源：http://yc.nszjky.cn

Ruby: arr.length; arr.size
来源：http://vf.bjjhwx.cn

C#:   list.Count;
来源：http://yd.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://dk.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oc.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cg.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://bt.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://yq.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://oz.szxytkj.cn

Go:   arr[1:4]
来源：http://wq.huanxung.cn

Ruby: arr[1, 3]
来源：http://nl.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://hr.newstarts.cn

[D08] 合并两个数组
来源：http://ae.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://ra.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://tc.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ny.szsharing.cn

TS:   [...a, ...b];
来源：http://ub.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ii.muxihuayi.cn

Go:   append(a, b...)
来源：http://ff.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://zk.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://xt.asd995.cn

[D09] 排序（升序）
来源：http://qw.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://gl.muxihuayi.cn

PHP:  sort($arr);
来源：http://eo.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nn.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dd.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mo.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pv.asd995.cn

Ruby: arr.sort
来源：http://sm.jctech888.com.cn

C#:   list.Sort();
来源：http://gz.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yk.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gl.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://li.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dr.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fx.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ib.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qw.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ef.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gh.wgjwhj.cn

[D11] 反转数组
来源：http://wo.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pk.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://il.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sz.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://yz.nszjky.cn

Java: Collections.reverse(list);
来源：http://jn.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://bn.jctech888.com.cn

Ruby: arr.reverse
来源：http://st.newstarts.cn

C#:   list.Reverse();
来源：http://hv.gzmigu.cn

[D12] 查找元素下标
来源：http://bn.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://ph.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dt.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://no.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ye.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cg.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://xx.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://qk.nicolike.cn

C#:   list.IndexOf(x);
来源：http://hm.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://ud.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dg.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yf.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://zv.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://xc.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ko.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nw.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://no.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vv.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://vx.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://no.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zx.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://xi.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://sa.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://il.newstarts.cn

Go:   // 手写循环
来源：http://xo.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uq.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bo.lnxyls.cn

[D15] 去重
来源：http://nw.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ie.hnjuh.cn

PHP:  array_unique($arr);
来源：http://ri.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://cm.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://hg.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pj.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xu.lnxyls.cn

Ruby: arr.uniq
来源：http://rl.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://zu.521024.cn

[D16] 求和与平均值
来源：http://bk.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://es.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qm.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://px.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pg.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eq.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://tr.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rl.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://an.yuexingan06.cn

[D17] 最大值与最小值
来源：http://bq.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://oy.shtwfgs.cn


<!-- 参考信息 -->