代发 wailian999

[C02] 默认参数
来源：http://vs.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://qr.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tx.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://sq.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tm.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dp.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dd.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://yr.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://dz.panjiajie.cn

[C03] 可变参数
来源：http://pb.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://yg.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rs.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jp.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nd.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sk.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sx.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://by.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oj.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://vq.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fc.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xc.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sa.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ng.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://gf.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://xz.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ni.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://dd.haigaiapp.cn

[C05] 返回多个值
来源：http://rp.shxzukj.cn

Py:   return a, b
来源：http://nr.hahajie.cn

PHP:  return [$a, $b];
来源：http://xs.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mm.9csxet.cn

TS:   return { a, b };
来源：http://ra.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hv.bjjhwx.cn

Go:   return a, b
来源：http://ma.gzmigu.cn

Ruby: return a, b
来源：http://yw.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://zq.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://xm.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://kt.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xa.9csxet.cn

JS:   const square = x => x * x;
来源：http://hl.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://po.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ml.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oh.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://jl.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bt.newstarts.cn

[C07] 把函数作为参数传入
来源：http://qe.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eo.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lj.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ou.shxzskj.cn

TS:   arr.map(String)
来源：http://nq.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nk.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jd.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://nq.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lk.yuntaijiaju.cn

[C08] 闭包
来源：http://gs.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jh.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fp.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tq.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://le.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pu.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gv.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fc.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ra.hnjuh.cn

[C09] 递归
来源：http://ch.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ui.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zk.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jg.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uf.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uh.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yw.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lm.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ag.haigaiapp.cn

[C10] 变量作用域
来源：http://ei.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zp.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fm.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pj.yuntaijiaju.cn

TS:   同 JS
来源：http://rp.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://lr.gzmigu.cn

Go:   花括号块级作用域
来源：http://xl.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ah.panjiajie.cn

C#:   块级作用域
来源：http://zt.huixiangedu.cn

[C11] 模块导入与导出
来源：http://xy.huixiangedu.cn

Py:   from module import func
来源：http://qv.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://er.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eq.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rc.bookmarksfly.cn

Java: import java.util.List;
来源：http://uw.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jh.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://ah.yuexingan06.cn

C#:   using System.Text;
来源：http://hh.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://gw.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://yc.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://kz.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://jh.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://de.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oe.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://rf.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://jl.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gs.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://jk.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://il.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xv.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://av.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kv.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rh.nszjky.cn

Go:   func add(a, b int) int
来源：http://eu.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ib.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xp.nicolike.cn

[C14] 泛型函数
来源：http://qw.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gv.haigaiapp.cn

PHP:  // 无泛型
来源：http://pv.bjjhwx.cn

JS:   // 无泛型
来源：http://fo.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hb.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bu.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xo.yuexingan06.cn

Ruby: # 无泛型
来源：http://sf.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vp.newstarts.cn

[C15] 解构 / 展开参数
来源：http://fq.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lp.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://pz.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ls.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wt.shtwfgs.cn

Java: // 无解构
来源：http://pk.hnjuh.cn

Go:   // 无解构
来源：http://be.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://lr.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://rj.nicolike.cn

[C16] 函数 / 方法重载
来源：http://xu.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ty.wgjwhj.cn

PHP:  // 无重载
来源：http://ie.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mo.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ug.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rj.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://zm.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://wr.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nf.hahajie.cn

================================================================================
来源：http://ve.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://uw.yuexingan06.cn

================================================================================
来源：http://fi.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://mh.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ba.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lc.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xb.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gp.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qu.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://zg.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://ng.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sp.nszjky.cn

[D02] 追加元素到末尾
来源：http://fp.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ot.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bg.521024.cn

JS:   arr.push(4);
来源：http://lu.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://yx.jctech888.com.cn

Java: list.add(4);
来源：http://sh.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://vm.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://di.huanxung.cn

C#:   list.Add(4);
来源：http://je.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://in.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://gz.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fn.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://df.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://fo.muxihuayi.cn

Java: list.add(0, 0);
来源：http://pi.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sl.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tt.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://ru.lnxyls.cn

[D04] 删除元素
来源：http://lx.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fd.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hm.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bg.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://bm.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://na.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vg.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kb.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ai.nszjky.cn

[D05] 访问与修改元素
来源：http://su.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gq.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sn.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dv.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://vd.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://dt.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://tr.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://su.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mw.shtwfgs.cn

[D06] 数组长度
来源：http://wf.nszjky.cn

Py:   len(arr)
来源：http://cj.colortex.cn

PHP:  count($arr);
来源：http://rz.521024.cn

JS:   arr.length
来源：http://cx.nicolike.cn

TS:   arr.length
来源：http://pk.huanxung.cn

Java: list.size();
来源：http://td.huixiangedu.cn

Go:   len(arr)
来源：http://gd.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://gl.lnxyls.cn

C#:   list.Count;
来源：http://ej.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://xv.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wr.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xc.521024.cn

JS:   arr.slice(1, 4);
来源：http://vd.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://hk.asd995.cn

Java: list.subList(1, 4);
来源：http://mx.hnjuh.cn

Go:   arr[1:4]
来源：http://rk.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://og.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://qr.nicolike.cn

[D08] 合并两个数组
来源：http://rk.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://sj.colortex.cn

PHP:  array_merge($a, $b);
来源：http://vm.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jf.huixiangedu.cn

TS:   [...a, ...b];
来源：http://pc.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bq.jctech888.com.cn

Go:   append(a, b...)
来源：http://hj.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://ta.521024.cn

C#:   a.Concat(b).ToList()
来源：http://ey.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://ii.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://dy.asd995.cn

PHP:  sort($arr);
来源：http://ug.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dx.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dr.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hg.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ew.9csxet.cn

Ruby: arr.sort
来源：http://sl.521024.cn

C#:   list.Sort();
来源：http://ba.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hr.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xk.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://la.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bj.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kd.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vd.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://th.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://it.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ym.huixinmuqiang.cn

[D11] 反转数组
来源：http://ds.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mc.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://nd.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xx.nszjky.cn

TS:   [...arr].reverse();
来源：http://rb.huanxung.cn

Java: Collections.reverse(list);
来源：http://fz.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://yf.nszjky.cn

Ruby: arr.reverse
来源：http://ro.521024.cn

C#:   list.Reverse();
来源：http://on.bookmarksfly.cn

[D12] 查找元素下标
来源：http://fm.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://ph.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zx.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hw.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mq.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pa.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://ee.szsharing.cn

Ruby: arr.index(x)
来源：http://qi.huanxung.cn

C#:   list.IndexOf(x);
来源：http://eh.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://jc.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ay.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wp.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://yi.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://ku.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qp.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vq.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://le.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ha.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://ih.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hl.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://do.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://ad.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://nx.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gf.lnxyls.cn

Go:   // 手写循环
来源：http://tg.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://if.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ds.wgjwhj.cn

[D15] 去重
来源：http://ct.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ee.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://zs.hahajie.cn

JS:   [...new Set(arr)]
来源：http://ya.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://kg.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kk.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gf.9csxet.cn

Ruby: arr.uniq
来源：http://np.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://hq.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://ez.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sg.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fu.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dr.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bk.gzmigu.cn

Go:   // 手写循环累加
来源：http://ei.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wm.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://pf.gzmigu.cn

[D17] 最大值与最小值
来源：http://nn.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://fy.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://ay.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wl.nszjky.cn

TS:   Math.max(...arr);
来源：http://pz.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://op.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lk.colortex.cn

Ruby: arr.max;  arr.min
来源：http://rt.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://de.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://rt.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qr.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://ar.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sp.huanxung.cn

TS:   nested.flat();
来源：http://rz.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zm.lnxyls.cn

Go:   // 手写双层循环
来源：http://lk.nszjky.cn

Ruby: nested.flatten
来源：http://oj.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rf.yuexingan06.cn


<!-- 参考信息 -->