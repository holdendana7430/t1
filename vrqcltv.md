代发 wailian999

Go:   a && b || !c
来源：http://hh.colortex.cn

Ruby: a && b || !c
来源：http://fw.chemitech.net.cn

C#:   a && b || !c
来源：http://wv.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hh.szsharing.cn

Py:   if not data: return
来源：http://fz.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://zj.panjiajie.cn

JS:   if (!data) return;
来源：http://hx.huanxung.cn

TS:   if (!data) return;
来源：http://pa.nicolike.cn

Java: if (data == null) return;
来源：http://uj.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://tb.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://rp.gzmigu.cn

C#:   if (data == null) return;
来源：http://ey.asd995.cn

================================================================================
来源：http://ta.panjiajie.cn

C. 函数与作用域
来源：http://xx.hahajie.cn

================================================================================
来源：http://bc.bjjhwx.cn

[C01] 定义函数
来源：http://ca.521024.cn

Py:   def add(a, b): return a + b
来源：http://av.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sx.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://hc.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fo.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ie.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qg.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://sw.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://li.shxzskj.cn

[C02] 默认参数
来源：http://yg.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://bp.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pu.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://sz.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ix.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rw.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xt.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://uf.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://gz.muxihuayi.cn

[C03] 可变参数
来源：http://dz.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://io.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yl.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dc.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bp.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sr.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xh.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tw.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vr.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://iq.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ms.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dw.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qe.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xi.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://mz.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://sf.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://pi.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://yk.yuexingan06.cn

[C05] 返回多个值
来源：http://lg.panjiajie.cn

Py:   return a, b
来源：http://un.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://yy.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://st.nicolike.cn

TS:   return { a, b };
来源：http://pq.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zh.hnjuh.cn

Go:   return a, b
来源：http://cn.jctech888.com.cn

Ruby: return a, b
来源：http://ui.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://jm.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://bq.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://rb.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sr.gzmigu.cn

JS:   const square = x => x * x;
来源：http://am.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://ay.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://md.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tj.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://ts.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zh.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://vf.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yu.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eq.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bb.yuexingan06.cn

TS:   arr.map(String)
来源：http://tf.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lx.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dq.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://vn.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jx.shtwfgs.cn

[C08] 闭包
来源：http://np.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wt.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hf.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wk.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ex.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gq.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bl.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://an.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tm.bookmarksfly.cn

[C09] 递归
来源：http://aq.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gv.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dm.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rq.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ex.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wl.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nc.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kv.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ib.shxzskj.cn

[C10] 变量作用域
来源：http://ve.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mb.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://te.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ik.shtwfgs.cn

TS:   同 JS
来源：http://fn.colortex.cn

Java: 方法内为块级作用域
来源：http://zr.hnjuh.cn

Go:   花括号块级作用域
来源：http://uj.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vm.521024.cn

C#:   块级作用域
来源：http://dj.panjiajie.cn

[C11] 模块导入与导出
来源：http://mv.gzmigu.cn

Py:   from module import func
来源：http://th.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bl.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zb.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fi.haigaiapp.cn

Java: import java.util.List;
来源：http://al.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ih.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://mj.bjjhwx.cn

C#:   using System.Text;
来源：http://sz.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://sz.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://bo.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://zb.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://wq.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://ln.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tl.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://lh.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://iv.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mr.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://dp.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ae.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ic.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xb.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ue.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cp.shxzukj.cn

Go:   func add(a, b int) int
来源：http://my.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fn.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://el.huixinmuqiang.cn

[C14] 泛型函数
来源：http://cu.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kc.shxzukj.cn

PHP:  // 无泛型
来源：http://lf.newstarts.cn

JS:   // 无泛型
来源：http://tc.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gp.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bn.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://km.hahajie.cn

Ruby: # 无泛型
来源：http://jz.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pb.szsharing.cn

[C15] 解构 / 展开参数
来源：http://zp.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oj.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://vx.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ut.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gp.haigaiapp.cn

Java: // 无解构
来源：http://ed.colortex.cn

Go:   // 无解构
来源：http://ft.yuexingan06.cn

Ruby: a, b = pair
来源：http://gk.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://cq.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://sr.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zl.haigaiapp.cn

PHP:  // 无重载
来源：http://wl.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ad.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://bw.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vx.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://mw.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://tu.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mg.hahajie.cn

================================================================================
来源：http://qt.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://df.nszjky.cn

================================================================================
来源：http://bq.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://mo.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gw.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mg.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fz.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yx.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ce.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://di.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://nv.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qn.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://vz.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ap.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sb.9csxet.cn

JS:   arr.push(4);
来源：http://tm.yuexingan06.cn

TS:   arr.push(4);
来源：http://vk.shtwfgs.cn

Java: list.add(4);
来源：http://tv.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://ww.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://lc.huanxung.cn

C#:   list.Add(4);
来源：http://se.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://bt.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://hd.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://li.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qf.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://zr.yuexingan06.cn

Java: list.add(0, 0);
来源：http://qe.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mm.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kc.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://rs.hnjuh.cn

[D04] 删除元素
来源：http://ej.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tv.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cq.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uy.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://fo.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ic.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sn.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hs.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vd.nszjky.cn

[D05] 访问与修改元素
来源：http://wl.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xl.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ne.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gd.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://fc.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://bx.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://rw.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bh.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://le.lnxyls.cn

[D06] 数组长度
来源：http://xo.newstarts.cn

Py:   len(arr)
来源：http://ah.shtwfgs.cn

PHP:  count($arr);
来源：http://lb.gzmigu.cn

JS:   arr.length
来源：http://py.muxihuayi.cn

TS:   arr.length
来源：http://lf.9csxet.cn

Java: list.size();
来源：http://bb.shxzukj.cn

Go:   len(arr)
来源：http://ko.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://yv.szsharing.cn

C#:   list.Count;
来源：http://oi.szsharing.cn

[D07] 切片 / 取子数组
来源：http://tb.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pe.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iv.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://iu.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://lj.panjiajie.cn

Java: list.subList(1, 4);
来源：http://pk.muxihuayi.cn

Go:   arr[1:4]
来源：http://xz.asd995.cn

Ruby: arr[1, 3]
来源：http://ff.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://pf.hnjuh.cn

[D08] 合并两个数组
来源：http://xw.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://xw.colortex.cn

PHP:  array_merge($a, $b);
来源：http://ey.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bn.chemitech.net.cn

TS:   [...a, ...b];
来源：http://xw.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ek.hnjuh.cn

Go:   append(a, b...)
来源：http://mc.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://ad.521024.cn

C#:   a.Concat(b).ToList()
来源：http://mp.szxytkj.cn

[D09] 排序（升序）
来源：http://zf.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://as.muxihuayi.cn

PHP:  sort($arr);
来源：http://bx.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fv.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://no.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kt.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nl.nszjky.cn

Ruby: arr.sort
来源：http://um.521024.cn

C#:   list.Sort();
来源：http://os.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ot.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ya.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ze.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fm.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oq.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eh.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mr.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hy.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xn.muxihuayi.cn

[D11] 反转数组
来源：http://en.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aw.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://sx.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kz.asd995.cn

TS:   [...arr].reverse();
来源：http://ap.hnjuh.cn

Java: Collections.reverse(list);
来源：http://ji.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://dj.lnxyls.cn

Ruby: arr.reverse
来源：http://td.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://ku.muxihuayi.cn

[D12] 查找元素下标
来源：http://pu.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://hq.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eh.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vy.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tt.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tj.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://nb.nszjky.cn

Ruby: arr.index(x)
来源：http://qb.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://mp.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://sj.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qg.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zs.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://cq.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://mm.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ze.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bt.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qq.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hv.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://hd.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eb.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oj.521024.cn

JS:   arr.map(x => x * 2)
来源：http://ql.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://du.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dl.yuntaijiaju.cn

Go:   // 手写循环
来源：http://zh.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zz.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ag.szsharing.cn

[D15] 去重
来源：http://jz.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kh.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://fw.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://sf.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://rw.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wk.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nq.bjjhwx.cn

Ruby: arr.uniq
来源：http://io.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://vq.huixiangedu.cn

[D16] 求和与平均值
来源：http://of.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kf.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vj.shxzukj.cn


<!-- 参考信息 -->