代发 wailian999

PHP:  $a && $b || !$c
来源：http://qj.huanxung.cn

JS:   a && b || !c
来源：http://vr.panjiajie.cn

TS:   a && b || !c
来源：http://wu.jianghongdianzi.cn

Java: a && b || !c
来源：http://xj.wgjwhj.cn

Go:   a && b || !c
来源：http://cu.nszjky.cn

Ruby: a && b || !c
来源：http://qp.jianghongdianzi.cn

C#:   a && b || !c
来源：http://wr.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ps.bjjhwx.cn

Py:   if not data: return
来源：http://zm.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://me.szsharing.cn

JS:   if (!data) return;
来源：http://rt.hnjuh.cn

TS:   if (!data) return;
来源：http://is.huixiangedu.cn

Java: if (data == null) return;
来源：http://lq.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://wz.asd995.cn

Ruby: return if data.nil?
来源：http://xo.haigaiapp.cn

C#:   if (data == null) return;
来源：http://ph.nicolike.cn

================================================================================
来源：http://qb.szsharing.cn

C. 函数与作用域
来源：http://lx.lnxyls.cn

================================================================================
来源：http://ex.huixiangedu.cn

[C01] 定义函数
来源：http://yo.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://hu.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://td.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://rm.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cy.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ob.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://on.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://xx.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zp.nicolike.cn

[C02] 默认参数
来源：http://pe.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://rq.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bq.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://ts.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jc.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cx.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qq.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://vw.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://bv.chemitech.net.cn

[C03] 可变参数
来源：http://eg.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://dh.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ny.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fe.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pu.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mz.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jf.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bs.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://df.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://rs.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pf.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mh.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bg.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vs.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://mq.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://fp.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://km.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://ic.hnjuh.cn

[C05] 返回多个值
来源：http://qt.jctech888.com.cn

Py:   return a, b
来源：http://yk.panjiajie.cn

PHP:  return [$a, $b];
来源：http://ey.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ve.nszjky.cn

TS:   return { a, b };
来源：http://ox.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ed.bookmarksfly.cn

Go:   return a, b
来源：http://km.nszjky.cn

Ruby: return a, b
来源：http://ue.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://vp.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://ne.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://mk.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yy.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://rs.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://dt.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vj.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pe.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://ua.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ei.9csxet.cn

[C07] 把函数作为参数传入
来源：http://it.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aq.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xx.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cj.newstarts.cn

TS:   arr.map(String)
来源：http://wv.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hg.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ii.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://cd.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://de.shtwfgs.cn

[C08] 闭包
来源：http://si.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://he.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ds.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fh.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pz.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xj.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uf.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mq.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ra.newstarts.cn

[C09] 递归
来源：http://ff.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lc.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mh.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lr.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ye.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sg.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sc.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qx.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wt.shtwfgs.cn

[C10] 变量作用域
来源：http://lx.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oi.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lq.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fu.muxihuayi.cn

TS:   同 JS
来源：http://wb.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://dq.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://jt.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bn.haigaiapp.cn

C#:   块级作用域
来源：http://ll.panjiajie.cn

[C11] 模块导入与导出
来源：http://cl.bookmarksfly.cn

Py:   from module import func
来源：http://ox.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aq.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gd.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lx.yuntaijiaju.cn

Java: import java.util.List;
来源：http://ny.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jq.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://bb.shtwfgs.cn

C#:   using System.Text;
来源：http://qa.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ix.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://dp.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://bc.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://mx.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://ho.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ue.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://fv.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://rn.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pt.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://cs.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ur.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tq.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hl.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hm.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qx.nicolike.cn

Go:   func add(a, b int) int
来源：http://da.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hy.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ar.jctech888.com.cn

[C14] 泛型函数
来源：http://wn.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tz.muxihuayi.cn

PHP:  // 无泛型
来源：http://pr.nszjky.cn

JS:   // 无泛型
来源：http://il.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nq.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rm.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nz.shxzskj.cn

Ruby: # 无泛型
来源：http://di.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ud.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://kg.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://py.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://fs.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ik.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ye.521024.cn

Java: // 无解构
来源：http://ec.szsharing.cn

Go:   // 无解构
来源：http://bl.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://xa.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://bo.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://lg.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://we.yuexingan06.cn

PHP:  // 无重载
来源：http://ma.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gv.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://ew.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rh.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://pv.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://mq.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sh.hahajie.cn

================================================================================
来源：http://ne.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://cw.chemitech.net.cn

================================================================================
来源：http://vp.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://td.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://af.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cn.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ys.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pq.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mr.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://sl.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://ow.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cl.szxytkj.cn

[D02] 追加元素到末尾
来源：http://fa.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fr.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bg.9csxet.cn

JS:   arr.push(4);
来源：http://dy.shxzukj.cn

TS:   arr.push(4);
来源：http://ib.panjiajie.cn

Java: list.add(4);
来源：http://dr.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://vs.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://mg.muxihuayi.cn

C#:   list.Add(4);
来源：http://qp.nicolike.cn

[D03] 在指定位置插入元素
来源：http://gr.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://im.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aa.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ut.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://cz.muxihuayi.cn

Java: list.add(0, 0);
来源：http://fk.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dg.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jg.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://we.nszjky.cn

[D04] 删除元素
来源：http://io.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xp.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://du.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://re.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://gu.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tt.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eu.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ry.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lx.huanxung.cn

[D05] 访问与修改元素
来源：http://mb.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qy.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nj.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fn.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://pb.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://so.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://rr.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tt.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cf.bookmarksfly.cn

[D06] 数组长度
来源：http://bv.jctech888.com.cn

Py:   len(arr)
来源：http://dy.huixiangedu.cn

PHP:  count($arr);
来源：http://vk.yuntaijiaju.cn

JS:   arr.length
来源：http://dc.jctech888.com.cn

TS:   arr.length
来源：http://hw.haigaiapp.cn

Java: list.size();
来源：http://lj.lnxyls.cn

Go:   len(arr)
来源：http://le.szsharing.cn

Ruby: arr.length; arr.size
来源：http://vv.muxihuayi.cn

C#:   list.Count;
来源：http://gy.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://fo.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ds.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fc.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://lw.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://vm.hahajie.cn

Java: list.subList(1, 4);
来源：http://ll.wgjwhj.cn

Go:   arr[1:4]
来源：http://ff.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://wf.521024.cn

C#:   list.GetRange(1, 3);
来源：http://bl.szxytkj.cn

[D08] 合并两个数组
来源：http://ek.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://sx.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://nz.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pw.jctech888.com.cn

TS:   [...a, ...b];
来源：http://du.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nk.nicolike.cn

Go:   append(a, b...)
来源：http://ml.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://gn.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://qp.szsharing.cn

[D09] 排序（升序）
来源：http://ux.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://me.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://hi.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qk.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dl.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oz.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mk.hnjuh.cn

Ruby: arr.sort
来源：http://nk.colortex.cn

C#:   list.Sort();
来源：http://hh.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ak.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qk.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kw.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kn.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mv.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xz.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wd.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jm.nszjky.cn

[D11] 反转数组
来源：http://ke.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ub.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://wj.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bi.nicolike.cn

TS:   [...arr].reverse();
来源：http://wj.szsharing.cn

Java: Collections.reverse(list);
来源：http://jj.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://dp.nicolike.cn

Ruby: arr.reverse
来源：http://ak.nicolike.cn

C#:   list.Reverse();
来源：http://uo.lnxyls.cn

[D12] 查找元素下标
来源：http://rc.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://yx.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kw.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wc.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ne.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qa.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://fz.wgjwhj.cn

Ruby: arr.index(x)
来源：http://cf.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://pf.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://ul.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qz.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lx.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://no.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://ix.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cn.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cq.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sh.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ld.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://df.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mf.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yo.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://xq.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://xb.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dt.jctech888.com.cn

Go:   // 手写循环
来源：http://zo.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ek.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hm.asd995.cn

[D15] 去重
来源：http://bp.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ev.gzmigu.cn

PHP:  array_unique($arr);
来源：http://ug.hahajie.cn

JS:   [...new Set(arr)]
来源：http://ro.521024.cn

TS:   [...new Set(arr)]
来源：http://sj.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dt.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rv.asd995.cn

Ruby: arr.uniq
来源：http://eh.chemitech.net.cn


<!-- 参考信息 -->